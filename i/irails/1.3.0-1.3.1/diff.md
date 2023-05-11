# Comparing `tmp/irails-1.3.0.tar.gz` & `tmp/irails-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.0.tar", last modified: Thu May 11 06:16:05 2023, max compression
+gzip compressed data, was "irails-1.3.1.tar", last modified: Thu May 11 10:59:45 2023, max compression
```

## Comparing `irails-1.3.0.tar` & `irails-1.3.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.185909 irails-1.3.0/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5079 2023-05-11 06:16:05.184912 irails-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.086601 irails-1.3.0/irails/
--rw-rw-rw-   0        0        0      331 2023-05-11 06:15:50.000000 irails-1.3.0/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.3.0/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.3.0/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.0/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.3.0/irails/auth.py
--rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.3.0/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.095575 irails-1.3.0/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.096573 irails-1.3.0/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.0/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.3.0/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.0/irails/cbv.py
--rw-rw-rw-   0        0        0     7319 2023-05-11 06:14:17.000000 irails-1.3.0/irails/config.py
--rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.3.0/irails/controller_utils.py
--rw-rw-rw-   0        0        0    32141 2023-05-11 05:41:05.000000 irails-1.3.0/irails/core.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.3.0/irails/database.py
--rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.3.0/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.0/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.3.0/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.0/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.110536 irails-1.3.0/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.0/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.3.0/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.3.0/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.3.0/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.0/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1556 2023-05-11 05:57:14.000000 irails-1.3.0/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1908 2023-05-11 05:08:52.000000 irails-1.3.0/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.3.0/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.052440 irails-1.3.0/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.142451 irails-1.3.0/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.0/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.0/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.0/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.0/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.0/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.0/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.3.0/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.0/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.145443 irails-1.3.0/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.0/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.147444 irails-1.3.0/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.0/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.162398 irails-1.3.0/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.0/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.3.0/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.0/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.0/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.0/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.0/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.0/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.0/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.0/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.055428 irails-1.3.0/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.166387 irails-1.3.0/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.0/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.0/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.0/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.3.0/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.170942 irails-1.3.0/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.0/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.0/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.173937 irails-1.3.0/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.059418 irails-1.3.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.176928 irails-1.3.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.180929 irails-1.3.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.060415 irails-1.3.0/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.181916 irails-1.3.0/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.0/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.3.0/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:16:05.093581 irails-1.3.0/irails.egg-info/
--rw-rw-rw-   0        0        0     5079 2023-05-11 06:16:04.000000 irails-1.3.0/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2312 2023-05-11 06:16:04.000000 irails-1.3.0/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 06:16:04.000000 irails-1.3.0/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-11 06:16:04.000000 irails-1.3.0/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      766 2023-05-11 06:16:04.000000 irails-1.3.0/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 06:16:04.000000 irails-1.3.0/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 06:16:05.186915 irails-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.316772 irails-1.3.1/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-11 10:59:45.316772 irails-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.217037 irails-1.3.1/irails/
+-rw-rw-rw-   0        0        0      331 2023-05-11 10:59:19.000000 irails-1.3.1/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.3.1/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.3.1/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.1/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.3.1/irails/auth.py
+-rw-rw-rw-   0        0        0    12241 2023-05-11 10:56:55.000000 irails-1.3.1/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.231996 irails-1.3.1/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.233991 irails-1.3.1/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.3.1/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.1/irails/cbv.py
+-rw-rw-rw-   0        0        0     7319 2023-05-11 06:14:17.000000 irails-1.3.1/irails/config.py
+-rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.3.1/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32141 2023-05-11 05:41:05.000000 irails-1.3.1/irails/core.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.3.1/irails/database.py
+-rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.3.1/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.1/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.3.1/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.1/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.246956 irails-1.3.1/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.1/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.3.1/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.3.1/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.3.1/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.1/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1556 2023-05-11 05:57:14.000000 irails-1.3.1/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1908 2023-05-11 05:08:52.000000 irails-1.3.1/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.3.1/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.170163 irails-1.3.1/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.261917 irails-1.3.1/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.1/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.1/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.1/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.1/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.1/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.1/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.3.1/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.1/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.264909 irails-1.3.1/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.1/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.265906 irails-1.3.1/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.1/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.284855 irails-1.3.1/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.1/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.3.1/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.1/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.1/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.1/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.1/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.1/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.1/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.1/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.174153 irails-1.3.1/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.292833 irails-1.3.1/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.1/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.1/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.1/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.3.1/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.296823 irails-1.3.1/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.1/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.1/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.299815 irails-1.3.1/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.178142 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.305799 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.310786 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.179138 irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.313778 irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.3.1/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.228007 irails-1.3.1/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2312 2023-05-11 10:59:45.000000 irails-1.3.1/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 10:59:45.317767 irails-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.1/setup.py
```

### Comparing `irails-1.3.0/PKG-INFO` & `irails-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: irails Version: 1.3.0 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.3.1 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.3.0/README.md` & `irails-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/_i18n.py` & `irails-1.3.1/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/_loader.py` & `irails-1.3.1/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/_utils.py` & `irails-1.3.1/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/auth.py` & `irails-1.3.1/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/base_controller.py` & `irails-1.3.1/irails/base_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,30 +159,42 @@
         def get_path(caller_frame,view_path:str="",context:dict={},local2context:bool=True ):
             # caller_file = caller_frame.f_code.co_filename
             # caller_lineno = caller_frame.f_lineno
             caller_function_name = caller_frame.f_code.co_name
             caller_locals = caller_frame.f_locals
             caller_class = caller_locals.get("self", None).__class__
             caller_classname:str = caller_class.__name__
-            caller_classname = caller_classname.replace("Controller","").lower()
+            caller_classname = caller_classname.lower().rstrip('controller')
             #caller_file = os.path.basename(caller.filename) 
             if local2context and not context:
                 del caller_locals['self']
                 context.update(caller_locals)
             if not view_path:
                 if self.__version__:
                     version_path = f"{self.__version__}/"
                 else:
                     version_path = ""
                 view_path = f"{caller_classname}/{version_path}{caller_function_name}.html" 
             return view_path,context
-            
-        caller_frame = inspect.currentframe().f_back
-        view_path,context = get_path(caller_frame)
+
+        if not view_path:    
+            caller_frame = inspect.currentframe()
+            caller_frame = caller_frame.f_back
+            #find frame the target controller's action method
+            frame_info = inspect.getframeinfo(caller_frame)
+            action_frame = caller_frame
+            while(frame_info[2]!='decorator' and not frame_info[0].endswith('controller_utils.py')):
+                caller_frame = caller_frame.f_back
+                frame_info = inspect.getframeinfo(caller_frame)
+                if not frame_info[2]=='decorator' and not frame_info[0].endswith('controller_utils.py'):
+                    action_frame = caller_frame
+            view_path,context = get_path(action_frame)
         
+        if not isinstance(context,dict):
+            context = {}
         if not 'flash' in context:
             context['flash'] = self._request.session['flash']
         template_path = os.path.join(self.__appdir__,"views")
         viewobj = _View(self._request,self._response, tmpl_path=template_path) 
         viewobj._templates.env.globals["url_for"] = url_for 
         viewobj._templates.env.globals["_"] = self._ 
         return viewobj(view_path,context,**kwargs)
```

### Comparing `irails-1.3.0/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.1/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/cbv.py` & `irails-1.3.1/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/config.py` & `irails-1.3.1/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/controller_utils.py` & `irails-1.3.1/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/core.py` & `irails-1.3.1/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/database.py` & `irails-1.3.1/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/midware.py` & `irails-1.3.1/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/midware_casbin.py` & `irails-1.3.1/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/midware_session.py` & `irails-1.3.1/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/mvc_router.py` & `irails-1.3.1/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/_app.py` & `irails-1.3.1/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/_controller.py` & `irails-1.3.1/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/_i18n.py` & `irails-1.3.1/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/_project.py` & `irails-1.3.1/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/_run.py` & `irails-1.3.1/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/_shell.py` & `irails-1.3.1/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/main.py` & `irails-1.3.1/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.1/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/app/home.tpl` & `irails-1.3.1/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.1/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.1/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.1/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.1/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.1/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.1/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails/view.py` & `irails-1.3.1/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails.egg-info/PKG-INFO` & `irails-1.3.1/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: irails Version: 1.3.0 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.3.1 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.3.0/irails.egg-info/SOURCES.txt` & `irails-1.3.1/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/irails.egg-info/requires.txt` & `irails-1.3.1/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.0/setup.py` & `irails-1.3.1/setup.py`

 * *Files identical despite different names*


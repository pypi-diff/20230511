# Comparing `tmp/irails-1.2.7.tar.gz` & `tmp/irails-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.2.7.tar", last modified: Thu May 11 05:35:44 2023, max compression
+gzip compressed data, was "irails-1.2.8.tar", last modified: Thu May 11 05:58:45 2023, max compression
```

## Comparing `irails-1.2.7.tar` & `irails-1.2.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.425657 irails-1.2.7/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5079 2023-05-11 05:35:44.425657 irails-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.367846 irails-1.2.7/irails/
--rw-rw-rw-   0        0        0      331 2023-05-11 05:35:30.000000 irails-1.2.7/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.7/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.7/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.7/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.7/irails/auth.py
--rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.7/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.374793 irails-1.2.7/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.375791 irails-1.2.7/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.7/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.7/irails/cbv.py
--rw-rw-rw-   0        0        0     7245 2023-05-11 05:30:32.000000 irails-1.2.7/irails/config.py
--rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.2.7/irails/controller_utils.py
--rw-rw-rw-   0        0        0    32135 2023-05-11 04:55:40.000000 irails-1.2.7/irails/core.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.7/irails/database.py
--rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.7/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.7/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.7/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.7/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.384779 irails-1.2.7/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.7/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.7/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.7/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.2.7/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.7/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1423 2023-05-10 10:55:35.000000 irails-1.2.7/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1908 2023-05-11 05:08:52.000000 irails-1.2.7/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.7/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.340880 irails-1.2.7/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.392746 irails-1.2.7/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.7/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.7/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.7/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.7/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.7/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.7/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.7/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.7/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.394741 irails-1.2.7/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.7/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.395738 irails-1.2.7/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.7/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.406709 irails-1.2.7/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.7/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.7/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.7/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.7/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.7/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.2.7/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.2.7/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.7/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.7/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.342874 irails-1.2.7/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.409701 irails-1.2.7/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.2.7/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.2.7/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.2.7/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.2.7/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.411695 irails-1.2.7/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.7/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.7/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.414687 irails-1.2.7/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.345868 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.418676 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.421667 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.345868 irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.423663 irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.7/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.373793 irails-1.2.7/irails.egg-info/
--rw-rw-rw-   0        0        0     5079 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2312 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      766 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 05:35:44.426655 irails-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.871629 irails-1.2.8/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-11 05:58:45.870614 irails-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.809444 irails-1.2.8/irails/
+-rw-rw-rw-   0        0        0      331 2023-05-11 05:58:33.000000 irails-1.2.8/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.8/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.8/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.8/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.8/irails/auth.py
+-rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.8/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.818422 irails-1.2.8/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.820333 irails-1.2.8/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.8/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.8/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.8/irails/cbv.py
+-rw-rw-rw-   0        0        0     7245 2023-05-11 05:30:32.000000 irails-1.2.8/irails/config.py
+-rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.2.8/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32141 2023-05-11 05:41:05.000000 irails-1.2.8/irails/core.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.8/irails/database.py
+-rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.8/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.8/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.8/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.8/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.827402 irails-1.2.8/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.8/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.8/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.8/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.2.8/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.8/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1556 2023-05-11 05:57:14.000000 irails-1.2.8/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1908 2023-05-11 05:08:52.000000 irails-1.2.8/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.8/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.777916 irails-1.2.8/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.836378 irails-1.2.8/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.8/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.8/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.8/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.8/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.8/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.8/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.8/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.8/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.838374 irails-1.2.8/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.8/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.839371 irails-1.2.8/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.8/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.850345 irails-1.2.8/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.8/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.8/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.8/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.8/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.8/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.2.8/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.2.8/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.8/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.8/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.780908 irails-1.2.8/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.854653 irails-1.2.8/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.2.8/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.2.8/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.2.8/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.2.8/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.856652 irails-1.2.8/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.8/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.8/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.858646 irails-1.2.8/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.785910 irails-1.2.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.861637 irails-1.2.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.865627 irails-1.2.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.786894 irails-1.2.8/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.867622 irails-1.2.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.8/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:58:45.815431 irails-1.2.8/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-11 05:58:45.000000 irails-1.2.8/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2312 2023-05-11 05:58:45.000000 irails-1.2.8/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:58:45.000000 irails-1.2.8/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-11 05:58:45.000000 irails-1.2.8/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-11 05:58:45.000000 irails-1.2.8/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 05:58:45.000000 irails-1.2.8/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:58:45.871629 irails-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.8/setup.py
```

### Comparing `irails-1.2.7/PKG-INFO` & `irails-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.7
+Version: 1.2.8
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
-Metadata-Version: 2.1 Name: irails Version: 1.2.7 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.8 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.7/README.md` & `irails-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/_i18n.py` & `irails-1.2.8/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/_loader.py` & `irails-1.2.8/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/_utils.py` & `irails-1.2.8/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/auth.py` & `irails-1.2.8/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/base_controller.py` & `irails-1.2.8/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.2.8/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.2.8/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/cbv.py` & `irails-1.2.8/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/config.py` & `irails-1.2.8/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/controller_utils.py` & `irails-1.2.8/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/core.py` & `irails-1.2.8/irails/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from fastapi.params import Depends
 from fastapi.utils import generate_unique_id
 from starlette.responses import JSONResponse, Response
 from starlette.routing import BaseRoute
 from fastapi.types import DecoratedCallable
 from .mvc_router import create_controller,MvcRouter as api,   register_controllers_to_app 
 from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
-from .config import config,ROOT_PATH,_log
+from .config import config,ROOT_PATH,_log,set_logger
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
 from ._utils import get_controller_name,get_snaked_name
 from ._i18n import load_app_translations
@@ -361,15 +361,15 @@
         if uri:
             database.check_migration(application.data_engine,uri,alembic_ini)
     except Exception as e:
         _log.disabled = False
         _log.error(e.args)
 def generate_mvc_app( ):
     global __is_debug
-    _log.disabled = False
+    set_logger(_log)
     from ._loader import _load_apps
     
     _log.info(_("\n\init mvc app..."))
     loaded,unloaded=_load_apps(debug=__is_debug) 
     _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %(loaded,unloaded))  
     if not len(__all_controller__)>0:
         raise RuntimeError(_("not found any controller class"))
```

### Comparing `irails-1.2.7/irails/database.py` & `irails-1.2.8/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/midware.py` & `irails-1.2.8/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/midware_casbin.py` & `irails-1.2.8/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/midware_session.py` & `irails-1.2.8/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/mvc_router.py` & `irails-1.2.8/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/_app.py` & `irails-1.2.8/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/_controller.py` & `irails-1.2.8/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/_i18n.py` & `irails-1.2.8/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/_project.py` & `irails-1.2.8/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/_shell.py` & `irails-1.2.8/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/main.py` & `irails-1.2.8/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/app/home.css.tpl` & `irails-1.2.8/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/app/home.tpl` & `irails-1.2.8/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.2.8/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.2.8/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.2.8/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.2.8/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/public/error_404.html` & `irails-1.2.8/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/public/error_500.html` & `irails-1.2.8/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.2.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.2.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.2.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.2.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.2.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails/view.py` & `irails-1.2.8/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails.egg-info/PKG-INFO` & `irails-1.2.8/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.7
+Version: 1.2.8
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
-Metadata-Version: 2.1 Name: irails Version: 1.2.7 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.8 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.7/irails.egg-info/SOURCES.txt` & `irails-1.2.8/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/irails.egg-info/requires.txt` & `irails-1.2.8/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.7/setup.py` & `irails-1.2.8/setup.py`

 * *Files identical despite different names*


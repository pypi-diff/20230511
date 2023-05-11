# Comparing `tmp/irails-1.3.1.tar.gz` & `tmp/irails-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.1.tar", last modified: Thu May 11 10:59:45 2023, max compression
+gzip compressed data, was "irails-1.3.2.tar", last modified: Thu May 11 15:36:16 2023, max compression
```

## Comparing `irails-1.3.1.tar` & `irails-1.3.2.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.316772 irails-1.3.1/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5079 2023-05-11 10:59:45.316772 irails-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.217037 irails-1.3.1/irails/
--rw-rw-rw-   0        0        0      331 2023-05-11 10:59:19.000000 irails-1.3.1/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.3.1/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.3.1/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.1/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.3.1/irails/auth.py
--rw-rw-rw-   0        0        0    12241 2023-05-11 10:56:55.000000 irails-1.3.1/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.231996 irails-1.3.1/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.233991 irails-1.3.1/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.3.1/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.1/irails/cbv.py
--rw-rw-rw-   0        0        0     7319 2023-05-11 06:14:17.000000 irails-1.3.1/irails/config.py
--rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.3.1/irails/controller_utils.py
--rw-rw-rw-   0        0        0    32141 2023-05-11 05:41:05.000000 irails-1.3.1/irails/core.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.3.1/irails/database.py
--rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.3.1/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.1/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.3.1/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.1/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.246956 irails-1.3.1/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.1/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.3.1/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.3.1/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.3.1/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.1/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1556 2023-05-11 05:57:14.000000 irails-1.3.1/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1908 2023-05-11 05:08:52.000000 irails-1.3.1/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.3.1/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.170163 irails-1.3.1/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.261917 irails-1.3.1/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.1/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.1/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.1/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.1/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.1/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.1/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.3.1/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.1/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.264909 irails-1.3.1/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.1/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.265906 irails-1.3.1/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.1/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.284855 irails-1.3.1/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.1/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.3.1/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.1/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.1/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.1/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.1/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.1/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.1/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.1/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.174153 irails-1.3.1/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.292833 irails-1.3.1/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.1/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.1/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.1/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.3.1/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.296823 irails-1.3.1/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.1/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.1/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.299815 irails-1.3.1/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.178142 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.305799 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.310786 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.179138 irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.313778 irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.3.1/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:59:45.228007 irails-1.3.1/irails.egg-info/
--rw-rw-rw-   0        0        0     5079 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2312 2023-05-11 10:59:45.000000 irails-1.3.1/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      766 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 10:59:44.000000 irails-1.3.1/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 10:59:45.317767 irails-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.579850 irails-1.3.2/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-11 15:36:16.578856 irails-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.494161 irails-1.3.2/irails/
+-rw-rw-rw-   0        0        0      306 2023-05-11 15:36:11.000000 irails-1.3.2/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.3.2/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2424 2023-05-11 15:31:46.000000 irails-1.3.2/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.2/irails/_utils.py
+-rw-rw-rw-   0        0        0    11722 2023-05-11 15:21:25.000000 irails-1.3.2/irails/auth.py
+-rw-rw-rw-   0        0        0    12404 2023-05-11 15:21:09.000000 irails-1.3.2/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.507039 irails-1.3.2/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.508036 irails-1.3.2/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.2/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.3.2/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.2/irails/cbv.py
+-rw-rw-rw-   0        0        0     6065 2023-05-11 15:19:41.000000 irails-1.3.2/irails/config.py
+-rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.3.2/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32262 2023-05-11 15:20:13.000000 irails-1.3.2/irails/core.py
+-rw-rw-rw-   0        0        0     6409 2023-05-11 15:21:34.000000 irails-1.3.2/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.2/irails/log.py
+-rw-rw-rw-   0        0        0     8673 2023-05-11 15:20:30.000000 irails-1.3.2/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.2/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.2/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.2/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.520004 irails-1.3.2/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.2/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7811 2023-05-11 15:34:41.000000 irails-1.3.2/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.3.2/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.3.2/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.2/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1556 2023-05-11 05:57:14.000000 irails-1.3.2/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.2/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     1855 2023-05-11 12:33:17.000000 irails-1.3.2/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.456208 irails-1.3.2/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.532982 irails-1.3.2/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.2/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.2/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.2/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.2/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.2/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.2/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.3.2/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.2/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.536958 irails-1.3.2/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.2/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.538954 irails-1.3.2/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.2/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.552917 irails-1.3.2/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.2/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.3.2/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.2/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.2/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.2/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.2/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.2/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.2/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.2/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.459208 irails-1.3.2/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.558899 irails-1.3.2/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.2/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.2/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.2/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      277 2023-05-11 11:03:51.000000 irails-1.3.2/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.561899 irails-1.3.2/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.2/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.2/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.565881 irails-1.3.2/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.462193 irails-1.3.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.569874 irails-1.3.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.573859 irails-1.3.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.463190 irails-1.3.2/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.575854 irails-1.3.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2677 2023-05-11 15:20:54.000000 irails-1.3.2/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:36:16.504043 irails-1.3.2/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-11 15:36:16.000000 irails-1.3.2/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2023-05-11 15:36:16.000000 irails-1.3.2/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:36:16.000000 irails-1.3.2/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-11 15:36:16.000000 irails-1.3.2/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-11 15:36:16.000000 irails-1.3.2/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 15:36:16.000000 irails-1.3.2/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:36:16.580842 irails-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.2/setup.py
```

### Comparing `irails-1.3.1/PKG-INFO` & `irails-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.1
+Version: 1.3.2
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
-Metadata-Version: 2.1 Name: irails Version: 1.3.1 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.3.2 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.3.1/README.md` & `irails-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/_i18n.py` & `irails-1.3.2/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/_loader.py` & `irails-1.3.2/irails/_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import importlib
 import sys,os
-from .config import config,ROOT_PATH,_log
+from .config import config,ROOT_PATH 
 from ._i18n import load_app_translations
 from gettext import gettext as _
 app_cfg=config.get('app')
 app_dirs = app_cfg.get("appdir")
 app_enabled = app_cfg.get("enabled")
 
 def __list_directories(dir):
@@ -27,41 +27,48 @@
 def load_module(module_name:str,module_path:str):
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(module_name, module_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         return module
     return None
-def _load_app(app_dir):
-    try:
-        _path = os.path.join(ROOT_PATH,app_dir.split(".")[0])
-        if _path not in sys.path:
-            sys.path.insert(-1,_path)
-        _log.info(_('Loading app:%s')%app_dir)
-        return importlib.import_module(app_dir)
-          
-    except ImportError as e:
-        _log.error(_("load app %s failed")%app_dir)
-        _log.error(e.args)
-        raise e
-    
+def _load_app(app_dir): 
+    from .log import _log
+    _modules = ['controllers','services','models']
+    cnt =  0
+    for m in _modules:
+        module_name = f"{app_dir}.{m}"
+        _log.info(_('Loading module:%s')%module_name)
+        try:
+            importlib.import_module(module_name) 
+            if m=='controllers':
+                cnt += 1
+        except ImportError as e:
+            if m=='controllers':
+                _log.error(_("load app %s failed")%app_dir)
+                _log.error(e.args)
+                cnt -= 1
+            else:
+                pass
+    return cnt
 def _load_apps(debug=False):
-    if ROOT_PATH not in sys.path:
-        sys.path.insert(-1,ROOT_PATH)
+    
     unloaded = 0
     loaded = 0
     for app_dir in app_dirs:
         app_list =  __list_directories(app_dir)
         for app in app_list:
             if __check_if_enabled(app):  
                 _dir = os.path.join(app_dir,app)
-                module = _load_app(f'{app_dir}.{app}')
-                if module:
-                    t =  load_app_translations(_dir)
-                    setattr(module,"_translation",t)
+                _abs_app_path = os.path.dirname(os.path.abspath(_dir))
+                if _abs_app_path not in sys.path:
+                    sys.path.insert(-1,_abs_app_path)
+                debug and print('load app:'+app)
+                n = _load_app(app)
+                if n:
                     loaded = loaded + 1
                 else:
                     unloaded = unloaded + 1
             else:
                 unloaded = unloaded + 1
```

### Comparing `irails-1.3.1/irails/_utils.py` & `irails-1.3.2/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/auth.py` & `irails-1.3.2/irails/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from starlette.authentication import AuthenticationBackend, AuthenticationError, SimpleUser, AuthCredentials,BaseUser
 from starlette.middleware.authentication import AuthenticationMiddleware
 from starlette.authentication import BaseUser,SimpleUser,UnauthenticatedUser
 from casbin.persist.adapters import FileAdapter
 from casbin.persist.adapter import Adapter
 # from .midware_casbin import CasbinMiddleware
  
-from .config import config,_log
+from .config import config
+from .log import _log
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Type, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
 
 AUTH_EXPIRED='[EXPIRED]!'
```

### Comparing `irails-1.3.1/irails/base_controller.py` & `irails-1.3.2/irails/base_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
  
+import re
 from fastapi import FastAPI,UploadFile,File,Header, Depends,HTTPException,Request,Response, status as StateCodes
 from fastapi.responses import RedirectResponse,HTMLResponse,PlainTextResponse
 from .view import _View
  
-from .config import config,ROOT_PATH,_log
+from .config import config,ROOT_PATH
+from .log import _log
 import os,uuid
 from hashlib import md5
 from typing import Dict
 from logging import Logger
 import inspect
 import datetime
 from irails._i18n import load_app_translations
@@ -37,21 +39,23 @@
     @property
     def _(self):
         m = getattr(self,'__appdir__').split(os.sep)
         if len(m)>2:
             m = os.sep.join(m[-2:])
         else:
             raise RuntimeError(f"load_app_translations:{m} is invalid app module") 
+        languages = ['zh']
         if 'lang' in self._session:
             languages = self._session['lang']
         else:
             language_header = self._request.headers.get('accept-language')
-            languages = language_header.split(',')
-            if languages:
-                languages = [languages[0]]
+            if language_header:
+                languages = language_header.split(',')
+                if languages:
+                    languages = [languages[0]]
         t = load_app_translations(module_dir=m,lan=languages)
         return t.gettext
     @property
     def log(self)->Logger:
         return _log
     @property 
     def cookies(self)->Dict[str,str]: 
@@ -159,15 +163,17 @@
         def get_path(caller_frame,view_path:str="",context:dict={},local2context:bool=True ):
             # caller_file = caller_frame.f_code.co_filename
             # caller_lineno = caller_frame.f_lineno
             caller_function_name = caller_frame.f_code.co_name
             caller_locals = caller_frame.f_locals
             caller_class = caller_locals.get("self", None).__class__
             caller_classname:str = caller_class.__name__
-            caller_classname = caller_classname.lower().rstrip('controller')
+            string = "TestController"
+            caller_classname = re.sub(r"Controller$", "", caller_classname).lower()
+             
             #caller_file = os.path.basename(caller.filename) 
             if local2context and not context:
                 del caller_locals['self']
                 context.update(caller_locals)
             if not view_path:
                 if self.__version__:
                     version_path = f"{self.__version__}/"
```

### Comparing `irails-1.3.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.2/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.2/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/cbv.py` & `irails-1.3.2/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/config.py` & `irails-1.3.2/irails/scripts/_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,231 +1,179 @@
-import os
-import sys
-import yaml
-import logging
-from hashlib import md5
-from typing import Dict
-import os.path
-import re
-
-
-def is_in_app(directory):
-    """
-    check exists controllers , views dir in :directory
-    """
-
-    controller_dir = os.path.join(directory, 'controllers')
-    views_dir = os.path.join(directory, 'views')
-    if not os.path.exists(controller_dir):
-        print(f"can't location `controller` dir")
-        return False
-    if not os.path.exists(views_dir):
-        print(f"can't location `views` dir")
-        return False
-    # initfile = os.path.join(controller_dir, '__init__.py')
-    # if not os.path.exists(initfile):
-    #     return False
-
-    return True
-
-
-def is_in_irails(directory):
-    """
-    check exists configs dir,   main.py and configs/general.yaml 
-    """
-
-    configs_dir = os.path.join(directory, 'configs')
-    # main_file = os.path.join(directory, 'main.py')
-
-    if not os.path.exists(configs_dir):  # or not os.path.exists(main_file):
-        return False
-    general_file = os.path.join(configs_dir, 'general.yaml')
-
-    if not os.path.exists(general_file):
-        return False
-
-    return True
-
-
-ROOT_PATH = os.path.realpath(os.curdir)
-
-IS_IN_irails = is_in_irails(ROOT_PATH)
-
-
-def is_cli_mode():
-    executeble = sys.argv[0]
-    executeble = os.path.basename(executeble)
-    # print(f"current executeble:" + executeble)
-    return (executeble.lower().startswith('irails'))
-
-
-def _extract_name(string):
-    match = re.search(r'{([^}]*)}', string)
-    if match:
-        return match.group(1)
-    else:
-        return None
-
-
-class YamlConfig:
-    _raw_config: Dict = {}
-
-    def __init__(self, filename: str = "", config: Dict = {}):
-        self.filename = filename
-        self.config = config
-        self.load()
-
-    def __getitem__(self, key: str):
-        return self.get(key)
-
-    def __setitem__(self, key: str, value):
-        self.set(key, value)
-
-    def reload(self) -> bool:
-        return self.load()
-
-    def load(self) -> bool:
-        if os.path.isfile(self.filename):
-            with open(self.filename, "r") as f:
-                self.config = yaml.safe_load(f)
-                YamlConfig._raw_config = self.config
-        elif os.path.isdir(self.filename):
-            self.config = self._merge_yaml_files(self.filename)
-            YamlConfig._raw_config = self.config
-        elif self.config:
+import argparse
+import sys,os,re
+from typing import Any
+from jinja2 import Template
+from irails._utils import is_valid_filename,get_controller_name,get_snaked_name
+from  irails.config import is_in_irails,is_in_app
+
+class Generator():
+    def __init__(self,args,dir) -> None:
+        self.args = args
+        self.dir = dir
+        pass
+    def gen_common(self):
+        '''#todo: check configs dir
+                  check data dir
+
+        '''
+        pass
+    def gen_tpl(self,tpl_file,dest,context={}, use_micro=True,dir_only=False):
+        tpl_dir = os.path.dirname(__file__)+"/tpls/app"
+        tpl_file = os.path.join(tpl_dir,tpl_file)
+        dest = os.path.normpath(dest)
+        if not os.path.exists(tpl_file):
+            raise Exception(f"{tpl_file} does not exists!")
+        if os.path.exists(dest):
+            print(f"{dest} is exists! skip..")
             return True
-        else:
-            if is_cli_mode():
-                pass
-            else:
-                raise Exception(f"{self.filename} is not a file or directory")
-            return False
+        dir = os.path.dirname(dest) 
+        os.makedirs(dir,exist_ok=True)
+        if not dir_only:
+            with open(tpl_file,'r') as f:
+                content = f.read()
+            dest_content = content
+            if use_micro:
+                template = Template(content)
+                dest_content = template.render(context)
+            
+            
+            with open(dest,'w') as f:
+                f.write(dest_content)
+            print(f"create {dest}")
         return True
-
-    def dump(self) -> str:
-        return yaml.safe_dump(self.config) if self.config else ""
-
-    def save(self) -> bool:
-        if not self.filename:
-            return False
-        with open(self.filename, "w") as f:
-            yaml.safe_dump(self.config, f)
+    def str_to_upper(self,name):
+        new_name = name.title().replace("_", "")
+        return new_name
+    def is_valid_class_name(self,name):
+        if not isinstance(name, str):
+            return False 
+        if not re.match(r'^[a-zA-Z_]', name):
+            return False 
+        if not re.match(r'^\w+$', name):
+            return False 
+        import keyword
+        if keyword.iskeyword(name):
+            return False 
         return True
-
-    def get(self, key: str, default=None):
-        value = self.config.get(key, default)
-        if isinstance(value, str):
-            value = self._resolve_value(value, key)
-        elif isinstance(value, dict):
-            value = YamlConfig(filename="", config=value)
-        return value
-
-    def set(self, key: str, value):
-        self.config[key] = value
-
-    def delete(self, key: str):
-        del self.config[key]
-
-    def _merge_dicts(self, dict1: Dict, dict2: Dict) -> Dict:
-        for key in dict2:
-            if key in dict1 and isinstance(dict1[key], dict) and isinstance(dict2[key], dict):
-                dict1[key] = self._merge_dicts(dict1[key], dict2[key])
-            else:
-                dict1[key] = dict2[key]
-        return dict1
-
-    def _merge_yaml_files(self, dir_path: str) -> Dict:
-        merged_config = {}
-        for file_name in os.listdir(dir_path):
-            file_path = os.path.join(dir_path, file_name)
-            if os.path.isfile(file_path) and file_name.endswith(".yaml"):
-                file_config = self._load_yaml_file(file_path)
-                if isinstance(file_config, dict):
-                    merged_config = self._merge_dicts(
-                        merged_config, file_config)
-            elif os.path.isdir(file_path):
-                dir_config = self._merge_yaml_files(file_path)
-                merged_config = self._merge_dicts(merged_config, dir_config)
-        return merged_config
-
-    def _load_yaml_file(self, file_path: str) -> Dict:
-        with open(file_path, "r") as f:
-            return yaml.safe_load(f)
-
-    def _resolve_value(self, value: str, key: str) -> str:
-        while "{" in value and "}" in value:
-            name = _extract_name(value)
-            if not name:
-                break
-            if name == key:
-                raise RuntimeError(
-                    f"Configure file error: circular reference `{name}`")
-            if "." in name:
-                segment_name, sub_key = name.split(".", 1)
-                if segment_name == "ROOT":
-                    # value = value.replace("{" + name + "}", self.config.get(sub_key, ""))
-                    value = value.replace(
-                        "{" + name + "}", YamlConfig(config=self._raw_config).get(sub_key, ""))
+    def ensure_line(self,filepath, line_to_add):
+        found = False
+        lines = []
+        if os.path.exists(filepath):
+            # Read in the file
+            with open(filepath, 'r') as file:
+                lines = file.readlines()
+
+                # Check if the line is already in the file
+                for line in lines:
+                    if line.strip() == line_to_add.strip():
+                        found = True
+                        break
+        else:
+            with open(filepath,'w') as file:
+                file.write(line_to_add)
+            return True              
+        # If the line is not in the file, add it
+        if not found:
+            lines.append('\n' + line_to_add.strip() + '\n')
+            with open(filepath, 'w') as file:
+                file.writelines(lines)
+
+    def __call__(self) -> Any:
+         
+        if not self.args.name:
+            print(f'controller name is empty,exit!')
+            exit()
+        name = self.args.name.pop(0)
+        if name:
+            if not is_valid_filename(name) :
+                print(f'{name} is not avalided!')
+                exit() 
+
+            store_dir = self.dir
+            controller_name:str = name
+            controler_path_name = get_snaked_name(controller_name)
+            # store_dir = os.path.join(store_dir,controler_path_name )
+            
+            # controller_name = self.str_to_upper(name)
+            if not self.is_valid_class_name(controller_name):
+                print(f"{controller_name} is a not valided class name,exit...")
+                exit() 
+            
+            dirs_items =  {
+                'controllers':{'tpl':'controller.tpl','dest':f'controllers/{controler_path_name}_controller.py','micro':True} , 
+                'models': {'tpl':'model.tpl','dest' : f'models/{controler_path_name}_model.py','micro':True},
+                'services':{'tpl':'service.tpl','dest': f'services/{controler_path_name}_service.py','micro':True },
+                'views': [
+                    {'tpl' : 'view.tpl','dest': f'views/{controler_path_name}/index.html','micro':False},
+                    {'tpl' : 'css.tpl','dest': f'views/{controler_path_name}/index.css','micro':False}
+                    ] ,
+                
+                'tests': {'tpl':'test.tpl','dest': f'tests/test_{controler_path_name}.py','micro':True}
+            }
+            context = {'ctrl_name':controller_name.title(),'ctrl_path':controler_path_name}
+            for dir in dirs_items:
+                _current_dir = store_dir#os.path.join(store_dir,dir)
+                os.makedirs(_current_dir,exist_ok=True)
+                items = dirs_items[dir]
+                if isinstance(items,list):
+                    _item = items
                 else:
-                    segment_config = self.config.get(segment_name, {})
-                    if isinstance(segment_config, dict):
-                        sub_keys = sub_key.split(".")
-                        sub_value = segment_config
-                        for sub_key in sub_keys:
-                            sub_value = sub_value.get(sub_key, {})
-                        value = value.replace("{" + name + "}", str(sub_value))
-            else:
-                value = value.replace(
-                    "{" + name + "}", self.config.get(name, ""))
-        return value
-
-
-config = YamlConfig(os.path.join(ROOT_PATH, "configs"))
-
-debug = False
-
-
-def set_logger(logger: logging.Logger):
-    log_config = config.get("log")
-    if not log_config:
-        return logger
-    __log_level = log_config.get('level', 'DEBUG')
-    __log_file = log_config.get('file',None)
-
-    debug = config.get("debug", False)
-    logger.name = logger.name or log_config.get("name", 'iRails')
-    if __log_file:
-        __log_file = os.path.abspath(__log_file)
-
-    log_format = log_config.get(
-        "msgfmt", "%(asctime)s %(name)s:%(levelname)s:%(message)s")
-    datefmt = log_config.get("datefmt", "%Y-%M-%d %H:%M:%S")
-    file_handler = None
-    if __log_file:
-        if debug:
-            try:
-                os.remove(__log_file)
-            except:
-                pass
-
-        file_handler = logging.FileHandler(__log_file, mode='a')
-        logger.addHandler(file_handler)
-     
-    
-    handler = logging.StreamHandler(sys.stdout)
-    handler.setLevel(logging._nameToLevel[__log_level])
-    handler.setFormatter(logging.Formatter(fmt=log_format, datefmt=datefmt))
-    logger.addHandler(handler)
-     
- 
-
-
-def __init_log():
-    __logCfg = config.get("log")
-    logger = logging.getLogger((__logCfg and __logCfg.get('name', 'IRAILS')) or 'iRails')
-    set_logger(logger)
-    return logger
+                    _item = [items]
+                for item in _item:
+                    tpl = item['tpl']
+                    dest = os.path.join(_current_dir , item['dest'])
+                    micro = item['micro']
+                    #controller file will generate last time
+                    self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=dir=='controllers') 
+            controller_file = os.path.join(_current_dir,'controllers',f"{controler_path_name}_controller.py")
+            __init_file = os.path.join(_current_dir,'controllers','__init__.py')
+            self.ensure_line(__init_file,f"from . import {controler_path_name}_controller")
+            __init_file = os.path.join(_current_dir,'models','__init__.py')
+            self.ensure_line(__init_file,f"from . import {controler_path_name}_model")
+            __init_file = os.path.join(_current_dir,'services','__init__.py')
+            self.ensure_line(__init_file,f"from . import {controler_path_name}_service")
+            acts = []
+            actions = self.args.name
+            if len(actions)==0:actions.append('index')
+            for action in actions:
+                acts.append(f"""
+    @api.get('/{action}')
+    def {action}(self):
+        return self.view()                
+""")
+                _view_file = os.path.join(_current_dir,'views',controler_path_name,f"{action}.html")
+                if not os.path.exists(_view_file):
+                    with open(_view_file,'w') as f:
+                        f.write(f"{controller_name}.{action} view file.in:{_view_file}")
+                    print(f'create {_view_file}')
+                else:
+                    print(f'{_view_file} was exists,skip generate')
+            actions = "\n".join(acts)
+            context['actions'] = actions    
+            self.gen_tpl(tpl_file=dirs_items['controllers']['tpl'],dest=controller_file,context=context,use_micro=True,dir_only=False) 
 
+        print("Done!")
+    pass
 
 
-_log = __init_log()
- 
+def main():
+     
+    cur_dir = os.path.abspath(os.curdir)
+    root_path = os.path.abspath(os.path.join(cur_dir,"../.."))
+    if os.path.exists(root_path) and  os.path.isdir(root_path): 
+        if not is_in_irails(root_path) or not is_in_app(cur_dir):
+            print(f"Please exec in irails project's app dir ,like `apps/app`")
+            exit()
+    self_file = __file__.lstrip("_").replace(".py",'')
+    parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [--name] `controller [action ...]` ...", description='create new controller')
+    parser.add_argument('--name',help="controller name to create")
+    parser.add_argument('args', nargs=argparse.REMAINDER)
+     
+    args = parser.parse_args()
+    if not any(args.__dict__.values()):
+        parser.print_help()
+    if not args.name:
+        args.name = args.args
+    else:
+        args.name = [args.name]
+    _gen = Generator(args,cur_dir)
+    _gen()
```

### Comparing `irails-1.3.1/irails/controller_utils.py` & `irails-1.3.2/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/core.py` & `irails-1.3.2/irails/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 from fastapi.params import Depends
 from fastapi.utils import generate_unique_id
 from starlette.responses import JSONResponse, Response
 from starlette.routing import BaseRoute
 from fastapi.types import DecoratedCallable
 from .mvc_router import create_controller,MvcRouter as api,   register_controllers_to_app 
 from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
-from .config import config,ROOT_PATH,_log,set_logger
+from .config import config,ROOT_PATH,_project_name
+from .log import _log,set_logger
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
+from ._loader import _load_apps
 from ._utils import get_controller_name,get_snaked_name
 from ._i18n import load_app_translations
 _=None
 __is_debug=config.get('debug',False)
 
 def __load_core_i18n():
     _dir = os.path.dirname(__file__)
@@ -88,25 +90,25 @@
     @property
     def public_auth_url(self):
         """public user auth url"""
         return self.__public_auth_url
     @public_auth_url.setter
     def public_auth_url(self,url):
         if self.__public_auth_url:
-            raise RuntimeError(_("public_auth_url only can be setting once time,current is:%s") % self.__public_auth_url)
+            _log.warning(_("public_auth_url only can be setting once time,current is:%s") % self.__public_auth_url)
         self.__public_auth_url = url
         
     @property
     def user_auth_url(self):
         """internal user auth url"""
         return self.__user_auth_url
     @user_auth_url.setter
     def user_auth_url(self,url):
         if self.__user_auth_url:
-            raise RuntimeError(_("user_auth_url only can be setting once time,current is:%s") % self.__user_auth_url)
+            _log.warning(_("user_auth_url only can be setting once time,current is:%s") % self.__user_auth_url)
         self.__user_auth_url = url
     @property
     def modify_authorization(self):
         return self.__authObj.casbin_auth.modify_authorization
     @property
     def authObj(self)->auth.AuthenticationBackend_:
         return self.__authObj
@@ -117,15 +119,16 @@
      
     @property 
     def data_engine(self)->database.Engine:
         return self._data_engine
     @data_engine.setter
     def data_engine(self,value):
         self._data_engine = value
-
+    def __repr__(self):
+        return f'<IRails:{self.title}>'
 __app = MvcApp( ) 
 
 __all_controller__ = {}
 
 application = __app
 api.init(application)
 
@@ -359,18 +362,21 @@
         alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
         uri = db_cfg.get("uri")
         if uri:
             database.check_migration(application.data_engine,uri,alembic_ini)
     except Exception as e:
         _log.disabled = False
         _log.error(e.args)
-def generate_mvc_app( ):
+def generate_mvc_app():
     global __is_debug
-    set_logger(_log)
-    from ._loader import _load_apps
+     
+    application.title = _project_name
+    
+    
+    
     
     _log.info(_("\n\init mvc app..."))
     loaded,unloaded=_load_apps(debug=__is_debug) 
     _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %(loaded,unloaded))  
     if not len(__all_controller__)>0:
         raise RuntimeError(_("not found any controller class"))
```

### Comparing `irails-1.3.1/irails/database.py` & `irails-1.3.2/irails/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,39 @@
 from ._utils import camelize_classname,pluralize_collection
  
 from alembic import command
 from alembic.config import Config
 import configparser
 import re,os
 from typing import Union
-from .config import _log
+from .log import _log
 DataMap = None
 mapped_base = None
 engine:Engine=None 
 class Base(DeclarativeBase):
     pass
 
  
 
 class Service():
     __all_generated = {}
+    engine:Engine = engine
     
     @classmethod
     @contextmanager 
     def get_session(cls):
         """Provide a transactional scope around a series of operations."""
+        if not cls.engine:
+            yield None
+            return
         if hasattr(cls,'_session_local'):
             session_local = getattr(cls,'_session_local')
         else:
             session_local =  sessionmaker(bind=engine)
-            setattr(cls,"_session_local", session_local)
+            setattr(cls,"_session_local", session_local) #cache sessionmaker object
         session = session_local()
         try:
             yield session
             session.commit()
         except Exception as e:
             session.rollback()
             raise e
```

### Comparing `irails-1.3.1/irails/midware.py` & `irails-1.3.2/irails/midware.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     request_validation_exception_handler,
 )
 from fastapi.exceptions import RequestValidationError
 from starlette.exceptions import HTTPException as StarletteHTTPException
 import traceback
 
 from starlette.staticfiles import PathLike
-from .config import _log,config
+from .config import config
+from .log import _log
 from .midware_session import (SessionMiddleware,FileStorage,MemoryStorage,RedisStorage,SessionStorage,_SESSION_STORAGES)
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.types import   Scope 
 from .view import _View,env_configs,static_format
 from .config import config,ROOT_PATH
 
 from fastapi.middleware import Middleware
```

### Comparing `irails-1.3.1/irails/midware_casbin.py` & `irails-1.3.2/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/midware_session.py` & `irails-1.3.2/irails/midware_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import itsdangerous
 from itsdangerous.exc import BadSignature
 
 from starlette.datastructures import MutableHeaders, Secret
 from starlette.requests import HTTPConnection
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
-from .config import _log
+from .log import _log
 from .base_controller import _session_key
 if sys.version_info >= (3, 8):  # pragma: no cover
     from typing import Literal
 else:  # pragma: no cover
     from typing_extensions import Literal
 from ._utils import iJSONEncoder,is_datetime_format
```

### Comparing `irails-1.3.1/irails/mvc_router.py` & `irails-1.3.2/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/_app.py` & `irails-1.3.2/irails/scripts/_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,19 +161,19 @@
                 'tests'
             ]
             context = {'app':app_name}
             for dir in dirs_items:
                 _current_dir = os.path.join(store_dir,dir)
                 os.makedirs(_current_dir,exist_ok=True)
                  
-            _init_file = os.path.normpath(os.path.join(store_dir,'__init__.py'))
-            with open(_init_file,'w') as f: #root path of app's dir
-                f.write(f"from .controllers import *")
+            # _init_file = os.path.normpath(os.path.join(store_dir,'__init__.py'))
+            # with open(_init_file,'w') as f: #root path of app's dir
+            #     f.write(f"from .controllers import *")
             
-            print(f"create {_init_file}")
+            # print(f"create {_init_file}")
 
             self.add_enabled_to_app(app_name)
             if self.set_root_controller_to_config(self.args.dir,app_name):
                 self.add_home_controller(self.args.dir,app_name)
                 self.add_home_view(self.args.dir,app_name)
             cnt += 1
         if cnt:
```

### Comparing `irails-1.3.1/irails/scripts/_i18n.py` & `irails-1.3.2/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/_project.py` & `irails-1.3.2/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/_run.py` & `irails-1.3.2/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/_shell.py` & `irails-1.3.2/irails/scripts/_shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 from functools import update_wrapper
 import os
 import sys
+from typing import Dict
 import click
 import irails
+from fastapi.testclient import TestClient
 
- 
+setattr(irails.application,'__name__',"irails.application.shell")
+from irails.database import Service
+
+def create_context()->Dict:
+    ctx = {}
+    test_client = TestClient(app = irails.application )
+  
+    ctx.update({'app':irails.application,
+                'service':Service,
+                'client':test_client})
+
+    return ctx
 def shell_command() -> None:
     """Run an interactive Python shell in the context of a given
     irails application.  The application will populate the default
     namespace of this shell according to its configuration.
 
     This is useful for executing small snippets of management code
     without having to manually configure the application.
     """
     import code
-
+     
+    irails.generate_mvc_app()
     banner = (
-        f"Python {sys.version} on {sys.platform}\n"
-        f"IRails: {irails.__version__}\n"
-        f"Instance: {irails.application}"
+        f"Python {sys.version} on {sys.platform}\n" 
+        f"Env: IRails {irails.__version__} on {irails.application.title}"
     )
-    ctx: dict = {}
-
+     
+    ctx = create_context()
     # Support the regular Python interpreter startup script if someone
     # is using it.
     startup = os.environ.get("PYTHONSTARTUP")
     if startup and os.path.isfile(startup):
         with open(startup) as f:
             eval(compile(f.read(), startup, "exec"), ctx)
-    irails.generate_mvc_app()
-    ctx.update({'application':irails.application})
 
+    
+    
     # Site, customize, or startup script can set a hook to call when
     # entering interactive mode. The default one sets up readline with
     # tab and history completion.
     interactive_hook = getattr(sys, "__interactivehook__", None)
 
     if interactive_hook is not None:
         try:
```

### Comparing `irails-1.3.1/irails/scripts/main.py` & `irails-1.3.2/irails/scripts/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import os
 import re
 def _ensure_cli():
     executable = os.path.basename(sys.argv[0])
     if not executable.startswith('irails'):
         sys.argv[0] = 'irails'
 _ensure_cli()
+
+sys.path.insert(-1,os.path.abspath(os.curdir))
 from irails import __version__
 def collect_features():
     """
     return files in current dir start with '_' no sub dir
     """
     
     dir_path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `irails-1.3.1/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.2/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/app/home.tpl` & `irails-1.3.2/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.2/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.2/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.2/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.2/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.2/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.2/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/irails/view.py` & `irails-1.3.2/irails/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Any, Mapping
 from fastapi import BackgroundTasks, Request,Response
 from fastapi.templating import Jinja2Templates
 from fastapi.exceptions import HTTPException
 import jinja2
  
-from .config import ROOT_PATH,config,_log
-
+from .config import ROOT_PATH,config 
+from .log import _log
 env_configs = {} 
 static_format = []
 def __get_view_configure():
     global static_format,env_configs
     env_options = config.get("view")# {'variable_start_string':'${','variable_end_string':'}'}
     if env_options:
         static_format = env_options.get('static_format',[])
```

### Comparing `irails-1.3.1/irails.egg-info/PKG-INFO` & `irails-1.3.2/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.1
+Version: 1.3.2
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
-Metadata-Version: 2.1 Name: irails Version: 1.3.1 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.3.2 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.3.1/irails.egg-info/SOURCES.txt` & `irails-1.3.2/irails.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 irails/auth.py
 irails/base_controller.py
 irails/cbv.py
 irails/config.py
 irails/controller_utils.py
 irails/core.py
 irails/database.py
+irails/log.py
 irails/midware.py
 irails/midware_casbin.py
 irails/midware_session.py
 irails/mvc_router.py
 irails/view.py
 irails.egg-info/PKG-INFO
 irails.egg-info/SOURCES.txt
```

### Comparing `irails-1.3.1/irails.egg-info/requires.txt` & `irails-1.3.2/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.1/setup.py` & `irails-1.3.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/irails-1.2.6.tar.gz` & `tmp/irails-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.2.6.tar", last modified: Wed May 10 11:40:37 2023, max compression
+gzip compressed data, was "irails-1.2.7.tar", last modified: Thu May 11 05:35:44 2023, max compression
```

## Comparing `irails-1.2.6.tar` & `irails-1.2.7.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.949333 irails-1.2.6/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5079 2023-05-10 11:40:37.948292 irails-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.872271 irails-1.2.6/irails/
--rw-rw-rw-   0        0        0      331 2023-05-10 11:40:23.000000 irails-1.2.6/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.6/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.6/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.6/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.6/irails/auth.py
--rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.6/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.884238 irails-1.2.6/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.885237 irails-1.2.6/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.6/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.6/irails/cbv.py
--rw-rw-rw-   0        0        0     7328 2023-05-10 11:08:55.000000 irails-1.2.6/irails/config.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.6/irails/controller_utils.py
--rw-rw-rw-   0        0        0    32113 2023-05-10 07:54:46.000000 irails-1.2.6/irails/core.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.6/irails/database.py
--rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.6/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.6/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.6/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.6/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.894212 irails-1.2.6/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.6/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.6/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.6/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.6/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.6/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1423 2023-05-10 10:55:35.000000 irails-1.2.6/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.6/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.840045 irails-1.2.6/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.902190 irails-1.2.6/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.6/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.6/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.6/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.6/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.6/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.6/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.6/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.6/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.905186 irails-1.2.6/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.6/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.907178 irails-1.2.6/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.6/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.922138 irails-1.2.6/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.6/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.6/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.6/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.6/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.6/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.2.6/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      656 2023-05-10 11:09:34.000000 irails-1.2.6/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.6/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.6/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.844036 irails-1.2.6/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.929119 irails-1.2.6/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.2.6/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.2.6/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.2.6/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.2.6/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.931994 irails-1.2.6/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.6/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.6/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.934131 irails-1.2.6/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.847030 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.938123 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.944130 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.848024 irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.946102 irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.6/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.881247 irails-1.2.6/irails.egg-info/
--rw-rw-rw-   0        0        0     5079 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2287 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      766 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 11:40:37.949333 irails-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.425657 irails-1.2.7/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-11 05:35:44.425657 irails-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.367846 irails-1.2.7/irails/
+-rw-rw-rw-   0        0        0      331 2023-05-11 05:35:30.000000 irails-1.2.7/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.7/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.7/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.7/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.7/irails/auth.py
+-rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.7/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.374793 irails-1.2.7/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.375791 irails-1.2.7/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.7/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.7/irails/cbv.py
+-rw-rw-rw-   0        0        0     7245 2023-05-11 05:30:32.000000 irails-1.2.7/irails/config.py
+-rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.2.7/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32135 2023-05-11 04:55:40.000000 irails-1.2.7/irails/core.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.7/irails/database.py
+-rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.7/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.7/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.7/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.7/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.384779 irails-1.2.7/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.7/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.7/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.7/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.2.7/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.7/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1423 2023-05-10 10:55:35.000000 irails-1.2.7/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1908 2023-05-11 05:08:52.000000 irails-1.2.7/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.7/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.340880 irails-1.2.7/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.392746 irails-1.2.7/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.7/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.7/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.7/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.7/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.7/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.7/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.7/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.7/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.394741 irails-1.2.7/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.7/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.395738 irails-1.2.7/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.7/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.406709 irails-1.2.7/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.7/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.7/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.7/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.7/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.7/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.2.7/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.2.7/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.7/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.7/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.342874 irails-1.2.7/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.409701 irails-1.2.7/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.2.7/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.2.7/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.2.7/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.2.7/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.411695 irails-1.2.7/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.7/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.7/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.414687 irails-1.2.7/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.345868 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.418676 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.421667 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.345868 irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.423663 irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.7/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:35:44.373793 irails-1.2.7/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2312 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 05:35:44.000000 irails-1.2.7/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:35:44.426655 irails-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.7/setup.py
```

### Comparing `irails-1.2.6/PKG-INFO` & `irails-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.6
+Version: 1.2.7
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
-Metadata-Version: 2.1 Name: irails Version: 1.2.6 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.7 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.6/README.md` & `irails-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/_i18n.py` & `irails-1.2.7/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/_loader.py` & `irails-1.2.7/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/_utils.py` & `irails-1.2.7/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/auth.py` & `irails-1.2.7/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/base_controller.py` & `irails-1.2.7/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.2.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.2.7/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/cbv.py` & `irails-1.2.7/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/config.py` & `irails-1.2.7/irails/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,92 @@
-import os,sys
+import os
+import sys
 import yaml
 import logging
 from hashlib import md5
 from typing import Dict
 import os.path
 import re
+
+
 def is_in_app(directory):
     """
     check exists controllers , views dir in :directory
     """
-    
+
     controller_dir = os.path.join(directory, 'controllers')
-    views_dir = os.path.join(directory, 'views')  
+    views_dir = os.path.join(directory, 'views')
     if not os.path.exists(controller_dir):
         print(f"can't location `controller` dir")
-        return False  
-    if  not os.path.exists(views_dir) :
+        return False
+    if not os.path.exists(views_dir):
         print(f"can't location `views` dir")
         return False
-    # initfile = os.path.join(controller_dir, '__init__.py') 
+    # initfile = os.path.join(controller_dir, '__init__.py')
     # if not os.path.exists(initfile):
     #     return False
-    
+
     return True
+
+
 def is_in_irails(directory):
     """
     check exists configs dir,   main.py and configs/general.yaml 
     """
-    
+
     configs_dir = os.path.join(directory, 'configs')
     # main_file = os.path.join(directory, 'main.py')
 
-    if not os.path.exists(configs_dir) :#or not os.path.exists(main_file):
-        return False  
+    if not os.path.exists(configs_dir):  # or not os.path.exists(main_file):
+        return False
     general_file = os.path.join(configs_dir, 'general.yaml')
 
     if not os.path.exists(general_file):
         return False
-    
+
     return True
+
+
 ROOT_PATH = os.path.realpath(os.curdir)
- 
+
 IS_IN_irails = is_in_irails(ROOT_PATH)
+
+
 def is_cli_mode():
     executeble = sys.argv[0]
     executeble = os.path.basename(executeble)
     # print(f"current executeble:" + executeble)
     return (executeble.lower().startswith('irails'))
 
+
 def _extract_name(string):
     match = re.search(r'{([^}]*)}', string)
     if match:
         return match.group(1)
     else:
         return None
 
- 
+
 class YamlConfig:
     _raw_config: Dict = {}
+
     def __init__(self, filename: str = "", config: Dict = {}):
         self.filename = filename
         self.config = config
         self.load()
+
     def __getitem__(self, key: str):
         return self.get(key)
+
     def __setitem__(self, key: str, value):
-       self.set(key, value)
+        self.set(key, value)
+
     def reload(self) -> bool:
         return self.load()
+
     def load(self) -> bool:
         if os.path.isfile(self.filename):
             with open(self.filename, "r") as f:
                 self.config = yaml.safe_load(f)
                 YamlConfig._raw_config = self.config
         elif os.path.isdir(self.filename):
             self.config = self._merge_yaml_files(self.filename)
@@ -81,125 +96,134 @@
         else:
             if is_cli_mode():
                 pass
             else:
                 raise Exception(f"{self.filename} is not a file or directory")
             return False
         return True
+
     def dump(self) -> str:
         return yaml.safe_dump(self.config) if self.config else ""
+
     def save(self) -> bool:
         if not self.filename:
             return False
         with open(self.filename, "w") as f:
             yaml.safe_dump(self.config, f)
         return True
+
     def get(self, key: str, default=None):
         value = self.config.get(key, default)
         if isinstance(value, str):
             value = self._resolve_value(value, key)
         elif isinstance(value, dict):
             value = YamlConfig(filename="", config=value)
         return value
+
     def set(self, key: str, value):
         self.config[key] = value
+
     def delete(self, key: str):
         del self.config[key]
+
     def _merge_dicts(self, dict1: Dict, dict2: Dict) -> Dict:
         for key in dict2:
             if key in dict1 and isinstance(dict1[key], dict) and isinstance(dict2[key], dict):
                 dict1[key] = self._merge_dicts(dict1[key], dict2[key])
             else:
                 dict1[key] = dict2[key]
         return dict1
+
     def _merge_yaml_files(self, dir_path: str) -> Dict:
         merged_config = {}
         for file_name in os.listdir(dir_path):
             file_path = os.path.join(dir_path, file_name)
             if os.path.isfile(file_path) and file_name.endswith(".yaml"):
                 file_config = self._load_yaml_file(file_path)
                 if isinstance(file_config, dict):
-                    merged_config = self._merge_dicts(merged_config, file_config)
+                    merged_config = self._merge_dicts(
+                        merged_config, file_config)
             elif os.path.isdir(file_path):
                 dir_config = self._merge_yaml_files(file_path)
                 merged_config = self._merge_dicts(merged_config, dir_config)
         return merged_config
+
     def _load_yaml_file(self, file_path: str) -> Dict:
         with open(file_path, "r") as f:
             return yaml.safe_load(f)
+
     def _resolve_value(self, value: str, key: str) -> str:
         while "{" in value and "}" in value:
             name = _extract_name(value)
             if not name:
                 break
             if name == key:
-                raise RuntimeError(f"Configure file error: circular reference `{name}`")
+                raise RuntimeError(
+                    f"Configure file error: circular reference `{name}`")
             if "." in name:
                 segment_name, sub_key = name.split(".", 1)
                 if segment_name == "ROOT":
                     # value = value.replace("{" + name + "}", self.config.get(sub_key, ""))
-                    value = value.replace("{" + name + "}", YamlConfig(config=self._raw_config).get(sub_key, ""))
+                    value = value.replace(
+                        "{" + name + "}", YamlConfig(config=self._raw_config).get(sub_key, ""))
                 else:
                     segment_config = self.config.get(segment_name, {})
                     if isinstance(segment_config, dict):
                         sub_keys = sub_key.split(".")
                         sub_value = segment_config
                         for sub_key in sub_keys:
                             sub_value = sub_value.get(sub_key, {})
                         value = value.replace("{" + name + "}", str(sub_value))
             else:
-                value = value.replace("{" + name + "}", self.config.get(name, ""))
+                value = value.replace(
+                    "{" + name + "}", self.config.get(name, ""))
         return value
-config = YamlConfig(os.path.join(ROOT_PATH,"configs") )
+
+
+config = YamlConfig(os.path.join(ROOT_PATH, "configs"))
 
 debug = False
-def set_logger(logger:logging.Logger):
-    __logCfg = config.get("log")
-    __log_level = __logCfg['level'] or 'DEBUG'
-    __log_file = __logCfg['file'] or None 
-    debug = config.get("debug",False)   
-    logger.name = __logCfg.get("name",'iRails')
+
+
+def set_logger(logger: logging.Logger):
+    log_config = config.get("log")
+    __log_level = log_config.get('level', 'DEBUG')
+    __log_file = log_config.get('file',None)
+
+    debug = config.get("debug", False)
+    logger.name = logger.name or log_config.get("name", 'iRails')
     if __log_file:
         __log_file = os.path.abspath(__log_file)
-    log_format="%(asctime)s %(name)s:%(levelname)s:%(message)s"
-    datefmt="%Y-%M-%d %H:%M:%S" 
+
+    log_format = log_config.get(
+        "msgfmt", "%(asctime)s %(name)s:%(levelname)s:%(message)s")
+    datefmt = log_config.get("datefmt", "%Y-%M-%d %H:%M:%S")
+    file_handler = None
     if __log_file:
         if debug:
             try:
                 os.remove(__log_file)
             except:
                 pass
-            import io
-            
-        handler = logging.FileHandler(__log_file,mode='a')
-        
-    else:
-        import sys
-        handler = logging.StreamHandler(sys.stdout)  
-    handler.setLevel(logging._nameToLevel[__log_level]) 
-    handler.setFormatter(logging.Formatter(fmt= log_format,datefmt=datefmt)) 
-    logger.addHandler(handler)
+
+        file_handler = logging.FileHandler(__log_file, mode='a')
+        logger.addHandler(file_handler)
+     
     
-    logger.setLevel(logging._nameToLevel[__log_level]) 
+    handler = logging.StreamHandler(sys.stdout)
+    handler.setLevel(logging._nameToLevel[__log_level])
+    handler.setFormatter(logging.Formatter(fmt=log_format, datefmt=datefmt))
+    logger.addHandler(handler)
+     
+ 
 
-def __init_log( ):
+
+def __init_log():
     __logCfg = config.get("log")
-    logger = logging.getLogger(__logCfg.get('name','IRAILS'))
-    # from fastapi.logger import logger
+    logger = logging.getLogger(__logCfg.get('name', 'IRAILS'))
     set_logger(logger)
     return logger
-     
 
 
 
-#test:
-# dbcfg = config.get('database')
-# uri = dbcfg.get("uri")
-# assert uri
-# errors = config.get("errors")
-# p404 = errors.get("error_404_page")
-# assert p404
-
 _log = __init_log()
-if _log:
-    _log.setLevel(logging.DEBUG)
-
+
```

### Comparing `irails-1.2.6/irails/controller_utils.py` & `irails-1.2.7/irails/controller_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,16 +316,16 @@
                 _constructor = getattr(cls,'_constructor_')
                 await _constructor(cls,request = kwargs['request'],response=kwargs['response'])
 
             if 'request' in kwargs and not has_request:  
                 del kwargs['request']  
             if 'response' in kwargs and not has_response:  
                 del kwargs['response']  
-            del kwargs["__has_request__"]
-            del kwargs["__has_response__"]
+            if '__has_request__' in kwargs:del kwargs["__has_request__"]  
+            if '__has_response__' in kwargs:del kwargs["__has_response__"]
             if inspect.iscoroutinefunction(func):
                 result = await func(*args, **kwargs)
             else:
                 result =  func(*args,**kwargs)
             if isinstance(result,tuple):result = result[0]
             if response and isinstance(result,Response): 
                 result.raw_headers.extend(response.raw_headers)
```

### Comparing `irails-1.2.6/irails/core.py` & `irails-1.2.7/irails/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,15 +341,15 @@
             doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
             if hasattr(r,'methods'):
                 methods = r.methods
             else:
                 methods = r.name
             if __is_debug:  
                 _log.info((str(methods),r.path,funcname) )
-            application.routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type}
+            application.routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type,"endpoint":r.endpoint}
       
     _log.info(_("static files mouting..."))
     midware.init(app=application,debug=__is_debug)
 
 def check_db_migrate():
     db_cfg = config.get("database")
     if __is_debug and db_cfg:
```

### Comparing `irails-1.2.6/irails/database.py` & `irails-1.2.7/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/midware.py` & `irails-1.2.7/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/midware_casbin.py` & `irails-1.2.7/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/midware_session.py` & `irails-1.2.7/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/mvc_router.py` & `irails-1.2.7/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/_app.py` & `irails-1.2.7/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/_controller.py` & `irails-1.2.7/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/_i18n.py` & `irails-1.2.7/irails/scripts/_i18n.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys,os,importlib
-
+from irails import __version__
 from irails.config import is_in_app, is_in_irails,YamlConfig
 cur_dir = os.path.abspath(os.curdir)
 root_path = os.path.abspath(os.path.join(cur_dir,"../.."))
 config = YamlConfig(os.path.join(root_path,"configs"))
 locales_path = os.path.abspath('locales') 
 
 import glob
@@ -102,15 +102,15 @@
 "Language-Team: \\n"
 "Language: {lang}\\n"
 "MIME-Version: 1.0\\n"
 "Content-Type: text/plain; charset=UTF-8\\n"
 "Content-Transfer-Encoding: 8bit\\n"
 "Plural-Forms: nplurals=1; plural=0;\\n"
 "Generated-By: pygettext.py 1.5\\n"
-"X-Generator: Poedit 3.2.2\\n"
+"X-Generator: irails i18n {version}\\n"
 """
 def split_pot(content:str):
     lines = content.split("\n")
     l = -1
     for line in lines:
         l+=1
         if line.startswith('"Generated-By'):
@@ -152,17 +152,17 @@
     import datetime
     d1 = datetime.datetime.now().strftime('%Y-%m-%d %H:%M%z')
     year = datetime.datetime.now().strftime('%Y')
      
      
     d2 = d1
     for lang in nelangs:
-        if len(lang)!=5:
+        if len(lang)!=5: #ensure like zh-CN ,en-US
             continue
-        header = po_header.replace("{d1}",d1).replace("{d2}",d2).replace("{lang}",lang).replace("{YEAR}",year)
+        header = po_header.replace("{d1}",d1).replace("{d2}",d2).replace("{lang}",lang).replace("{YEAR}",year).replace("{version}",__version__)
         path = os.path.join(locales_path,f"{lang}.po")
         with open(path,'w') as f:
             f.write(header+"\n"+_pot_content)
             
             print(f"generated {path}")
         #gen html files
```

### Comparing `irails-1.2.6/irails/scripts/_project.py` & `irails-1.2.7/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/_run.py` & `irails-1.2.7/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/main.py` & `irails-1.2.7/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/app/home.css.tpl` & `irails-1.2.7/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/app/home.tpl` & `irails-1.2.7/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.2.7/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.2.7/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.2.7/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/public/error_404.html` & `irails-1.2.7/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/public/error_500.html` & `irails-1.2.7/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.2.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.2.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.2.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails/view.py` & `irails-1.2.7/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/irails.egg-info/PKG-INFO` & `irails-1.2.7/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.6
+Version: 1.2.7
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
-Metadata-Version: 2.1 Name: irails Version: 1.2.6 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.7 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.6/irails.egg-info/SOURCES.txt` & `irails-1.2.7/irails.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
 irails/scripts/__init__.py
 irails/scripts/_app.py
 irails/scripts/_controller.py
 irails/scripts/_i18n.py
 irails/scripts/_project.py
 irails/scripts/_run.py
+irails/scripts/_shell.py
 irails/scripts/main.py
 irails/scripts/tpls/app/controller.tpl
 irails/scripts/tpls/app/css.tpl
 irails/scripts/tpls/app/home.css.tpl
 irails/scripts/tpls/app/home.tpl
 irails/scripts/tpls/app/model.tpl
 irails/scripts/tpls/app/service.tpl
```

### Comparing `irails-1.2.6/irails.egg-info/requires.txt` & `irails-1.2.7/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.6/setup.py` & `irails-1.2.7/setup.py`

 * *Files identical despite different names*


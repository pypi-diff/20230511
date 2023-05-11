# Comparing `tmp/wagtailyoast-0.0.8.tar.gz` & `tmp/wagtailyoast-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtailyoast-0.0.8.tar", last modified: Wed May  5 07:39:57 2021, max compression
+gzip compressed data, was "dist/wagtailyoast-0.0.9.tar", last modified: Thu Jul 15 16:35:23 2021, max compression
```

## Comparing `wagtailyoast-0.0.8.tar` & `wagtailyoast-0.0.9.tar`

### file list

```diff
@@ -1,79 +1,83 @@
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/
--rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1160 2020-11-27 16:49:11.000000 wagtailyoast-0.0.8/setup.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2020-08-30 14:11:51.000000 wagtailyoast-0.0.8/LICENSE
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/tests/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/tests/migrations/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      979 2020-08-30 14:17:01.000000 wagtailyoast-0.0.8/tests/migrations/0001_initial.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-08-29 13:24:28.000000 wagtailyoast-0.0.8/tests/migrations/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-08-29 13:24:28.000000 wagtailyoast-0.0.8/tests/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1199 2020-09-12 15:46:31.000000 wagtailyoast-0.0.8/tests/models.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1439 2020-09-12 17:03:53.000000 wagtailyoast-0.0.8/tests/blocks.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/tests/management/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/tests/management/commands/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3019 2020-09-12 17:04:33.000000 wagtailyoast-0.0.8/tests/management/commands/init.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-06-15 14:21:45.000000 wagtailyoast-0.0.8/tests/management/commands/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-06-15 14:21:45.000000 wagtailyoast-0.0.8/tests/management/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1217 2020-09-12 15:46:31.000000 wagtailyoast-0.0.8/tests/constants.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-08-29 13:24:28.000000 wagtailyoast-0.0.8/wagtailyoast/__init__.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/templates/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/templates/wagtailyoast/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/templates/wagtailyoast/edit_handlers/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      728 2020-09-12 17:00:18.000000 wagtailyoast-0.0.8/wagtailyoast/templates/wagtailyoast/edit_handlers/yoast_panel.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      405 2020-08-30 13:21:48.000000 wagtailyoast-0.0.8/wagtailyoast/templates/wagtailyoast/edit_handlers/yoast_list.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1437 2021-05-05 07:35:54.000000 wagtailyoast-0.0.8/wagtailyoast/edit_handlers.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      538 2020-09-12 15:10:09.000000 wagtailyoast-0.0.8/wagtailyoast/context.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1417 2020-11-27 16:50:23.000000 wagtailyoast-0.0.8/wagtailyoast/wagtail_hooks.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      131 2020-09-12 17:00:18.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/yoastworker.js
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/common/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      356 2020-09-12 15:56:51.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/common/WithContext.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3031 2020-09-12 17:00:18.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/common/Panel.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3150 2020-09-12 16:46:35.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/common/ResultContainers.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       87 2020-08-29 16:25:50.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/yoastanalysis.js
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/scss/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       62 2020-06-15 14:21:45.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/scss/postcss.config.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      231 2020-08-30 13:45:47.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/scss/styles.scss
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-08-30 16:37:45.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.1.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-08-31 16:17:42.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.3.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-09-12 17:15:19.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.6.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-08-30 16:37:45.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.1.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-09-12 14:57:13.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.5.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-09-12 14:57:13.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.5.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-11-27 16:56:05.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.7.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-11-27 16:56:05.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.7.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2021-05-05 07:39:56.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.8.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-08-31 16:17:42.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.3.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2021-05-05 07:39:56.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.8.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-08-31 16:17:42.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.3.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557195 2020-08-30 16:37:45.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.1.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-11-27 16:56:05.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.7.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-09-12 14:57:13.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.5.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2021-05-05 07:39:56.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.8.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-09-12 17:15:19.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.6.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-08-30 16:38:16.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.2.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-09-12 17:15:19.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.6.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-08-30 16:38:16.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.2.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557195 2020-08-30 16:38:16.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.2.js
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2021-05-05 07:39:56.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.8.css
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-08-30 16:37:45.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.1.css
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-08-31 16:17:42.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.3.css
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-08-30 16:38:16.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.2.css
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-09-12 14:57:13.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.5.css
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-09-12 17:15:19.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.6.css
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-11-27 16:56:05.000000 wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.7.css
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/setup.cfg
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      134 2020-08-30 14:13:52.000000 wagtailyoast-0.0.8/MANIFEST.in
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast.egg-info/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       19 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast.egg-info/top_level.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast.egg-info/dependency_links.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3688 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast.egg-info/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2734 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/wagtailyoast.egg-info/SOURCES.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3688 2021-05-05 07:39:57.000000 wagtailyoast-0.0.8/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2180 2020-11-27 16:53:31.000000 wagtailyoast-0.0.8/README.rst
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/
+-rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1160 2020-11-27 16:49:11.000000 wagtailyoast-0.0.9/setup.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2020-08-30 14:11:51.000000 wagtailyoast-0.0.9/LICENSE
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/tests/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/tests/migrations/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      979 2020-08-30 14:17:01.000000 wagtailyoast-0.0.9/tests/migrations/0001_initial.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-08-29 13:24:28.000000 wagtailyoast-0.0.9/tests/migrations/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-08-29 13:24:28.000000 wagtailyoast-0.0.9/tests/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1199 2021-07-15 16:30:53.000000 wagtailyoast-0.0.9/tests/models.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1439 2020-09-12 17:03:53.000000 wagtailyoast-0.0.9/tests/blocks.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/tests/management/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/tests/management/commands/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3019 2020-09-12 17:04:33.000000 wagtailyoast-0.0.9/tests/management/commands/init.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-06-15 14:21:45.000000 wagtailyoast-0.0.9/tests/management/commands/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-06-15 14:21:45.000000 wagtailyoast-0.0.9/tests/management/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1217 2020-09-12 15:46:31.000000 wagtailyoast-0.0.9/tests/constants.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-08-29 13:24:28.000000 wagtailyoast-0.0.9/wagtailyoast/__init__.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/templates/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/templates/wagtailyoast/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/templates/wagtailyoast/edit_handlers/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      728 2021-05-12 06:56:14.000000 wagtailyoast-0.0.9/wagtailyoast/templates/wagtailyoast/edit_handlers/yoast_panel.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      405 2020-08-30 13:21:48.000000 wagtailyoast-0.0.9/wagtailyoast/templates/wagtailyoast/edit_handlers/yoast_list.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1437 2021-07-15 16:30:53.000000 wagtailyoast-0.0.9/wagtailyoast/edit_handlers.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      571 2021-07-15 16:31:43.000000 wagtailyoast-0.0.9/wagtailyoast/context.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1458 2021-07-15 16:31:43.000000 wagtailyoast-0.0.9/wagtailyoast/wagtail_hooks.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      131 2020-09-12 17:00:18.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/yoastworker.js
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/common/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      356 2020-09-12 15:56:51.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/common/WithContext.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3048 2021-07-15 16:31:43.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/common/Panel.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3150 2021-05-12 07:09:18.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/common/ResultContainers.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       87 2020-08-29 16:25:50.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/yoastanalysis.js
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/scss/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       62 2020-06-15 14:21:45.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/scss/postcss.config.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      231 2020-08-30 13:45:47.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/scss/styles.scss
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-08-30 16:37:45.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.1.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-08-31 16:17:42.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.3.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-09-12 17:15:19.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.6.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-08-30 16:37:45.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.1.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-09-12 14:57:13.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.5.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-09-12 14:57:13.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.5.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-11-27 16:56:05.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.7.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-11-27 16:56:05.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.7.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557585 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.9.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2021-05-05 07:39:56.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.8.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-08-31 16:17:42.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.3.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.9.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2021-05-05 07:39:56.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.8.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-08-31 16:17:42.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.3.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557195 2020-08-30 16:37:45.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.1.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.9.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-11-27 16:56:05.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.7.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557568 2020-09-12 14:57:13.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.5.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2021-05-05 07:39:56.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.8.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-09-12 17:15:19.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.6.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-08-30 16:38:16.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.2.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2554988 2020-09-12 17:15:19.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.6.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1019 2020-08-30 16:38:16.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.2.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)  2557195 2020-08-30 16:38:16.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.2.js
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.9.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2021-05-05 07:39:56.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.8.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-08-30 16:37:45.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.1.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-08-31 16:17:42.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.3.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-08-30 16:38:16.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.2.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-09-12 14:57:13.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.5.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-09-12 17:15:19.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.6.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      214 2020-11-27 16:56:05.000000 wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/css/styles0.0.7.css
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/setup.cfg
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      134 2020-08-30 14:13:52.000000 wagtailyoast-0.0.9/MANIFEST.in
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/wagtailyoast.egg-info/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       19 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast.egg-info/top_level.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3765 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast.egg-info/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2972 2021-07-15 16:35:22.000000 wagtailyoast-0.0.9/wagtailyoast.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3765 2021-07-15 16:35:23.000000 wagtailyoast-0.0.9/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2249 2021-07-15 16:31:43.000000 wagtailyoast-0.0.9/README.rst
```

### Comparing `wagtailyoast-0.0.8/setup.py` & `wagtailyoast-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/LICENSE` & `wagtailyoast-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/tests/migrations/0001_initial.py` & `wagtailyoast-0.0.9/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/tests/models.py` & `wagtailyoast-0.0.9/tests/models.py`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/tests/blocks.py` & `wagtailyoast-0.0.9/tests/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/tests/management/commands/init.py` & `wagtailyoast-0.0.9/tests/management/commands/init.py`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/tests/constants.py` & `wagtailyoast-0.0.9/tests/constants.py`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/templates/wagtailyoast/edit_handlers/yoast_panel.html` & `wagtailyoast-0.0.9/wagtailyoast/templates/wagtailyoast/edit_handlers/yoast_panel.html`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/edit_handlers.py` & `wagtailyoast-0.0.9/wagtailyoast/edit_handlers.py`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/context.py` & `wagtailyoast-0.0.9/wagtailyoast/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 except pkg_resources.DistributionNotFound:
     #  Develop part
     with open(os.path.join(settings.BASE_DIR, 'package.json')) as package:
         data = json.load(package)
         VERSION = data['version']
 
 LOCALE = settings.WY_LOCALE
+STATIC_URL = settings.STATIC_URL
```

### Comparing `wagtailyoast-0.0.8/wagtailyoast/wagtail_hooks.py` & `wagtailyoast-0.0.9/wagtailyoast/wagtail_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
     Add Yoast javascript files : Analysis and Worker
     :return: HTML <scripts>
     """
     cxt = json.dumps({
         'version': context.VERSION,
         'locale': context.LOCALE,
+        'staticUrl': context.STATIC_URL,
     })
     js_files = [
         'wagtailyoast/dist/js/yoastworker%s.js' % context.VERSION,
         'wagtailyoast/dist/js/yoastanalysis%s.js' % context.VERSION,
     ]
     js_includes = format_html_join(
         '\n',
```

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/common/Panel.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/common/Panel.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
     /**
      * Controller of Yoast Panel
      *
      * @param {object} context The context of wagtailyoast/context.py
      */
     constructor(context) {
         super(context);
-        this.workerUrl = `${this.baseUrl}/static/wagtailyoast/dist/js/yoastworker${this.context.version}.js`;
+        this.workerUrl = `${this.baseUrl}${this.context.staticUrl}wagtailyoast/dist/js/yoastworker${this.context.version}.js`;
         this.worker = new AnalysisWorkerWrapper(createWorker(this.workerUrl));
     }
 
     /**
      * Get HTML preview of wagtail page
      *
      * @returns {string}
```

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/src/js/common/ResultContainers.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/src/js/common/ResultContainers.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.1.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.1.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.3.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.3.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.6.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.6.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.1.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.1.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.5.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.5.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.5.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.5.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.7.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.7.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.7.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.7.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.8.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.8.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.3.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.3.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.8.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.8.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.3.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.9.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.1.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.1.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.7.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.3.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.5.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.5.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.8.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.7.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.6.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.6.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.2.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.8.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.6.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.2.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.2.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/styles0.0.2.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.2.js` & `wagtailyoast-0.0.9/wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.2.js`

 * *Files identical despite different names*

### Comparing `wagtailyoast-0.0.8/wagtailyoast.egg-info/PKG-INFO` & `wagtailyoast-0.0.9/wagtailyoast.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wagtailyoast
-Version: 0.0.8
+Version: 0.0.9
 Summary: Yoast For Wagtail
 Home-page: https://github.com/Aleksi44/wagtailyoast
 Author: Alexis Le Baron
 Author-email: alexis@stationspatiale.com
 License: GPL-3.0
 Description: *****************
         Wagtail Yoast SEO
@@ -37,18 +37,19 @@
         ::
         
             INSTALLED_APPS = [
                 ...
                 'wagtailyoast',
             ]
         
-        Add locale used for Yoast in your `settings.py` :
+        Add locale used for Yoast and make sure you have STATIC_URL set up in your `settings.py` :
         ::
         
             WY_LOCALE = 'en_US'
+            STATIC_URL = '/static/'
         
         
         Add YoastPannel to your Page models :
         
         ::
         
             from wagtail.admin.edit_handlers import TabbedInterface, ObjectList
```

### Comparing `wagtailyoast-0.0.8/wagtailyoast.egg-info/SOURCES.txt` & `wagtailyoast-0.0.9/wagtailyoast.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,35 +22,39 @@
 wagtailyoast/static/wagtailyoast/dist/css/styles0.0.1.css
 wagtailyoast/static/wagtailyoast/dist/css/styles0.0.2.css
 wagtailyoast/static/wagtailyoast/dist/css/styles0.0.3.css
 wagtailyoast/static/wagtailyoast/dist/css/styles0.0.5.css
 wagtailyoast/static/wagtailyoast/dist/css/styles0.0.6.css
 wagtailyoast/static/wagtailyoast/dist/css/styles0.0.7.css
 wagtailyoast/static/wagtailyoast/dist/css/styles0.0.8.css
+wagtailyoast/static/wagtailyoast/dist/css/styles0.0.9.css
 wagtailyoast/static/wagtailyoast/dist/js/styles0.0.1.js
 wagtailyoast/static/wagtailyoast/dist/js/styles0.0.2.js
 wagtailyoast/static/wagtailyoast/dist/js/styles0.0.3.js
 wagtailyoast/static/wagtailyoast/dist/js/styles0.0.5.js
 wagtailyoast/static/wagtailyoast/dist/js/styles0.0.6.js
 wagtailyoast/static/wagtailyoast/dist/js/styles0.0.7.js
 wagtailyoast/static/wagtailyoast/dist/js/styles0.0.8.js
+wagtailyoast/static/wagtailyoast/dist/js/styles0.0.9.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.1.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.2.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.3.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.5.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.6.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.7.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.8.js
+wagtailyoast/static/wagtailyoast/dist/js/yoastanalysis0.0.9.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.1.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.2.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.3.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.5.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.6.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.7.js
 wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.8.js
+wagtailyoast/static/wagtailyoast/dist/js/yoastworker0.0.9.js
 wagtailyoast/static/wagtailyoast/src/js/yoastanalysis.js
 wagtailyoast/static/wagtailyoast/src/js/yoastworker.js
 wagtailyoast/static/wagtailyoast/src/js/common/Panel.js
 wagtailyoast/static/wagtailyoast/src/js/common/ResultContainers.js
 wagtailyoast/static/wagtailyoast/src/js/common/WithContext.js
 wagtailyoast/static/wagtailyoast/src/scss/postcss.config.js
 wagtailyoast/static/wagtailyoast/src/scss/styles.scss
```

### Comparing `wagtailyoast-0.0.8/PKG-INFO` & `wagtailyoast-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wagtailyoast
-Version: 0.0.8
+Version: 0.0.9
 Summary: Yoast For Wagtail
 Home-page: https://github.com/Aleksi44/wagtailyoast
 Author: Alexis Le Baron
 Author-email: alexis@stationspatiale.com
 License: GPL-3.0
 Description: *****************
         Wagtail Yoast SEO
@@ -37,18 +37,19 @@
         ::
         
             INSTALLED_APPS = [
                 ...
                 'wagtailyoast',
             ]
         
-        Add locale used for Yoast in your `settings.py` :
+        Add locale used for Yoast and make sure you have STATIC_URL set up in your `settings.py` :
         ::
         
             WY_LOCALE = 'en_US'
+            STATIC_URL = '/static/'
         
         
         Add YoastPannel to your Page models :
         
         ::
         
             from wagtail.admin.edit_handlers import TabbedInterface, ObjectList
```

### Comparing `wagtailyoast-0.0.8/README.rst` & `wagtailyoast-0.0.9/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 ::
 
     INSTALLED_APPS = [
         ...
         'wagtailyoast',
     ]
 
-Add locale used for Yoast in your `settings.py` :
+Add locale used for Yoast and make sure you have STATIC_URL set up in your `settings.py` :
 ::
 
     WY_LOCALE = 'en_US'
+    STATIC_URL = '/static/'
 
 
 Add YoastPannel to your Page models :
 
 ::
 
     from wagtail.admin.edit_handlers import TabbedInterface, ObjectList
```


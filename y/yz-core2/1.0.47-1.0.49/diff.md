# Comparing `tmp/yz-core2-1.0.47.tar.gz` & `tmp/yz-core2-1.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.47.tar", last modified: Sat May  6 03:13:16 2023, max compression
+gzip compressed data, was "yz-core2-1.0.49.tar", last modified: Thu May 11 09:21:01 2023, max compression
```

## Comparing `yz-core2-1.0.47.tar` & `yz-core2-1.0.49.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.476584 yz-core2-1.0.47/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.47/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-06 03:13:16.476447 yz-core2-1.0.47/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.47/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-05-06 03:13:16.476623 yz-core2-1.0.47/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-05-06 03:13:09.000000 yz-core2-1.0.47/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.459320 yz-core2-1.0.47/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.47/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.47/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.47/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.460296 yz-core2-1.0.47/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3386 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.461205 yz-core2-1.0.47/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.462309 yz-core2-1.0.47/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.463123 yz-core2-1.0.47/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.463731 yz-core2-1.0.47/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-05-05 06:04:45.000000 yz-core2-1.0.47/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.464397 yz-core2-1.0.47/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.47/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.464722 yz-core2-1.0.47/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.465910 yz-core2-1.0.47/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.47/yzcore/extensions/storage/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.466231 yz-core2-1.0.47/yzcore/extensions/storage/azure/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7286 2023-05-06 03:12:37.000000 yz-core2-1.0.47/yzcore/extensions/storage/azure/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10660 2023-05-06 03:12:38.000000 yz-core2-1.0.47/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.47/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.466441 yz-core2-1.0.47/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8091 2023-05-06 03:12:37.000000 yz-core2-1.0.47/yzcore/extensions/storage/minio/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.467440 yz-core2-1.0.47/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8886 2023-05-06 03:12:37.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.468064 yz-core2-1.0.47/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    12259 2023-05-06 03:12:38.000000 yz-core2-1.0.47/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.47/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-04-24 09:03:30.000000 yz-core2-1.0.47/yzcore/extensions/storage/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.47/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.468681 yz-core2-1.0.47/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.469084 yz-core2-1.0.47/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.469699 yz-core2-1.0.47/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.469909 yz-core2-1.0.47/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.470704 yz-core2-1.0.47/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.471142 yz-core2-1.0.47/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.471440 yz-core2-1.0.47/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.471622 yz-core2-1.0.47/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.472003 yz-core2-1.0.47/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.472140 yz-core2-1.0.47/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.472908 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.473639 yz-core2-1.0.47/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.474038 yz-core2-1.0.47/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.474203 yz-core2-1.0.47/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.476128 yz-core2-1.0.47/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-04-26 02:34:51.000000 yz-core2-1.0.47/yzcore/utils/decorator.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/encoding.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1834 2023-04-21 07:30:35.000000 yz-core2-1.0.47/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.485937 yz-core2-1.0.49/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.49/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-11 09:21:01.485784 yz-core2-1.0.49/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.49/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-05-11 09:21:01.485978 yz-core2-1.0.49/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-05-11 09:20:51.000000 yz-core2-1.0.49/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.471148 yz-core2-1.0.49/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.49/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.49/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.49/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.471948 yz-core2-1.0.49/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3386 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.472978 yz-core2-1.0.49/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.473880 yz-core2-1.0.49/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.474391 yz-core2-1.0.49/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.474965 yz-core2-1.0.49/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-05-05 06:04:45.000000 yz-core2-1.0.49/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.475558 yz-core2-1.0.49/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2599 2023-05-08 08:37:20.000000 yz-core2-1.0.49/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.49/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.475815 yz-core2-1.0.49/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.476801 yz-core2-1.0.49/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.49/yzcore/extensions/storage/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.477117 yz-core2-1.0.49/yzcore/extensions/storage/azure/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7411 2023-05-11 08:40:13.000000 yz-core2-1.0.49/yzcore/extensions/storage/azure/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10752 2023-05-11 08:37:54.000000 yz-core2-1.0.49/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.49/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.477311 yz-core2-1.0.49/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8216 2023-05-11 08:40:13.000000 yz-core2-1.0.49/yzcore/extensions/storage/minio/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.478249 yz-core2-1.0.49/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8886 2023-05-06 03:12:37.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.478718 yz-core2-1.0.49/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    12259 2023-05-06 03:12:38.000000 yz-core2-1.0.49/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.49/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-04-24 09:03:30.000000 yz-core2-1.0.49/yzcore/extensions/storage/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.49/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.479314 yz-core2-1.0.49/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.479562 yz-core2-1.0.49/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.479975 yz-core2-1.0.49/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.480188 yz-core2-1.0.49/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.480958 yz-core2-1.0.49/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.481353 yz-core2-1.0.49/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.481572 yz-core2-1.0.49/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.481740 yz-core2-1.0.49/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.482212 yz-core2-1.0.49/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.482342 yz-core2-1.0.49/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.482952 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.483404 yz-core2-1.0.49/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.483738 yz-core2-1.0.49/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.483917 yz-core2-1.0.49/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.485467 yz-core2-1.0.49/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/crypto.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-05-10 06:22:06.000000 yz-core2-1.0.49/yzcore/utils/decorator.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/encoding.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.49/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.47/LICENSE` & `yz-core2-1.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/PKG-INFO` & `yz-core2-1.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.47
+Version: 1.0.49
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.47/README.md` & `yz-core2-1.0.49/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/setup.py` & `yz-core2-1.0.49/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.47",
+    version="1.0.49",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
```

### Comparing `yz-core2-1.0.47/tests/test_setting_reload.py` & `yz-core2-1.0.49/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/tests/test_uid.py` & `yz-core2-1.0.49/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.49/yz_core2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.47
+Version: 1.0.49
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.47/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.49/yz_core2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/core/datastructures.py` & `yz-core2-1.0.49/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/core/encoders.py` & `yz-core2-1.0.49/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/core/management/__init__.py` & `yz-core2-1.0.49/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.49/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.49/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/core/management/templates.py` & `yz-core2-1.0.49/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/core/storage.py` & `yz-core2-1.0.49/yzcore/core/storage.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/db/db_session.py` & `yz-core2-1.0.49/yzcore/db/db_session.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.49/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.49/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/decorators.py` & `yz-core2-1.0.49/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/default_settings.py` & `yz-core2-1.0.49/yzcore/default_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     ID_URL: AnyUrl = None
     GENERATE_UUID_PATH: str = '/uuid/generate/'
     EXPLAIN_UUID_PATH: str = '/uuid/explain/'
     TRANSLATE_PATH: str = '/uuid/translate/'
     MAKE_UUID_PATH: str = '/uuid/make/'
 
     STORAGE_CONF: dict = None
+    STORAGE_ORG_ENABLE: bool = False  # 启用组织自定义对象存储
 
 
 default_setting = DefaultSetting()
 
 
 def reload_reload_settings(instance):
     settings = default_setting
```

### Comparing `yz-core2-1.0.47/yzcore/exceptions.py` & `yz-core2-1.0.49/yzcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.49/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/azure/__init__.py` & `yz-core2-1.0.49/yzcore/extensions/storage/azure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @desc: azure blob对象存储封装
 """
 
 from datetime import datetime, timedelta
 import os
 from io import BufferedReader, BytesIO
 from typing import Union
+from urllib.parse import unquote
 
 from yzcore.extensions.storage.base import StorageManagerBase, StorageRequestError, IMAGE_FORMAT_SET
 from yzcore.extensions.storage.schemas import AzureConfig
 from yzcore.utils.time_utils import datetime2str
 
 
 try:
@@ -113,17 +114,20 @@
             resource_url = self.scheme + ':' + resource_url
         return resource_url
 
     @property
     def host(self):
         return u'//{}/{}'.format(self.endpoint, self.bucket_name)
 
-    def get_key_from_url(self, url):
+    def get_key_from_url(self, url, urldecode=False):
         """从URL中获取对象存储key"""
-        return url.split(self.bucket_name + '/')[-1]
+        path = url.split(self.bucket_name + '/')[-1]
+        if urldecode:
+            path = unquote(path)
+        return path
 
     def iter_objects(self, prefix='', marker=None, delimiter=None, max_keys=100):
         objects = self.container_client.list_blobs(name_starts_with=prefix, results_per_page=max_keys)
         _result = []
         for obj in objects:
             _result.append({
                 'key': obj.name,
```

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/base.py` & `yz-core2-1.0.49/yzcore/extensions/storage/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,21 +272,24 @@
         return True
 
     @staticmethod
     def parse_content_type(filename):
         ext = filename.split('.')[-1].lower()
         return CONTENT_TYPE.get(ext, 'application/octet-stream')
 
-    def get_key_from_url(self, url):
+    def get_key_from_url(self, url, urldecode=False):
         """从URL中获取对象存储key"""
         if url.startswith('//'):
             url = 'https:' + url
         elif not url.startswith('http'):
             url = 'https://' + url
         url_parse = urlparse(url)
-        return url_parse.path[1:]  # 去掉最前面的 /
+        path = url_parse.path
+        if urldecode:
+            path = unquote(path)
+        return path[1:]  # 去掉最前面的 /
 
     @staticmethod
     def get_filename(key):
         """从key中提取文件名，不包含路径"""
         key = unquote(key)
         return key.split('/')[-1]
```

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/const.py` & `yz-core2-1.0.49/yzcore/extensions/storage/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.49/yzcore/extensions/storage/minio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 @author: zhouwei
 @date: 2022/11/09
 @desc: minio对象存储封装
 """
 import json
 import os
+from urllib.parse import unquote
 
 from yzcore.extensions.storage.base import StorageManagerBase, StorageRequestError, logger, IMAGE_FORMAT_SET
 from yzcore.extensions.storage.schemas import MinioConfig
 from yzcore.utils.time_utils import datetime2str
 from datetime import timedelta, datetime
 
 
@@ -198,17 +199,20 @@
         }
         return data
 
     @property
     def host(self):
         return u'//{}/{}'.format(self.endpoint, self.bucket_name)
 
-    def get_key_from_url(self, url):
+    def get_key_from_url(self, url, urldecode=False):
         """从URL中获取对象存储key"""
-        return url.split(self.bucket_name + '/')[-1]
+        path = url.split(self.bucket_name + '/')[-1]
+        if urldecode:
+            path = unquote(path)
+        return path
 
     def get_file_url(self, key, with_scheme=False):
         if not any((self.image_domain, self.asset_domain)):
             resource_url = u"//{}/{}/{}".format(self.endpoint, self.bucket_name, key)
         elif key.split('.')[-1].lower() in IMAGE_FORMAT_SET:
             resource_url = u"//{domain}/{bucket}/{key}".format(
                 domain=self.image_domain, bucket=self.bucket_name, key=key)
```

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.49/yzcore/extensions/storage/obs/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.49/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.49/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/obs/utils.py` & `yz-core2-1.0.49/yzcore/extensions/storage/obs/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.49/yzcore/extensions/storage/oss/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.49/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/storage/schemas.py` & `yz-core2-1.0.49/yzcore/extensions/storage/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/extensions/uid.py` & `yz-core2-1.0.49/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/logger/__init__.py` & `yz-core2-1.0.49/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/logger/config.py` & `yz-core2-1.0.49/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/logger/filters.py` & `yz-core2-1.0.49/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/logger/handlers.py` & `yz-core2-1.0.49/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/request/aio_http.py` & `yz-core2-1.0.49/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/response/response.py` & `yz-core2-1.0.49/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/response/response_code.py` & `yz-core2-1.0.49/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.49/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.49/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/app_template/views.py` & `yz-core2-1.0.49/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.49/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/project_template/README.md` & `yz-core2-1.0.49/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.49/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.49/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.49/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.49/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/utils/check_sys.py` & `yz-core2-1.0.49/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/utils/crypto.py` & `yz-core2-1.0.49/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/utils/decorator.py` & `yz-core2-1.0.49/yzcore/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/utils/encoding.py` & `yz-core2-1.0.49/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/utils/nacos.py` & `yz-core2-1.0.49/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.47/yzcore/utils/time_utils.py` & `yz-core2-1.0.49/yzcore/utils/time_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 __all__ = [
     "get_zero_time",
     "get_today_date",
     "datetime2timestamp",
     "timestamp2datetime",
     "datetime2str",
+    "timestamp2str",
 ]
 
 
 def get_zero_time(
         date_time: datetime = None,
         is_timestamp: bool = True
 ):
@@ -77,7 +78,18 @@
     :param dt:
     :param fmt
     :return: "2023-04-18 18:54:59"
     """
     if dt.tzinfo:
         dt = dt.astimezone(Beijing)
     return dt.strftime(fmt)
+
+
+def timestamp2str(timestamp, fmt='%Y-%m-%d %H:%M:%S'):
+    """
+    时间戳转字符串
+    :param timestamp: int|float
+    :param fmt:
+    :return: "2023-04-18 18:54:59"
+    """
+    dt = datetime.datetime.fromtimestamp(timestamp, tz=Beijing)
+    return dt.strftime(fmt)
```


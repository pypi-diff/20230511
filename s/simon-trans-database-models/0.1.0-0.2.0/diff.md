# Comparing `tmp/simon-trans-database-models-0.1.0.tar.gz` & `tmp/simon-trans-database-models-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simon-trans-database-models-0.1.0.tar", max compression
+gzip compressed data, was "simon-trans-database-models-0.2.0.tar", max compression
```

## Comparing `simon-trans-database-models-0.1.0.tar` & `simon-trans-database-models-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      419 2023-05-09 11:58:22.418438 simon-trans-database-models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 12:02:01.486897 simon-trans-database-models-0.1.0/simon_trans_database_models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 12:02:01.661283 simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-09 12:07:07.042187 simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/env.py
--rw-r--r--   0        0        0       40 2023-05-09 12:02:01.660293 simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/README
--rw-r--r--   0        0        0      534 2023-05-09 12:02:01.661283 simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/script.py.mako
--rw-r--r--   0        0        0      947 2023-05-09 12:14:37.839292 simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/versions/014fdfa9a966_add_solar_system_table.py
--rw-r--r--   0        0        0     3340 2023-05-09 12:07:40.648474 simon-trans-database-models-0.1.0/simon_trans_database_models/alembic.ini
--rw-r--r--   0        0        0       63 2023-05-09 12:14:33.752103 simon-trans-database-models-0.1.0/simon_trans_database_models/tables/__init__.py
--rw-r--r--   0        0        0      160 2023-05-09 12:03:14.572783 simon-trans-database-models-0.1.0/simon_trans_database_models/tables/base.py
--rw-r--r--   0        0        0      413 2023-05-09 12:14:37.845276 simon-trans-database-models-0.1.0/simon_trans_database_models/tables/solar_system.py
--rw-r--r--   0        0        0      785 2023-05-09 12:46:50.878644 simon-trans-database-models-0.1.0/setup.py
--rw-r--r--   0        0        0      451 2023-05-09 12:46:50.878644 simon-trans-database-models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      419 2023-05-11 08:42:43.029396 simon-trans-database-models-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 12:02:01.486897 simon-trans-database-models-0.2.0/simon_trans_database_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 12:02:01.661283 simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/__init__.py
+-rw-r--r--   0        0        0     2130 2023-05-09 12:07:07.042187 simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/env.py
+-rw-r--r--   0        0        0       40 2023-05-09 12:02:01.660293 simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/README
+-rw-r--r--   0        0        0      534 2023-05-09 12:02:01.661283 simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/script.py.mako
+-rw-r--r--   0        0        0      947 2023-05-09 12:14:37.839292 simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/versions/014fdfa9a966_add_solar_system_table.py
+-rw-r--r--   0        0        0     5721 2023-05-11 08:40:31.107426 simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/versions/5eee6d4b6713_add_weather_forecast_table.py
+-rw-r--r--   0        0        0     3340 2023-05-09 12:07:40.648474 simon-trans-database-models-0.2.0/simon_trans_database_models/alembic.ini
+-rw-r--r--   0        0        0      110 2023-05-11 08:37:58.452366 simon-trans-database-models-0.2.0/simon_trans_database_models/tables/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-09 12:03:14.572783 simon-trans-database-models-0.2.0/simon_trans_database_models/tables/base.py
+-rw-r--r--   0        0        0      413 2023-05-09 12:14:37.845276 simon-trans-database-models-0.2.0/simon_trans_database_models/tables/solar_system.py
+-rw-r--r--   0        0        0     4212 2023-05-11 08:40:31.115406 simon-trans-database-models-0.2.0/simon_trans_database_models/tables/weather_forecast.py
+-rw-r--r--   0        0        0      785 2023-05-11 08:43:23.113301 simon-trans-database-models-0.2.0/setup.py
+-rw-r--r--   0        0        0      451 2023-05-11 08:43:23.113301 simon-trans-database-models-0.2.0/PKG-INFO
```

### Comparing `simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/env.py` & `simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/script.py.mako` & `simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `simon-trans-database-models-0.1.0/simon_trans_database_models/alembic/versions/014fdfa9a966_add_solar_system_table.py` & `simon-trans-database-models-0.2.0/simon_trans_database_models/alembic/versions/014fdfa9a966_add_solar_system_table.py`

 * *Files identical despite different names*

### Comparing `simon-trans-database-models-0.1.0/simon_trans_database_models/alembic.ini` & `simon-trans-database-models-0.2.0/simon_trans_database_models/alembic.ini`

 * *Files identical despite different names*

### Comparing `simon-trans-database-models-0.1.0/setup.py` & `simon-trans-database-models-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['marshmallow==3.14.1', 'sqlalchemy==1.3.18']
 
 setup_kwargs = {
     'name': 'simon-trans-database-models',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': None,
     'author': 'Pintér Tamás',
     'author_email': 'tamas.pinter@pannonszoftver.hu',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```


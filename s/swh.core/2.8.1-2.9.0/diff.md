# Comparing `tmp/swh.core-2.8.1.tar.gz` & `tmp/swh.core-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.core-2.8.1.tar", last modified: Mon May 30 15:09:47 2022, max compression
+gzip compressed data, was "dist/swh.core-2.9.0.tar", last modified: Mon May 30 15:41:13 2022, max compression
```

## Comparing `swh.core-2.8.1.tar` & `swh.core-2.9.0.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      141 2022-05-30 15:09:44.000000 swh.core-2.8.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2022-05-30 15:09:44.000000 swh.core-2.8.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      872 2022-05-30 15:09:44.000000 swh.core-2.8.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2022-05-30 15:09:44.000000 swh.core-2.8.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-05-30 15:09:44.000000 swh.core-2.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       19 2022-05-30 15:09:44.000000 swh.core-2.8.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-05-30 15:09:44.000000 swh.core-2.8.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      288 2022-05-30 15:09:44.000000 swh.core-2.8.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-05-30 15:09:44.000000 swh.core-2.8.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)       95 2022-05-30 15:09:44.000000 swh.core-2.8.1/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     1320 2022-05-30 15:09:47.000000 swh.core-2.8.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      293 2022-05-30 15:09:44.000000 swh.core-2.8.1/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      712 2022-05-30 15:09:44.000000 swh.core-2.8.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      293 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      383 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6489 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/db.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      152 2022-05-30 15:09:44.000000 swh.core-2.8.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      852 2022-05-30 15:09:44.000000 swh.core-2.8.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-05-30 15:09:44.000000 swh.core-2.8.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       99 2022-05-30 15:09:44.000000 swh.core-2.8.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      188 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements-db-pytestplugin.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements-db.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       53 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements-github.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      147 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements-http.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements-logging.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2022-05-30 15:09:44.000000 swh.core-2.8.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2022-05-30 15:09:47.000000 swh.core-2.8.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2950 2022-05-30 15:09:44.000000 swh.core-2.8.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      143 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/__main__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/api/
--rw-r--r--   0 jenkins    (115) docker     (999)    18149 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6340 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/asynchronous.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2073 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/classes.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1192 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/gunicorn_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5812 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/negotiation.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10535 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/serializers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/api/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4292 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/server_testing.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7863 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_async.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2755 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_classes.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4880 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_gunicorn.py
--rw-r--r--   0 jenkins    (115) docker     (999)      862 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5708 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_rpc_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5170 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_rpc_client_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4418 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_rpc_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4871 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_rpc_server_asynchronous.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8925 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)       63 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/api_async.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)     5872 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/cli/__init__.py
--rwxr-xr-x   0 jenkins    (115) docker     (999)    13334 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/cli/db.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2050 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/collections.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8496 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/config.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/
--rw-r--r--   0 jenkins    (115) docker     (999)    10619 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4888 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)    22500 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/db_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10362 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)      664 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/sql/35-dbversion.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      683 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/sql/36-dbmodule.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2158 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/data/cli/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/data/cli/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       41 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      293 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      156 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      246 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli/sql/50-data.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       41 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/0-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      156 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      126 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/50-data.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/upgrades/001.sql
--rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/upgrades/002.sql
--rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/upgrades/003.sql
--rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/upgrades/004.sql
--rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/upgrades/005.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      196 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/data/cli_new/sql/upgrades/006.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/pytest_plugin/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/pytest_plugin/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/db/tests/pytest_plugin/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      425 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/pytest_plugin/data/0-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      940 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/pytest_plugin/data/1-data.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5829 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/pytest_plugin/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12824 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13970 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/test_db.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6779 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/db/tests/test_db_utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/github/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/github/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6106 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/github/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/github/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/github/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6431 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/github/tests/test_github_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1440 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/github/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7953 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/github/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4331 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/logger.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)    11503 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3126 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/sentry.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16708 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/statsd.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6471 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tarball.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)       98 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/data/archives/
--rw-r--r--   0 jenkins    (115) docker     (999)  1087901 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/groff-1.02.tar.Z
--rw-r--r--   0 jenkins    (115) docker     (999)    10240 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.tar
--rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.tar.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)      181 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)      190 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.tar.lz
--rw-r--r--   0 jenkins    (115) docker     (999)    10240 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.tar.x
--rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.tbz
--rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.tbz2
--rw-r--r--   0 jenkins    (115) docker     (999)      162 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/hello.zip
--rw-r--r--   0 jenkins    (115) docker     (999)   845917 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/msk316src.zip
--rw-r--r--   0 jenkins    (115) docker     (999)    45185 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/archives/tokei-12.1.2.crate
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/data/http_example.com/
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/http_example.com/something.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/data/https_example.com/
--rw-r--r--   0 jenkins    (115) docker     (999)       23 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) docker     (999)       28 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
--rw-r--r--   0 jenkins    (115) docker     (999)       25 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/https_example.com/file.json_visit1
--rw-r--r--   0 jenkins    (115) docker     (999)        9 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/https_example.com/other.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/data/https_forge.s.o/
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/data/https_www.reference.com/
--rw-r--r--   0 jenkins    (115) docker     (999)       17 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/fixture/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/fixture/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      401 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/fixture/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/fixture/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh/core/tests/fixture/data/https_example.com/
--rw-r--r--   0 jenkins    (115) docker     (999)       25 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/fixture/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) docker     (999)      797 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/fixture/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10782 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2439 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_collections.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9879 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3581 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_logger.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4018 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3015 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_sentry.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18221 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_statsd.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7733 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_tarball.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5422 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5788 2022-05-30 15:09:44.000000 swh.core-2.8.1/swh/core/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh.core.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1320 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh.core.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     4501 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh.core.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh.core.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      177 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh.core.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      688 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh.core.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       20 2022-05-30 15:09:47.000000 swh.core-2.8.1/swh.core.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1993 2022-05-30 15:09:44.000000 swh.core-2.8.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      141 2022-05-30 15:41:10.000000 swh.core-2.9.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2022-05-30 15:41:10.000000 swh.core-2.9.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      872 2022-05-30 15:41:10.000000 swh.core-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2022-05-30 15:41:10.000000 swh.core-2.9.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-05-30 15:41:10.000000 swh.core-2.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       19 2022-05-30 15:41:10.000000 swh.core-2.9.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-05-30 15:41:10.000000 swh.core-2.9.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      288 2022-05-30 15:41:10.000000 swh.core-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-05-30 15:41:10.000000 swh.core-2.9.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)       95 2022-05-30 15:41:10.000000 swh.core-2.9.0/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     1320 2022-05-30 15:41:13.000000 swh.core-2.9.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      293 2022-05-30 15:41:10.000000 swh.core-2.9.0/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      712 2022-05-30 15:41:10.000000 swh.core-2.9.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      293 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      383 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6489 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/db.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      152 2022-05-30 15:41:10.000000 swh.core-2.9.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      852 2022-05-30 15:41:10.000000 swh.core-2.9.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-05-30 15:41:10.000000 swh.core-2.9.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       99 2022-05-30 15:41:10.000000 swh.core-2.9.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      188 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements-db-pytestplugin.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements-db.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       53 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements-github.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      147 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements-http.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements-logging.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2022-05-30 15:41:10.000000 swh.core-2.9.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2022-05-30 15:41:13.000000 swh.core-2.9.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2950 2022-05-30 15:41:10.000000 swh.core-2.9.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      143 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/__main__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)    18149 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6340 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/asynchronous.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2073 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/classes.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1192 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5812 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/negotiation.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10535 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/serializers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/api/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4292 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/server_testing.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7863 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_async.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2755 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_classes.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4880 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_gunicorn.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      862 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5708 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_rpc_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5170 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_rpc_client_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4418 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_rpc_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4871 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_rpc_server_asynchronous.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8925 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       63 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/api_async.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5872 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/cli/__init__.py
+-rwxr-xr-x   0 jenkins    (115) docker     (999)    13968 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/cli/db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2050 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/collections.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8496 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/config.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/
+-rw-r--r--   0 jenkins    (115) docker     (999)    10619 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4888 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    22500 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/db_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10362 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)      664 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/sql/35-dbversion.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      683 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/sql/36-dbmodule.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2158 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/data/cli/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/data/cli/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       41 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      293 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      156 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      246 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli/sql/50-data.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       41 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/0-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      156 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      126 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/50-data.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/upgrades/001.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/upgrades/002.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/upgrades/003.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/upgrades/004.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)       82 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/upgrades/005.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      196 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/data/cli_new/sql/upgrades/006.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/pytest_plugin/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/pytest_plugin/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/db/tests/pytest_plugin/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      425 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/pytest_plugin/data/0-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      940 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/pytest_plugin/data/1-data.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5829 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/pytest_plugin/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12824 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13970 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6779 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/db/tests/test_db_utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/github/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/github/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6106 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/github/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/github/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/github/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6431 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/github/tests/test_github_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1440 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/github/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7953 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/github/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4331 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/logger.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)    11503 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3126 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/sentry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16708 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/statsd.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6471 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tarball.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)       98 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) docker     (999)  1087901 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/groff-1.02.tar.Z
+-rw-r--r--   0 jenkins    (115) docker     (999)    10240 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.tar
+-rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.tar.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)      181 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)      190 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.tar.lz
+-rw-r--r--   0 jenkins    (115) docker     (999)    10240 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.tar.x
+-rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.tbz
+-rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.tbz2
+-rw-r--r--   0 jenkins    (115) docker     (999)      162 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/hello.zip
+-rw-r--r--   0 jenkins    (115) docker     (999)   845917 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/msk316src.zip
+-rw-r--r--   0 jenkins    (115) docker     (999)    45185 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/archives/tokei-12.1.2.crate
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/data/http_example.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/http_example.com/something.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)       23 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) docker     (999)       28 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
+-rw-r--r--   0 jenkins    (115) docker     (999)       25 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/https_example.com/file.json_visit1
+-rw-r--r--   0 jenkins    (115) docker     (999)        9 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/https_example.com/other.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/data/https_forge.s.o/
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/data/https_www.reference.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)       17 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/fixture/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/fixture/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      401 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/fixture/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/fixture/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh/core/tests/fixture/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)       25 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/fixture/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      797 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/fixture/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10782 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2439 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_collections.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9879 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3581 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_logger.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4018 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3015 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_sentry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18221 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_statsd.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7733 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_tarball.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5422 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5788 2022-05-30 15:41:10.000000 swh.core-2.9.0/swh/core/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh.core.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1320 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh.core.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4501 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh.core.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh.core.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      177 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh.core.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      688 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh.core.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       20 2022-05-30 15:41:13.000000 swh.core-2.9.0/swh.core.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1993 2022-05-30 15:41:10.000000 swh.core-2.9.0/tox.ini
```

### Comparing `swh.core-2.8.1/.pre-commit-config.yaml` & `swh.core-2.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/CODE_OF_CONDUCT.md` & `swh.core-2.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/LICENSE` & `swh.core-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/PKG-INFO` & `swh.core-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 2.8.1
+Version: 2.9.0
 Summary: Software Heritage core utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DCORE/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-core
```

### Comparing `swh.core-2.8.1/conftest.py` & `swh.core-2.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/docs/db.rst` & `swh.core-2.9.0/docs/db.rst`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/mypy.ini` & `swh.core-2.9.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/setup.py` & `swh.core-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/__init__.py` & `swh.core-2.9.0/swh/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/asynchronous.py` & `swh.core-2.9.0/swh/core/api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/classes.py` & `swh.core-2.9.0/swh/core/api/classes.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/gunicorn_config.py` & `swh.core-2.9.0/swh/core/api/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/negotiation.py` & `swh.core-2.9.0/swh/core/api/negotiation.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/serializers.py` & `swh.core-2.9.0/swh/core/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/server_testing.py` & `swh.core-2.9.0/swh/core/api/tests/server_testing.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_async.py` & `swh.core-2.9.0/swh/core/api/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_classes.py` & `swh.core-2.9.0/swh/core/api/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_gunicorn.py` & `swh.core-2.9.0/swh/core/api/tests/test_gunicorn.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_init.py` & `swh.core-2.9.0/swh/core/api/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_rpc_client.py` & `swh.core-2.9.0/swh/core/api/tests/test_rpc_client.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_rpc_client_server.py` & `swh.core-2.9.0/swh/core/api/tests/test_rpc_client_server.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_rpc_server.py` & `swh.core-2.9.0/swh/core/api/tests/test_rpc_server.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_rpc_server_asynchronous.py` & `swh.core-2.9.0/swh/core/api/tests/test_rpc_server_asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/api/tests/test_serializers.py` & `swh.core-2.9.0/swh/core/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/cli/__init__.py` & `swh.core-2.9.0/swh/core/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/cli/db.py` & `swh.core-2.9.0/swh/core/cli/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import warnings
 
 import click
 
 from swh.core.cli import CONTEXT_SETTINGS
 from swh.core.cli import swh as swh_cli_group
 
-warnings.filterwarnings("ignore")  # noqa prevent psycopg from telling us sh*t
+warnings.filterwarnings("ignore")  # noqa prevent psycopg from side-tracking us
 
 
 logger = logging.getLogger(__name__)
 
 
 @swh_cli_group.group(name="db", context_settings=CONTEXT_SETTINGS)
 @click.option(
@@ -252,28 +252,32 @@
 @click.option(
     "--all/--no-all",
     "show_all",
     help="Show version history.",
     default=False,
     show_default=True,
 )
+@click.option("--module-config-key", help="Module config key to lookup.", default=None)
 @click.pass_context
-def db_version(ctx, module, show_all):
+def db_version(ctx, module, show_all, module_config_key=None):
     """Print the database version for the Software Heritage.
 
     Example::
 
         swh db version -d swh-test
+        swh db version scheduler
+        swh db version scrubber --module-config-key=scrubber_db
 
     """
     from swh.core.db.db_utils import get_database_info, import_swhmodule
 
-    # use the db cnx from the config file; the expected config entry is the
-    # given module name
-    cfg = ctx.obj["config"].get(module, {})
+    # use the db cnx from the config file; the expected config entry is either the given
+    # module_config_key or defaulting to the module name (if module_config_key is not
+    # provided)
+    cfg = ctx.obj["config"].get(module_config_key or module, {})
     dbname = get_dburl_from_config(cfg)
 
     if not dbname:
         raise click.BadParameter(
             "Missing the postgresql connection configuration. Either fix your "
             "configuration file or use the --dbname option."
         )
@@ -324,34 +328,39 @@
     default=None,
 )
 @click.option(
     "--interactive/--non-interactive",
     help="Do not ask questions (use default answer to all questions)",
     default=True,
 )
+@click.option(
+    "--module-config-key", help="Module configuration key to lookup.", default=None
+)
 @click.pass_context
-def db_upgrade(ctx, module, to_version, interactive):
+def db_upgrade(ctx, module, to_version, interactive, module_config_key):
     """Upgrade the database for given module (to a given version if specified).
 
     Examples::
 
         swh db upgrade storage
         swh db upgrade scheduler --to-version=10
+        swh db upgrade scrubber --to-version=10 --module-config-key=scrubber_db
 
     """
     from swh.core.db.db_utils import (
         get_database_info,
         import_swhmodule,
         swh_db_upgrade,
         swh_set_db_module,
     )
 
-    # use the db cnx from the config file; the expected config entry is the
-    # given module name
-    cfg = ctx.obj["config"].get(module, {})
+    # use the db cnx from the config file; the expected config entry is either the given
+    # module_config_key or defaulting to the module name (if module_config_key is not
+    # provided)
+    cfg = ctx.obj["config"].get(module_config_key or module, {})
     dbname = get_dburl_from_config(cfg)
 
     if not dbname:
         raise click.BadParameter(
             "Missing the postgresql connection configuration. Either fix your "
             "configuration file or use the --dbname option."
         )
```

### Comparing `swh.core-2.8.1/swh/core/collections.py` & `swh.core-2.9.0/swh/core/collections.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/config.py` & `swh.core-2.9.0/swh/core/config.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/__init__.py` & `swh.core-2.9.0/swh/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/common.py` & `swh.core-2.9.0/swh/core/db/common.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/db_utils.py` & `swh.core-2.9.0/swh/core/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/pytest_plugin.py` & `swh.core-2.9.0/swh/core/db/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/sql/35-dbversion.sql` & `swh.core-2.9.0/swh/core/db/sql/35-dbversion.sql`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/sql/36-dbmodule.sql` & `swh.core-2.9.0/swh/core/db/sql/36-dbmodule.sql`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/tests/conftest.py` & `swh.core-2.9.0/swh/core/db/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/tests/pytest_plugin/data/1-data.sql` & `swh.core-2.9.0/swh/core/db/tests/pytest_plugin/data/1-data.sql`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/tests/pytest_plugin/test_pytest_plugin.py` & `swh.core-2.9.0/swh/core/db/tests/pytest_plugin/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/tests/test_cli.py` & `swh.core-2.9.0/swh/core/db/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/tests/test_db.py` & `swh.core-2.9.0/swh/core/db/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/db/tests/test_db_utils.py` & `swh.core-2.9.0/swh/core/db/tests/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/github/pytest_plugin.py` & `swh.core-2.9.0/swh/core/github/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/github/tests/test_github_utils.py` & `swh.core-2.9.0/swh/core/github/tests/test_github_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/github/tests/test_pytest_plugin.py` & `swh.core-2.9.0/swh/core/github/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/github/utils.py` & `swh.core-2.9.0/swh/core/github/utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/logger.py` & `swh.core-2.9.0/swh/core/logger.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/pytest_plugin.py` & `swh.core-2.9.0/swh/core/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/sentry.py` & `swh.core-2.9.0/swh/core/sentry.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/statsd.py` & `swh.core-2.9.0/swh/core/statsd.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tarball.py` & `swh.core-2.9.0/swh/core/tarball.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/data/archives/groff-1.02.tar.Z` & `swh.core-2.9.0/swh/core/tests/data/archives/groff-1.02.tar.Z`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/data/archives/hello.tar` & `swh.core-2.9.0/swh/core/tests/data/archives/hello.tar`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/data/archives/hello.tar.x` & `swh.core-2.9.0/swh/core/tests/data/archives/hello.tar.x`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/data/archives/msk316src.zip` & `swh.core-2.9.0/swh/core/tests/data/archives/msk316src.zip`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/data/archives/tokei-12.1.2.crate` & `swh.core-2.9.0/swh/core/tests/data/archives/tokei-12.1.2.crate`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/fixture/test_pytest_plugin.py` & `swh.core-2.9.0/swh/core/tests/fixture/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_cli.py` & `swh.core-2.9.0/swh/core/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_collections.py` & `swh.core-2.9.0/swh/core/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_config.py` & `swh.core-2.9.0/swh/core/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_logger.py` & `swh.core-2.9.0/swh/core/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_pytest_plugin.py` & `swh.core-2.9.0/swh/core/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_sentry.py` & `swh.core-2.9.0/swh/core/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_statsd.py` & `swh.core-2.9.0/swh/core/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_tarball.py` & `swh.core-2.9.0/swh/core/tests/test_tarball.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/tests/test_utils.py` & `swh.core-2.9.0/swh/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh/core/utils.py` & `swh.core-2.9.0/swh/core/utils.py`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh.core.egg-info/PKG-INFO` & `swh.core-2.9.0/swh.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 2.8.1
+Version: 2.9.0
 Summary: Software Heritage core utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DCORE/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-core
```

### Comparing `swh.core-2.8.1/swh.core.egg-info/SOURCES.txt` & `swh.core-2.9.0/swh.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/swh.core.egg-info/requires.txt` & `swh.core-2.9.0/swh.core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `swh.core-2.8.1/tox.ini` & `swh.core-2.9.0/tox.ini`

 * *Files identical despite different names*


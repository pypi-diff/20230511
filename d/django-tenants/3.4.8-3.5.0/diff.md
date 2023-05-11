# Comparing `tmp/django-tenants-3.4.8.tar.gz` & `tmp/django-tenants-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tenants-3.4.8.tar", last modified: Thu Feb  9 20:29:16 2023, max compression
+gzip compressed data, was "django-tenants-3.5.0.tar", last modified: Thu May 11 14:10:19 2023, max compression
```

## Comparing `django-tenants-3.4.8.tar` & `django-tenants-3.5.0.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.618485 django-tenants-3.4.8/
--rw-r--r--   0 tom        (501) staff       (20)     1024 2023-02-09 20:27:08.000000 django-tenants-3.4.8/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)      293 2023-02-09 20:27:08.000000 django-tenants-3.4.8/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)    10906 2023-02-09 20:29:16.618291 django-tenants-3.4.8/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     9849 2023-02-09 20:27:08.000000 django-tenants-3.4.8/README.rst
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.592252 django-tenants-3.4.8/django_tenants/
--rw-r--r--   0 tom        (501) staff       (20)       65 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      244 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/admin.py
--rw-r--r--   0 tom        (501) staff       (20)     2172 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/apps.py
--rw-r--r--   0 tom        (501) staff       (20)      510 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/cache.py
--rw-r--r--   0 tom        (501) staff       (20)    30396 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/clone.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.593347 django-tenants-3.4.8/django_tenants/files/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/files/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2759 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/files/storage.py
--rw-r--r--   0 tom        (501) staff       (20)      610 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/files/storages.py
--rw-r--r--   0 tom        (501) staff       (20)      474 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/log.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.593495 django-tenants-3.4.8/django_tenants/management/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.594853 django-tenants-3.4.8/django_tenants/management/commands/
--rw-r--r--   0 tom        (501) staff       (20)     6668 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1964 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/all_tenants_command.py
--rw-r--r--   0 tom        (501) staff       (20)     6365 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/clone_tenant.py
--rw-r--r--   0 tom        (501) staff       (20)      488 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/collectstatic_schemas.py
--rw-r--r--   0 tom        (501) staff       (20)      694 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/create_missing_schemas.py
--rw-r--r--   0 tom        (501) staff       (20)     5142 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/create_tenant.py
--rw-r--r--   0 tom        (501) staff       (20)      180 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/create_tenant_superuser.py
--rw-r--r--   0 tom        (501) staff       (20)     1218 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/delete_tenant.py
--rw-r--r--   0 tom        (501) staff       (20)      119 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/migrate.py
--rw-r--r--   0 tom        (501) staff       (20)     5855 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/migrate_schemas.py
--rw-r--r--   0 tom        (501) staff       (20)     1508 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/rename_schema.py
--rw-r--r--   0 tom        (501) staff       (20)     2019 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/management/commands/tenant_command.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.595458 django-tenants-3.4.8/django_tenants/middleware/
--rw-r--r--   0 tom        (501) staff       (20)      418 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/middleware/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1050 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/middleware/default.py
--rw-r--r--   0 tom        (501) staff       (20)     3548 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/middleware/main.py
--rw-r--r--   0 tom        (501) staff       (20)     3171 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/middleware/subfolder.py
--rw-r--r--   0 tom        (501) staff       (20)      601 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/middleware/suspicious.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.595914 django-tenants-3.4.8/django_tenants/migration_executors/
--rw-r--r--   0 tom        (501) staff       (20)      449 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/migration_executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2917 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/migration_executors/base.py
--rw-r--r--   0 tom        (501) staff       (20)     2857 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/migration_executors/multiproc.py
--rw-r--r--   0 tom        (501) staff       (20)     1000 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/migration_executors/standard.py
--rw-r--r--   0 tom        (501) staff       (20)     9842 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.596223 django-tenants-3.4.8/django_tenants/postgresql_backend/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/postgresql_backend/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     7545 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/postgresql_backend/base.py
--rw-r--r--   0 tom        (501) staff       (20)     2196 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/postgresql_backend/introspection.py
--rw-r--r--   0 tom        (501) staff       (20)     2173 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/routers.py
--rw-r--r--   0 tom        (501) staff       (20)     1008 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/signals.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.596526 django-tenants-3.4.8/django_tenants/staticfiles/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/staticfiles/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3552 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/staticfiles/finders.py
--rw-r--r--   0 tom        (501) staff       (20)     3106 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/staticfiles/storage.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.596637 django-tenants-3.4.8/django_tenants/template/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/template/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.596911 django-tenants-3.4.8/django_tenants/template/loaders/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/template/loaders/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      634 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/template/loaders/cached.py
--rw-r--r--   0 tom        (501) staff       (20)     1504 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/template/loaders/filesystem.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.586904 django-tenants-3.4.8/django_tenants/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.597126 django-tenants-3.4.8/django_tenants/templates/admin/
--rw-r--r--   0 tom        (501) staff       (20)     3032 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/templates/admin/app_list.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.587006 django-tenants-3.4.8/django_tenants/templates/admin/django_tenants/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.597233 django-tenants-3.4.8/django_tenants/templates/admin/django_tenants/tenant/
--rw-r--r--   0 tom        (501) staff       (20)      655 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/templates/admin/django_tenants/tenant/change_form.html
--rw-r--r--   0 tom        (501) staff       (20)     3860 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/templates/admin/index.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.597425 django-tenants-3.4.8/django_tenants/templatetags/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/templatetags/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1841 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/templatetags/tenant.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.597726 django-tenants-3.4.8/django_tenants/test/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/test/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5308 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/test/cases.py
--rw-r--r--   0 tom        (501) staff       (20)     1272 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/test/client.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.599152 django-tenants-3.4.8/django_tenants/tests/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      491 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_cache.py
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_fast_tenants.py
--rw-r--r--   0 tom        (501) staff       (20)      674 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_middleware.py
--rw-r--r--   0 tom        (501) staff       (20)     5629 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_multi_types.py
--rw-r--r--   0 tom        (501) staff       (20)     6403 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_routes.py
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_settings.py
--rw-r--r--   0 tom        (501) staff       (20)     1759 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_subfolder_case.py
--rw-r--r--   0 tom        (501) staff       (20)    28879 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_tenants.py
--rw-r--r--   0 tom        (501) staff       (20)     3123 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_urlresolvers.py
--rw-r--r--   0 tom        (501) staff       (20)     1898 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     1272 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/test_validation_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     1884 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/tests/testcases.py
--rw-r--r--   0 tom        (501) staff       (20)     3112 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/urlresolvers.py
--rw-r--r--   0 tom        (501) staff       (20)    10700 2023-02-09 20:27:08.000000 django-tenants-3.4.8/django_tenants/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.592910 django-tenants-3.4.8/django_tenants.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    10906 2023-02-09 20:29:16.000000 django-tenants-3.4.8/django_tenants.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    11813 2023-02-09 20:29:16.000000 django-tenants-3.4.8/django_tenants.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-09 20:29:16.000000 django-tenants-3.4.8/django_tenants.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-09 20:29:01.000000 django-tenants-3.4.8/django_tenants.egg-info/not-zip-safe
--rw-r--r--   0 tom        (501) staff       (20)       18 2023-02-09 20:29:16.000000 django-tenants-3.4.8/django_tenants.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       15 2023-02-09 20:29:16.000000 django-tenants-3.4.8/django_tenants.egg-info/top_level.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.600462 django-tenants-3.4.8/docs/
--rw-r--r--   0 tom        (501) staff       (20)     2995 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/Makefile
--rw-r--r--   0 tom        (501) staff       (20)     6524 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/conf.py
--rw-r--r--   0 tom        (501) staff       (20)      405 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/credits.rst
--rw-r--r--   0 tom        (501) staff       (20)     1154 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/examples.rst
--rw-r--r--   0 tom        (501) staff       (20)     9096 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/files.rst
--rw-r--r--   0 tom        (501) staff       (20)     4872 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/index.rst
--rw-r--r--   0 tom        (501) staff       (20)    12780 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/install.rst
--rw-r--r--   0 tom        (501) staff       (20)      301 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/involved.rst
--rw-r--r--   0 tom        (501) staff       (20)      666 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/links.rst
--rw-r--r--   0 tom        (501) staff       (20)      105 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/requirements.txt
--rw-r--r--   0 tom        (501) staff       (20)     5310 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/test.rst
--rw-r--r--   0 tom        (501) staff       (20)    20988 2023-02-09 20:27:08.000000 django-tenants-3.4.8/docs/use.rst
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.600596 django-tenants-3.4.8/dts_test_project/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.600802 django-tenants-3.4.8/dts_test_project/customers/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/customers/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.601011 django-tenants-3.4.8/dts_test_project/customers/migrations/
--rw-r--r--   0 tom        (501) staff       (20)     1524 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/customers/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/customers/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      772 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/customers/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.601205 django-tenants-3.4.8/dts_test_project/dts_multi_type2/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_multi_type2/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.601434 django-tenants-3.4.8/dts_test_project/dts_multi_type2/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      423 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_multi_type2/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_multi_type2/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      249 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_multi_type2/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.601610 django-tenants-3.4.8/dts_test_project/dts_test_app/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.601821 django-tenants-3.4.8/dts_test_project/dts_test_app/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      868 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      422 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.587814 django-tenants-3.4.8/dts_test_project/dts_test_app/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.602036 django-tenants-3.4.8/dts_test_project/dts_test_app/static/css/
--rw-r--r--   0 tom        (501) staff       (20)       45 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/static/css/global.css
--rw-r--r--   0 tom        (501) staff       (20)       54 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/static/css/project.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.602148 django-tenants-3.4.8/dts_test_project/dts_test_app/templates/
--rw-r--r--   0 tom        (501) staff       (20)      232 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/templates/index.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.588211 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.588139 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/other/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.588078 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/other/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.602258 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/other/static/css/
--rw-r--r--   0 tom        (501) staff       (20)       34 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/other/static/css/project.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.602364 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/other/templates/
--rw-r--r--   0 tom        (501) staff       (20)      227 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/other/templates/index.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.588350 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/test/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.588290 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/test/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.602482 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/test/static/css/
--rw-r--r--   0 tom        (501) staff       (20)       33 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/test/static/css/project.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.602591 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/test/templates/
--rw-r--r--   0 tom        (501) staff       (20)      226 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_app/tenants/test/templates/index.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.602896 django-tenants-3.4.8/dts_test_project/dts_test_project/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_project/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3621 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_project/settings.py
--rw-r--r--   0 tom        (501) staff       (20)      298 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/dts_test_project/urls.py
--rw-r--r--   0 tom        (501) staff       (20)      259 2023-02-09 20:27:08.000000 django-tenants-3.4.8/dts_test_project/manage.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.589980 django-tenants-3.4.8/examples/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.603001 django-tenants-3.4.8/examples/tenant_multi_types/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.603416 django-tenants-3.4.8/examples/tenant_multi_types/customers/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      276 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/admin.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.603950 django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/
--rw-r--r--   0 tom        (501) staff       (20)     1005 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)     1042 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/0002_auto_20171207_1616.py
--rw-r--r--   0 tom        (501) staff       (20)      713 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/0003_auto_20190404_1612.py
--rw-r--r--   0 tom        (501) staff       (20)      508 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/0004_client_type.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      495 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/models.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/customers/views.py
--rw-r--r--   0 tom        (501) staff       (20)      270 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/manage.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.604563 django-tenants-3.4.8/examples/tenant_multi_types/templates/
--rw-r--r--   0 tom        (501) staff       (20)     2693 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/templates/base.html
--rw-r--r--   0 tom        (501) staff       (20)     6804 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/templates/index_public.html
--rw-r--r--   0 tom        (501) staff       (20)      605 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/templates/index_tenant.html
--rw-r--r--   0 tom        (501) staff       (20)       82 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/templates/index_type_2.html
--rw-r--r--   0 tom        (501) staff       (20)      869 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/templates/random_form.html
--rw-r--r--   0 tom        (501) staff       (20)      676 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/templates/upload_file.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.605635 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      133 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/context_processors.py
--rw-r--r--   0 tom        (501) staff       (20)      544 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/middleware.py
--rw-r--r--   0 tom        (501) staff       (20)      203 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/set_tenant_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     8261 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/settings.py
--rw-r--r--   0 tom        (501) staff       (20)      244 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_public.py
--rw-r--r--   0 tom        (501) staff       (20)      563 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_type1.py
--rw-r--r--   0 tom        (501) staff       (20)      236 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_type2.py
--rw-r--r--   0 tom        (501) staff       (20)     1029 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/views.py
--rw-r--r--   0 tom        (501) staff       (20)     1482 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/wsgi.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.606267 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      105 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.606479 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      489 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      108 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/models.py
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/tests.py
--rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_both/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.607187 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      245 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      105 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/apps.py
--rw-r--r--   0 tom        (501) staff       (20)       73 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/forms.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.607295 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/management/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/management/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.607490 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/management/commands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/management/commands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      409 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/management/commands/dtest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.607706 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/migrations/
--rw-r--r--   0 tom        (501) staff       (20)     1228 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      339 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/models.py
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/tests.py
--rw-r--r--   0 tom        (501) staff       (20)     2554 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.608330 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      183 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      112 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.608606 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      494 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      113 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/models.py
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/tests.py
--rw-r--r--   0 tom        (501) staff       (20)      127 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_two_only/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.608742 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.609424 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      276 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/admin.py
--rw-r--r--   0 tom        (501) staff       (20)       73 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/forms.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.610023 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/
--rw-r--r--   0 tom        (501) staff       (20)     1005 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)     1042 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/0002_auto_20171207_1616.py
--rw-r--r--   0 tom        (501) staff       (20)      713 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/0003_auto_20190404_1612.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      359 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/models.py
--rw-r--r--   0 tom        (501) staff       (20)     2502 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/views.py
--rw-r--r--   0 tom        (501) staff       (20)      268 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/manage.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.610718 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/
--rw-r--r--   0 tom        (501) staff       (20)     2693 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/base.html
--rw-r--r--   0 tom        (501) staff       (20)     6804 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/index_public.html
--rw-r--r--   0 tom        (501) staff       (20)      605 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/index_tenant.html
--rw-r--r--   0 tom        (501) staff       (20)      869 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/random_form.html
--rw-r--r--   0 tom        (501) staff       (20)      676 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/upload_file.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.611569 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      236 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/admin.py
--rw-r--r--   0 tom        (501) staff       (20)       96 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.611713 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/management/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/management/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.611954 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/management/commands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/management/commands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      409 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/management/commands/dtest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.612385 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      923 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)      521 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/migrations/0002_uploadfile.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      339 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/models.py
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/tests.py
--rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.613283 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      133 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/context_processors.py
--rw-r--r--   0 tom        (501) staff       (20)     7160 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/settings.py
--rw-r--r--   0 tom        (501) staff       (20)      242 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/urls_public.py
--rw-r--r--   0 tom        (501) staff       (20)      552 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/urls_tenants.py
--rw-r--r--   0 tom        (501) staff       (20)     1029 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/views.py
--rw-r--r--   0 tom        (501) staff       (20)     1476 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/wsgi.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.613404 django-tenants-3.4.8/examples/tenant_tutorial/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.614189 django-tenants-3.4.8/examples/tenant_tutorial/customers/
--rw-r--r--   0 tom        (501) staff       (20)       54 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      276 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      221 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/apps.py
--rw-r--r--   0 tom        (501) staff       (20)       73 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/forms.py
--rwxr-xr-x   0 tom        (501) staff       (20)     1069 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/handlers.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.614709 django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/
--rw-r--r--   0 tom        (501) staff       (20)     1005 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)     1042 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/0002_auto_20171207_1616.py
--rw-r--r--   0 tom        (501) staff       (20)      713 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/0003_auto_20190404_1612.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      359 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/models.py
--rw-r--r--   0 tom        (501) staff       (20)     2502 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/customers/views.py
--rw-r--r--   0 tom        (501) staff       (20)      258 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/manage.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.615380 django-tenants-3.4.8/examples/tenant_tutorial/templates/
--rw-r--r--   0 tom        (501) staff       (20)     2247 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/templates/base.html
--rw-r--r--   0 tom        (501) staff       (20)     6804 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/templates/index_public.html
--rw-r--r--   0 tom        (501) staff       (20)      605 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/templates/index_tenant.html
--rw-r--r--   0 tom        (501) staff       (20)      869 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/templates/random_form.html
--rw-r--r--   0 tom        (501) staff       (20)      676 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/templates/upload_file.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.616245 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      236 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/admin.py
--rw-r--r--   0 tom        (501) staff       (20)       96 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.616376 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/management/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/management/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.616659 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/management/commands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/management/commands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      409 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/management/commands/dtest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.617091 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      923 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)      521 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/migrations/0002_uploadfile.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      339 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/models.py
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/tests.py
--rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-02-09 20:29:16.618080 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      544 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/middleware.py
--rw-r--r--   0 tom        (501) staff       (20)     6991 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/settings.py
--rw-r--r--   0 tom        (501) staff       (20)      232 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/urls_public.py
--rw-r--r--   0 tom        (501) staff       (20)      552 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/urls_tenants.py
--rw-r--r--   0 tom        (501) staff       (20)     1029 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/views.py
--rw-r--r--   0 tom        (501) staff       (20)     1446 2023-02-09 20:27:08.000000 django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/wsgi.py
--rw-r--r--   0 tom        (501) staff       (20)       59 2023-02-09 20:27:08.000000 django-tenants-3.4.8/requirements.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-02-09 20:29:16.618528 django-tenants-3.4.8/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     1971 2023-02-09 20:29:13.000000 django-tenants-3.4.8/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.629073 django-tenants-3.5.0/
+-rw-r--r--   0 tom        (501) staff       (20)     1024 2023-02-09 20:27:08.000000 django-tenants-3.5.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)      293 2023-02-09 20:27:08.000000 django-tenants-3.5.0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)    10945 2023-05-11 14:10:19.628859 django-tenants-3.5.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     9849 2023-02-09 20:27:08.000000 django-tenants-3.5.0/README.rst
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.584005 django-tenants-3.5.0/django_tenants/
+-rw-r--r--   0 tom        (501) staff       (20)       65 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      244 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)     2172 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)      510 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/cache.py
+-rw-r--r--   0 tom        (501) staff       (20)    30396 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/clone.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.586985 django-tenants-3.5.0/django_tenants/files/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/files/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2759 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/files/storage.py
+-rw-r--r--   0 tom        (501) staff       (20)      610 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/files/storages.py
+-rw-r--r--   0 tom        (501) staff       (20)      474 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/log.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.587248 django-tenants-3.5.0/django_tenants/management/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.591565 django-tenants-3.5.0/django_tenants/management/commands/
+-rw-r--r--   0 tom        (501) staff       (20)     6668 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1964 2023-05-11 14:07:12.000000 django-tenants-3.5.0/django_tenants/management/commands/all_tenants_command.py
+-rw-r--r--   0 tom        (501) staff       (20)     6365 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/clone_tenant.py
+-rw-r--r--   0 tom        (501) staff       (20)      488 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/collectstatic_schemas.py
+-rw-r--r--   0 tom        (501) staff       (20)      694 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/create_missing_schemas.py
+-rw-r--r--   0 tom        (501) staff       (20)     5142 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/create_tenant.py
+-rw-r--r--   0 tom        (501) staff       (20)      180 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/create_tenant_superuser.py
+-rw-r--r--   0 tom        (501) staff       (20)     1218 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/delete_tenant.py
+-rw-r--r--   0 tom        (501) staff       (20)      119 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/migrate.py
+-rw-r--r--   0 tom        (501) staff       (20)     5855 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/migrate_schemas.py
+-rw-r--r--   0 tom        (501) staff       (20)     1508 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/management/commands/rename_schema.py
+-rw-r--r--   0 tom        (501) staff       (20)     2304 2023-05-11 14:07:12.000000 django-tenants-3.5.0/django_tenants/management/commands/tenant_command.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.592982 django-tenants-3.5.0/django_tenants/middleware/
+-rw-r--r--   0 tom        (501) staff       (20)      418 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/middleware/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1050 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/middleware/default.py
+-rw-r--r--   0 tom        (501) staff       (20)     3548 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/middleware/main.py
+-rw-r--r--   0 tom        (501) staff       (20)     3171 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/middleware/subfolder.py
+-rw-r--r--   0 tom        (501) staff       (20)      601 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/middleware/suspicious.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.593775 django-tenants-3.5.0/django_tenants/migration_executors/
+-rw-r--r--   0 tom        (501) staff       (20)      449 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/migration_executors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2917 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/migration_executors/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     2857 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/migration_executors/multiproc.py
+-rw-r--r--   0 tom        (501) staff       (20)     1000 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/migration_executors/standard.py
+-rw-r--r--   0 tom        (501) staff       (20)     9842 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.594318 django-tenants-3.5.0/django_tenants/postgresql_backend/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/postgresql_backend/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     7721 2023-05-11 14:07:12.000000 django-tenants-3.5.0/django_tenants/postgresql_backend/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     2283 2023-05-11 14:07:12.000000 django-tenants-3.5.0/django_tenants/postgresql_backend/introspection.py
+-rw-r--r--   0 tom        (501) staff       (20)     2173 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/routers.py
+-rw-r--r--   0 tom        (501) staff       (20)     1008 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/signals.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.594863 django-tenants-3.5.0/django_tenants/staticfiles/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/staticfiles/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3552 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/staticfiles/finders.py
+-rw-r--r--   0 tom        (501) staff       (20)     3106 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/staticfiles/storage.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.595044 django-tenants-3.5.0/django_tenants/template/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/template/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.595562 django-tenants-3.5.0/django_tenants/template/loaders/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/template/loaders/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      634 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/template/loaders/cached.py
+-rw-r--r--   0 tom        (501) staff       (20)     1504 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/template/loaders/filesystem.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.571345 django-tenants-3.5.0/django_tenants/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.595949 django-tenants-3.5.0/django_tenants/templates/admin/
+-rw-r--r--   0 tom        (501) staff       (20)     3032 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/templates/admin/app_list.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.571580 django-tenants-3.5.0/django_tenants/templates/admin/django_tenants/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.596126 django-tenants-3.5.0/django_tenants/templates/admin/django_tenants/tenant/
+-rw-r--r--   0 tom        (501) staff       (20)      655 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/templates/admin/django_tenants/tenant/change_form.html
+-rw-r--r--   0 tom        (501) staff       (20)     3860 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/templates/admin/index.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.596439 django-tenants-3.5.0/django_tenants/templatetags/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/templatetags/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1841 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/templatetags/tenant.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.596950 django-tenants-3.5.0/django_tenants/test/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/test/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5308 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/test/cases.py
+-rw-r--r--   0 tom        (501) staff       (20)     1272 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/test/client.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.599265 django-tenants-3.5.0/django_tenants/tests/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      491 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_cache.py
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_fast_tenants.py
+-rw-r--r--   0 tom        (501) staff       (20)      674 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_middleware.py
+-rw-r--r--   0 tom        (501) staff       (20)     5629 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_multi_types.py
+-rw-r--r--   0 tom        (501) staff       (20)     6403 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_routes.py
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_settings.py
+-rw-r--r--   0 tom        (501) staff       (20)     1759 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_subfolder_case.py
+-rw-r--r--   0 tom        (501) staff       (20)    29048 2023-05-11 14:07:12.000000 django-tenants-3.5.0/django_tenants/tests/test_tenants.py
+-rw-r--r--   0 tom        (501) staff       (20)     3123 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_urlresolvers.py
+-rw-r--r--   0 tom        (501) staff       (20)     1898 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     1272 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/test_validation_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     1884 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/tests/testcases.py
+-rw-r--r--   0 tom        (501) staff       (20)     3112 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/urlresolvers.py
+-rw-r--r--   0 tom        (501) staff       (20)    10700 2023-02-09 20:27:08.000000 django-tenants-3.5.0/django_tenants/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.585885 django-tenants-3.5.0/django_tenants.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    10945 2023-05-11 14:10:19.000000 django-tenants-3.5.0/django_tenants.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    11813 2023-05-11 14:10:19.000000 django-tenants-3.5.0/django_tenants.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-11 14:10:19.000000 django-tenants-3.5.0/django_tenants.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-09 20:29:01.000000 django-tenants-3.5.0/django_tenants.egg-info/not-zip-safe
+-rw-r--r--   0 tom        (501) staff       (20)       17 2023-05-11 14:10:19.000000 django-tenants-3.5.0/django_tenants.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       15 2023-05-11 14:10:19.000000 django-tenants-3.5.0/django_tenants.egg-info/top_level.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.601419 django-tenants-3.5.0/docs/
+-rw-r--r--   0 tom        (501) staff       (20)     2995 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/Makefile
+-rw-r--r--   0 tom        (501) staff       (20)     6524 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/conf.py
+-rw-r--r--   0 tom        (501) staff       (20)      405 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/credits.rst
+-rw-r--r--   0 tom        (501) staff       (20)     1154 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/examples.rst
+-rw-r--r--   0 tom        (501) staff       (20)     9096 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/files.rst
+-rw-r--r--   0 tom        (501) staff       (20)     4872 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/index.rst
+-rw-r--r--   0 tom        (501) staff       (20)    12780 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/install.rst
+-rw-r--r--   0 tom        (501) staff       (20)      301 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/involved.rst
+-rw-r--r--   0 tom        (501) staff       (20)      666 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/links.rst
+-rw-r--r--   0 tom        (501) staff       (20)      105 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/requirements.txt
+-rw-r--r--   0 tom        (501) staff       (20)     5310 2023-02-09 20:27:08.000000 django-tenants-3.5.0/docs/test.rst
+-rw-r--r--   0 tom        (501) staff       (20)    21490 2023-05-11 14:07:12.000000 django-tenants-3.5.0/docs/use.rst
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.601612 django-tenants-3.5.0/dts_test_project/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.601956 django-tenants-3.5.0/dts_test_project/customers/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/customers/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.602312 django-tenants-3.5.0/dts_test_project/customers/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)     1524 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/customers/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/customers/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      772 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/customers/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.602618 django-tenants-3.5.0/dts_test_project/dts_multi_type2/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_multi_type2/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.603012 django-tenants-3.5.0/dts_test_project/dts_multi_type2/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      423 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_multi_type2/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_multi_type2/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      249 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_multi_type2/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.603401 django-tenants-3.5.0/dts_test_project/dts_test_app/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.603787 django-tenants-3.5.0/dts_test_project/dts_test_app/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      868 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      422 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.573354 django-tenants-3.5.0/dts_test_project/dts_test_app/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.604131 django-tenants-3.5.0/dts_test_project/dts_test_app/static/css/
+-rw-r--r--   0 tom        (501) staff       (20)       45 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/static/css/global.css
+-rw-r--r--   0 tom        (501) staff       (20)       54 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/static/css/project.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.604329 django-tenants-3.5.0/dts_test_project/dts_test_app/templates/
+-rw-r--r--   0 tom        (501) staff       (20)      232 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/templates/index.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.574276 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.574143 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/other/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.573905 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/other/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.604539 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/other/static/css/
+-rw-r--r--   0 tom        (501) staff       (20)       34 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/other/static/css/project.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.604716 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/other/templates/
+-rw-r--r--   0 tom        (501) staff       (20)      227 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/other/templates/index.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.574678 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/test/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.574547 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/test/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.604896 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/test/static/css/
+-rw-r--r--   0 tom        (501) staff       (20)       33 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/test/static/css/project.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.605072 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/test/templates/
+-rw-r--r--   0 tom        (501) staff       (20)      226 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_app/tenants/test/templates/index.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.605568 django-tenants-3.5.0/dts_test_project/dts_test_project/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_project/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3621 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_project/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)      298 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/dts_test_project/urls.py
+-rw-r--r--   0 tom        (501) staff       (20)      259 2023-02-09 20:27:08.000000 django-tenants-3.5.0/dts_test_project/manage.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.577723 django-tenants-3.5.0/examples/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.605750 django-tenants-3.5.0/examples/tenant_multi_types/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.606424 django-tenants-3.5.0/examples/tenant_multi_types/customers/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      276 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/admin.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.607305 django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)     1005 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)     1042 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/0002_auto_20171207_1616.py
+-rw-r--r--   0 tom        (501) staff       (20)      713 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/0003_auto_20190404_1612.py
+-rw-r--r--   0 tom        (501) staff       (20)      508 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/0004_client_type.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      495 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/models.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/customers/views.py
+-rw-r--r--   0 tom        (501) staff       (20)      270 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/manage.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.608382 django-tenants-3.5.0/examples/tenant_multi_types/templates/
+-rw-r--r--   0 tom        (501) staff       (20)     2693 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/templates/base.html
+-rw-r--r--   0 tom        (501) staff       (20)     6804 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/templates/index_public.html
+-rw-r--r--   0 tom        (501) staff       (20)      605 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/templates/index_tenant.html
+-rw-r--r--   0 tom        (501) staff       (20)       82 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/templates/index_type_2.html
+-rw-r--r--   0 tom        (501) staff       (20)      869 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/templates/random_form.html
+-rw-r--r--   0 tom        (501) staff       (20)      676 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/templates/upload_file.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.610087 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      133 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/context_processors.py
+-rw-r--r--   0 tom        (501) staff       (20)      544 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/middleware.py
+-rw-r--r--   0 tom        (501) staff       (20)      203 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/set_tenant_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     8261 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)      244 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_public.py
+-rw-r--r--   0 tom        (501) staff       (20)      563 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_type1.py
+-rw-r--r--   0 tom        (501) staff       (20)      236 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_type2.py
+-rw-r--r--   0 tom        (501) staff       (20)     1029 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/views.py
+-rw-r--r--   0 tom        (501) staff       (20)     1482 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/wsgi.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.611180 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      105 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.611536 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      489 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      108 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/models.py
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_both/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.612749 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      245 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      105 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)       73 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/forms.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.612933 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/management/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/management/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.613275 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/management/commands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/management/commands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      409 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/management/commands/dtest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.613694 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)     1228 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      339 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/models.py
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)     2554 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.614817 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      183 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      112 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.615215 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      494 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      113 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/models.py
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)      127 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_two_only/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.615404 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.616407 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      276 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)       73 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/forms.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.617238 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)     1005 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)     1042 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/0002_auto_20171207_1616.py
+-rw-r--r--   0 tom        (501) staff       (20)      713 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/0003_auto_20190404_1612.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      359 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/models.py
+-rw-r--r--   0 tom        (501) staff       (20)     2502 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/views.py
+-rw-r--r--   0 tom        (501) staff       (20)      268 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/manage.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.618232 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/
+-rw-r--r--   0 tom        (501) staff       (20)     2693 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/base.html
+-rw-r--r--   0 tom        (501) staff       (20)     6804 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/index_public.html
+-rw-r--r--   0 tom        (501) staff       (20)      605 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/index_tenant.html
+-rw-r--r--   0 tom        (501) staff       (20)      869 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/random_form.html
+-rw-r--r--   0 tom        (501) staff       (20)      676 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/upload_file.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.619382 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      236 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)       96 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.619557 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/management/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/management/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.619918 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/management/commands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/management/commands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      409 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/management/commands/dtest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.620480 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      923 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)      521 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/migrations/0002_uploadfile.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      339 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/models.py
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.621782 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      133 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/context_processors.py
+-rw-r--r--   0 tom        (501) staff       (20)     7160 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)      242 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/urls_public.py
+-rw-r--r--   0 tom        (501) staff       (20)      552 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/urls_tenants.py
+-rw-r--r--   0 tom        (501) staff       (20)     1029 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/views.py
+-rw-r--r--   0 tom        (501) staff       (20)     1476 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/wsgi.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.621979 django-tenants-3.5.0/examples/tenant_tutorial/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.623375 django-tenants-3.5.0/examples/tenant_tutorial/customers/
+-rw-r--r--   0 tom        (501) staff       (20)       54 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      276 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      221 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)       73 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/forms.py
+-rwxr-xr-x   0 tom        (501) staff       (20)     1069 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/handlers.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.624191 django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)     1005 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)     1042 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/0002_auto_20171207_1616.py
+-rw-r--r--   0 tom        (501) staff       (20)      713 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/0003_auto_20190404_1612.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      359 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/models.py
+-rw-r--r--   0 tom        (501) staff       (20)     2502 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/customers/views.py
+-rw-r--r--   0 tom        (501) staff       (20)      258 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/manage.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.625080 django-tenants-3.5.0/examples/tenant_tutorial/templates/
+-rw-r--r--   0 tom        (501) staff       (20)     2247 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/templates/base.html
+-rw-r--r--   0 tom        (501) staff       (20)     6804 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/templates/index_public.html
+-rw-r--r--   0 tom        (501) staff       (20)      605 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/templates/index_tenant.html
+-rw-r--r--   0 tom        (501) staff       (20)      869 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/templates/random_form.html
+-rw-r--r--   0 tom        (501) staff       (20)      676 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/templates/upload_file.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.626200 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      236 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)       96 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.626398 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/management/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/management/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.626717 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/management/commands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/management/commands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      409 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/management/commands/dtest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.627280 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      923 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)      521 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/migrations/0002_uploadfile.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      339 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/models.py
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)       63 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-11 14:10:19.628573 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      544 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/middleware.py
+-rw-r--r--   0 tom        (501) staff       (20)     6991 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)      232 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/urls_public.py
+-rw-r--r--   0 tom        (501) staff       (20)      552 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/urls_tenants.py
+-rw-r--r--   0 tom        (501) staff       (20)     1029 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/views.py
+-rw-r--r--   0 tom        (501) staff       (20)     1446 2023-02-09 20:27:08.000000 django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/wsgi.py
+-rw-r--r--   0 tom        (501) staff       (20)       59 2023-05-11 14:07:12.000000 django-tenants-3.5.0/requirements.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-11 14:10:19.629117 django-tenants-3.5.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2007 2023-05-11 14:10:14.000000 django-tenants-3.5.0/setup.py
```

### Comparing `django-tenants-3.4.8/LICENSE` & `django-tenants-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/PKG-INFO` & `django-tenants-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tenants
-Version: 3.4.8
+Version: 3.5.0
 Summary: Tenant support for Django using PostgreSQL schemas.
 Home-page: https://github.com/django-tenants/django-tenants
 Author: Thomas Turner
 Author-email: tom@twt.me.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
```

### Comparing `django-tenants-3.4.8/README.rst` & `django-tenants-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/apps.py` & `django-tenants-3.5.0/django_tenants/apps.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/clone.py` & `django-tenants-3.5.0/django_tenants/clone.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/files/storage.py` & `django-tenants-3.5.0/django_tenants/files/storage.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/files/storages.py` & `django-tenants-3.5.0/django_tenants/files/storages.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/__init__.py` & `django-tenants-3.5.0/django_tenants/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/all_tenants_command.py` & `django-tenants-3.5.0/django_tenants/management/commands/all_tenants_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         parser.add_argument('command_name', nargs='+', help='The command name you want to run')
 
     def run_from_argv(self, argv):
         """
         Changes the option_list to use the options from the wrapped command.
         """
         # load the command object.
-        if len(argv) <= 3:
+        if len(argv) <= 2:
             return
         
         no_public = "--no-public" in argv
         
         command_args = [argv[0]]
         
         command_args.extend(argv[3:] if no_public else argv[2:])
```

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/clone_tenant.py` & `django-tenants-3.5.0/django_tenants/management/commands/clone_tenant.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/create_missing_schemas.py` & `django-tenants-3.5.0/django_tenants/management/commands/create_missing_schemas.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/create_tenant.py` & `django-tenants-3.5.0/django_tenants/management/commands/create_tenant.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/delete_tenant.py` & `django-tenants-3.5.0/django_tenants/management/commands/delete_tenant.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/migrate_schemas.py` & `django-tenants-3.5.0/django_tenants/management/commands/migrate_schemas.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/rename_schema.py` & `django-tenants-3.5.0/django_tenants/management/commands/rename_schema.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/management/commands/tenant_command.py` & `django-tenants-3.5.0/django_tenants/management/commands/tenant_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,8 +45,17 @@
         tenant = self.get_tenant_from_options_or_interactive(schema_name=schema_namespace.schema_name)
         connection.set_tenant(tenant)
         klass.run_from_argv(args)
 
     def handle(self, *args, **options):
         tenant = self.get_tenant_from_options_or_interactive(**options)
         connection.set_tenant(tenant)
-        call_command(*args, **options)
+
+        # options comes including {"command_name": ["x", "y"]}
+        # Incase of multiple argument passed.
+
+        command_name = options.pop("command_name")
+
+        if isinstance(command_name, list):
+            call_command(command_name[0], *command_name[1:])
+        else:
+            call_command(*args, **options)
```

### Comparing `django-tenants-3.4.8/django_tenants/middleware/default.py` & `django-tenants-3.5.0/django_tenants/middleware/default.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/middleware/main.py` & `django-tenants-3.5.0/django_tenants/middleware/main.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/middleware/subfolder.py` & `django-tenants-3.5.0/django_tenants/middleware/subfolder.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/middleware/suspicious.py` & `django-tenants-3.5.0/django_tenants/middleware/suspicious.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/migration_executors/base.py` & `django-tenants-3.5.0/django_tenants/migration_executors/base.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/migration_executors/multiproc.py` & `django-tenants-3.5.0/django_tenants/migration_executors/multiproc.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/migration_executors/standard.py` & `django-tenants-3.5.0/django_tenants/migration_executors/standard.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/models.py` & `django-tenants-3.5.0/django_tenants/models.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/postgresql_backend/base.py` & `django-tenants-3.5.0/django_tenants/postgresql_backend/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,28 @@
 from django.utils.module_loading import import_string
 
 from django_tenants.postgresql_backend.introspection import DatabaseSchemaIntrospection
 from django_tenants.utils import get_public_schema_name, get_limit_set_calls
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 import django.db.utils
-import psycopg2
+
+try:
+     from django.db.backends.postgresql.psycopg_any import is_psycopg3
+except ImportError:
+    is_psycopg3 = False
+
+if is_psycopg3:
+    import psycopg
+else:
+    import psycopg2 as psycopg
 
 
 DatabaseError = django.db.utils.DatabaseError
-IntegrityError = psycopg2.IntegrityError
+IntegrityError = psycopg.IntegrityError
 
 ORIGINAL_BACKEND = getattr(settings, 'ORIGINAL_BACKEND', 'django.db.backends.postgresql')
 
 original_backend = import_module(ORIGINAL_BACKEND + '.base')
 
 EXTRA_SEARCH_PATHS = getattr(settings, 'PG_EXTRA_SEARCH_PATHS', [])
 
@@ -156,15 +165,15 @@
             # In the event that an error already happened in this transaction and we are going
             # to rollback we should just ignore database error when setting the search_path
             # if the next instruction is not a rollback it will just fail also, so
             # we do not have to worry that it's not the good one
             try:
                 formatted_search_paths = ['\'{}\''.format(s) for s in search_paths]
                 cursor_for_search_path.execute('SET search_path = {0}'.format(','.join(formatted_search_paths)))
-            except (django.db.utils.DatabaseError, psycopg2.InternalError):
+            except (django.db.utils.DatabaseError, psycopg.InternalError):
                 self.search_path_set_schemas = None
             else:
                 self.search_path_set_schemas = search_paths
             if name:
                 cursor_for_search_path.close()
         return cursor
```

### Comparing `django-tenants-3.4.8/django_tenants/postgresql_backend/introspection.py` & `django-tenants-3.5.0/django_tenants/postgresql_backend/introspection.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,23 @@
     def __init__(self, cursor, connection):
         self.cursor = cursor
         self.connection = connection
         self.original_search_path = None
 
     def __enter__(self):
         self.cursor.execute('SHOW search_path')
-        self.original_search_path = self.cursor.fetchone()[0].split(',')
+        self.original_search_path = [
+            search_path.strip().replace('"', '')
+            for search_path in self.cursor.fetchone()[0].split(',')
+        ]
         self.cursor.execute(f"SET search_path = '{self.connection.schema_name}'")
 
     def __exit__(self, *args, **kwargs):
         formatted_search_paths = ', '.join(
-            f"'{search_path.strip()}'"
+            f"'{search_path}'"
             for search_path in self.original_search_path
         )
         self.cursor.execute(f'SET search_path = {formatted_search_paths}')
 
 
 class DatabaseSchemaIntrospection(DatabaseIntrospection):
     """
```

### Comparing `django-tenants-3.4.8/django_tenants/routers.py` & `django-tenants-3.5.0/django_tenants/routers.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/signals.py` & `django-tenants-3.5.0/django_tenants/signals.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/staticfiles/finders.py` & `django-tenants-3.5.0/django_tenants/staticfiles/finders.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/staticfiles/storage.py` & `django-tenants-3.5.0/django_tenants/staticfiles/storage.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/template/loaders/cached.py` & `django-tenants-3.5.0/django_tenants/template/loaders/cached.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/template/loaders/filesystem.py` & `django-tenants-3.5.0/django_tenants/template/loaders/filesystem.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/templates/admin/app_list.html` & `django-tenants-3.5.0/django_tenants/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/templates/admin/django_tenants/tenant/change_form.html` & `django-tenants-3.5.0/django_tenants/templates/admin/django_tenants/tenant/change_form.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/templates/admin/index.html` & `django-tenants-3.5.0/django_tenants/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/templatetags/tenant.py` & `django-tenants-3.5.0/django_tenants/templatetags/tenant.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/test/cases.py` & `django-tenants-3.5.0/django_tenants/test/cases.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/test/client.py` & `django-tenants-3.5.0/django_tenants/test/client.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_fast_tenants.py` & `django-tenants-3.5.0/django_tenants/tests/test_fast_tenants.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_middleware.py` & `django-tenants-3.5.0/django_tenants/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_multi_types.py` & `django-tenants-3.5.0/django_tenants/tests/test_multi_types.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_routes.py` & `django-tenants-3.5.0/django_tenants/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_settings.py` & `django-tenants-3.5.0/django_tenants/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_subfolder_case.py` & `django-tenants-3.5.0/django_tenants/tests/test_subfolder_case.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_tenants.py` & `django-tenants-3.5.0/django_tenants/tests/test_tenants.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,23 +160,27 @@
 
         # test if data is still there
         self.assertEqual(DummyModel.objects.count(), 2)
 
         self.created = [domain, tenant]
 
     def test_switching_search_path(self):
-        tenant1 = get_tenant_model()(schema_name='tenant1')
+        """
+        IMPORTANT: using schema_name with underscore here. See
+        https://github.com/django-tenants/django-tenants/pull/829
+        """
+        tenant1 = get_tenant_model()(schema_name='tenant`1')
         tenant1.save()
 
         domain1 = get_tenant_domain_model()(tenant=tenant1, domain='something.test.com')
         domain1.save()
 
         connection.set_schema_to_public()
 
-        tenant2 = get_tenant_model()(schema_name='tenant2')
+        tenant2 = get_tenant_model()(schema_name='Tenant_2')
         tenant2.save()
 
         domain2 = get_tenant_domain_model()(tenant=tenant2, domain='example.com')
         domain2.save()
 
         # go to tenant1's path
         connection.set_tenant(tenant1)
@@ -306,15 +310,15 @@
 
         self.assertTrue(schema_exists(tenant.schema_name))
 
         self.created = [tenant]
 
     def test_tenant_schema_creation_with_special_chars(self):
         """Tests using special characters in schema name."""
-        schema_names = ('test-hyphen', 'test@at', 'test`backtick')
+        schema_names = ('test-hyphen', 'test@at', 'test`backtick', 'country_BD')
 
         Client = get_tenant_model()
         for schema_name in schema_names:
             tenant = Client(schema_name=schema_name)
             tenant.save()
             self.assertTrue(schema_exists(tenant.schema_name))
```

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_urlresolvers.py` & `django-tenants-3.5.0/django_tenants/tests/test_urlresolvers.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_utils.py` & `django-tenants-3.5.0/django_tenants/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/test_validation_utils.py` & `django-tenants-3.5.0/django_tenants/tests/test_validation_utils.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/tests/testcases.py` & `django-tenants-3.5.0/django_tenants/tests/testcases.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/urlresolvers.py` & `django-tenants-3.5.0/django_tenants/urlresolvers.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants/utils.py` & `django-tenants-3.5.0/django_tenants/utils.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/django_tenants.egg-info/PKG-INFO` & `django-tenants-3.5.0/django_tenants.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tenants
-Version: 3.4.8
+Version: 3.5.0
 Summary: Tenant support for Django using PostgreSQL schemas.
 Home-page: https://github.com/django-tenants/django-tenants
 Author: Thomas Turner
 Author-email: tom@twt.me.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
```

### Comparing `django-tenants-3.4.8/django_tenants.egg-info/SOURCES.txt` & `django-tenants-3.5.0/django_tenants.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/Makefile` & `django-tenants-3.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/conf.py` & `django-tenants-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/examples.rst` & `django-tenants-3.5.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/files.rst` & `django-tenants-3.5.0/docs/files.rst`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/index.rst` & `django-tenants-3.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/install.rst` & `django-tenants-3.5.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/links.rst` & `django-tenants-3.5.0/docs/links.rst`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/test.rst` & `django-tenants-3.5.0/docs/test.rst`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/docs/use.rst` & `django-tenants-3.5.0/docs/use.rst`

 * *Files 4% similar despite different names*

```diff
@@ -303,14 +303,42 @@
 .. code-block:: bash
 
     ./manage.py migrate_schemas myapp 0001_initial --fake
 
 in case you're just switching your ``myapp`` application to use South migrations.
 
 
+Running the ``migrate`` will work however all it does is forward over to ``migrate_schemas``.
+
+
+
+To run the migration only on the public tenant do the following.
+
+
+.. code-block:: bash
+
+    ./manage.py migrate_schemas --shared
+
+
+To exlclude running migration on the public do the following
+
+
+.. code-block:: bash
+
+    ./manage.py migrate_schemas --tenant
+ 
+
+To run only migration only on a single tenant run the following.
+
+.. code-block:: bash
+    
+    python manage.py migrate --schema="demo"
+    
+
+
 migrate_schemas in Parallel
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You can run tenant migrations in parallel like this:
 
 .. code-block:: bash
```

### Comparing `django-tenants-3.4.8/dts_test_project/customers/migrations/0001_initial.py` & `django-tenants-3.5.0/dts_test_project/customers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/dts_test_project/customers/models.py` & `django-tenants-3.5.0/dts_test_project/customers/models.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/dts_test_project/dts_test_app/migrations/0001_initial.py` & `django-tenants-3.5.0/dts_test_project/dts_test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/dts_test_project/dts_test_project/settings.py` & `django-tenants-3.5.0/dts_test_project/dts_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/0001_initial.py` & `django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/0002_auto_20171207_1616.py` & `django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/0002_auto_20171207_1616.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/customers/migrations/0003_auto_20190404_1612.py` & `django-tenants-3.5.0/examples/tenant_multi_types/customers/migrations/0003_auto_20190404_1612.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/templates/base.html` & `django-tenants-3.5.0/examples/tenant_multi_types/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/templates/index_public.html` & `django-tenants-3.5.0/examples/tenant_multi_types/templates/index_public.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/templates/index_tenant.html` & `django-tenants-3.5.0/examples/tenant_multi_types/templates/index_tenant.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/templates/random_form.html` & `django-tenants-3.5.0/examples/tenant_multi_types/templates/random_form.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/templates/upload_file.html` & `django-tenants-3.5.0/examples/tenant_multi_types/templates/upload_file.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/middleware.py` & `django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/middleware.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/settings.py` & `django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/settings.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_type1.py` & `django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/urls_type1.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/views.py` & `django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/views.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/tenant_multi_types_tutorial/wsgi.py` & `django-tenants-3.5.0/examples/tenant_multi_types/tenant_multi_types_tutorial/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/migrations/0001_initial.py` & `django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_multi_types/tenant_type_one_only/views.py` & `django-tenants-3.5.0/examples/tenant_multi_types/tenant_type_one_only/views.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/0001_initial.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/0002_auto_20171207_1616.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/0002_auto_20171207_1616.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/migrations/0003_auto_20190404_1612.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/migrations/0003_auto_20190404_1612.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/customers/views.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/customers/views.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/base.html` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/index_public.html` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/index_public.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/index_tenant.html` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/index_tenant.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/random_form.html` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/random_form.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/templates/upload_file.html` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/templates/upload_file.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/migrations/0001_initial.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_only/migrations/0002_uploadfile.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_only/migrations/0002_uploadfile.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/settings.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/settings.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/urls_tenants.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/urls_tenants.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/views.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/views.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/wsgi.py` & `django-tenants-3.5.0/examples/tenant_subfolder_tutorial/tenant_subfolder_tutorial/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/customers/handlers.py` & `django-tenants-3.5.0/examples/tenant_tutorial/customers/handlers.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/0001_initial.py` & `django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/0002_auto_20171207_1616.py` & `django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/0002_auto_20171207_1616.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/customers/migrations/0003_auto_20190404_1612.py` & `django-tenants-3.5.0/examples/tenant_tutorial/customers/migrations/0003_auto_20190404_1612.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/customers/views.py` & `django-tenants-3.5.0/examples/tenant_tutorial/customers/views.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/templates/base.html` & `django-tenants-3.5.0/examples/tenant_tutorial/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/templates/index_public.html` & `django-tenants-3.5.0/examples/tenant_tutorial/templates/index_public.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/templates/index_tenant.html` & `django-tenants-3.5.0/examples/tenant_tutorial/templates/index_tenant.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/templates/random_form.html` & `django-tenants-3.5.0/examples/tenant_tutorial/templates/random_form.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/templates/upload_file.html` & `django-tenants-3.5.0/examples/tenant_tutorial/templates/upload_file.html`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/migrations/0001_initial.py` & `django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/tenant_only/migrations/0002_uploadfile.py` & `django-tenants-3.5.0/examples/tenant_tutorial/tenant_only/migrations/0002_uploadfile.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/middleware.py` & `django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/middleware.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/settings.py` & `django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/settings.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/urls_tenants.py` & `django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/urls_tenants.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/views.py` & `django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/views.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/examples/tenant_tutorial/tenant_tutorial/wsgi.py` & `django-tenants-3.5.0/examples/tenant_tutorial/tenant_tutorial/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-tenants-3.4.8/setup.py` & `django-tenants-3.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import exists
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-__version__ = "3.4.8"
+__version__ = "3.5.0"
 
 setup(
     name='django-tenants',
     version=__version__,
     author='Thomas Turner',
     author_email='tom@twt.me.uk',
     packages=[
@@ -44,19 +44,20 @@
         'Framework :: Django :: 2.1',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     install_requires=[
-        'Django >= 2.1,<=4.2',
+        'Django >=2.1,<4.3',
     ],
     zip_safe=False,
 )
```


# Comparing `tmp/wc-django-envoyer-0.2.2.tar.gz` & `tmp/wc-django-envoyer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-envoyer-0.2.2.tar", last modified: Wed May 10 13:31:31 2023, max compression
+gzip compressed data, was "wc-django-envoyer-0.2.3.tar", last modified: Thu May 11 13:50:26 2023, max compression
```

## Comparing `wc-django-envoyer-0.2.2.tar` & `wc-django-envoyer-0.2.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      407 2023-05-10 13:29:01.000000 wc-django-envoyer-0.2.2/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      153 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7392 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     6431 2023-05-10 13:24:36.000000 wc-django-envoyer-0.2.2/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1762 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/setup.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.271869 wc-django-envoyer-0.2.2/tests/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2192 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/tests/test_celery.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3981 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/tests/test_run.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      593 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.271869 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7392 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1919 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      285 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.271869 wc-django-envoyer-0.2.2/wcd_envoyer/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      453 2023-05-10 13:28:56.000000 wc-django-envoyer-0.2.2/wcd_envoyer/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/admin/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1156 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2889 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/templates.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2320 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/utils.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      322 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/apps.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/channels/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5974 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backend.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      952 2023-05-10 13:20:17.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/console.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4478 2023-05-10 12:13:08.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/django_sendmail.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/registry_base.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/renderers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      560 2023-05-10 13:16:57.000000 wc-django-envoyer-0.2.2/wcd_envoyer/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/const.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1191 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1186 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/shortcuts.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      640 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/tasks.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       89 2023-05-10 11:42:54.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      393 2023-05-10 11:46:44.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      386 2023-05-10 13:28:21.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/handlers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1261 2023-05-10 13:29:11.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/events.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       40 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0002_auto_20230505_0852.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/utils.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     8672 2023-05-10 13:07:02.000000 wc-django-envoyer-0.2.2/wcd_envoyer/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/services/templates_resolver.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-05-08 09:18:19.000000 wc-django-envoyer-0.2.2/wcd_envoyer/shortcuts.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      129 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/signals.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/utils/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/functional.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/registry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      855 2023-05-10 13:20:23.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/types.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.969982 wc-django-envoyer-0.2.3/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      487 2023-05-11 13:50:20.000000 wc-django-envoyer-0.2.3/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      153 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7472 2023-05-11 13:50:26.969982 wc-django-envoyer-0.2.3/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     6431 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-05-11 13:50:26.969982 wc-django-envoyer-0.2.3/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1762 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/tests/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2192 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/tests/test_celery.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3981 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/tests/test_run.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      593 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7472 2023-05-11 13:50:26.000000 wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1919 2023-05-11 13:50:26.000000 wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-05-11 13:50:26.000000 wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      285 2023-05-11 13:50:26.000000 wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-05-11 13:50:26.000000 wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      453 2023-05-11 13:49:36.000000 wc-django-envoyer-0.2.3/wcd_envoyer/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/admin/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/admin/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/admin/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/admin/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1779 2023-05-11 13:49:16.000000 wc-django-envoyer-0.2.3/wcd_envoyer/admin/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2889 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/admin/templates.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2320 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/admin/utils.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      322 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/apps.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/channels/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5692 2023-05-11 13:41:27.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/backend.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/channels/backends/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/backends/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      952 2023-05-10 13:20:17.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/backends/console.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4478 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/backends/django_sendmail.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/registry_base.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/channels/renderers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      560 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1191 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1186 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      640 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/tasks.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/pxd_actions_tracker/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       89 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/pxd_actions_tracker/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      393 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/pxd_actions_tracker/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      386 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/pxd_actions_tracker/handlers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1261 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/events.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       40 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.965982 wc-django-envoyer-0.2.3/wcd_envoyer/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/migrations/0002_auto_20230505_0852.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.969982 wc-django-envoyer-0.2.3/wcd_envoyer/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/models/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/models/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/models/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.969982 wc-django-envoyer-0.2.3/wcd_envoyer/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     8672 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/services/templates_resolver.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-05-08 09:18:19.000000 wc-django-envoyer-0.2.3/wcd_envoyer/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      129 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.3/wcd_envoyer/signals.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-11 13:50:26.969982 wc-django-envoyer-0.2.3/wcd_envoyer/utils/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/utils/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/utils/functional.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/utils/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.3/wcd_envoyer/utils/registry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      855 2023-05-10 14:27:34.000000 wc-django-envoyer-0.2.3/wcd_envoyer/utils/types.py
```

### Comparing `wc-django-envoyer-0.2.2/LICENSE` & `wc-django-envoyer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/Makefile` & `wc-django-envoyer-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/PKG-INFO` & `wc-django-envoyer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-envoyer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Message sender to different channels.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -230,14 +230,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.3]
+### Added
+- Messages use the same form as templates for data field.
+
 ## [0.2.2]
 ### Added
 - Errors tracking.
 
 ## [0.2.0]
 ### Added
 - Celery sender.
```

### Comparing `wc-django-envoyer-0.2.2/README.md` & `wc-django-envoyer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/setup.py` & `wc-django-envoyer-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/tests/test_celery.py` & `wc-django-envoyer-0.2.3/tests/test_celery.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/tests/test_run.py` & `wc-django-envoyer-0.2.3/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/tox.ini` & `wc-django-envoyer-0.2.3/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/PKG-INFO` & `wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-envoyer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Message sender to different channels.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -230,14 +230,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.3]
+### Added
+- Messages use the same form as templates for data field.
+
 ## [0.2.2]
 ### Added
 - Errors tracking.
 
 ## [0.2.0]
 ### Added
 - Celery sender.
```

### Comparing `wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/SOURCES.txt` & `wc-django-envoyer-0.2.3/wc_django_envoyer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/admin/messages.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/admin/messages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 from django.contrib import admin
 from django.contrib.messages import INFO
 
 from wcd_envoyer.models import Message
 from wcd_envoyer.shortcuts import default_sender
 from django.utils.translation import pgettext, pgettext_lazy
 
-from .utils import JsonDataAdminMixin
+from .utils import JsonDataAdminMixin, FormAdminMixin
 
 
 @admin.register(Message)
-class MessageAdmin(JsonDataAdminMixin, admin.ModelAdmin):
+class MessageAdmin(JsonDataAdminMixin, FormAdminMixin, admin.ModelAdmin):
     messages_sender = default_sender
     actions = 'resend_action',
     list_display = 'channel', 'event', 'status', 'created_at', 'updated_at',
     list_filter = 'channel', 'event', 'status',
     readonly_fields = 'json_data', 'created_at', 'updated_at',
     date_hierarchy = 'created_at'
     search_fields = 'channel', 'event', 'recipients', 'data', 'status',
 
+    def get_backend_form_class(self, request, obj, backend):
+        BaseForm = backend.template_form_class
+        message_untangled_fields = ['status', 'recipients'] + [
+            field for field in getattr(BaseForm.Meta, 'untangled_fields', [])
+            if field not in {'is_active'}
+        ]
+
+        class MessageForm(BaseForm, self.form):
+            class Meta(BaseForm.Meta):
+                fields = 'channel', 'event', 'recipients', 'data', 'status',
+                model = self.model
+                untangled_fields = message_untangled_fields
+
+        return MessageForm
+
     def resend_action(self, request, qs):
         messages = list(qs)
         self.messages_sender.resend(messages)
 
         self.message_user(
             request=request,
             message=(
```

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/admin/templates.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/admin/templates.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/admin/utils.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/admin/utils.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/channels/backend.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/channels/backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,22 +41,15 @@
 
     def normalize_message_data(
         self,
         config: 'ChannelConfig',
         message_data: MessageData,
         context: dict = {},
     ):
-        return message_data
-        for recipient in self.recipients_resolver(message_data.recipients):
-            yield MessageData(
-                message_data.channel,
-                message_data.event,
-                recipients=[recipient],
-                context=message_data.context,
-            )
+        yield message_data
 
     def make_message(
         self,
         message_data: MessageData,
         template: 'Template',
         context: dict = {}
     ) -> 'Message':
```

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/console.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/channels/backends/console.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/django_sendmail.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/channels/backends/django_sendmail.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/channels/forms.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/channels/forms.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/channels/registry_base.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/channels/registry_base.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/conf.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/conf.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/sender.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/services/sender.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/shortcuts.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/tasks.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/contrib/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/events.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/events.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0001_initial.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0002_auto_20230505_0852.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/migrations/0002_auto_20230505_0852.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/models/channels.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/models/channels.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/models/messages.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/models/messages.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/services/sender.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/services/sender.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/services/templates_resolver.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/services/templates_resolver.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/shortcuts.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/utils/functional.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/utils/functional.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/utils/models.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/utils/models.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.2/wcd_envoyer/utils/types.py` & `wc-django-envoyer-0.2.3/wcd_envoyer/utils/types.py`

 * *Files identical despite different names*


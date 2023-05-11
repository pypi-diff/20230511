# Comparing `tmp/django-otp-1.1.6.tar.gz` & `tmp/django_otp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-otp-1.1.6.tar", last modified: Tue Mar  7 14:51:05 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-otp-1.1.6.tar` & `django_otp-1.2.0.tar`

### file list

```diff
@@ -1,119 +1,97 @@
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)    15204 2023-03-07 14:50:46.000000 django-otp-1.1.6/CHANGES.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1297 2022-01-13 18:26:38.000000 django-otp-1.1.6/LICENSE
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      375 2022-01-13 18:26:38.000000 django-otp-1.1.6/MANIFEST.in
--rw-r--r--   0 psagers   (1000) psagers   (1000)     6882 2023-03-07 14:51:05.000000 django-otp-1.1.6/PKG-INFO
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     6011 2022-01-13 18:26:38.000000 django-otp-1.1.6/README.rst
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/docs/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     5693 2022-01-13 18:26:38.000000 django-otp-1.1.6/docs/Makefile
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/docs/ext/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      217 2022-01-13 18:26:38.000000 django-otp-1.1.6/docs/ext/otpdocs.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/docs/source/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     8625 2022-03-13 17:17:47.000000 django-otp-1.1.6/docs/source/auth.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)       54 2022-01-13 18:26:38.000000 django-otp-1.1.6/docs/source/changes.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     8834 2023-03-07 14:50:46.000000 django-otp-1.1.6/docs/source/conf.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2870 2022-01-13 18:26:38.000000 django-otp-1.1.6/docs/source/extend.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1478 2022-01-13 18:26:38.000000 django-otp-1.1.6/docs/source/index.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)    18296 2022-01-13 18:26:38.000000 django-otp-1.1.6/docs/source/overview.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      118 2023-03-07 14:51:05.000000 django-otp-1.1.6/setup.cfg
--rwxrwxr-x   0 psagers   (1000) psagers   (1000)     1180 2023-03-07 14:50:46.000000 django-otp-1.1.6/setup.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     5330 2022-12-12 20:29:16.000000 django-otp-1.1.6/src/django_otp/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2532 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/admin.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      630 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/conf.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      967 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/decorators.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)    13087 2022-03-13 17:02:09.000000 django-otp-1.1.6/src/django_otp/forms.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/locale/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/locale/de/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/locale/de/LC_MESSAGES/
--rw-r--r--   0 psagers   (1000) psagers   (1000)     2350 2023-03-07 14:49:37.000000 django-otp-1.1.6/src/django_otp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 psagers   (1000) psagers   (1000)     3363 2023-03-07 14:49:37.000000 django-otp-1.1.6/src/django_otp/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/locale/es/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/locale/es/LC_MESSAGES/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2288 2022-11-10 22:21:34.000000 django-otp-1.1.6/src/django_otp/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     3283 2022-11-10 22:21:34.000000 django-otp-1.1.6/src/django_otp/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/locale/fr/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2331 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2668 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2404 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/middleware.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)    12331 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/models.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     5512 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/oath.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/__init__.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      119 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      681 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/admin.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      164 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/apps.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      804 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/conf.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1221 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/0001_initial.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      792 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      486 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      768 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/__init__.py
--rw-r--r--   0 psagers   (1000) psagers   (1000)     2794 2023-03-06 17:11:14.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/models.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/templates/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/templates/otp/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/templates/otp/email/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)       12 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     5865 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_email/tests.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      118 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     4217 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/admin.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      163 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/apps.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/migrations/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1660 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      753 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/migrations/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     3852 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/models.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/templates/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/templates/otp_hotp/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      607 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
--rw-rw-r--   0 psagers   (1000) psagers   (1000)    13113 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_hotp/tests.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      120 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      996 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/admin.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      165 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/apps.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      689 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/lib.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/management/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/management/__init__.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/management/commands/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/management/commands/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1078 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/migrations/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1444 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/migrations/0001_initial.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      761 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/migrations/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1934 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/models.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     7994 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_static/tests.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      118 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     4243 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/admin.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      163 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/apps.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/migrations/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2110 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      753 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/migrations/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     5177 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/models.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/templates/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/templates/otp_totp/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      607 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
--rw-rw-r--   0 psagers   (1000) psagers   (1000)    10899 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/plugins/otp_totp/tests.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/templates/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/templates/otp/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp/templates/otp/admin111/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2855 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/templates/otp/admin111/login.html
--rw-rw-r--   0 psagers   (1000) psagers   (1000)    15125 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/tests.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     2421 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/util.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1695 2022-01-13 18:26:38.000000 django-otp-1.1.6/src/django_otp/views.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp.egg-info/
--rw-r--r--   0 psagers   (1000) psagers   (1000)     6882 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp.egg-info/PKG-INFO
--rw-r--r--   0 psagers   (1000) psagers   (1000)     3297 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp.egg-info/SOURCES.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)        1 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp.egg-info/dependency_links.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)        1 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp.egg-info/not-zip-safe
--rw-r--r--   0 psagers   (1000) psagers   (1000)       29 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp.egg-info/requires.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)       11 2023-03-07 14:51:05.000000 django-otp-1.1.6/src/django_otp.egg-info/top_level.txt
+-rw-r--r--   0        0        0    15815 2020-02-02 00:00:00.000000 django_otp-1.2.0/CHANGES.rst
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 django_otp-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/ext/otpdocs.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/.spell.utf-8.add
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/auth.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/changes.rst
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/extend.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/overview.rst
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/admin.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/conf.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/decorators.py
+-rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/forms.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/middleware.py
+-rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/models.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/oath.py
+-rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/tests.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/util.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/views.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/admin.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/apps.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/conf.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/models.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/tests.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/__init__.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/apps.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/models.py
+-rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/tests.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/admin.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/apps.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/lib.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/models.py
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/management/commands/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/__init__.py
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/apps.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/models.py
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/tests.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/templates/otp/admin111/login.html
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/config/github.toml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/config/sample.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/backends.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/config.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/settings.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/urls.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/views.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/about.html
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/home.html
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/navbar.html
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/root.html
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/bs5/input.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/bs5/select.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/otp/email/custom.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/otp/email/token.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/registration/login.html
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 django_otp-1.2.0/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp-1.2.0/.hgignore
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 django_otp-1.2.0/README.rst
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 django_otp-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 django_otp-1.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-otp-1.1.6/CHANGES.rst` & `django_otp-1.2.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v1.2.0 - May 11, 2023 - Tooling, TOTP images
+--------------------------------------------------------------------------------
+
+- This project is now managed with `hatch`_, which replaces setuptools, pipenv,
+  and tox. Users of the package should not be impacted. Developers can refer to
+  the readme for details. If you're packaging this project from source, I
+  suggest relying on pip's isolated builds rather than using hatch directly.
+
+- `#123`_: Add support for passing an image parameter in the otpauth URL.
+
+
+.. _hatch: https://hatch.pypa.io/
+.. _#123: https://github.com/django-otp/django-otp/pull/123
+
+
 v1.1.6 - March 07, 2023 - German translation
 --------------------------------------------------------------------------------
 
 - `#116`_: Add German translation
 
 .. _#116: https://github.com/django-otp/django-otp/pull/116
```

### Comparing `django-otp-1.1.6/PKG-INFO` & `django_otp-1.2.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,431 +1,409 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
-00000020: 676f 2d6f 7470 0a56 6572 7369 6f6e 3a20  go-otp.Version: 
-00000030: 312e 312e 360a 5375 6d6d 6172 793a 2041  1.1.6.Summary: A
-00000040: 2070 6c75 6767 6162 6c65 2066 7261 6d65   pluggable frame
-00000050: 776f 726b 2066 6f72 2061 6464 696e 6720  work for adding 
-00000060: 7477 6f2d 6661 6374 6f72 2061 7574 6865  two-factor authe
-00000070: 6e74 6963 6174 696f 6e20 746f 2044 6a61  ntication to Dja
-00000080: 6e67 6f20 7573 696e 6720 6f6e 652d 7469  ngo using one-ti
-00000090: 6d65 2070 6173 7377 6f72 6473 2e0a 486f  me passwords..Ho
-000000a0: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-000000b0: 2f67 6974 6875 622e 636f 6d2f 646a 616e  /github.com/djan
-000000c0: 676f 2d6f 7470 2f64 6a61 6e67 6f2d 6f74  go-otp/django-ot
-000000d0: 700a 4175 7468 6f72 3a20 5065 7465 7220  p.Author: Peter 
-000000e0: 5361 6765 7273 6f6e 0a41 7574 686f 722d  Sagerson.Author-
-000000f0: 656d 6169 6c3a 2070 7361 6765 7273 4069  email: psagers@i
-00000100: 676e 6f72 6172 652e 6e65 740a 4c69 6365  gnorare.net.Lice
-00000110: 6e73 653a 2042 5344 0a50 726f 6a65 6374  nse: BSD.Project
-00000120: 2d55 524c 3a20 446f 6375 6d65 6e74 6174  -URL: Documentat
-00000130: 696f 6e2c 2068 7474 7073 3a2f 2f64 6a61  ion, https://dja
-00000140: 6e67 6f2d 6f74 702d 6f66 6669 6369 616c  ngo-otp-official
-00000150: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000160: 0a50 726f 6a65 6374 2d55 524c 3a20 536f  .Project-URL: So
-00000170: 7572 6365 2c20 6874 7470 733a 2f2f 6769  urce, https://gi
-00000180: 7468 7562 2e63 6f6d 2f64 6a61 6e67 6f2d  thub.com/django-
-00000190: 6f74 702f 646a 616e 676f 2d6f 7470 0a50  otp/django-otp.P
-000001a0: 6c61 7466 6f72 6d3a 2055 4e4b 4e4f 574e  latform: UNKNOWN
-000001b0: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-000001c0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-000001d0: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
-000001e0: 6e2f 5374 6162 6c65 0a43 6c61 7373 6966  n/Stable.Classif
-000001f0: 6965 723a 2046 7261 6d65 776f 726b 203a  ier: Framework :
-00000200: 3a20 446a 616e 676f 0a43 6c61 7373 6966  : Django.Classif
-00000210: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000220: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-00000230: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
-00000240: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
-00000250: 4170 7072 6f76 6564 203a 3a20 4253 4420  Approved :: BSD 
-00000260: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
-00000270: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000290: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
-000002a0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002c0: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790a  on :: 3 :: Only.
-000002d0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-000002e0: 6320 3a3a 2053 6563 7572 6974 790a 436c  c :: Security.Cl
-000002f0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000300: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000310: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000320: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
-00000330: 6f64 756c 6573 0a50 726f 7669 6465 732d  odules.Provides-
-00000340: 4578 7472 613a 2071 7263 6f64 650a 4c69  Extra: qrcode.Li
-00000350: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000360: 4e53 450a 0a64 6a61 6e67 6f2d 6f74 700a  NSE..django-otp.
-00000370: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e 2069  ==========.... i
-00000380: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-00000390: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000003a0: 7069 2f76 2f64 6a61 6e67 6f2d 6f74 703f  pi/v/django-otp?
-000003b0: 636f 6c6f 723d 626c 7565 0a20 2020 3a74  color=blue.   :t
-000003c0: 6172 6765 743a 2068 7474 7073 3a2f 2f70  arget: https://p
-000003d0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-000003e0: 646a 616e 676f 2d6f 7470 2f0a 2020 203a  django-otp/.   :
-000003f0: 616c 743a 2050 7950 490a 2e2e 2069 6d61  alt: PyPI... ima
-00000400: 6765 3a3a 2068 7474 7073 3a2f 2f69 6d67  ge:: https://img
-00000410: 2e73 6869 656c 6473 2e69 6f2f 7265 6164  .shields.io/read
-00000420: 7468 6564 6f63 732f 646a 616e 676f 2d6f  thedocs/django-o
-00000430: 7470 2d6f 6666 6963 6961 6c0a 2020 203a  tp-official.   :
-00000440: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000450: 646a 616e 676f 2d6f 7470 2d6f 6666 6963  django-otp-offic
-00000460: 6961 6c2e 7265 6164 7468 6564 6f63 732e  ial.readthedocs.
-00000470: 696f 2f0a 2020 203a 616c 743a 2044 6f63  io/.   :alt: Doc
-00000480: 756d 656e 7461 7469 6f6e 0a2e 2e20 696d  umentation... im
-00000490: 6167 653a 3a20 6874 7470 733a 2f2f 696d  age:: https://im
-000004a0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000004b0: 6765 2f67 6974 6875 622d 646a 616e 676f  ge/github-django
-000004c0: 2d2d 6f74 702d 6772 6565 6e0a 2020 203a  --otp-green.   :
-000004d0: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-000004e0: 6769 7468 7562 2e63 6f6d 2f64 6a61 6e67  github.com/djang
-000004f0: 6f2d 6f74 702f 646a 616e 676f 2d6f 7470  o-otp/django-otp
-00000500: 0a20 2020 3a61 6c74 3a20 536f 7572 6365  .   :alt: Source
-00000510: 0a0a 5468 6973 2070 726f 6a65 6374 206d  ..This project m
-00000520: 616b 6573 2069 7420 6561 7379 2074 6f20  akes it easy to 
-00000530: 6164 6420 7375 7070 6f72 7420 666f 7220  add support for 
-00000540: 606f 6e65 2d74 696d 6520 7061 7373 776f  `one-time passwo
-00000550: 7264 730a 3c68 7474 703a 2f2f 656e 2e77  rds.<http://en.w
-00000560: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00000570: 692f 4f6e 652d 7469 6d65 5f70 6173 7377  i/One-time_passw
-00000580: 6f72 643e 605f 2028 4f54 5073 2920 746f  ord>`_ (OTPs) to
-00000590: 2044 6a61 6e67 6f2e 2049 7420 6361 6e20   Django. It can 
-000005a0: 6265 0a69 6e74 6567 7261 7465 6420 6174  be.integrated at
-000005b0: 2076 6172 696f 7573 206c 6576 656c 732c   various levels,
-000005c0: 2064 6570 656e 6469 6e67 206f 6e20 686f   depending on ho
-000005d0: 7720 6d75 6368 2063 7573 746f 6d69 7a61  w much customiza
-000005e0: 7469 6f6e 2069 7320 7265 7175 6972 6564  tion is required
-000005f0: 2e0a 4974 2069 6e74 6567 7261 7465 7320  ..It integrates 
-00000600: 7769 7468 2060 6064 6a61 6e67 6f2e 636f  with ``django.co
-00000610: 6e74 7269 622e 6175 7468 6060 2c20 616c  ntrib.auth``, al
-00000620: 7468 6f75 6768 2069 7420 6973 206e 6f74  though it is not
-00000630: 2061 2044 6a61 6e67 6f0a 6175 7468 656e   a Django.authen
-00000640: 7469 6361 7469 6f6e 2062 6163 6b65 6e64  tication backend
-00000650: 2e20 5468 6520 7072 696d 6172 7920 7461  . The primary ta
-00000660: 7267 6574 2069 7320 6465 7665 6c6f 7065  rget is develope
-00000670: 7273 2077 6973 6869 6e67 2074 6f20 696e  rs wishing to in
-00000680: 636f 7270 6f72 6174 650a 4f54 5073 2069  corporate.OTPs i
-00000690: 6e74 6f20 7468 6569 7220 446a 616e 676f  nto their Django
-000006a0: 2070 726f 6a65 6374 7320 6173 2061 2066   projects as a f
-000006b0: 6f72 6d20 6f66 2060 7477 6f2d 6661 6374  orm of `two-fact
-000006c0: 6f72 2061 7574 6865 6e74 6963 6174 696f  or authenticatio
-000006d0: 6e0a 3c68 7474 703a 2f2f 656e 2e77 696b  n.<http://en.wik
-000006e0: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-000006f0: 5477 6f2d 6661 6374 6f72 5f61 7574 6865  Two-factor_authe
-00000700: 6e74 6963 6174 696f 6e3e 605f 2e0a 0a53  ntication>`_...S
-00000710: 6576 6572 616c 2073 696d 706c 6520 4f54  everal simple OT
-00000720: 5020 706c 7567 696e 7320 6172 6520 696e  P plugins are in
-00000730: 636c 7564 6564 2061 6e64 206d 6f72 6520  cluded and more 
-00000740: 6172 6520 6176 6169 6c61 626c 6520 7365  are available se
-00000750: 7061 7261 7465 6c79 2e20 5468 6973 0a70  parately. This.p
-00000760: 6163 6b61 6765 2061 6c73 6f20 696e 636c  ackage also incl
-00000770: 7564 6573 2061 6e20 696d 706c 656d 656e  udes an implemen
-00000780: 7461 7469 6f6e 206f 6620 4f41 5448 2060  tation of OATH `
-00000790: 484f 5450 0a3c 6874 7470 3a2f 2f74 6f6f  HOTP.<http://too
-000007a0: 6c73 2e69 6574 662e 6f72 672f 6874 6d6c  ls.ietf.org/html
-000007b0: 2f72 6663 3432 3236 3e60 5f20 616e 6420  /rfc4226>`_ and 
-000007c0: 6054 4f54 500a 3c68 7474 703a 2f2f 746f  `TOTP.<http://to
-000007d0: 6f6c 732e 6965 7466 2e6f 7267 2f68 746d  ols.ietf.org/htm
-000007e0: 6c2f 7266 6336 3233 383e 605f 2066 6f72  l/rfc6238>`_ for
-000007f0: 2063 6f6e 7665 6e69 656e 6365 2c20 6173   convenience, as
-00000800: 2074 6865 7365 2061 7265 2073 7461 6e64   these are stand
-00000810: 6172 640a 4f54 5020 616c 676f 7269 7468  ard.OTP algorith
-00000820: 6d73 2075 7365 6420 6279 206d 756c 7469  ms used by multi
-00000830: 706c 6520 706c 7567 696e 732e 0a0a 4966  ple plugins...If
-00000840: 2079 6f75 2772 6520 6c6f 6f6b 696e 6720   you're looking 
-00000850: 666f 7220 6120 6869 6768 6572 2d6c 6576  for a higher-lev
-00000860: 656c 206f 7220 6d6f 7265 206f 7069 6e69  el or more opini
-00000870: 6f6e 6174 6564 2073 6f6c 7574 696f 6e2c  onated solution,
-00000880: 2079 6f75 206d 6967 6874 2062 650a 696e   you might be.in
-00000890: 7465 7265 7374 6564 2069 6e20 6064 6a61  terested in `dja
-000008a0: 6e67 6f2d 7477 6f2d 6661 6374 6f72 2d61  ngo-two-factor-a
-000008b0: 7574 680a 3c68 7474 7073 3a2f 2f67 6974  uth.<https://git
-000008c0: 6875 622e 636f 6d2f 426f 756b 652f 646a  hub.com/Bouke/dj
-000008d0: 616e 676f 2d74 776f 2d66 6163 746f 722d  ango-two-factor-
-000008e0: 6175 7468 3e60 5f2e 0a0a 5374 6174 7573  auth>`_...Status
-000008f0: 0a2d 2d2d 2d2d 2d0a 0a54 6869 7320 7072  .------..This pr
-00000900: 6f6a 6563 7420 6973 2073 7461 626c 6520  oject is stable 
-00000910: 616e 6420 6d61 696e 7461 696e 6564 2c20  and maintained, 
-00000920: 6275 7420 6973 206e 6f20 6c6f 6e67 6572  but is no longer
-00000930: 2061 6374 6976 656c 7920 7573 6564 2062   actively used b
-00000940: 7920 7468 650a 6175 7468 6f72 2061 6e64  y the.author and
-00000950: 2069 7320 6e6f 7420 7365 6569 6e67 206d   is not seeing m
-00000960: 7563 6820 6f6e 676f 696e 6720 696e 7665  uch ongoing inve
-00000970: 7374 6d65 6e74 2e20 416e 796f 6e65 2069  stment. Anyone i
-00000980: 6e74 6572 6573 7465 6420 696e 2074 616b  nterested in tak
-00000990: 696e 670a 6f76 6572 2061 7370 6563 7473  ing.over aspects
-000009a0: 206f 6620 7468 6520 7072 6f6a 6563 7420   of the project 
-000009b0: 7368 6f75 6c64 2060 636f 6e74 6163 7420  should `contact 
-000009c0: 6d65 203c 6874 7470 733a 2f2f 6769 7468  me <https://gith
-000009d0: 7562 2e63 6f6d 2f70 7361 6765 7273 3e60  ub.com/psagers>`
-000009e0: 5f2e 0a0a 5765 6c6c 2d66 6f72 6d65 6420  _...Well-formed 
-000009f0: 6973 7375 6573 2061 6e64 2070 756c 6c20  issues and pull 
-00000a00: 7265 7175 6573 7473 2061 7265 2077 656c  requests are wel
-00000a10: 636f 6d65 2c20 6275 7420 706c 6561 7365  come, but please
-00000a20: 2073 6565 2074 6865 0a43 6f6e 7472 6962   see the.Contrib
-00000a30: 7574 696e 6720 7365 6374 696f 6e20 6f66  uting section of
-00000a40: 2074 6865 2052 4541 444d 4520 6669 7273   the README firs
-00000a50: 742e 0a0a 2e2e 2065 6e64 2d6f 662d 646f  t..... end-of-do
-00000a60: 632d 696e 7472 6f0a 0a0a 5468 6520 4675  c-intro...The Fu
-00000a70: 7475 7265 0a2d 2d2d 2d2d 2d2d 2d2d 2d0a  ture.----------.
-00000a80: 0a4f 6e63 6520 7570 6f6e 2061 2074 696d  .Once upon a tim
-00000a90: 652c 2065 7665 7279 7468 696e 6720 7761  e, everything wa
-00000aa0: 7320 7573 6572 6e61 6d65 7320 616e 6420  s usernames and 
-00000ab0: 7061 7373 776f 7264 732e 204f 7220 6576  passwords. Or ev
-00000ac0: 656e 2069 6e20 7468 6520 6361 7365 206f  en in the case o
-00000ad0: 660a 6f74 6865 7220 6175 7468 656e 7469  f.other authenti
-00000ae0: 6361 7469 6f6e 206d 6563 6861 6e69 736d  cation mechanism
-00000af0: 732c 2061 2075 7365 7220 7761 7320 6569  s, a user was ei
-00000b00: 7468 6572 2061 7574 6865 6e74 6963 6174  ther authenticat
-00000b10: 6564 206f 7220 6e6f 740a 2861 6e6f 6e79  ed or not.(anony
-00000b20: 6d6f 7573 2069 6e20 446a 616e 676f 2773  mous in Django's
-00000b30: 2074 6572 6d69 6e6f 6c6f 6779 292e 2054   terminology). T
-00000b40: 6865 6e20 7468 6572 6520 7761 7320 7477  hen there was tw
-00000b50: 6f2d 6661 6374 6f72 2061 7574 6865 6e74  o-factor authent
-00000b60: 6963 6174 696f 6e2c 0a77 6869 6368 2063  ication,.which c
-00000b70: 6f75 6c64 2073 696d 706c 7920 6265 2061  ould simply be a
-00000b80: 6e20 696d 706c 656d 656e 7461 7469 6f6e  n implementation
-00000b90: 2064 6574 6169 6c20 696e 2061 2062 696e   detail in a bin
-00000ba0: 6172 7920 6175 7468 656e 7469 6361 7469  ary authenticati
-00000bb0: 6f6e 2073 7461 7465 2c0a 6275 7420 636f  on state,.but co
-00000bc0: 756c 6420 616c 736f 2069 6d70 6c79 206c  uld also imply l
-00000bd0: 6576 656c 7320 6f72 2064 6567 7265 6573  evels or degrees
-00000be0: 206f 6620 6175 7468 656e 7469 6361 7469   of authenticati
-00000bf0: 6f6e 2e0a 0a54 6865 7365 2064 6179 732c  on...These days,
-00000c00: 2069 7427 7320 696e 6372 6561 7369 6e67   it's increasing
-00000c10: 6c79 2063 6f6d 6d6f 6e20 746f 2073 6565  ly common to see
-00000c20: 2073 6974 6573 2077 6974 6820 6d6f 7265   sites with more
-00000c30: 206e 7561 6e63 6564 0a61 7574 6865 6e74   nuanced.authent
-00000c40: 6963 6174 696f 6e20 7374 6174 652e 2041  ication state. A
-00000c50: 2073 6974 6520 6d69 6768 7420 7265 6d65   site might reme
-00000c60: 6d62 6572 2077 686f 2079 6f75 2061 7265  mber who you are
-00000c70: 2066 6f72 6576 6572 e280 9473 6f20 796f   forever...so yo
-00000c80: 7527 7265 206e 6f74 0a61 6e6f 6e79 6d6f  u're not.anonymo
-00000c90: 7573 e280 9462 7574 2069 6620 796f 7520  us...but if you 
-00000ca0: 7472 7920 746f 2064 6f20 616e 7974 6869  try to do anythi
-00000cb0: 6e67 2070 7269 7661 7465 2c20 796f 7520  ng private, you 
-00000cc0: 6861 7665 2074 6f20 7265 2d61 7574 6865  have to re-authe
-00000cd0: 6e74 6963 6174 652e 0a59 6f75 206d 6179  nticate..You may
-00000ce0: 2062 6520 6162 6c65 2074 6f20 6368 6f6f   be able to choo
-00000cf0: 7365 2066 726f 6d20 616d 6f6e 6720 616c  se from among al
-00000d00: 6c20 6f66 2074 6865 2061 7574 6865 6e74  l of the authent
-00000d10: 6963 6174 696f 6e20 6d65 6368 616e 6973  ication mechanis
-00000d20: 6d73 2079 6f75 0a68 6176 6520 636f 6e66  ms you.have conf
-00000d30: 6967 7572 6564 2c20 6f72 206f 6e6c 7920  igured, or only 
-00000d40: 6672 6f6d 2073 6f6d 6520 6f66 2074 6865  from some of the
-00000d50: 6d2e 2053 7065 6369 6669 6320 6d65 6368  m. Specific mech
-00000d60: 616e 6973 6d73 206d 6179 2062 6520 7265  anisms may be re
-00000d70: 7175 6972 6564 0a66 6f72 2073 7065 6369  quired.for speci
-00000d80: 6669 6320 6163 7469 6f6e 732c 2073 7563  fic actions, suc
-00000d90: 6820 6173 2075 7369 6e67 2079 6f75 7220  h as using your 
-00000da0: 5532 4620 6465 7669 6365 2074 6f20 6163  U2F device to ac
-00000db0: 6365 7373 2079 6f75 7220 5532 4620 7365  cess your U2F se
-00000dc0: 7474 696e 6773 2e0a 0a49 6e20 7368 6f72  ttings...In shor
-00000dd0: 742c 2074 6865 2077 6f72 6c64 2073 6565  t, the world see
-00000de0: 6d73 2074 6f20 6265 206d 6f76 696e 6720  ms to be moving 
-00000df0: 6265 796f 6e64 2074 6865 2061 7373 756d  beyond the assum
-00000e00: 7074 696f 6e73 2074 6861 7420 6f72 6967  ptions that orig
-00000e10: 696e 616c 6c79 0a69 6e66 6f72 6d65 6420  inally.informed 
-00000e20: 446a 616e 676f 2773 2065 7373 656e 7469  Django's essenti
-00000e30: 616c 2061 7574 6865 6e74 6963 6174 696f  al authenticatio
-00000e40: 6e20 6465 7369 676e 2e20 4966 2049 2077  n design. If I w
-00000e50: 6572 6520 7374 696c 6c20 696e 7665 7374  ere still invest
-00000e60: 696e 6720 696e 0a44 6a61 6e67 6f20 6765  ing in.Django ge
-00000e70: 6e65 7261 6c6c 792c 2049 2077 6f75 6c64  nerally, I would
-00000e80: 2070 726f 6261 626c 7920 7374 6172 7420   probably start 
-00000e90: 6120 6e65 7720 6d75 6c74 692d 6661 6374  a new multi-fact
-00000ea0: 6f72 2061 7574 6865 6e74 6963 6174 696f  or authenticatio
-00000eb0: 6e0a 7072 6f6a 6563 7420 7468 6174 2077  n.project that w
-00000ec0: 6f75 6c64 2072 6566 6c65 6374 2074 6865  ould reflect the
-00000ed0: 7365 2063 6861 6e67 6573 2e20 4974 2077  se changes. It w
-00000ee0: 6f75 6c64 2069 6e63 6f72 706f 7261 7465  ould incorporate
-00000ef0: 2074 6865 2069 6465 6120 7468 6174 2061   the idea that a
-00000f00: 0a75 7365 7220 6d61 7920 6265 2061 7574  .user may be aut
-00000f10: 6865 6e74 6963 6174 6564 2062 7920 7661  henticated by va
-00000f20: 7269 6f75 7320 636f 6d62 696e 6174 696f  rious combinatio
-00000f30: 6e73 206f 6620 6d65 6368 616e 6973 6d73  ns of mechanisms
-00000f40: 2061 7420 616e 7920 7469 6d65 2061 6e64   at any time and
-00000f50: 0a74 6861 7420 6469 6666 6572 656e 7420  .that different 
-00000f60: 636f 6d62 696e 6174 696f 6e73 206d 6179  combinations may
-00000f70: 2062 6520 7265 7175 6972 6564 2074 6f20   be required to 
-00000f80: 7361 7469 7366 7920 6469 7665 7273 6520  satisfy diverse 
-00000f90: 6175 7468 6f72 697a 6174 696f 6e0a 7265  authorization.re
-00000fa0: 7175 6972 656d 656e 7473 2061 6372 6f73  quirements acros
-00000fb0: 7320 7468 6520 7369 7465 2e20 4974 2077  s the site. It w
-00000fc0: 6f75 6c64 206d 6f73 7420 6c69 6b65 6c79  ould most likely
-00000fd0: 2074 7279 2074 6f20 6469 7365 6e74 616e   try to disentan
-00000fe0: 676c 650a 6175 7468 656e 7469 6361 7469  gle.authenticati
-00000ff0: 6f6e 2070 6572 7369 7374 656e 6365 2066  on persistence f
-00001000: 726f 6d20 7365 7373 696f 6e73 2c20 6174  rom sessions, at
-00001010: 206c 6561 7374 2074 6f20 736f 6d65 2065   least to some e
-00001020: 7874 656e 742e 204d 616e 7920 7369 7465  xtent. Many site
-00001030: 730a 776f 756c 6420 6e6f 7420 7265 7175  s.would not requ
-00001040: 6972 6520 616c 6c20 6f66 2074 6869 7320  ire all of this 
-00001050: 666c 6578 6962 696c 6974 792c 2062 7574  flexibility, but
-00001060: 2069 7420 776f 756c 6420 6f70 656e 2075   it would open u
-00001070: 7020 706f 7373 6962 696c 6974 6965 730a  p possibilities.
-00001080: 666f 7220 6265 7474 6572 2065 7870 6572  for better exper
-00001090: 6965 6e63 6573 2062 7920 6e6f 7420 6173  iences by not as
-000010a0: 6b69 6e67 2075 7365 7273 2066 6f72 206d  king users for m
-000010b0: 6f72 6520 7468 616e 2077 6520 7265 7175  ore than we requ
-000010c0: 6972 6520 6174 2061 6e79 0a70 6f69 6e74  ire at any.point
-000010d0: 2e0a 0a49 6620 616e 796f 6e65 2068 6173  ...If anyone has
-000010e0: 2061 206d 696e 6420 746f 2074 616b 6520   a mind to take 
-000010f0: 6f6e 2061 2070 726f 6a65 6374 206c 696b  on a project lik
-00001100: 6520 7468 6973 2c20 4927 6420 6265 2068  e this, I'd be h
-00001110: 6170 7079 2074 6f20 6f66 6665 720a 7768  appy to offer.wh
-00001120: 6174 6576 6572 2061 6476 6963 6520 6f72  atever advice or
-00001130: 206c 6573 736f 6e73 206c 6561 726e 6564   lessons learned
-00001140: 2074 6861 7420 4920 6361 6e2e 0a0a 0a44   that I can....D
-00001150: 6576 656c 6f70 6d65 6e74 0a2d 2d2d 2d2d  evelopment.-----
-00001160: 2d2d 2d2d 2d2d 0a0a 4465 7665 6c6f 706d  ------..Developm
-00001170: 656e 7420 6465 7065 6e64 656e 6369 6573  ent dependencies
-00001180: 2061 7265 2064 6566 696e 6564 2069 6e20   are defined in 
-00001190: 7468 6520 5069 7066 696c 653b 2075 7365  the Pipfile; use
-000011a0: 2060 7069 7065 6e76 605f 2074 6f20 7365   `pipenv`_ to se
-000011b0: 7420 7570 2061 0a73 7569 7461 626c 6520  t up a.suitable 
-000011c0: 7368 656c 6c2e 0a0a 5468 6520 7465 7374  shell...The test
-000011d0: 7320 696e 2074 6f78 2e69 6e69 2063 6f76  s in tox.ini cov
-000011e0: 6572 2061 2072 6570 7265 7365 6e74 6174  er a representat
-000011f0: 6976 6520 7361 6d70 6c65 206f 6620 7375  ive sample of su
-00001200: 7070 6f72 7465 6420 5079 7468 6f6e 2061  pported Python a
-00001210: 6e64 0a44 6a61 6e67 6f20 7665 7273 696f  nd.Django versio
-00001220: 6e73 2c20 6173 2077 656c 6c20 6173 2072  ns, as well as r
-00001230: 756e 6e69 6e67 2060 666c 616b 6538 605f  unning `flake8`_
-00001240: 2061 6e64 2060 6973 6f72 7460 5f20 666f   and `isort`_ fo
-00001250: 7220 6c69 6e74 696e 6720 616e 6420 7374  r linting and st
-00001260: 796c 650a 636f 6e73 6973 7465 6e63 792e  yle.consistency.
-00001270: 2050 6c65 6173 6520 7275 6e20 6074 6f78   Please run `tox
-00001280: 6020 6265 666f 7265 2063 6865 636b 696e  ` before checkin
-00001290: 6720 696e 2061 6e64 2073 656e 6469 6e67  g in and sending
-000012a0: 2061 2070 756c 6c20 7265 7175 6573 742e   a pull request.
-000012b0: 0a0a 0a43 6f6e 7472 6962 7574 696e 670a  ...Contributing.
-000012c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4173  ------------..As
-000012d0: 206d 656e 7469 6f6e 6564 2061 626f 7665   mentioned above
-000012e0: 2c20 7468 6973 2070 726f 6a65 6374 2069  , this project i
-000012f0: 7320 7374 6162 6c65 2061 6e64 206d 6174  s stable and mat
-00001300: 7572 652e 2049 7373 7565 7320 616e 6420  ure. Issues and 
-00001310: 7075 6c6c 2072 6571 7565 7374 730a 6172  pull requests.ar
-00001320: 6520 7765 6c63 6f6d 6520 666f 7220 696d  e welcome for im
-00001330: 706f 7274 616e 7420 6275 6773 2061 6e64  portant bugs and
-00001340: 2069 6d70 726f 7665 6d65 6e74 732e 2046   improvements. F
-00001350: 6f72 206e 6f6e 2d74 7269 7669 616c 2063  or non-trivial c
-00001360: 6861 6e67 6573 2c20 6974 2773 0a6f 6674  hanges, it's.oft
-00001370: 656e 2061 2067 6f6f 6420 6964 6561 2074  en a good idea t
-00001380: 6f20 7374 6172 7420 6279 206f 7065 6e69  o start by openi
-00001390: 6e67 2061 6e20 6973 7375 6520 746f 2074  ng an issue to t
-000013a0: 7261 636b 2074 6865 206e 6565 6420 666f  rack the need fo
-000013b0: 7220 6120 6368 616e 6765 0a61 6e64 2074  r a change.and t
-000013c0: 6865 6e20 6f70 7469 6f6e 616c 6c79 206f  hen optionally o
-000013d0: 7065 6e20 6120 7075 6c6c 2072 6571 7565  pen a pull reque
-000013e0: 7374 2077 6974 6820 6120 7072 6f70 6f73  st with a propos
-000013f0: 6564 2072 6573 6f6c 7574 696f 6e2e 2049  ed resolution. I
-00001400: 7373 7565 7320 616e 640a 7075 6c6c 2072  ssues and.pull r
-00001410: 6571 7565 7374 7320 7368 6f75 6c64 2061  equests should a
-00001420: 6c73 6f20 6265 2066 6f63 7573 6564 206f  lso be focused o
-00001430: 6e20 6120 7369 6e67 6c65 2074 6869 6e67  n a single thing
-00001440: 2e20 5075 6c6c 2072 6571 7565 7374 7320  . Pull requests 
-00001450: 7468 6174 0a62 756e 646c 6520 746f 6765  that.bundle toge
-00001460: 7468 6572 2061 2062 756e 6368 206f 6620  ther a bunch of 
-00001470: 6c6f 6f73 656c 7920 7265 6c61 7465 6420  loosely related 
-00001480: 636f 6d6d 6974 7320 6172 6520 756e 6c69  commits are unli
-00001490: 6b65 6c79 2074 6f20 676f 2061 6e79 7768  kely to go anywh
-000014a0: 6572 652e 0a0a 416e 6f74 6865 7220 676f  ere...Another go
-000014b0: 6f64 2072 756c 6520 6f66 2074 6875 6d62  od rule of thumb
-000014c0: e280 9466 6f72 2061 6e79 2070 726f 6a65  ...for any proje
-000014d0: 6374 2c20 6275 7420 6573 7065 6369 616c  ct, but especial
-000014e0: 6c79 2061 206d 6174 7572 6520 6f6e 65e2  ly a mature one.
-000014f0: 8094 6973 2074 6f0a 6b65 6570 2063 6861  ..is to.keep cha
-00001500: 6e67 6573 2061 7320 7369 6d70 6c65 2061  nges as simple a
-00001510: 7320 706f 7373 6962 6c65 2e20 496e 2070  s possible. In p
-00001520: 6172 7469 6375 6c61 722c 2074 6865 7265  articular, there
-00001530: 2073 686f 756c 6420 6265 2061 2068 6967   should be a hig
-00001540: 6820 6261 720a 666f 7220 6164 6469 6e67  h bar.for adding
-00001550: 206e 6577 2064 6570 656e 6465 6e63 6965   new dependencie
-00001560: 732e 2041 6c74 686f 7567 6820 6974 2063  s. Although it c
-00001570: 616e 2774 2062 6520 7275 6c65 6420 6f75  an't be ruled ou
-00001580: 742c 2069 7420 7365 656d 7320 6869 6768  t, it seems high
-00001590: 6c79 0a75 6e6c 696b 656c 7920 7468 6174  ly.unlikely that
-000015a0: 2061 206e 6577 2072 756e 7469 6d65 2064   a new runtime d
-000015b0: 6570 656e 6465 6e63 7920 7769 6c6c 2065  ependency will e
-000015c0: 7665 7220 6265 2061 6464 6564 2e20 4e65  ver be added. Ne
-000015d0: 7720 7465 7374 696e 670a 6465 7065 6e64  w testing.depend
-000015e0: 656e 6369 6573 2061 7265 206d 6f72 6520  encies are more 
-000015f0: 6c69 6b65 6c79 2c20 6275 7420 6f6e 6c79  likely, but only
-00001600: 2069 6620 7468 6572 6527 7320 6e6f 206f   if there's no o
-00001610: 7468 6572 2077 6179 2074 6f20 6164 6472  ther way to addr
-00001620: 6573 7320 616e 0a69 6d70 6f72 7461 6e74  ess an.important
-00001630: 206e 6565 642e 0a0a 4966 2074 6865 7265   need...If there
-00001640: 2773 2061 2064 6576 656c 6f70 6d65 6e74  's a development
-00001650: 2074 6f6f 6c20 7468 6174 2079 6f75 2764   tool that you'd
-00001660: 206c 696b 6520 746f 2075 7365 2077 6974   like to use wit
-00001670: 6820 7468 6973 2070 726f 6a65 6374 2c20  h this project, 
-00001680: 7468 650a 6669 7273 7420 7374 6570 2069  the.first step i
-00001690: 7320 746f 2074 7279 2074 6f20 7570 6461  s to try to upda
-000016a0: 7465 2063 6f6e 6669 6720 6669 6c65 7320  te config files 
-000016b0: 2873 6574 7570 2e63 6667 206f 7220 7369  (setup.cfg or si
-000016c0: 6d69 6c61 7229 2074 6f20 696e 7465 6772  milar) to integr
-000016d0: 6174 650a 7468 6520 746f 6f6c 2077 6974  ate.the tool wit
-000016e0: 6820 7468 6520 6578 6973 7469 6e67 2063  h the existing c
-000016f0: 6f64 652e 2041 2062 6974 206f 6620 636f  ode. A bit of co
-00001700: 6e66 6967 7572 6174 696f 6e20 676c 7565  nfiguration glue
-00001710: 2066 6f72 2070 6f70 756c 6172 2074 6f6f   for popular too
-00001720: 6c73 0a73 686f 756c 6420 616c 7761 7973  ls.should always
-00001730: 2062 6520 7361 6665 2e20 4966 2074 6861   be safe. If tha
-00001740: 7427 7320 6e6f 7420 706f 7373 6962 6c65  t's not possible
-00001750: 2c20 7765 2063 616e 2063 6f6e 7369 6465  , we can conside
-00001760: 7220 6d6f 6469 6679 696e 6720 7468 650a  r modifying the.
-00001770: 636f 6465 2074 6f20 6265 2063 6f6d 7061  code to be compa
-00001780: 7469 626c 6520 7769 7468 2061 2062 726f  tible with a bro
-00001790: 6164 6572 2072 616e 6765 206f 6620 746f  ader range of to
-000017a0: 6f6c 7320 2877 6974 686f 7574 2062 7265  ols (without bre
-000017b0: 616b 696e 6720 616e 790a 6578 6973 7469  aking any.existi
-000017c0: 6e67 2063 6f6d 7061 7469 6269 6c69 7469  ng compatibiliti
-000017d0: 6573 292e 204f 6e6c 7920 6173 2061 206c  es). Only as a l
-000017e0: 6173 7420 7265 736f 7274 2077 6f75 6c64  ast resort would
-000017f0: 2061 206e 6577 2074 6573 7469 6e67 206f   a new testing o
-00001800: 720a 6465 7665 6c6f 706d 656e 7420 746f  r.development to
-00001810: 6f6c 2062 6520 696e 636f 7270 6f72 6174  ol be incorporat
-00001820: 6564 2069 6e74 6f20 7468 6520 7072 6f6a  ed into the proj
-00001830: 6563 7420 6173 2061 2064 6570 656e 6465  ect as a depende
-00001840: 6e63 792e 0a0a 4974 2773 2061 6c73 6f20  ncy...It's also 
-00001850: 676f 6f64 2074 6f20 7265 6d65 6d62 6572  good to remember
-00001860: 2074 6861 7420 7772 6974 696e 6720 7468   that writing th
-00001870: 6520 636f 6465 2069 7320 7479 7069 6361  e code is typica
-00001880: 6c6c 7920 7468 6520 6c65 6173 7420 7061  lly the least pa
-00001890: 7274 206f 660a 7468 6520 776f 726b 2e20  rt of.the work. 
-000018a0: 5468 6973 2069 7320 7472 7565 2066 6f72  This is true for
-000018b0: 2073 6f66 7477 6172 6520 6465 7665 6c6f   software develo
-000018c0: 706d 656e 7420 696e 2067 656e 6572 616c  pment in general
-000018d0: 2c20 6275 7420 6573 7065 6369 616c 6c79  , but especially
-000018e0: 2061 0a73 6d61 6c6c 2073 7461 626c 6520   a.small stable 
-000018f0: 7072 6f6a 6563 7420 6c69 6b65 2074 6869  project like thi
-00001900: 732e 2054 6865 2062 756c 6b20 6f66 2074  s. The bulk of t
-00001910: 6865 2077 6f72 6b20 6973 2069 6e20 6075  he work is in `u
-00001920: 6e64 6572 7374 616e 6469 6e67 2074 6865  nderstanding the
-00001930: 0a70 726f 626c 656d 203c 6874 7470 3a2f  .problem <http:/
-00001940: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-00001950: 2f77 6174 6368 3f76 3d66 3834 6e35 6f46  /watch?v=f84n5oF
-00001960: 6f5a 4263 3e60 5f2c 2064 6574 6572 6d69  oZBc>`_, determi
-00001970: 6e69 6e67 2074 6865 2064 6573 6972 6564  ning the desired
-00001980: 0a61 7474 7269 6275 7465 7320 6f66 2061  .attributes of a
-00001990: 2073 6f6c 7574 696f 6e2c 2072 6573 6561   solution, resea
-000019a0: 7263 6869 6e67 2061 6e64 2065 7661 6c75  rching and evalu
-000019b0: 6174 696e 6720 616c 7465 726e 6174 6976  ating alternativ
-000019c0: 6573 2c20 7772 6974 696e 670a 646f 6375  es, writing.docu
-000019d0: 6d65 6e74 6174 696f 6e2c 2064 6573 6967  mentation, desig
-000019e0: 6e69 6e67 2061 2074 6573 7469 6e67 2073  ning a testing s
-000019f0: 7472 6174 6567 792c 2065 7463 2e20 5772  trategy, etc. Wr
-00001a00: 6974 696e 6720 7468 6520 636f 6465 2069  iting the code i
-00001a10: 7473 656c 6620 7465 6e64 730a 746f 2062  tself tends.to b
-00001a20: 6520 6120 6d69 6e6f 7220 6d61 7474 6572  e a minor matter
-00001a30: 2074 6861 7420 656d 6572 6765 7320 6672   that emerges fr
-00001a40: 6f6d 2074 6861 7420 7072 6f63 6573 732e  om that process.
-00001a50: 0a0a 0a2e 2e20 5f70 6970 656e 763a 2068  ..... _pipenv: h
-00001a60: 7474 7073 3a2f 2f70 6970 656e 762e 7265  ttps://pipenv.re
-00001a70: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00001a80: 6c61 7465 7374 2f0a 2e2e 205f 666c 616b  latest/... _flak
-00001a90: 6538 3a20 6874 7470 733a 2f2f 7079 7069  e8: https://pypi
-00001aa0: 2e6f 7267 2f70 726f 6a65 6374 2f66 6c61  .org/project/fla
-00001ab0: 6b65 382f 0a2e 2e20 5f69 736f 7274 3a20  ke8/... _isort: 
-00001ac0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00001ad0: 2f70 726f 6a65 6374 2f69 736f 7274 2f0a  /project/isort/.
-00001ae0: 0a0a                                     ..
+00000000: 2e2e 2076 696d 3a20 7477 3d38 3020 6c62  .. vim: tw=80 lb
+00000010: 720a 0a64 6a61 6e67 6f2d 6f74 700a 3d3d  r..django-otp.==
+00000020: 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e 2069 6d61  ========.... ima
+00000030: 6765 3a3a 2068 7474 7073 3a2f 2f69 6d67  ge:: https://img
+00000040: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000050: 2f76 2f64 6a61 6e67 6f2d 6f74 703f 636f  /v/django-otp?co
+00000060: 6c6f 723d 626c 7565 0a20 2020 3a74 6172  lor=blue.   :tar
+00000070: 6765 743a 2068 7474 7073 3a2f 2f70 7970  get: https://pyp
+00000080: 692e 6f72 672f 7072 6f6a 6563 742f 646a  i.org/project/dj
+00000090: 616e 676f 2d6f 7470 2f0a 2020 203a 616c  ango-otp/.   :al
+000000a0: 743a 2050 7950 490a 2e2e 2069 6d61 6765  t: PyPI... image
+000000b0: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
+000000c0: 6869 656c 6473 2e69 6f2f 7265 6164 7468  hields.io/readth
+000000d0: 6564 6f63 732f 646a 616e 676f 2d6f 7470  edocs/django-otp
+000000e0: 2d6f 6666 6963 6961 6c0a 2020 203a 7461  -official.   :ta
+000000f0: 7267 6574 3a20 6874 7470 733a 2f2f 646a  rget: https://dj
+00000100: 616e 676f 2d6f 7470 2d6f 6666 6963 6961  ango-otp-officia
+00000110: 6c2e 7265 6164 7468 6564 6f63 732e 696f  l.readthedocs.io
+00000120: 2f0a 2020 203a 616c 743a 2044 6f63 756d  /.   :alt: Docum
+00000130: 656e 7461 7469 6f6e 0a2e 2e20 696d 6167  entation... imag
+00000140: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
+00000150: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000160: 2f67 6974 6875 622d 646a 616e 676f 2d2d  /github-django--
+00000170: 6f74 702d 6772 6565 6e0a 2020 203a 7461  otp-green.   :ta
+00000180: 7267 6574 3a20 6874 7470 733a 2f2f 6769  rget: https://gi
+00000190: 7468 7562 2e63 6f6d 2f64 6a61 6e67 6f2d  thub.com/django-
+000001a0: 6f74 702f 646a 616e 676f 2d6f 7470 0a20  otp/django-otp. 
+000001b0: 2020 3a61 6c74 3a20 536f 7572 6365 0a0a    :alt: Source..
+000001c0: 5468 6973 2070 726f 6a65 6374 206d 616b  This project mak
+000001d0: 6573 2069 7420 6561 7379 2074 6f20 6164  es it easy to ad
+000001e0: 6420 7375 7070 6f72 7420 666f 7220 606f  d support for `o
+000001f0: 6e65 2d74 696d 6520 7061 7373 776f 7264  ne-time password
+00000200: 730a 3c68 7474 703a 2f2f 656e 2e77 696b  s.<http://en.wik
+00000210: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00000220: 4f6e 652d 7469 6d65 5f70 6173 7377 6f72  One-time_passwor
+00000230: 643e 605f 2028 4f54 5073 2920 746f 2044  d>`_ (OTPs) to D
+00000240: 6a61 6e67 6f2e 2049 7420 6361 6e20 6265  jango. It can be
+00000250: 0a69 6e74 6567 7261 7465 6420 6174 2076  .integrated at v
+00000260: 6172 696f 7573 206c 6576 656c 732c 2064  arious levels, d
+00000270: 6570 656e 6469 6e67 206f 6e20 686f 7720  epending on how 
+00000280: 6d75 6368 2063 7573 746f 6d69 7a61 7469  much customizati
+00000290: 6f6e 2069 7320 7265 7175 6972 6564 2e0a  on is required..
+000002a0: 4974 2069 6e74 6567 7261 7465 7320 7769  It integrates wi
+000002b0: 7468 2060 6064 6a61 6e67 6f2e 636f 6e74  th ``django.cont
+000002c0: 7269 622e 6175 7468 6060 2c20 616c 7468  rib.auth``, alth
+000002d0: 6f75 6768 2069 7420 6973 206e 6f74 2061  ough it is not a
+000002e0: 2044 6a61 6e67 6f0a 6175 7468 656e 7469   Django.authenti
+000002f0: 6361 7469 6f6e 2062 6163 6b65 6e64 2e20  cation backend. 
+00000300: 5468 6520 7072 696d 6172 7920 7461 7267  The primary targ
+00000310: 6574 2069 7320 6465 7665 6c6f 7065 7273  et is developers
+00000320: 2077 6973 6869 6e67 2074 6f20 696e 636f   wishing to inco
+00000330: 7270 6f72 6174 650a 4f54 5073 2069 6e74  rporate.OTPs int
+00000340: 6f20 7468 6569 7220 446a 616e 676f 2070  o their Django p
+00000350: 726f 6a65 6374 7320 6173 2061 2066 6f72  rojects as a for
+00000360: 6d20 6f66 2060 7477 6f2d 6661 6374 6f72  m of `two-factor
+00000370: 2061 7574 6865 6e74 6963 6174 696f 6e0a   authentication.
+00000380: 3c68 7474 703a 2f2f 656e 2e77 696b 6970  <http://en.wikip
+00000390: 6564 6961 2e6f 7267 2f77 696b 692f 5477  edia.org/wiki/Tw
+000003a0: 6f2d 6661 6374 6f72 5f61 7574 6865 6e74  o-factor_authent
+000003b0: 6963 6174 696f 6e3e 605f 2e0a 0a53 6576  ication>`_...Sev
+000003c0: 6572 616c 2073 696d 706c 6520 4f54 5020  eral simple OTP 
+000003d0: 706c 7567 696e 7320 6172 6520 696e 636c  plugins are incl
+000003e0: 7564 6564 2061 6e64 206d 6f72 6520 6172  uded and more ar
+000003f0: 6520 6176 6169 6c61 626c 6520 7365 7061  e available sepa
+00000400: 7261 7465 6c79 2e20 5468 6973 0a70 6163  rately. This.pac
+00000410: 6b61 6765 2061 6c73 6f20 696e 636c 7564  kage also includ
+00000420: 6573 2061 6e20 696d 706c 656d 656e 7461  es an implementa
+00000430: 7469 6f6e 206f 6620 4f41 5448 2060 484f  tion of OATH `HO
+00000440: 5450 0a3c 6874 7470 3a2f 2f74 6f6f 6c73  TP.<http://tools
+00000450: 2e69 6574 662e 6f72 672f 6874 6d6c 2f72  .ietf.org/html/r
+00000460: 6663 3432 3236 3e60 5f20 616e 6420 6054  fc4226>`_ and `T
+00000470: 4f54 500a 3c68 7474 703a 2f2f 746f 6f6c  OTP.<http://tool
+00000480: 732e 6965 7466 2e6f 7267 2f68 746d 6c2f  s.ietf.org/html/
+00000490: 7266 6336 3233 383e 605f 2066 6f72 2063  rfc6238>`_ for c
+000004a0: 6f6e 7665 6e69 656e 6365 2c20 6173 2074  onvenience, as t
+000004b0: 6865 7365 2061 7265 2073 7461 6e64 6172  hese are standar
+000004c0: 640a 4f54 5020 616c 676f 7269 7468 6d73  d.OTP algorithms
+000004d0: 2075 7365 6420 6279 206d 756c 7469 706c   used by multipl
+000004e0: 6520 706c 7567 696e 732e 0a0a 4966 2079  e plugins...If y
+000004f0: 6f75 2772 6520 6c6f 6f6b 696e 6720 666f  ou're looking fo
+00000500: 7220 6120 6869 6768 6572 2d6c 6576 656c  r a higher-level
+00000510: 206f 7220 6d6f 7265 206f 7069 6e69 6f6e   or more opinion
+00000520: 6174 6564 2073 6f6c 7574 696f 6e2c 2079  ated solution, y
+00000530: 6f75 206d 6967 6874 2062 650a 696e 7465  ou might be.inte
+00000540: 7265 7374 6564 2069 6e20 6064 6a61 6e67  rested in `djang
+00000550: 6f2d 7477 6f2d 6661 6374 6f72 2d61 7574  o-two-factor-aut
+00000560: 680a 3c68 7474 7073 3a2f 2f67 6974 6875  h.<https://githu
+00000570: 622e 636f 6d2f 426f 756b 652f 646a 616e  b.com/Bouke/djan
+00000580: 676f 2d74 776f 2d66 6163 746f 722d 6175  go-two-factor-au
+00000590: 7468 3e60 5f2e 0a0a 5374 6174 7573 0a2d  th>`_...Status.-
+000005a0: 2d2d 2d2d 2d0a 0a54 6869 7320 7072 6f6a  -----..This proj
+000005b0: 6563 7420 6973 2073 7461 626c 6520 616e  ect is stable an
+000005c0: 6420 6d61 696e 7461 696e 6564 2c20 6275  d maintained, bu
+000005d0: 7420 6973 206e 6f20 6c6f 6e67 6572 2061  t is no longer a
+000005e0: 6374 6976 656c 7920 7573 6564 2062 7920  ctively used by 
+000005f0: 7468 650a 6175 7468 6f72 2061 6e64 2069  the.author and i
+00000600: 7320 6e6f 7420 7365 6569 6e67 206d 7563  s not seeing muc
+00000610: 6820 6f6e 676f 696e 6720 696e 7665 7374  h ongoing invest
+00000620: 6d65 6e74 2e0a 0a57 656c 6c2d 666f 726d  ment...Well-form
+00000630: 6564 2069 7373 7565 7320 616e 6420 7075  ed issues and pu
+00000640: 6c6c 2072 6571 7565 7374 7320 6172 6520  ll requests are 
+00000650: 7765 6c63 6f6d 652c 2062 7574 2070 6c65  welcome, but ple
+00000660: 6173 6520 7365 6520 434f 4e54 5249 4255  ase see CONTRIBU
+00000670: 5449 4e47 2e6d 640a 6669 7273 742e 2047  TING.md.first. G
+00000680: 656e 6572 616c 2071 7565 7374 696f 6e73  eneral questions
+00000690: 2061 6e64 2069 6465 6173 2073 686f 756c   and ideas shoul
+000006a0: 6420 6265 2064 6972 6563 7465 6420 746f  d be directed to
+000006b0: 2074 6865 2044 6973 6375 7373 696f 6e73   the Discussions
+000006c0: 0a73 6563 7469 6f6e 3b20 6973 7375 6573  .section; issues
+000006d0: 2073 686f 756c 6420 6265 2072 6573 6572   should be reser
+000006e0: 7665 6420 666f 7220 636f 6e66 6972 6d65  ved for confirme
+000006f0: 6420 6275 6773 2e0a 0a2e 2e20 656e 642d  d bugs..... end-
+00000700: 6f66 2d64 6f63 2d69 6e74 726f 0a0a 0a44  of-doc-intro...D
+00000710: 6576 656c 6f70 6d65 6e74 0a2d 2d2d 2d2d  evelopment.-----
+00000720: 2d2d 2d2d 2d2d 0a0a 5468 6973 2070 726f  ------..This pro
+00000730: 6a65 6374 2069 7320 6275 696c 7420 616e  ject is built an
+00000740: 6420 6d61 6e61 6765 6420 7769 7468 2060  d managed with `
+00000750: 6861 7463 6860 5f2e 2049 6620 796f 7520  hatch`_. If you 
+00000760: 646f 6e27 7420 6861 7665 2068 6174 6368  don't have hatch
+00000770: 2c20 490a 7265 636f 6d6d 656e 6420 696e  , I.recommend in
+00000780: 7374 616c 6c69 6e67 2069 7420 7769 7468  stalling it with
+00000790: 2060 7069 7078 605f 3a20 6060 7069 7078   `pipx`_: ``pipx
+000007a0: 2069 6e73 7461 6c6c 2068 6174 6368 6060   install hatch``
+000007b0: 2e0a 0a60 6070 7970 726f 6a65 6374 2e74  ...``pyproject.t
+000007c0: 6f6d 6c60 6020 6465 6669 6e65 7320 7365  oml`` defines se
+000007d0: 7665 7261 6c20 7573 6566 756c 2073 6372  veral useful scr
+000007e0: 6970 7473 2066 6f72 2064 6576 656c 6f70  ipts for develop
+000007f0: 6d65 6e74 2061 6e64 2074 6573 7469 6e67  ment and testing
+00000800: 2e0a 5468 6520 6465 6661 756c 7420 656e  ..The default en
+00000810: 7669 726f 6e6d 656e 7420 696e 636c 7564  vironment includ
+00000820: 6573 2061 6c6c 2064 6576 2061 6e64 2074  es all dev and t
+00000830: 6573 7420 6465 7065 6e64 656e 6369 6573  est dependencies
+00000840: 2066 6f72 2071 7569 636b 6c79 0a72 756e   for quickly.run
+00000850: 6e69 6e67 2074 6573 7473 2e20 5468 6520  ning tests. The 
+00000860: 6060 7465 7374 6060 2065 6e76 6972 6f6e  ``test`` environ
+00000870: 6d65 6e74 2064 6566 696e 6573 2074 6865  ment defines the
+00000880: 2074 6573 7420 6d61 7472 6978 2066 6f72   test matrix for
+00000890: 2072 756e 6e69 6e67 2074 6865 0a66 756c   running the.ful
+000008a0: 6c20 7661 6c69 6461 7469 6f6e 2073 7569  l validation sui
+000008b0: 7465 2e20 4576 6572 7974 6869 6e67 2069  te. Everything i
+000008c0: 7320 6578 6563 7574 6564 2069 6e20 7468  s executed in th
+000008d0: 6520 636f 6e74 6578 7420 6f66 2074 6865  e context of the
+000008e0: 2044 6a61 6e67 6f0a 7072 6f6a 6563 7420   Django.project 
+000008f0: 696e 2074 6573 742f 7465 7374 5c5f 7072  in test/test\_pr
+00000900: 6f6a 6563 742e 0a0a 4173 2061 2071 7569  oject...As a qui
+00000910: 636b 2070 7269 6d65 722c 2068 6174 6368  ck primer, hatch
+00000920: 2073 6372 6970 7473 2063 616e 2062 6520   scripts can be 
+00000930: 7275 6e20 7769 7468 2060 6068 6174 6368  run with ``hatch
+00000940: 2072 756e 205b 3c65 6e76 3e3a 5d3c 7363   run [<env>:]<sc
+00000950: 7269 7074 3e60 602e 0a54 6f20 7275 6e20  ript>``..To run 
+00000960: 6c69 6e74 6572 7320 616e 6420 7465 7374  linters and test
+00000970: 7320 696e 2074 6865 2064 6566 6175 6c74  s in the default
+00000980: 2065 6e76 6972 6f6e 6d65 6e74 2c20 6a75   environment, ju
+00000990: 7374 2072 756e 0a60 6068 6174 6368 2072  st run.``hatch r
+000009a0: 756e 2063 6865 636b 6060 2e20 5468 6973  un check``. This
+000009b0: 2073 686f 756c 6420 7275 6e20 7465 7374   should run test
+000009c0: 7320 7769 7468 2079 6f75 7220 6465 6661  s with your defa
+000009d0: 756c 7420 5079 7468 6f6e 2076 6572 7369  ult Python versi
+000009e0: 6f6e 2061 6e64 0a74 6865 206c 6174 6573  on and.the lates
+000009f0: 7420 446a 616e 676f 2e20 4f74 6865 7220  t Django. Other 
+00000a00: 7363 7269 7074 7320 696e 636c 7564 653a  scripts include:
+00000a10: 0a0a 2a20 2a2a 6d61 6e61 6765 2a2a 3a20  ..* **manage**: 
+00000a20: 5275 6e20 6120 6d61 6e61 6765 6d65 6e74  Run a management
+00000a30: 2063 6f6d 6d61 6e64 2076 6961 2074 6865   command via the
+00000a40: 2074 6573 7420 7072 6f6a 6563 742e 2054   test project. T
+00000a50: 6869 7320 6361 6e20 6265 2075 7365 6420  his can be used 
+00000a60: 746f 0a20 2067 656e 6572 6174 6520 6d69  to.  generate mi
+00000a70: 6772 6174 696f 6e73 2e0a 2a20 2a2a 6c69  grations..* **li
+00000a80: 6e74 2a2a 3a20 5275 6e20 616c 6c20 6c69  nt**: Run all li
+00000a90: 6e74 6572 732e 0a2a 202a 2a66 6978 2a2a  nters..* **fix**
+00000aa0: 3a20 5275 6e20 616c 6c20 6669 7865 7273  : Run all fixers
+00000ab0: 2074 6f20 6164 6472 6573 7320 6c69 6e74   to address lint
+00000ac0: 696e 6720 6973 7375 6573 2e20 5468 6973  ing issues. This
+00000ad0: 206d 6179 206e 6f74 2066 6978 2065 7665   may not fix eve
+00000ae0: 7279 0a20 2069 7373 7565 2072 6570 6f72  ry.  issue repor
+00000af0: 7465 6420 6279 206c 696e 742e 0a2a 202a  ted by lint..* *
+00000b00: 2a74 6573 742a 2a3a 2052 756e 2061 6c6c  *test**: Run all
+00000b10: 2074 6573 7473 2e0a 2a20 2a2a 6368 6563   tests..* **chec
+00000b20: 6b2a 2a3a 2052 756e 206c 696e 7465 7273  k**: Run linters
+00000b30: 2061 6e64 2074 6573 7473 2e0a 2a20 2a2a   and tests..* **
+00000b40: 7761 726e 2a2a 3a20 5275 6e20 7465 7374  warn**: Run test
+00000b50: 7320 7769 7468 2061 6c6c 2077 6172 6e69  s with all warni
+00000b60: 6e67 7320 656e 6162 6c65 642e 2054 6869  ngs enabled. Thi
+00000b70: 7320 6973 2065 7370 6563 6961 6c6c 7920  s is especially 
+00000b80: 7573 6566 756c 2066 6f72 0a20 2073 6565  useful for.  see
+00000b90: 696e 6720 6465 7072 6563 6174 696f 6e20  ing deprecation 
+00000ba0: 7761 726e 696e 6773 2069 6e20 6e65 7720  warnings in new 
+00000bb0: 7665 7273 696f 6e73 206f 6620 446a 616e  versions of Djan
+00000bc0: 676f 2e0a 2a20 2a2a 636f 762a 2a3a 2052  go..* **cov**: R
+00000bd0: 756e 2074 6573 7473 2061 6e64 2070 7269  un tests and pri
+00000be0: 6e74 2061 2063 6f64 6520 636f 7665 7261  nt a code covera
+00000bf0: 6765 2072 6570 6f72 742e 0a0a 546f 2072  ge report...To r
+00000c00: 756e 2074 6865 2066 756c 6c20 7465 7374  un the full test
+00000c10: 206d 6174 7269 782c 2072 756e 2060 6068   matrix, run ``h
+00000c20: 6174 6368 2072 756e 2074 6573 743a 7275  atch run test:ru
+00000c30: 6e60 602e 2059 6f75 2077 696c 6c20 6e65  n``. You will ne
+00000c40: 6564 206d 756c 7469 706c 650a 7370 6563  ed multiple.spec
+00000c50: 6966 6963 2050 7974 686f 6e20 7665 7273  ific Python vers
+00000c60: 696f 6e73 2069 6e73 7461 6c6c 6564 2066  ions installed f
+00000c70: 6f72 2074 6869 732e 0a0a 596f 7520 6361  or this...You ca
+00000c80: 6e20 636c 6561 6e20 7570 2074 6865 2068  n clean up the h
+00000c90: 6174 6368 2065 6e76 6972 6f6e 6d65 6e74  atch environment
+00000ca0: 7320 7769 7468 2060 6068 6174 6368 2065  s with ``hatch e
+00000cb0: 6e76 2070 7275 6e65 6060 2c20 666f 7220  nv prune``, for 
+00000cc0: 6578 616d 706c 6520 746f 0a66 6f72 6365  example to.force
+00000cd0: 2064 6570 656e 6465 6e63 7920 7570 6461   dependency upda
+00000ce0: 7465 732e 0a0a 5468 6520 7072 6f6a 6563  tes...The projec
+00000cf0: 7420 756e 6465 7220 6060 7465 7374 6060  t under ``test``
+00000d00: 2063 616e 2062 6520 7275 6e20 6173 2061   can be run as a
+00000d10: 2073 696d 706c 6520 696e 7465 7261 6374   simple interact
+00000d20: 6976 6520 7465 7374 2065 6e76 6972 6f6e  ive test environ
+00000d30: 6d65 6e74 2e0a 5275 6e20 6060 6861 7463  ment..Run ``hatc
+00000d40: 6820 7275 6e20 6d61 6e61 6765 2072 756e  h run manage run
+00000d50: 7365 7276 6572 6060 2061 6e64 206f 7065  server`` and ope
+00000d60: 6e20 6974 2069 6e20 6120 6272 6f77 7365  n it in a browse
+00000d70: 722e 2054 6869 7320 6861 7320 616e 0a69  r. This has an.i
+00000d80: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
+00000d90: 2074 6865 206c 6f67 696e 2066 6f72 6d20   the login form 
+00000da0: 616e 6420 7669 6577 7320 7769 7468 2064  and views with d
+00000db0: 6966 6665 7265 6e74 2063 6f6d 6269 6e61  ifferent combina
+00000dc0: 7469 6f6e 7320 6f66 0a64 6563 6f72 6174  tions of.decorat
+00000dd0: 6f72 732c 2077 6869 6368 2079 6f75 2063  ors, which you c
+00000de0: 616e 2065 7870 6572 696d 656e 7420 7769  an experiment wi
+00000df0: 7468 206f 7220 7573 6520 746f 2074 6573  th or use to tes
+00000e00: 7420 6368 616e 6765 732e 0a0a 436f 6e66  t changes...Conf
+00000e10: 6967 7572 6174 696f 6e0a 7e7e 7e7e 7e7e  iguration.~~~~~~
+00000e20: 7e7e 7e7e 7e7e 7e0a 0a42 7920 6465 6661  ~~~~~~~..By defa
+00000e30: 756c 742c 2074 6865 2074 6573 7420 7072  ult, the test pr
+00000e40: 6f6a 6563 7420 7573 6573 2053 514c 6974  oject uses SQLit
+00000e50: 652e 2042 6563 6175 7365 2053 514c 6974  e. Because SQLit
+00000e60: 6520 646f 6573 6e27 7420 7375 7070 6f72  e doesn't suppor
+00000e70: 7420 726f 770a 6c6f 636b 696e 672c 2073  t row.locking, s
+00000e80: 6f6d 6520 636f 6e63 7572 7265 6e63 7920  ome concurrency 
+00000e90: 7465 7374 7320 7769 6c6c 2062 6520 736b  tests will be sk
+00000ea0: 6970 7065 642e 2054 6f20 7465 7374 2061  ipped. To test a
+00000eb0: 6761 696e 7374 2050 6f73 7467 7265 5351  gainst PostgreSQ
+00000ec0: 4c2c 2079 6f75 0a63 616e 2061 6464 2061  L, you.can add a
+00000ed0: 206c 6f63 616c 2063 6f6e 6669 6775 7261   local configura
+00000ee0: 7469 6f6e 2066 696c 6520 7468 6174 2070  tion file that p
+00000ef0: 6f69 6e74 7320 746f 2079 6f75 7220 6461  oints to your da
+00000f00: 7461 6261 7365 2e0a 0a43 6f6e 6669 6775  tabase...Configu
+00000f10: 7261 7469 6f6e 2069 7320 7461 6b65 6e20  ration is taken 
+00000f20: 6672 6f6d 2054 4f4d 4c20 6669 6c65 7320  from TOML files 
+00000f30: 7374 6f72 6564 2075 6e64 6572 2060 6074  stored under ``t
+00000f40: 6573 742f 636f 6e66 6967 6060 2e20 4120  est/config``. A 
+00000f50: 636f 6e66 6967 0a66 696c 6520 6e61 6d65  config.file name
+00000f60: 6420 6060 656e 762d 3c65 6e76 2d6e 616d  d ``env-<env-nam
+00000f70: 653e 2e74 6f6d 6c60 6020 7769 6c6c 2062  e>.toml`` will b
+00000f80: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
+00000f90: 6170 706c 6965 6420 7768 656e 2072 756e  applied when run
+00000fa0: 6e69 6e67 0a69 6e73 6964 6520 6120 6d61  ning.inside a ma
+00000fb0: 7463 6869 6e67 2068 6174 6368 2065 6e76  tching hatch env
+00000fc0: 6972 6f6e 6d65 6e74 2e20 466f 7220 6578  ironment. For ex
+00000fd0: 616d 706c 652c 2060 6065 6e76 2d64 6566  ample, ``env-def
+00000fe0: 6175 6c74 2e74 6f6d 6c60 6020 6170 706c  ault.toml`` appl
+00000ff0: 6965 730a 746f 2074 6865 2064 6566 6175  ies.to the defau
+00001000: 6c74 2064 6576 656c 6f70 6d65 6e74 2065  lt development e
+00001010: 6e76 6972 6f6e 6d65 6e74 2061 6e64 2060  nvironment and `
+00001020: 6065 6e76 2d74 6573 742e 746f 6d6c 6060  `env-test.toml``
+00001030: 2061 7070 6c69 6573 2074 6f20 7468 6520   applies to the 
+00001040: 7465 7374 0a6d 6174 7269 7820 656e 7669  test.matrix envi
+00001050: 726f 6e6d 656e 7473 2e0a 0a57 6974 6820  ronments...With 
+00001060: 6120 7769 6465 2d6f 7065 6e20 506f 7374  a wide-open Post
+00001070: 6772 6553 514c 2069 6e73 7461 6c6c 2c20  greSQL install, 
+00001080: 616e 2060 6065 6e76 2d74 6573 742e 746f  an ``env-test.to
+00001090: 6d6c 6060 206d 6967 6874 206c 6f6f 6b20  ml`` might look 
+000010a0: 6c69 6b65 2074 6869 733a 0a0a 2e2e 2063  like this:.... c
+000010b0: 6f64 652d 626c 6f63 6b3a 3a20 746f 6d6c  ode-block:: toml
+000010c0: 0a0a 2020 205b 6461 7461 6261 7365 5d0a  ..   [database].
+000010d0: 2020 2045 4e47 494e 4520 3d20 2264 6a61     ENGINE = "dja
+000010e0: 6e67 6f2e 6462 2e62 6163 6b65 6e64 732e  ngo.db.backends.
+000010f0: 706f 7374 6772 6573 716c 220a 2020 204e  postgresql".   N
+00001100: 414d 4520 3d20 2264 6a61 6e67 6f2d 6f74  AME = "django-ot
+00001110: 7022 0a20 2020 5553 4552 203d 2022 706f  p".   USER = "po
+00001120: 7374 6772 6573 220a 0a46 6f72 2064 6576  stgres"..For dev
+00001130: 656c 6f70 6d65 6e74 2c20 7468 6520 636f  elopment, the co
+00001140: 6e66 6967 2066 696c 6520 6361 6e20 616c  nfig file can al
+00001150: 736f 2062 6520 7573 6564 2074 6f20 696e  so be used to in
+00001160: 6a65 6374 2044 6a61 6e67 6f20 6170 7073  ject Django apps
+00001170: 2061 6e64 0a6d 6964 646c 6577 6172 652c   and.middleware,
+00001180: 206f 7220 746f 206f 7665 7272 6964 6520   or to override 
+00001190: 6172 6269 7472 6172 7920 446a 616e 676f  arbitrary Django
+000011a0: 2073 6574 7469 6e67 732e 2053 6565 0a60   settings. See.`
+000011b0: 6074 6573 742f 636f 6e66 6967 2f73 616d  `test/config/sam
+000011c0: 706c 652e 746f 6d6c 6060 2066 6f72 2061  ple.toml`` for a
+000011d0: 2066 756c 6c20 6465 7363 7269 7074 696f   full descriptio
+000011e0: 6e2e 0a0a 596f 7520 6361 6e20 616c 736f  n...You can also
+000011f0: 2066 6f72 6365 2061 2073 7065 6369 6669   force a specifi
+00001200: 6320 636f 6e66 6967 2066 696c 6520 6279  c config file by
+00001210: 2073 6574 7469 6e67 2074 6865 2065 6e76   setting the env
+00001220: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00001230: 650a 6060 444a 414e 474f 5f4f 5450 5f43  e.``DJANGO_OTP_C
+00001240: 4f4e 4649 4760 6020 746f 2061 2070 6174  ONFIG`` to a pat
+00001250: 682e 0a0a 0a54 6865 2046 7574 7572 650a  h....The Future.
+00001260: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4f6e 6365  ----------..Once
+00001270: 2075 706f 6e20 6120 7469 6d65 2c20 6576   upon a time, ev
+00001280: 6572 7974 6869 6e67 2077 6173 2075 7365  erything was use
+00001290: 726e 616d 6573 2061 6e64 2070 6173 7377  rnames and passw
+000012a0: 6f72 6473 2e20 4f72 2065 7665 6e20 696e  ords. Or even in
+000012b0: 2074 6865 2063 6173 6520 6f66 0a6f 7468   the case of.oth
+000012c0: 6572 2061 7574 6865 6e74 6963 6174 696f  er authenticatio
+000012d0: 6e20 6d65 6368 616e 6973 6d73 2c20 6120  n mechanisms, a 
+000012e0: 7573 6572 2077 6173 2065 6974 6865 7220  user was either 
+000012f0: 6175 7468 656e 7469 6361 7465 6420 6f72  authenticated or
+00001300: 206e 6f74 0a28 616e 6f6e 796d 6f75 7320   not.(anonymous 
+00001310: 696e 2044 6a61 6e67 6f27 7320 7465 726d  in Django's term
+00001320: 696e 6f6c 6f67 7929 2e20 5468 656e 2074  inology). Then t
+00001330: 6865 7265 2077 6173 2074 776f 2d66 6163  here was two-fac
+00001340: 746f 7220 6175 7468 656e 7469 6361 7469  tor authenticati
+00001350: 6f6e 2c0a 7768 6963 6820 636f 756c 6420  on,.which could 
+00001360: 7369 6d70 6c79 2062 6520 616e 2069 6d70  simply be an imp
+00001370: 6c65 6d65 6e74 6174 696f 6e20 6465 7461  lementation deta
+00001380: 696c 2069 6e20 6120 6269 6e61 7279 2061  il in a binary a
+00001390: 7574 6865 6e74 6963 6174 696f 6e20 7374  uthentication st
+000013a0: 6174 652c 0a62 7574 2063 6f75 6c64 2061  ate,.but could a
+000013b0: 6c73 6f20 696d 706c 7920 6c65 7665 6c73  lso imply levels
+000013c0: 206f 7220 6465 6772 6565 7320 6f66 2061   or degrees of a
+000013d0: 7574 6865 6e74 6963 6174 696f 6e2e 0a0a  uthentication...
+000013e0: 5468 6573 6520 6461 7973 2c20 6974 2773  These days, it's
+000013f0: 2069 6e63 7265 6173 696e 676c 7920 636f   increasingly co
+00001400: 6d6d 6f6e 2074 6f20 7365 6520 7369 7465  mmon to see site
+00001410: 7320 7769 7468 206d 6f72 6520 6e75 616e  s with more nuan
+00001420: 6365 640a 6175 7468 656e 7469 6361 7469  ced.authenticati
+00001430: 6f6e 2073 7461 7465 2e20 4120 7369 7465  on state. A site
+00001440: 206d 6967 6874 2072 656d 656d 6265 7220   might remember 
+00001450: 7768 6f20 796f 7520 6172 6520 666f 7265  who you are fore
+00001460: 7665 72e2 8094 736f 2079 6f75 2772 6520  ver...so you're 
+00001470: 6e6f 740a 616e 6f6e 796d 6f75 73e2 8094  not.anonymous...
+00001480: 6275 7420 6966 2079 6f75 2074 7279 2074  but if you try t
+00001490: 6f20 646f 2061 6e79 7468 696e 6720 7072  o do anything pr
+000014a0: 6976 6174 652c 2079 6f75 2068 6176 6520  ivate, you have 
+000014b0: 746f 2072 652d 6175 7468 656e 7469 6361  to re-authentica
+000014c0: 7465 2e0a 596f 7520 6d61 7920 6265 2061  te..You may be a
+000014d0: 626c 6520 746f 2063 686f 6f73 6520 6672  ble to choose fr
+000014e0: 6f6d 2061 6d6f 6e67 2061 6c6c 206f 6620  om among all of 
+000014f0: 7468 6520 6175 7468 656e 7469 6361 7469  the authenticati
+00001500: 6f6e 206d 6563 6861 6e69 736d 7320 796f  on mechanisms yo
+00001510: 750a 6861 7665 2063 6f6e 6669 6775 7265  u.have configure
+00001520: 642c 206f 7220 6f6e 6c79 2066 726f 6d20  d, or only from 
+00001530: 736f 6d65 206f 6620 7468 656d 2e20 5370  some of them. Sp
+00001540: 6563 6966 6963 206d 6563 6861 6e69 736d  ecific mechanism
+00001550: 7320 6d61 7920 6265 2072 6571 7569 7265  s may be require
+00001560: 640a 666f 7220 7370 6563 6966 6963 2061  d.for specific a
+00001570: 6374 696f 6e73 2c20 7375 6368 2061 7320  ctions, such as 
+00001580: 7573 696e 6720 796f 7572 2055 3246 2064  using your U2F d
+00001590: 6576 6963 6520 746f 2061 6363 6573 7320  evice to access 
+000015a0: 796f 7572 2055 3246 2073 6574 7469 6e67  your U2F setting
+000015b0: 732e 0a0a 496e 2073 686f 7274 2c20 7468  s...In short, th
+000015c0: 6520 776f 726c 6420 7365 656d 7320 746f  e world seems to
+000015d0: 2062 6520 6d6f 7669 6e67 2062 6579 6f6e   be moving beyon
+000015e0: 6420 7468 6520 6173 7375 6d70 7469 6f6e  d the assumption
+000015f0: 7320 7468 6174 206f 7269 6769 6e61 6c6c  s that originall
+00001600: 790a 696e 666f 726d 6564 2044 6a61 6e67  y.informed Djang
+00001610: 6f27 7320 6573 7365 6e74 6961 6c20 6175  o's essential au
+00001620: 7468 656e 7469 6361 7469 6f6e 2064 6573  thentication des
+00001630: 6967 6e2e 2049 6620 4920 7765 7265 2073  ign. If I were s
+00001640: 7469 6c6c 2069 6e76 6573 7469 6e67 2069  till investing i
+00001650: 6e0a 446a 616e 676f 2067 656e 6572 616c  n.Django general
+00001660: 6c79 2c20 4920 776f 756c 6420 7072 6f62  ly, I would prob
+00001670: 6162 6c79 2073 7461 7274 2061 206e 6577  ably start a new
+00001680: 206d 756c 7469 2d66 6163 746f 7220 6175   multi-factor au
+00001690: 7468 656e 7469 6361 7469 6f6e 0a70 726f  thentication.pro
+000016a0: 6a65 6374 2074 6861 7420 776f 756c 6420  ject that would 
+000016b0: 7265 666c 6563 7420 7468 6573 6520 6368  reflect these ch
+000016c0: 616e 6765 732e 2049 7420 776f 756c 6420  anges. It would 
+000016d0: 696e 636f 7270 6f72 6174 6520 7468 6520  incorporate the 
+000016e0: 6964 6561 2074 6861 7420 610a 7573 6572  idea that a.user
+000016f0: 206d 6179 2062 6520 6175 7468 656e 7469   may be authenti
+00001700: 6361 7465 6420 6279 2076 6172 696f 7573  cated by various
+00001710: 2063 6f6d 6269 6e61 7469 6f6e 7320 6f66   combinations of
+00001720: 206d 6563 6861 6e69 736d 7320 6174 2061   mechanisms at a
+00001730: 6e79 2074 696d 6520 616e 640a 7468 6174  ny time and.that
+00001740: 2064 6966 6665 7265 6e74 2063 6f6d 6269   different combi
+00001750: 6e61 7469 6f6e 7320 6d61 7920 6265 2072  nations may be r
+00001760: 6571 7569 7265 6420 746f 2073 6174 6973  equired to satis
+00001770: 6679 2064 6976 6572 7365 2061 7574 686f  fy diverse autho
+00001780: 7269 7a61 7469 6f6e 0a72 6571 7569 7265  rization.require
+00001790: 6d65 6e74 7320 6163 726f 7373 2074 6865  ments across the
+000017a0: 2073 6974 652e 2049 7420 776f 756c 6420   site. It would 
+000017b0: 6d6f 7374 206c 696b 656c 7920 7472 7920  most likely try 
+000017c0: 746f 2064 6973 656e 7461 6e67 6c65 0a61  to disentangle.a
+000017d0: 7574 6865 6e74 6963 6174 696f 6e20 7065  uthentication pe
+000017e0: 7273 6973 7465 6e63 6520 6672 6f6d 2073  rsistence from s
+000017f0: 6573 7369 6f6e 732c 2061 7420 6c65 6173  essions, at leas
+00001800: 7420 746f 2073 6f6d 6520 6578 7465 6e74  t to some extent
+00001810: 2e20 4d61 6e79 2073 6974 6573 0a77 6f75  . Many sites.wou
+00001820: 6c64 206e 6f74 2072 6571 7569 7265 2061  ld not require a
+00001830: 6c6c 206f 6620 7468 6973 2066 6c65 7869  ll of this flexi
+00001840: 6269 6c69 7479 2c20 6275 7420 6974 2077  bility, but it w
+00001850: 6f75 6c64 206f 7065 6e20 7570 2070 6f73  ould open up pos
+00001860: 7369 6269 6c69 7469 6573 0a66 6f72 2062  sibilities.for b
+00001870: 6574 7465 7220 6578 7065 7269 656e 6365  etter experience
+00001880: 7320 6279 206e 6f74 2061 736b 696e 6720  s by not asking 
+00001890: 7573 6572 7320 666f 7220 6d6f 7265 2074  users for more t
+000018a0: 6861 6e20 7765 2072 6571 7569 7265 2061  han we require a
+000018b0: 7420 616e 790a 706f 696e 742e 0a0a 4966  t any.point...If
+000018c0: 2061 6e79 6f6e 6520 6861 7320 6120 6d69   anyone has a mi
+000018d0: 6e64 2074 6f20 7461 6b65 206f 6e20 6120  nd to take on a 
+000018e0: 7072 6f6a 6563 7420 6c69 6b65 2074 6869  project like thi
+000018f0: 732c 2049 2764 2062 6520 6861 7070 7920  s, I'd be happy 
+00001900: 746f 206f 6666 6572 0a77 6861 7465 7665  to offer.whateve
+00001910: 7220 6164 7669 6365 206f 7220 6c65 7373  r advice or less
+00001920: 6f6e 7320 6c65 6172 6e65 6420 7468 6174  ons learned that
+00001930: 2049 2063 616e 2e0a 0a0a 2e2e 205f 6861   I can...... _ha
+00001940: 7463 683a 2068 7474 7073 3a2f 2f68 6174  tch: https://hat
+00001950: 6368 2e70 7970 612e 696f 2f0a 2e2e 205f  ch.pypa.io/... _
+00001960: 7069 7078 3a20 6874 7470 733a 2f2f 7079  pipx: https://py
+00001970: 7061 2e67 6974 6875 622e 696f 2f70 6970  pa.github.io/pip
+00001980: 782f 0a                                  x/.
```

### Comparing `django-otp-1.1.6/README.rst` & `django_otp-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,376 +1,468 @@
-00000000: 646a 616e 676f 2d6f 7470 0a3d 3d3d 3d3d  django-otp.=====
-00000010: 3d3d 3d3d 3d0a 0a2e 2e20 696d 6167 653a  =====.... image:
-00000020: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000030: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
-00000040: 646a 616e 676f 2d6f 7470 3f63 6f6c 6f72  django-otp?color
-00000050: 3d62 6c75 650a 2020 203a 7461 7267 6574  =blue.   :target
-00000060: 3a20 6874 7470 733a 2f2f 7079 7069 2e6f  : https://pypi.o
-00000070: 7267 2f70 726f 6a65 6374 2f64 6a61 6e67  rg/project/djang
-00000080: 6f2d 6f74 702f 0a20 2020 3a61 6c74 3a20  o-otp/.   :alt: 
-00000090: 5079 5049 0a2e 2e20 696d 6167 653a 3a20  PyPI... image:: 
-000000a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000000b0: 6c64 732e 696f 2f72 6561 6474 6865 646f  lds.io/readthedo
-000000c0: 6373 2f64 6a61 6e67 6f2d 6f74 702d 6f66  cs/django-otp-of
-000000d0: 6669 6369 616c 0a20 2020 3a74 6172 6765  ficial.   :targe
-000000e0: 743a 2068 7474 7073 3a2f 2f64 6a61 6e67  t: https://djang
-000000f0: 6f2d 6f74 702d 6f66 6669 6369 616c 2e72  o-otp-official.r
-00000100: 6561 6474 6865 646f 6373 2e69 6f2f 0a20  eadthedocs.io/. 
-00000110: 2020 3a61 6c74 3a20 446f 6375 6d65 6e74    :alt: Document
-00000120: 6174 696f 6e0a 2e2e 2069 6d61 6765 3a3a  ation... image::
-00000130: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
-00000140: 656c 6473 2e69 6f2f 6261 6467 652f 6769  elds.io/badge/gi
-00000150: 7468 7562 2d64 6a61 6e67 6f2d 2d6f 7470  thub-django--otp
-00000160: 2d67 7265 656e 0a20 2020 3a74 6172 6765  -green.   :targe
-00000170: 743a 2068 7474 7073 3a2f 2f67 6974 6875  t: https://githu
-00000180: 622e 636f 6d2f 646a 616e 676f 2d6f 7470  b.com/django-otp
-00000190: 2f64 6a61 6e67 6f2d 6f74 700a 2020 203a  /django-otp.   :
-000001a0: 616c 743a 2053 6f75 7263 650a 0a54 6869  alt: Source..Thi
-000001b0: 7320 7072 6f6a 6563 7420 6d61 6b65 7320  s project makes 
-000001c0: 6974 2065 6173 7920 746f 2061 6464 2073  it easy to add s
-000001d0: 7570 706f 7274 2066 6f72 2060 6f6e 652d  upport for `one-
-000001e0: 7469 6d65 2070 6173 7377 6f72 6473 0a3c  time passwords.<
-000001f0: 6874 7470 3a2f 2f65 6e2e 7769 6b69 7065  http://en.wikipe
-00000200: 6469 612e 6f72 672f 7769 6b69 2f4f 6e65  dia.org/wiki/One
-00000210: 2d74 696d 655f 7061 7373 776f 7264 3e60  -time_password>`
-00000220: 5f20 284f 5450 7329 2074 6f20 446a 616e  _ (OTPs) to Djan
-00000230: 676f 2e20 4974 2063 616e 2062 650a 696e  go. It can be.in
-00000240: 7465 6772 6174 6564 2061 7420 7661 7269  tegrated at vari
-00000250: 6f75 7320 6c65 7665 6c73 2c20 6465 7065  ous levels, depe
-00000260: 6e64 696e 6720 6f6e 2068 6f77 206d 7563  nding on how muc
-00000270: 6820 6375 7374 6f6d 697a 6174 696f 6e20  h customization 
-00000280: 6973 2072 6571 7569 7265 642e 0a49 7420  is required..It 
-00000290: 696e 7465 6772 6174 6573 2077 6974 6820  integrates with 
-000002a0: 6060 646a 616e 676f 2e63 6f6e 7472 6962  ``django.contrib
-000002b0: 2e61 7574 6860 602c 2061 6c74 686f 7567  .auth``, althoug
-000002c0: 6820 6974 2069 7320 6e6f 7420 6120 446a  h it is not a Dj
-000002d0: 616e 676f 0a61 7574 6865 6e74 6963 6174  ango.authenticat
-000002e0: 696f 6e20 6261 636b 656e 642e 2054 6865  ion backend. The
-000002f0: 2070 7269 6d61 7279 2074 6172 6765 7420   primary target 
-00000300: 6973 2064 6576 656c 6f70 6572 7320 7769  is developers wi
-00000310: 7368 696e 6720 746f 2069 6e63 6f72 706f  shing to incorpo
-00000320: 7261 7465 0a4f 5450 7320 696e 746f 2074  rate.OTPs into t
-00000330: 6865 6972 2044 6a61 6e67 6f20 7072 6f6a  heir Django proj
-00000340: 6563 7473 2061 7320 6120 666f 726d 206f  ects as a form o
-00000350: 6620 6074 776f 2d66 6163 746f 7220 6175  f `two-factor au
-00000360: 7468 656e 7469 6361 7469 6f6e 0a3c 6874  thentication.<ht
-00000370: 7470 3a2f 2f65 6e2e 7769 6b69 7065 6469  tp://en.wikipedi
-00000380: 612e 6f72 672f 7769 6b69 2f54 776f 2d66  a.org/wiki/Two-f
-00000390: 6163 746f 725f 6175 7468 656e 7469 6361  actor_authentica
-000003a0: 7469 6f6e 3e60 5f2e 0a0a 5365 7665 7261  tion>`_...Severa
-000003b0: 6c20 7369 6d70 6c65 204f 5450 2070 6c75  l simple OTP plu
-000003c0: 6769 6e73 2061 7265 2069 6e63 6c75 6465  gins are include
-000003d0: 6420 616e 6420 6d6f 7265 2061 7265 2061  d and more are a
-000003e0: 7661 696c 6162 6c65 2073 6570 6172 6174  vailable separat
-000003f0: 656c 792e 2054 6869 730a 7061 636b 6167  ely. This.packag
-00000400: 6520 616c 736f 2069 6e63 6c75 6465 7320  e also includes 
-00000410: 616e 2069 6d70 6c65 6d65 6e74 6174 696f  an implementatio
-00000420: 6e20 6f66 204f 4154 4820 6048 4f54 500a  n of OATH `HOTP.
-00000430: 3c68 7474 703a 2f2f 746f 6f6c 732e 6965  <http://tools.ie
-00000440: 7466 2e6f 7267 2f68 746d 6c2f 7266 6334  tf.org/html/rfc4
-00000450: 3232 363e 605f 2061 6e64 2060 544f 5450  226>`_ and `TOTP
-00000460: 0a3c 6874 7470 3a2f 2f74 6f6f 6c73 2e69  .<http://tools.i
-00000470: 6574 662e 6f72 672f 6874 6d6c 2f72 6663  etf.org/html/rfc
-00000480: 3632 3338 3e60 5f20 666f 7220 636f 6e76  6238>`_ for conv
-00000490: 656e 6965 6e63 652c 2061 7320 7468 6573  enience, as thes
-000004a0: 6520 6172 6520 7374 616e 6461 7264 0a4f  e are standard.O
-000004b0: 5450 2061 6c67 6f72 6974 686d 7320 7573  TP algorithms us
-000004c0: 6564 2062 7920 6d75 6c74 6970 6c65 2070  ed by multiple p
-000004d0: 6c75 6769 6e73 2e0a 0a49 6620 796f 7527  lugins...If you'
-000004e0: 7265 206c 6f6f 6b69 6e67 2066 6f72 2061  re looking for a
-000004f0: 2068 6967 6865 722d 6c65 7665 6c20 6f72   higher-level or
-00000500: 206d 6f72 6520 6f70 696e 696f 6e61 7465   more opinionate
-00000510: 6420 736f 6c75 7469 6f6e 2c20 796f 7520  d solution, you 
-00000520: 6d69 6768 7420 6265 0a69 6e74 6572 6573  might be.interes
-00000530: 7465 6420 696e 2060 646a 616e 676f 2d74  ted in `django-t
-00000540: 776f 2d66 6163 746f 722d 6175 7468 0a3c  wo-factor-auth.<
-00000550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000560: 6f6d 2f42 6f75 6b65 2f64 6a61 6e67 6f2d  om/Bouke/django-
-00000570: 7477 6f2d 6661 6374 6f72 2d61 7574 683e  two-factor-auth>
-00000580: 605f 2e0a 0a53 7461 7475 730a 2d2d 2d2d  `_...Status.----
-00000590: 2d2d 0a0a 5468 6973 2070 726f 6a65 6374  --..This project
-000005a0: 2069 7320 7374 6162 6c65 2061 6e64 206d   is stable and m
-000005b0: 6169 6e74 6169 6e65 642c 2062 7574 2069  aintained, but i
-000005c0: 7320 6e6f 206c 6f6e 6765 7220 6163 7469  s no longer acti
-000005d0: 7665 6c79 2075 7365 6420 6279 2074 6865  vely used by the
-000005e0: 0a61 7574 686f 7220 616e 6420 6973 206e  .author and is n
-000005f0: 6f74 2073 6565 696e 6720 6d75 6368 206f  ot seeing much o
-00000600: 6e67 6f69 6e67 2069 6e76 6573 746d 656e  ngoing investmen
-00000610: 742e 2041 6e79 6f6e 6520 696e 7465 7265  t. Anyone intere
-00000620: 7374 6564 2069 6e20 7461 6b69 6e67 0a6f  sted in taking.o
-00000630: 7665 7220 6173 7065 6374 7320 6f66 2074  ver aspects of t
-00000640: 6865 2070 726f 6a65 6374 2073 686f 756c  he project shoul
-00000650: 6420 6063 6f6e 7461 6374 206d 6520 3c68  d `contact me <h
-00000660: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000670: 6d2f 7073 6167 6572 733e 605f 2e0a 0a57  m/psagers>`_...W
-00000680: 656c 6c2d 666f 726d 6564 2069 7373 7565  ell-formed issue
-00000690: 7320 616e 6420 7075 6c6c 2072 6571 7565  s and pull reque
-000006a0: 7374 7320 6172 6520 7765 6c63 6f6d 652c  sts are welcome,
-000006b0: 2062 7574 2070 6c65 6173 6520 7365 6520   but please see 
-000006c0: 7468 650a 436f 6e74 7269 6275 7469 6e67  the.Contributing
-000006d0: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
-000006e0: 5245 4144 4d45 2066 6972 7374 2e0a 0a2e  README first....
-000006f0: 2e20 656e 642d 6f66 2d64 6f63 2d69 6e74  . end-of-doc-int
-00000700: 726f 0a0a 0a54 6865 2046 7574 7572 650a  ro...The Future.
-00000710: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4f6e 6365  ----------..Once
-00000720: 2075 706f 6e20 6120 7469 6d65 2c20 6576   upon a time, ev
-00000730: 6572 7974 6869 6e67 2077 6173 2075 7365  erything was use
-00000740: 726e 616d 6573 2061 6e64 2070 6173 7377  rnames and passw
-00000750: 6f72 6473 2e20 4f72 2065 7665 6e20 696e  ords. Or even in
-00000760: 2074 6865 2063 6173 6520 6f66 0a6f 7468   the case of.oth
-00000770: 6572 2061 7574 6865 6e74 6963 6174 696f  er authenticatio
-00000780: 6e20 6d65 6368 616e 6973 6d73 2c20 6120  n mechanisms, a 
-00000790: 7573 6572 2077 6173 2065 6974 6865 7220  user was either 
-000007a0: 6175 7468 656e 7469 6361 7465 6420 6f72  authenticated or
-000007b0: 206e 6f74 0a28 616e 6f6e 796d 6f75 7320   not.(anonymous 
-000007c0: 696e 2044 6a61 6e67 6f27 7320 7465 726d  in Django's term
-000007d0: 696e 6f6c 6f67 7929 2e20 5468 656e 2074  inology). Then t
-000007e0: 6865 7265 2077 6173 2074 776f 2d66 6163  here was two-fac
-000007f0: 746f 7220 6175 7468 656e 7469 6361 7469  tor authenticati
-00000800: 6f6e 2c0a 7768 6963 6820 636f 756c 6420  on,.which could 
-00000810: 7369 6d70 6c79 2062 6520 616e 2069 6d70  simply be an imp
-00000820: 6c65 6d65 6e74 6174 696f 6e20 6465 7461  lementation deta
-00000830: 696c 2069 6e20 6120 6269 6e61 7279 2061  il in a binary a
-00000840: 7574 6865 6e74 6963 6174 696f 6e20 7374  uthentication st
-00000850: 6174 652c 0a62 7574 2063 6f75 6c64 2061  ate,.but could a
-00000860: 6c73 6f20 696d 706c 7920 6c65 7665 6c73  lso imply levels
-00000870: 206f 7220 6465 6772 6565 7320 6f66 2061   or degrees of a
-00000880: 7574 6865 6e74 6963 6174 696f 6e2e 0a0a  uthentication...
-00000890: 5468 6573 6520 6461 7973 2c20 6974 2773  These days, it's
-000008a0: 2069 6e63 7265 6173 696e 676c 7920 636f   increasingly co
-000008b0: 6d6d 6f6e 2074 6f20 7365 6520 7369 7465  mmon to see site
-000008c0: 7320 7769 7468 206d 6f72 6520 6e75 616e  s with more nuan
-000008d0: 6365 640a 6175 7468 656e 7469 6361 7469  ced.authenticati
-000008e0: 6f6e 2073 7461 7465 2e20 4120 7369 7465  on state. A site
-000008f0: 206d 6967 6874 2072 656d 656d 6265 7220   might remember 
-00000900: 7768 6f20 796f 7520 6172 6520 666f 7265  who you are fore
-00000910: 7665 72e2 8094 736f 2079 6f75 2772 6520  ver...so you're 
-00000920: 6e6f 740a 616e 6f6e 796d 6f75 73e2 8094  not.anonymous...
-00000930: 6275 7420 6966 2079 6f75 2074 7279 2074  but if you try t
-00000940: 6f20 646f 2061 6e79 7468 696e 6720 7072  o do anything pr
-00000950: 6976 6174 652c 2079 6f75 2068 6176 6520  ivate, you have 
-00000960: 746f 2072 652d 6175 7468 656e 7469 6361  to re-authentica
-00000970: 7465 2e0a 596f 7520 6d61 7920 6265 2061  te..You may be a
-00000980: 626c 6520 746f 2063 686f 6f73 6520 6672  ble to choose fr
-00000990: 6f6d 2061 6d6f 6e67 2061 6c6c 206f 6620  om among all of 
-000009a0: 7468 6520 6175 7468 656e 7469 6361 7469  the authenticati
-000009b0: 6f6e 206d 6563 6861 6e69 736d 7320 796f  on mechanisms yo
-000009c0: 750a 6861 7665 2063 6f6e 6669 6775 7265  u.have configure
-000009d0: 642c 206f 7220 6f6e 6c79 2066 726f 6d20  d, or only from 
-000009e0: 736f 6d65 206f 6620 7468 656d 2e20 5370  some of them. Sp
-000009f0: 6563 6966 6963 206d 6563 6861 6e69 736d  ecific mechanism
-00000a00: 7320 6d61 7920 6265 2072 6571 7569 7265  s may be require
-00000a10: 640a 666f 7220 7370 6563 6966 6963 2061  d.for specific a
-00000a20: 6374 696f 6e73 2c20 7375 6368 2061 7320  ctions, such as 
-00000a30: 7573 696e 6720 796f 7572 2055 3246 2064  using your U2F d
-00000a40: 6576 6963 6520 746f 2061 6363 6573 7320  evice to access 
-00000a50: 796f 7572 2055 3246 2073 6574 7469 6e67  your U2F setting
-00000a60: 732e 0a0a 496e 2073 686f 7274 2c20 7468  s...In short, th
-00000a70: 6520 776f 726c 6420 7365 656d 7320 746f  e world seems to
-00000a80: 2062 6520 6d6f 7669 6e67 2062 6579 6f6e   be moving beyon
-00000a90: 6420 7468 6520 6173 7375 6d70 7469 6f6e  d the assumption
-00000aa0: 7320 7468 6174 206f 7269 6769 6e61 6c6c  s that originall
-00000ab0: 790a 696e 666f 726d 6564 2044 6a61 6e67  y.informed Djang
-00000ac0: 6f27 7320 6573 7365 6e74 6961 6c20 6175  o's essential au
-00000ad0: 7468 656e 7469 6361 7469 6f6e 2064 6573  thentication des
-00000ae0: 6967 6e2e 2049 6620 4920 7765 7265 2073  ign. If I were s
-00000af0: 7469 6c6c 2069 6e76 6573 7469 6e67 2069  till investing i
-00000b00: 6e0a 446a 616e 676f 2067 656e 6572 616c  n.Django general
-00000b10: 6c79 2c20 4920 776f 756c 6420 7072 6f62  ly, I would prob
-00000b20: 6162 6c79 2073 7461 7274 2061 206e 6577  ably start a new
-00000b30: 206d 756c 7469 2d66 6163 746f 7220 6175   multi-factor au
-00000b40: 7468 656e 7469 6361 7469 6f6e 0a70 726f  thentication.pro
-00000b50: 6a65 6374 2074 6861 7420 776f 756c 6420  ject that would 
-00000b60: 7265 666c 6563 7420 7468 6573 6520 6368  reflect these ch
-00000b70: 616e 6765 732e 2049 7420 776f 756c 6420  anges. It would 
-00000b80: 696e 636f 7270 6f72 6174 6520 7468 6520  incorporate the 
-00000b90: 6964 6561 2074 6861 7420 610a 7573 6572  idea that a.user
-00000ba0: 206d 6179 2062 6520 6175 7468 656e 7469   may be authenti
-00000bb0: 6361 7465 6420 6279 2076 6172 696f 7573  cated by various
-00000bc0: 2063 6f6d 6269 6e61 7469 6f6e 7320 6f66   combinations of
-00000bd0: 206d 6563 6861 6e69 736d 7320 6174 2061   mechanisms at a
-00000be0: 6e79 2074 696d 6520 616e 640a 7468 6174  ny time and.that
-00000bf0: 2064 6966 6665 7265 6e74 2063 6f6d 6269   different combi
-00000c00: 6e61 7469 6f6e 7320 6d61 7920 6265 2072  nations may be r
-00000c10: 6571 7569 7265 6420 746f 2073 6174 6973  equired to satis
-00000c20: 6679 2064 6976 6572 7365 2061 7574 686f  fy diverse autho
-00000c30: 7269 7a61 7469 6f6e 0a72 6571 7569 7265  rization.require
-00000c40: 6d65 6e74 7320 6163 726f 7373 2074 6865  ments across the
-00000c50: 2073 6974 652e 2049 7420 776f 756c 6420   site. It would 
-00000c60: 6d6f 7374 206c 696b 656c 7920 7472 7920  most likely try 
-00000c70: 746f 2064 6973 656e 7461 6e67 6c65 0a61  to disentangle.a
-00000c80: 7574 6865 6e74 6963 6174 696f 6e20 7065  uthentication pe
-00000c90: 7273 6973 7465 6e63 6520 6672 6f6d 2073  rsistence from s
-00000ca0: 6573 7369 6f6e 732c 2061 7420 6c65 6173  essions, at leas
-00000cb0: 7420 746f 2073 6f6d 6520 6578 7465 6e74  t to some extent
-00000cc0: 2e20 4d61 6e79 2073 6974 6573 0a77 6f75  . Many sites.wou
-00000cd0: 6c64 206e 6f74 2072 6571 7569 7265 2061  ld not require a
-00000ce0: 6c6c 206f 6620 7468 6973 2066 6c65 7869  ll of this flexi
-00000cf0: 6269 6c69 7479 2c20 6275 7420 6974 2077  bility, but it w
-00000d00: 6f75 6c64 206f 7065 6e20 7570 2070 6f73  ould open up pos
-00000d10: 7369 6269 6c69 7469 6573 0a66 6f72 2062  sibilities.for b
-00000d20: 6574 7465 7220 6578 7065 7269 656e 6365  etter experience
-00000d30: 7320 6279 206e 6f74 2061 736b 696e 6720  s by not asking 
-00000d40: 7573 6572 7320 666f 7220 6d6f 7265 2074  users for more t
-00000d50: 6861 6e20 7765 2072 6571 7569 7265 2061  han we require a
-00000d60: 7420 616e 790a 706f 696e 742e 0a0a 4966  t any.point...If
-00000d70: 2061 6e79 6f6e 6520 6861 7320 6120 6d69   anyone has a mi
-00000d80: 6e64 2074 6f20 7461 6b65 206f 6e20 6120  nd to take on a 
-00000d90: 7072 6f6a 6563 7420 6c69 6b65 2074 6869  project like thi
-00000da0: 732c 2049 2764 2062 6520 6861 7070 7920  s, I'd be happy 
-00000db0: 746f 206f 6666 6572 0a77 6861 7465 7665  to offer.whateve
-00000dc0: 7220 6164 7669 6365 206f 7220 6c65 7373  r advice or less
-00000dd0: 6f6e 7320 6c65 6172 6e65 6420 7468 6174  ons learned that
-00000de0: 2049 2063 616e 2e0a 0a0a 4465 7665 6c6f   I can....Develo
-00000df0: 706d 656e 740a 2d2d 2d2d 2d2d 2d2d 2d2d  pment.----------
-00000e00: 2d0a 0a44 6576 656c 6f70 6d65 6e74 2064  -..Development d
-00000e10: 6570 656e 6465 6e63 6965 7320 6172 6520  ependencies are 
-00000e20: 6465 6669 6e65 6420 696e 2074 6865 2050  defined in the P
-00000e30: 6970 6669 6c65 3b20 7573 6520 6070 6970  ipfile; use `pip
-00000e40: 656e 7660 5f20 746f 2073 6574 2075 7020  env`_ to set up 
-00000e50: 610a 7375 6974 6162 6c65 2073 6865 6c6c  a.suitable shell
-00000e60: 2e0a 0a54 6865 2074 6573 7473 2069 6e20  ...The tests in 
-00000e70: 746f 782e 696e 6920 636f 7665 7220 6120  tox.ini cover a 
-00000e80: 7265 7072 6573 656e 7461 7469 7665 2073  representative s
-00000e90: 616d 706c 6520 6f66 2073 7570 706f 7274  ample of support
-00000ea0: 6564 2050 7974 686f 6e20 616e 640a 446a  ed Python and.Dj
-00000eb0: 616e 676f 2076 6572 7369 6f6e 732c 2061  ango versions, a
-00000ec0: 7320 7765 6c6c 2061 7320 7275 6e6e 696e  s well as runnin
-00000ed0: 6720 6066 6c61 6b65 3860 5f20 616e 6420  g `flake8`_ and 
-00000ee0: 6069 736f 7274 605f 2066 6f72 206c 696e  `isort`_ for lin
-00000ef0: 7469 6e67 2061 6e64 2073 7479 6c65 0a63  ting and style.c
-00000f00: 6f6e 7369 7374 656e 6379 2e20 506c 6561  onsistency. Plea
-00000f10: 7365 2072 756e 2060 746f 7860 2062 6566  se run `tox` bef
-00000f20: 6f72 6520 6368 6563 6b69 6e67 2069 6e20  ore checking in 
-00000f30: 616e 6420 7365 6e64 696e 6720 6120 7075  and sending a pu
-00000f40: 6c6c 2072 6571 7565 7374 2e0a 0a0a 436f  ll request....Co
-00000f50: 6e74 7269 6275 7469 6e67 0a2d 2d2d 2d2d  ntributing.-----
-00000f60: 2d2d 2d2d 2d2d 2d0a 0a41 7320 6d65 6e74  -------..As ment
-00000f70: 696f 6e65 6420 6162 6f76 652c 2074 6869  ioned above, thi
-00000f80: 7320 7072 6f6a 6563 7420 6973 2073 7461  s project is sta
-00000f90: 626c 6520 616e 6420 6d61 7475 7265 2e20  ble and mature. 
-00000fa0: 4973 7375 6573 2061 6e64 2070 756c 6c20  Issues and pull 
-00000fb0: 7265 7175 6573 7473 0a61 7265 2077 656c  requests.are wel
-00000fc0: 636f 6d65 2066 6f72 2069 6d70 6f72 7461  come for importa
-00000fd0: 6e74 2062 7567 7320 616e 6420 696d 7072  nt bugs and impr
-00000fe0: 6f76 656d 656e 7473 2e20 466f 7220 6e6f  ovements. For no
-00000ff0: 6e2d 7472 6976 6961 6c20 6368 616e 6765  n-trivial change
-00001000: 732c 2069 7427 730a 6f66 7465 6e20 6120  s, it's.often a 
-00001010: 676f 6f64 2069 6465 6120 746f 2073 7461  good idea to sta
-00001020: 7274 2062 7920 6f70 656e 696e 6720 616e  rt by opening an
-00001030: 2069 7373 7565 2074 6f20 7472 6163 6b20   issue to track 
-00001040: 7468 6520 6e65 6564 2066 6f72 2061 2063  the need for a c
-00001050: 6861 6e67 650a 616e 6420 7468 656e 206f  hange.and then o
-00001060: 7074 696f 6e61 6c6c 7920 6f70 656e 2061  ptionally open a
-00001070: 2070 756c 6c20 7265 7175 6573 7420 7769   pull request wi
-00001080: 7468 2061 2070 726f 706f 7365 6420 7265  th a proposed re
-00001090: 736f 6c75 7469 6f6e 2e20 4973 7375 6573  solution. Issues
-000010a0: 2061 6e64 0a70 756c 6c20 7265 7175 6573   and.pull reques
-000010b0: 7473 2073 686f 756c 6420 616c 736f 2062  ts should also b
-000010c0: 6520 666f 6375 7365 6420 6f6e 2061 2073  e focused on a s
-000010d0: 696e 676c 6520 7468 696e 672e 2050 756c  ingle thing. Pul
-000010e0: 6c20 7265 7175 6573 7473 2074 6861 740a  l requests that.
-000010f0: 6275 6e64 6c65 2074 6f67 6574 6865 7220  bundle together 
-00001100: 6120 6275 6e63 6820 6f66 206c 6f6f 7365  a bunch of loose
-00001110: 6c79 2072 656c 6174 6564 2063 6f6d 6d69  ly related commi
-00001120: 7473 2061 7265 2075 6e6c 696b 656c 7920  ts are unlikely 
-00001130: 746f 2067 6f20 616e 7977 6865 7265 2e0a  to go anywhere..
-00001140: 0a41 6e6f 7468 6572 2067 6f6f 6420 7275  .Another good ru
-00001150: 6c65 206f 6620 7468 756d 62e2 8094 666f  le of thumb...fo
-00001160: 7220 616e 7920 7072 6f6a 6563 742c 2062  r any project, b
-00001170: 7574 2065 7370 6563 6961 6c6c 7920 6120  ut especially a 
-00001180: 6d61 7475 7265 206f 6e65 e280 9469 7320  mature one...is 
-00001190: 746f 0a6b 6565 7020 6368 616e 6765 7320  to.keep changes 
-000011a0: 6173 2073 696d 706c 6520 6173 2070 6f73  as simple as pos
-000011b0: 7369 626c 652e 2049 6e20 7061 7274 6963  sible. In partic
-000011c0: 756c 6172 2c20 7468 6572 6520 7368 6f75  ular, there shou
-000011d0: 6c64 2062 6520 6120 6869 6768 2062 6172  ld be a high bar
-000011e0: 0a66 6f72 2061 6464 696e 6720 6e65 7720  .for adding new 
-000011f0: 6465 7065 6e64 656e 6369 6573 2e20 416c  dependencies. Al
-00001200: 7468 6f75 6768 2069 7420 6361 6e27 7420  though it can't 
-00001210: 6265 2072 756c 6564 206f 7574 2c20 6974  be ruled out, it
-00001220: 2073 6565 6d73 2068 6967 686c 790a 756e   seems highly.un
-00001230: 6c69 6b65 6c79 2074 6861 7420 6120 6e65  likely that a ne
-00001240: 7720 7275 6e74 696d 6520 6465 7065 6e64  w runtime depend
-00001250: 656e 6379 2077 696c 6c20 6576 6572 2062  ency will ever b
-00001260: 6520 6164 6465 642e 204e 6577 2074 6573  e added. New tes
-00001270: 7469 6e67 0a64 6570 656e 6465 6e63 6965  ting.dependencie
-00001280: 7320 6172 6520 6d6f 7265 206c 696b 656c  s are more likel
-00001290: 792c 2062 7574 206f 6e6c 7920 6966 2074  y, but only if t
-000012a0: 6865 7265 2773 206e 6f20 6f74 6865 7220  here's no other 
-000012b0: 7761 7920 746f 2061 6464 7265 7373 2061  way to address a
-000012c0: 6e0a 696d 706f 7274 616e 7420 6e65 6564  n.important need
-000012d0: 2e0a 0a49 6620 7468 6572 6527 7320 6120  ...If there's a 
-000012e0: 6465 7665 6c6f 706d 656e 7420 746f 6f6c  development tool
-000012f0: 2074 6861 7420 796f 7527 6420 6c69 6b65   that you'd like
-00001300: 2074 6f20 7573 6520 7769 7468 2074 6869   to use with thi
-00001310: 7320 7072 6f6a 6563 742c 2074 6865 0a66  s project, the.f
-00001320: 6972 7374 2073 7465 7020 6973 2074 6f20  irst step is to 
-00001330: 7472 7920 746f 2075 7064 6174 6520 636f  try to update co
-00001340: 6e66 6967 2066 696c 6573 2028 7365 7475  nfig files (setu
-00001350: 702e 6366 6720 6f72 2073 696d 696c 6172  p.cfg or similar
-00001360: 2920 746f 2069 6e74 6567 7261 7465 0a74  ) to integrate.t
-00001370: 6865 2074 6f6f 6c20 7769 7468 2074 6865  he tool with the
-00001380: 2065 7869 7374 696e 6720 636f 6465 2e20   existing code. 
-00001390: 4120 6269 7420 6f66 2063 6f6e 6669 6775  A bit of configu
-000013a0: 7261 7469 6f6e 2067 6c75 6520 666f 7220  ration glue for 
-000013b0: 706f 7075 6c61 7220 746f 6f6c 730a 7368  popular tools.sh
-000013c0: 6f75 6c64 2061 6c77 6179 7320 6265 2073  ould always be s
-000013d0: 6166 652e 2049 6620 7468 6174 2773 206e  afe. If that's n
-000013e0: 6f74 2070 6f73 7369 626c 652c 2077 6520  ot possible, we 
-000013f0: 6361 6e20 636f 6e73 6964 6572 206d 6f64  can consider mod
-00001400: 6966 7969 6e67 2074 6865 0a63 6f64 6520  ifying the.code 
-00001410: 746f 2062 6520 636f 6d70 6174 6962 6c65  to be compatible
-00001420: 2077 6974 6820 6120 6272 6f61 6465 7220   with a broader 
-00001430: 7261 6e67 6520 6f66 2074 6f6f 6c73 2028  range of tools (
-00001440: 7769 7468 6f75 7420 6272 6561 6b69 6e67  without breaking
-00001450: 2061 6e79 0a65 7869 7374 696e 6720 636f   any.existing co
-00001460: 6d70 6174 6962 696c 6974 6965 7329 2e20  mpatibilities). 
-00001470: 4f6e 6c79 2061 7320 6120 6c61 7374 2072  Only as a last r
-00001480: 6573 6f72 7420 776f 756c 6420 6120 6e65  esort would a ne
-00001490: 7720 7465 7374 696e 6720 6f72 0a64 6576  w testing or.dev
-000014a0: 656c 6f70 6d65 6e74 2074 6f6f 6c20 6265  elopment tool be
-000014b0: 2069 6e63 6f72 706f 7261 7465 6420 696e   incorporated in
-000014c0: 746f 2074 6865 2070 726f 6a65 6374 2061  to the project a
-000014d0: 7320 6120 6465 7065 6e64 656e 6379 2e0a  s a dependency..
-000014e0: 0a49 7427 7320 616c 736f 2067 6f6f 6420  .It's also good 
-000014f0: 746f 2072 656d 656d 6265 7220 7468 6174  to remember that
-00001500: 2077 7269 7469 6e67 2074 6865 2063 6f64   writing the cod
-00001510: 6520 6973 2074 7970 6963 616c 6c79 2074  e is typically t
-00001520: 6865 206c 6561 7374 2070 6172 7420 6f66  he least part of
-00001530: 0a74 6865 2077 6f72 6b2e 2054 6869 7320  .the work. This 
-00001540: 6973 2074 7275 6520 666f 7220 736f 6674  is true for soft
-00001550: 7761 7265 2064 6576 656c 6f70 6d65 6e74  ware development
-00001560: 2069 6e20 6765 6e65 7261 6c2c 2062 7574   in general, but
-00001570: 2065 7370 6563 6961 6c6c 7920 610a 736d   especially a.sm
-00001580: 616c 6c20 7374 6162 6c65 2070 726f 6a65  all stable proje
-00001590: 6374 206c 696b 6520 7468 6973 2e20 5468  ct like this. Th
-000015a0: 6520 6275 6c6b 206f 6620 7468 6520 776f  e bulk of the wo
-000015b0: 726b 2069 7320 696e 2060 756e 6465 7273  rk is in `unders
-000015c0: 7461 6e64 696e 6720 7468 650a 7072 6f62  tanding the.prob
-000015d0: 6c65 6d20 3c68 7474 703a 2f2f 7777 772e  lem <http://www.
-000015e0: 796f 7574 7562 652e 636f 6d2f 7761 7463  youtube.com/watc
-000015f0: 683f 763d 6638 346e 356f 466f 5a42 633e  h?v=f84n5oFoZBc>
-00001600: 605f 2c20 6465 7465 726d 696e 696e 6720  `_, determining 
-00001610: 7468 6520 6465 7369 7265 640a 6174 7472  the desired.attr
-00001620: 6962 7574 6573 206f 6620 6120 736f 6c75  ibutes of a solu
-00001630: 7469 6f6e 2c20 7265 7365 6172 6368 696e  tion, researchin
-00001640: 6720 616e 6420 6576 616c 7561 7469 6e67  g and evaluating
-00001650: 2061 6c74 6572 6e61 7469 7665 732c 2077   alternatives, w
-00001660: 7269 7469 6e67 0a64 6f63 756d 656e 7461  riting.documenta
-00001670: 7469 6f6e 2c20 6465 7369 676e 696e 6720  tion, designing 
-00001680: 6120 7465 7374 696e 6720 7374 7261 7465  a testing strate
-00001690: 6779 2c20 6574 632e 2057 7269 7469 6e67  gy, etc. Writing
-000016a0: 2074 6865 2063 6f64 6520 6974 7365 6c66   the code itself
-000016b0: 2074 656e 6473 0a74 6f20 6265 2061 206d   tends.to be a m
-000016c0: 696e 6f72 206d 6174 7465 7220 7468 6174  inor matter that
-000016d0: 2065 6d65 7267 6573 2066 726f 6d20 7468   emerges from th
-000016e0: 6174 2070 726f 6365 7373 2e0a 0a0a 2e2e  at process......
-000016f0: 205f 7069 7065 6e76 3a20 6874 7470 733a   _pipenv: https:
-00001700: 2f2f 7069 7065 6e76 2e72 6561 6474 6865  //pipenv.readthe
-00001710: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00001720: 742f 0a2e 2e20 5f66 6c61 6b65 383a 2068  t/... _flake8: h
-00001730: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00001740: 7072 6f6a 6563 742f 666c 616b 6538 2f0a  project/flake8/.
-00001750: 2e2e 205f 6973 6f72 743a 2068 7474 7073  .. _isort: https
-00001760: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00001770: 6563 742f 6973 6f72 742f 0a              ect/isort/.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
+00000020: 676f 2d6f 7470 0a56 6572 7369 6f6e 3a20  go-otp.Version: 
+00000030: 312e 322e 300a 5375 6d6d 6172 793a 2041  1.2.0.Summary: A
+00000040: 2070 6c75 6767 6162 6c65 2066 7261 6d65   pluggable frame
+00000050: 776f 726b 2066 6f72 2061 6464 696e 6720  work for adding 
+00000060: 7477 6f2d 6661 6374 6f72 2061 7574 6865  two-factor authe
+00000070: 6e74 6963 6174 696f 6e20 746f 2044 6a61  ntication to Dja
+00000080: 6e67 6f20 7573 696e 6720 6f6e 652d 7469  ngo using one-ti
+00000090: 6d65 2070 6173 7377 6f72 6473 2e0a 5072  me passwords..Pr
+000000a0: 6f6a 6563 742d 5552 4c3a 2048 6f6d 6570  oject-URL: Homep
+000000b0: 6167 652c 2068 7474 7073 3a2f 2f67 6974  age, https://git
+000000c0: 6875 622e 636f 6d2f 646a 616e 676f 2d6f  hub.com/django-o
+000000d0: 7470 2f64 6a61 6e67 6f2d 6f74 700a 5072  tp/django-otp.Pr
+000000e0: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
+000000f0: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
+00000100: 2f2f 646a 616e 676f 2d6f 7470 2d6f 6666  //django-otp-off
+00000110: 6963 6961 6c2e 7265 6164 7468 6564 6f63  icial.readthedoc
+00000120: 732e 696f 2f0a 4175 7468 6f72 2d65 6d61  s.io/.Author-ema
+00000130: 696c 3a20 5065 7465 7220 5361 6765 7273  il: Peter Sagers
+00000140: 6f6e 203c 7073 6167 6572 7340 6967 6e6f  on <psagers@igno
+00000150: 7261 7265 2e6e 6574 3e0a 4c69 6365 6e73  rare.net>.Licens
+00000160: 652d 4578 7072 6573 7369 6f6e 3a20 556e  e-Expression: Un
+00000170: 6c69 6365 6e73 650a 4c69 6365 6e73 652d  license.License-
+00000180: 4669 6c65 3a20 4c49 4345 4e53 450a 436c  File: LICENSE.Cl
+00000190: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
+000001a0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000001b0: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
+000001c0: 7461 626c 650a 436c 6173 7369 6669 6572  table.Classifier
+000001d0: 3a20 4672 616d 6577 6f72 6b20 3a3a 2044  : Framework :: D
+000001e0: 6a61 6e67 6f0a 436c 6173 7369 6669 6572  jango.Classifier
+000001f0: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000200: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000210: 730a 436c 6173 7369 6669 6572 3a20 4c69  s.Classifier: Li
+00000220: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000230: 726f 7665 6420 3a3a 2054 6865 2055 6e6c  roved :: The Unl
+00000240: 6963 656e 7365 2028 556e 6c69 6365 6e73  icense (Unlicens
+00000250: 6529 0a43 6c61 7373 6966 6965 723a 2050  e).Classifier: P
+00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000270: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000280: 2033 0a43 6c61 7373 6966 6965 723a 2050   3.Classifier: P
+00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002b0: 2033 203a 3a20 4f6e 6c79 0a43 6c61 7373   3 :: Only.Class
+000002c0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+000002d0: 5365 6375 7269 7479 0a43 6c61 7373 6966  Security.Classif
+000002e0: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
+000002f0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+00000300: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
+00000310: 3a3a 2050 7974 686f 6e20 4d6f 6475 6c65  :: Python Module
+00000320: 730a 5265 7175 6972 6573 2d50 7974 686f  s.Requires-Pytho
+00000330: 6e3a 203e 3d33 2e37 0a52 6571 7569 7265  n: >=3.7.Require
+00000340: 732d 4469 7374 3a20 646a 616e 676f 3e3d  s-Dist: django>=
+00000350: 332e 320a 5072 6f76 6964 6573 2d45 7874  3.2.Provides-Ext
+00000360: 7261 3a20 7172 636f 6465 0a52 6571 7569  ra: qrcode.Requi
+00000370: 7265 732d 4469 7374 3a20 7172 636f 6465  res-Dist: qrcode
+00000380: 3b20 6578 7472 6120 3d3d 2027 7172 636f  ; extra == 'qrco
+00000390: 6465 270a 4465 7363 7269 7074 696f 6e2d  de'.Description-
+000003a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+000003b0: 7874 2f78 2d72 7374 0a0a 2e2e 2076 696d  xt/x-rst.... vim
+000003c0: 3a20 7477 3d38 3020 6c62 720a 0a64 6a61  : tw=80 lbr..dja
+000003d0: 6e67 6f2d 6f74 700a 3d3d 3d3d 3d3d 3d3d  ngo-otp.========
+000003e0: 3d3d 0a0a 2e2e 2069 6d61 6765 3a3a 2068  ==.... image:: h
+000003f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000400: 6473 2e69 6f2f 7079 7069 2f76 2f64 6a61  ds.io/pypi/v/dja
+00000410: 6e67 6f2d 6f74 703f 636f 6c6f 723d 626c  ngo-otp?color=bl
+00000420: 7565 0a20 2020 3a74 6172 6765 743a 2068  ue.   :target: h
+00000430: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000440: 7072 6f6a 6563 742f 646a 616e 676f 2d6f  project/django-o
+00000450: 7470 2f0a 2020 203a 616c 743a 2050 7950  tp/.   :alt: PyP
+00000460: 490a 2e2e 2069 6d61 6765 3a3a 2068 7474  I... image:: htt
+00000470: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000480: 2e69 6f2f 7265 6164 7468 6564 6f63 732f  .io/readthedocs/
+00000490: 646a 616e 676f 2d6f 7470 2d6f 6666 6963  django-otp-offic
+000004a0: 6961 6c0a 2020 203a 7461 7267 6574 3a20  ial.   :target: 
+000004b0: 6874 7470 733a 2f2f 646a 616e 676f 2d6f  https://django-o
+000004c0: 7470 2d6f 6666 6963 6961 6c2e 7265 6164  tp-official.read
+000004d0: 7468 6564 6f63 732e 696f 2f0a 2020 203a  thedocs.io/.   :
+000004e0: 616c 743a 2044 6f63 756d 656e 7461 7469  alt: Documentati
+000004f0: 6f6e 0a2e 2e20 696d 6167 653a 3a20 6874  on... image:: ht
+00000500: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000510: 732e 696f 2f62 6164 6765 2f67 6974 6875  s.io/badge/githu
+00000520: 622d 646a 616e 676f 2d2d 6f74 702d 6772  b-django--otp-gr
+00000530: 6565 6e0a 2020 203a 7461 7267 6574 3a20  een.   :target: 
+00000540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000550: 6f6d 2f64 6a61 6e67 6f2d 6f74 702f 646a  om/django-otp/dj
+00000560: 616e 676f 2d6f 7470 0a20 2020 3a61 6c74  ango-otp.   :alt
+00000570: 3a20 536f 7572 6365 0a0a 5468 6973 2070  : Source..This p
+00000580: 726f 6a65 6374 206d 616b 6573 2069 7420  roject makes it 
+00000590: 6561 7379 2074 6f20 6164 6420 7375 7070  easy to add supp
+000005a0: 6f72 7420 666f 7220 606f 6e65 2d74 696d  ort for `one-tim
+000005b0: 6520 7061 7373 776f 7264 730a 3c68 7474  e passwords.<htt
+000005c0: 703a 2f2f 656e 2e77 696b 6970 6564 6961  p://en.wikipedia
+000005d0: 2e6f 7267 2f77 696b 692f 4f6e 652d 7469  .org/wiki/One-ti
+000005e0: 6d65 5f70 6173 7377 6f72 643e 605f 2028  me_password>`_ (
+000005f0: 4f54 5073 2920 746f 2044 6a61 6e67 6f2e  OTPs) to Django.
+00000600: 2049 7420 6361 6e20 6265 0a69 6e74 6567   It can be.integ
+00000610: 7261 7465 6420 6174 2076 6172 696f 7573  rated at various
+00000620: 206c 6576 656c 732c 2064 6570 656e 6469   levels, dependi
+00000630: 6e67 206f 6e20 686f 7720 6d75 6368 2063  ng on how much c
+00000640: 7573 746f 6d69 7a61 7469 6f6e 2069 7320  ustomization is 
+00000650: 7265 7175 6972 6564 2e0a 4974 2069 6e74  required..It int
+00000660: 6567 7261 7465 7320 7769 7468 2060 6064  egrates with ``d
+00000670: 6a61 6e67 6f2e 636f 6e74 7269 622e 6175  jango.contrib.au
+00000680: 7468 6060 2c20 616c 7468 6f75 6768 2069  th``, although i
+00000690: 7420 6973 206e 6f74 2061 2044 6a61 6e67  t is not a Djang
+000006a0: 6f0a 6175 7468 656e 7469 6361 7469 6f6e  o.authentication
+000006b0: 2062 6163 6b65 6e64 2e20 5468 6520 7072   backend. The pr
+000006c0: 696d 6172 7920 7461 7267 6574 2069 7320  imary target is 
+000006d0: 6465 7665 6c6f 7065 7273 2077 6973 6869  developers wishi
+000006e0: 6e67 2074 6f20 696e 636f 7270 6f72 6174  ng to incorporat
+000006f0: 650a 4f54 5073 2069 6e74 6f20 7468 6569  e.OTPs into thei
+00000700: 7220 446a 616e 676f 2070 726f 6a65 6374  r Django project
+00000710: 7320 6173 2061 2066 6f72 6d20 6f66 2060  s as a form of `
+00000720: 7477 6f2d 6661 6374 6f72 2061 7574 6865  two-factor authe
+00000730: 6e74 6963 6174 696f 6e0a 3c68 7474 703a  ntication.<http:
+00000740: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00000750: 7267 2f77 696b 692f 5477 6f2d 6661 6374  rg/wiki/Two-fact
+00000760: 6f72 5f61 7574 6865 6e74 6963 6174 696f  or_authenticatio
+00000770: 6e3e 605f 2e0a 0a53 6576 6572 616c 2073  n>`_...Several s
+00000780: 696d 706c 6520 4f54 5020 706c 7567 696e  imple OTP plugin
+00000790: 7320 6172 6520 696e 636c 7564 6564 2061  s are included a
+000007a0: 6e64 206d 6f72 6520 6172 6520 6176 6169  nd more are avai
+000007b0: 6c61 626c 6520 7365 7061 7261 7465 6c79  lable separately
+000007c0: 2e20 5468 6973 0a70 6163 6b61 6765 2061  . This.package a
+000007d0: 6c73 6f20 696e 636c 7564 6573 2061 6e20  lso includes an 
+000007e0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+000007f0: 6620 4f41 5448 2060 484f 5450 0a3c 6874  f OATH `HOTP.<ht
+00000800: 7470 3a2f 2f74 6f6f 6c73 2e69 6574 662e  tp://tools.ietf.
+00000810: 6f72 672f 6874 6d6c 2f72 6663 3432 3236  org/html/rfc4226
+00000820: 3e60 5f20 616e 6420 6054 4f54 500a 3c68  >`_ and `TOTP.<h
+00000830: 7474 703a 2f2f 746f 6f6c 732e 6965 7466  ttp://tools.ietf
+00000840: 2e6f 7267 2f68 746d 6c2f 7266 6336 3233  .org/html/rfc623
+00000850: 383e 605f 2066 6f72 2063 6f6e 7665 6e69  8>`_ for conveni
+00000860: 656e 6365 2c20 6173 2074 6865 7365 2061  ence, as these a
+00000870: 7265 2073 7461 6e64 6172 640a 4f54 5020  re standard.OTP 
+00000880: 616c 676f 7269 7468 6d73 2075 7365 6420  algorithms used 
+00000890: 6279 206d 756c 7469 706c 6520 706c 7567  by multiple plug
+000008a0: 696e 732e 0a0a 4966 2079 6f75 2772 6520  ins...If you're 
+000008b0: 6c6f 6f6b 696e 6720 666f 7220 6120 6869  looking for a hi
+000008c0: 6768 6572 2d6c 6576 656c 206f 7220 6d6f  gher-level or mo
+000008d0: 7265 206f 7069 6e69 6f6e 6174 6564 2073  re opinionated s
+000008e0: 6f6c 7574 696f 6e2c 2079 6f75 206d 6967  olution, you mig
+000008f0: 6874 2062 650a 696e 7465 7265 7374 6564  ht be.interested
+00000900: 2069 6e20 6064 6a61 6e67 6f2d 7477 6f2d   in `django-two-
+00000910: 6661 6374 6f72 2d61 7574 680a 3c68 7474  factor-auth.<htt
+00000920: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000930: 426f 756b 652f 646a 616e 676f 2d74 776f  Bouke/django-two
+00000940: 2d66 6163 746f 722d 6175 7468 3e60 5f2e  -factor-auth>`_.
+00000950: 0a0a 5374 6174 7573 0a2d 2d2d 2d2d 2d0a  ..Status.------.
+00000960: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00000970: 2073 7461 626c 6520 616e 6420 6d61 696e   stable and main
+00000980: 7461 696e 6564 2c20 6275 7420 6973 206e  tained, but is n
+00000990: 6f20 6c6f 6e67 6572 2061 6374 6976 656c  o longer activel
+000009a0: 7920 7573 6564 2062 7920 7468 650a 6175  y used by the.au
+000009b0: 7468 6f72 2061 6e64 2069 7320 6e6f 7420  thor and is not 
+000009c0: 7365 6569 6e67 206d 7563 6820 6f6e 676f  seeing much ongo
+000009d0: 696e 6720 696e 7665 7374 6d65 6e74 2e0a  ing investment..
+000009e0: 0a57 656c 6c2d 666f 726d 6564 2069 7373  .Well-formed iss
+000009f0: 7565 7320 616e 6420 7075 6c6c 2072 6571  ues and pull req
+00000a00: 7565 7374 7320 6172 6520 7765 6c63 6f6d  uests are welcom
+00000a10: 652c 2062 7574 2070 6c65 6173 6520 7365  e, but please se
+00000a20: 6520 434f 4e54 5249 4255 5449 4e47 2e6d  e CONTRIBUTING.m
+00000a30: 640a 6669 7273 742e 2047 656e 6572 616c  d.first. General
+00000a40: 2071 7565 7374 696f 6e73 2061 6e64 2069   questions and i
+00000a50: 6465 6173 2073 686f 756c 6420 6265 2064  deas should be d
+00000a60: 6972 6563 7465 6420 746f 2074 6865 2044  irected to the D
+00000a70: 6973 6375 7373 696f 6e73 0a73 6563 7469  iscussions.secti
+00000a80: 6f6e 3b20 6973 7375 6573 2073 686f 756c  on; issues shoul
+00000a90: 6420 6265 2072 6573 6572 7665 6420 666f  d be reserved fo
+00000aa0: 7220 636f 6e66 6972 6d65 6420 6275 6773  r confirmed bugs
+00000ab0: 2e0a 0a2e 2e20 656e 642d 6f66 2d64 6f63  ..... end-of-doc
+00000ac0: 2d69 6e74 726f 0a0a 0a44 6576 656c 6f70  -intro...Develop
+00000ad0: 6d65 6e74 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ment.-----------
+00000ae0: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
+00000af0: 7320 6275 696c 7420 616e 6420 6d61 6e61  s built and mana
+00000b00: 6765 6420 7769 7468 2060 6861 7463 6860  ged with `hatch`
+00000b10: 5f2e 2049 6620 796f 7520 646f 6e27 7420  _. If you don't 
+00000b20: 6861 7665 2068 6174 6368 2c20 490a 7265  have hatch, I.re
+00000b30: 636f 6d6d 656e 6420 696e 7374 616c 6c69  commend installi
+00000b40: 6e67 2069 7420 7769 7468 2060 7069 7078  ng it with `pipx
+00000b50: 605f 3a20 6060 7069 7078 2069 6e73 7461  `_: ``pipx insta
+00000b60: 6c6c 2068 6174 6368 6060 2e0a 0a60 6070  ll hatch``...``p
+00000b70: 7970 726f 6a65 6374 2e74 6f6d 6c60 6020  yproject.toml`` 
+00000b80: 6465 6669 6e65 7320 7365 7665 7261 6c20  defines several 
+00000b90: 7573 6566 756c 2073 6372 6970 7473 2066  useful scripts f
+00000ba0: 6f72 2064 6576 656c 6f70 6d65 6e74 2061  or development a
+00000bb0: 6e64 2074 6573 7469 6e67 2e0a 5468 6520  nd testing..The 
+00000bc0: 6465 6661 756c 7420 656e 7669 726f 6e6d  default environm
+00000bd0: 656e 7420 696e 636c 7564 6573 2061 6c6c  ent includes all
+00000be0: 2064 6576 2061 6e64 2074 6573 7420 6465   dev and test de
+00000bf0: 7065 6e64 656e 6369 6573 2066 6f72 2071  pendencies for q
+00000c00: 7569 636b 6c79 0a72 756e 6e69 6e67 2074  uickly.running t
+00000c10: 6573 7473 2e20 5468 6520 6060 7465 7374  ests. The ``test
+00000c20: 6060 2065 6e76 6972 6f6e 6d65 6e74 2064  `` environment d
+00000c30: 6566 696e 6573 2074 6865 2074 6573 7420  efines the test 
+00000c40: 6d61 7472 6978 2066 6f72 2072 756e 6e69  matrix for runni
+00000c50: 6e67 2074 6865 0a66 756c 6c20 7661 6c69  ng the.full vali
+00000c60: 6461 7469 6f6e 2073 7569 7465 2e20 4576  dation suite. Ev
+00000c70: 6572 7974 6869 6e67 2069 7320 6578 6563  erything is exec
+00000c80: 7574 6564 2069 6e20 7468 6520 636f 6e74  uted in the cont
+00000c90: 6578 7420 6f66 2074 6865 2044 6a61 6e67  ext of the Djang
+00000ca0: 6f0a 7072 6f6a 6563 7420 696e 2074 6573  o.project in tes
+00000cb0: 742f 7465 7374 5c5f 7072 6f6a 6563 742e  t/test\_project.
+00000cc0: 0a0a 4173 2061 2071 7569 636b 2070 7269  ..As a quick pri
+00000cd0: 6d65 722c 2068 6174 6368 2073 6372 6970  mer, hatch scrip
+00000ce0: 7473 2063 616e 2062 6520 7275 6e20 7769  ts can be run wi
+00000cf0: 7468 2060 6068 6174 6368 2072 756e 205b  th ``hatch run [
+00000d00: 3c65 6e76 3e3a 5d3c 7363 7269 7074 3e60  <env>:]<script>`
+00000d10: 602e 0a54 6f20 7275 6e20 6c69 6e74 6572  `..To run linter
+00000d20: 7320 616e 6420 7465 7374 7320 696e 2074  s and tests in t
+00000d30: 6865 2064 6566 6175 6c74 2065 6e76 6972  he default envir
+00000d40: 6f6e 6d65 6e74 2c20 6a75 7374 2072 756e  onment, just run
+00000d50: 0a60 6068 6174 6368 2072 756e 2063 6865  .``hatch run che
+00000d60: 636b 6060 2e20 5468 6973 2073 686f 756c  ck``. This shoul
+00000d70: 6420 7275 6e20 7465 7374 7320 7769 7468  d run tests with
+00000d80: 2079 6f75 7220 6465 6661 756c 7420 5079   your default Py
+00000d90: 7468 6f6e 2076 6572 7369 6f6e 2061 6e64  thon version and
+00000da0: 0a74 6865 206c 6174 6573 7420 446a 616e  .the latest Djan
+00000db0: 676f 2e20 4f74 6865 7220 7363 7269 7074  go. Other script
+00000dc0: 7320 696e 636c 7564 653a 0a0a 2a20 2a2a  s include:..* **
+00000dd0: 6d61 6e61 6765 2a2a 3a20 5275 6e20 6120  manage**: Run a 
+00000de0: 6d61 6e61 6765 6d65 6e74 2063 6f6d 6d61  management comma
+00000df0: 6e64 2076 6961 2074 6865 2074 6573 7420  nd via the test 
+00000e00: 7072 6f6a 6563 742e 2054 6869 7320 6361  project. This ca
+00000e10: 6e20 6265 2075 7365 6420 746f 0a20 2067  n be used to.  g
+00000e20: 656e 6572 6174 6520 6d69 6772 6174 696f  enerate migratio
+00000e30: 6e73 2e0a 2a20 2a2a 6c69 6e74 2a2a 3a20  ns..* **lint**: 
+00000e40: 5275 6e20 616c 6c20 6c69 6e74 6572 732e  Run all linters.
+00000e50: 0a2a 202a 2a66 6978 2a2a 3a20 5275 6e20  .* **fix**: Run 
+00000e60: 616c 6c20 6669 7865 7273 2074 6f20 6164  all fixers to ad
+00000e70: 6472 6573 7320 6c69 6e74 696e 6720 6973  dress linting is
+00000e80: 7375 6573 2e20 5468 6973 206d 6179 206e  sues. This may n
+00000e90: 6f74 2066 6978 2065 7665 7279 0a20 2069  ot fix every.  i
+00000ea0: 7373 7565 2072 6570 6f72 7465 6420 6279  ssue reported by
+00000eb0: 206c 696e 742e 0a2a 202a 2a74 6573 742a   lint..* **test*
+00000ec0: 2a3a 2052 756e 2061 6c6c 2074 6573 7473  *: Run all tests
+00000ed0: 2e0a 2a20 2a2a 6368 6563 6b2a 2a3a 2052  ..* **check**: R
+00000ee0: 756e 206c 696e 7465 7273 2061 6e64 2074  un linters and t
+00000ef0: 6573 7473 2e0a 2a20 2a2a 7761 726e 2a2a  ests..* **warn**
+00000f00: 3a20 5275 6e20 7465 7374 7320 7769 7468  : Run tests with
+00000f10: 2061 6c6c 2077 6172 6e69 6e67 7320 656e   all warnings en
+00000f20: 6162 6c65 642e 2054 6869 7320 6973 2065  abled. This is e
+00000f30: 7370 6563 6961 6c6c 7920 7573 6566 756c  specially useful
+00000f40: 2066 6f72 0a20 2073 6565 696e 6720 6465   for.  seeing de
+00000f50: 7072 6563 6174 696f 6e20 7761 726e 696e  precation warnin
+00000f60: 6773 2069 6e20 6e65 7720 7665 7273 696f  gs in new versio
+00000f70: 6e73 206f 6620 446a 616e 676f 2e0a 2a20  ns of Django..* 
+00000f80: 2a2a 636f 762a 2a3a 2052 756e 2074 6573  **cov**: Run tes
+00000f90: 7473 2061 6e64 2070 7269 6e74 2061 2063  ts and print a c
+00000fa0: 6f64 6520 636f 7665 7261 6765 2072 6570  ode coverage rep
+00000fb0: 6f72 742e 0a0a 546f 2072 756e 2074 6865  ort...To run the
+00000fc0: 2066 756c 6c20 7465 7374 206d 6174 7269   full test matri
+00000fd0: 782c 2072 756e 2060 6068 6174 6368 2072  x, run ``hatch r
+00000fe0: 756e 2074 6573 743a 7275 6e60 602e 2059  un test:run``. Y
+00000ff0: 6f75 2077 696c 6c20 6e65 6564 206d 756c  ou will need mul
+00001000: 7469 706c 650a 7370 6563 6966 6963 2050  tiple.specific P
+00001010: 7974 686f 6e20 7665 7273 696f 6e73 2069  ython versions i
+00001020: 6e73 7461 6c6c 6564 2066 6f72 2074 6869  nstalled for thi
+00001030: 732e 0a0a 596f 7520 6361 6e20 636c 6561  s...You can clea
+00001040: 6e20 7570 2074 6865 2068 6174 6368 2065  n up the hatch e
+00001050: 6e76 6972 6f6e 6d65 6e74 7320 7769 7468  nvironments with
+00001060: 2060 6068 6174 6368 2065 6e76 2070 7275   ``hatch env pru
+00001070: 6e65 6060 2c20 666f 7220 6578 616d 706c  ne``, for exampl
+00001080: 6520 746f 0a66 6f72 6365 2064 6570 656e  e to.force depen
+00001090: 6465 6e63 7920 7570 6461 7465 732e 0a0a  dency updates...
+000010a0: 5468 6520 7072 6f6a 6563 7420 756e 6465  The project unde
+000010b0: 7220 6060 7465 7374 6060 2063 616e 2062  r ``test`` can b
+000010c0: 6520 7275 6e20 6173 2061 2073 696d 706c  e run as a simpl
+000010d0: 6520 696e 7465 7261 6374 6976 6520 7465  e interactive te
+000010e0: 7374 2065 6e76 6972 6f6e 6d65 6e74 2e0a  st environment..
+000010f0: 5275 6e20 6060 6861 7463 6820 7275 6e20  Run ``hatch run 
+00001100: 6d61 6e61 6765 2072 756e 7365 7276 6572  manage runserver
+00001110: 6060 2061 6e64 206f 7065 6e20 6974 2069  `` and open it i
+00001120: 6e20 6120 6272 6f77 7365 722e 2054 6869  n a browser. Thi
+00001130: 7320 6861 7320 616e 0a69 6d70 6c65 6d65  s has an.impleme
+00001140: 6e74 6174 696f 6e20 6f66 2074 6865 206c  ntation of the l
+00001150: 6f67 696e 2066 6f72 6d20 616e 6420 7669  ogin form and vi
+00001160: 6577 7320 7769 7468 2064 6966 6665 7265  ews with differe
+00001170: 6e74 2063 6f6d 6269 6e61 7469 6f6e 7320  nt combinations 
+00001180: 6f66 0a64 6563 6f72 6174 6f72 732c 2077  of.decorators, w
+00001190: 6869 6368 2079 6f75 2063 616e 2065 7870  hich you can exp
+000011a0: 6572 696d 656e 7420 7769 7468 206f 7220  eriment with or 
+000011b0: 7573 6520 746f 2074 6573 7420 6368 616e  use to test chan
+000011c0: 6765 732e 0a0a 436f 6e66 6967 7572 6174  ges...Configurat
+000011d0: 696f 6e0a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ion.~~~~~~~~~~~~
+000011e0: 7e0a 0a42 7920 6465 6661 756c 742c 2074  ~..By default, t
+000011f0: 6865 2074 6573 7420 7072 6f6a 6563 7420  he test project 
+00001200: 7573 6573 2053 514c 6974 652e 2042 6563  uses SQLite. Bec
+00001210: 6175 7365 2053 514c 6974 6520 646f 6573  ause SQLite does
+00001220: 6e27 7420 7375 7070 6f72 7420 726f 770a  n't support row.
+00001230: 6c6f 636b 696e 672c 2073 6f6d 6520 636f  locking, some co
+00001240: 6e63 7572 7265 6e63 7920 7465 7374 7320  ncurrency tests 
+00001250: 7769 6c6c 2062 6520 736b 6970 7065 642e  will be skipped.
+00001260: 2054 6f20 7465 7374 2061 6761 696e 7374   To test against
+00001270: 2050 6f73 7467 7265 5351 4c2c 2079 6f75   PostgreSQL, you
+00001280: 0a63 616e 2061 6464 2061 206c 6f63 616c  .can add a local
+00001290: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+000012a0: 696c 6520 7468 6174 2070 6f69 6e74 7320  ile that points 
+000012b0: 746f 2079 6f75 7220 6461 7461 6261 7365  to your database
+000012c0: 2e0a 0a43 6f6e 6669 6775 7261 7469 6f6e  ...Configuration
+000012d0: 2069 7320 7461 6b65 6e20 6672 6f6d 2054   is taken from T
+000012e0: 4f4d 4c20 6669 6c65 7320 7374 6f72 6564  OML files stored
+000012f0: 2075 6e64 6572 2060 6074 6573 742f 636f   under ``test/co
+00001300: 6e66 6967 6060 2e20 4120 636f 6e66 6967  nfig``. A config
+00001310: 0a66 696c 6520 6e61 6d65 6420 6060 656e  .file named ``en
+00001320: 762d 3c65 6e76 2d6e 616d 653e 2e74 6f6d  v-<env-name>.tom
+00001330: 6c60 6020 7769 6c6c 2062 6520 6175 746f  l`` will be auto
+00001340: 6d61 7469 6361 6c6c 7920 6170 706c 6965  matically applie
+00001350: 6420 7768 656e 2072 756e 6e69 6e67 0a69  d when running.i
+00001360: 6e73 6964 6520 6120 6d61 7463 6869 6e67  nside a matching
+00001370: 2068 6174 6368 2065 6e76 6972 6f6e 6d65   hatch environme
+00001380: 6e74 2e20 466f 7220 6578 616d 706c 652c  nt. For example,
+00001390: 2060 6065 6e76 2d64 6566 6175 6c74 2e74   ``env-default.t
+000013a0: 6f6d 6c60 6020 6170 706c 6965 730a 746f  oml`` applies.to
+000013b0: 2074 6865 2064 6566 6175 6c74 2064 6576   the default dev
+000013c0: 656c 6f70 6d65 6e74 2065 6e76 6972 6f6e  elopment environ
+000013d0: 6d65 6e74 2061 6e64 2060 6065 6e76 2d74  ment and ``env-t
+000013e0: 6573 742e 746f 6d6c 6060 2061 7070 6c69  est.toml`` appli
+000013f0: 6573 2074 6f20 7468 6520 7465 7374 0a6d  es to the test.m
+00001400: 6174 7269 7820 656e 7669 726f 6e6d 656e  atrix environmen
+00001410: 7473 2e0a 0a57 6974 6820 6120 7769 6465  ts...With a wide
+00001420: 2d6f 7065 6e20 506f 7374 6772 6553 514c  -open PostgreSQL
+00001430: 2069 6e73 7461 6c6c 2c20 616e 2060 6065   install, an ``e
+00001440: 6e76 2d74 6573 742e 746f 6d6c 6060 206d  nv-test.toml`` m
+00001450: 6967 6874 206c 6f6f 6b20 6c69 6b65 2074  ight look like t
+00001460: 6869 733a 0a0a 2e2e 2063 6f64 652d 626c  his:.... code-bl
+00001470: 6f63 6b3a 3a20 746f 6d6c 0a0a 2020 205b  ock:: toml..   [
+00001480: 6461 7461 6261 7365 5d0a 2020 2045 4e47  database].   ENG
+00001490: 494e 4520 3d20 2264 6a61 6e67 6f2e 6462  INE = "django.db
+000014a0: 2e62 6163 6b65 6e64 732e 706f 7374 6772  .backends.postgr
+000014b0: 6573 716c 220a 2020 204e 414d 4520 3d20  esql".   NAME = 
+000014c0: 2264 6a61 6e67 6f2d 6f74 7022 0a20 2020  "django-otp".   
+000014d0: 5553 4552 203d 2022 706f 7374 6772 6573  USER = "postgres
+000014e0: 220a 0a46 6f72 2064 6576 656c 6f70 6d65  "..For developme
+000014f0: 6e74 2c20 7468 6520 636f 6e66 6967 2066  nt, the config f
+00001500: 696c 6520 6361 6e20 616c 736f 2062 6520  ile can also be 
+00001510: 7573 6564 2074 6f20 696e 6a65 6374 2044  used to inject D
+00001520: 6a61 6e67 6f20 6170 7073 2061 6e64 0a6d  jango apps and.m
+00001530: 6964 646c 6577 6172 652c 206f 7220 746f  iddleware, or to
+00001540: 206f 7665 7272 6964 6520 6172 6269 7472   override arbitr
+00001550: 6172 7920 446a 616e 676f 2073 6574 7469  ary Django setti
+00001560: 6e67 732e 2053 6565 0a60 6074 6573 742f  ngs. See.``test/
+00001570: 636f 6e66 6967 2f73 616d 706c 652e 746f  config/sample.to
+00001580: 6d6c 6060 2066 6f72 2061 2066 756c 6c20  ml`` for a full 
+00001590: 6465 7363 7269 7074 696f 6e2e 0a0a 596f  description...Yo
+000015a0: 7520 6361 6e20 616c 736f 2066 6f72 6365  u can also force
+000015b0: 2061 2073 7065 6369 6669 6320 636f 6e66   a specific conf
+000015c0: 6967 2066 696c 6520 6279 2073 6574 7469  ig file by setti
+000015d0: 6e67 2074 6865 2065 6e76 6972 6f6e 6d65  ng the environme
+000015e0: 6e74 2076 6172 6961 626c 650a 6060 444a  nt variable.``DJ
+000015f0: 414e 474f 5f4f 5450 5f43 4f4e 4649 4760  ANGO_OTP_CONFIG`
+00001600: 6020 746f 2061 2070 6174 682e 0a0a 0a54  ` to a path....T
+00001610: 6865 2046 7574 7572 650a 2d2d 2d2d 2d2d  he Future.------
+00001620: 2d2d 2d2d 0a0a 4f6e 6365 2075 706f 6e20  ----..Once upon 
+00001630: 6120 7469 6d65 2c20 6576 6572 7974 6869  a time, everythi
+00001640: 6e67 2077 6173 2075 7365 726e 616d 6573  ng was usernames
+00001650: 2061 6e64 2070 6173 7377 6f72 6473 2e20   and passwords. 
+00001660: 4f72 2065 7665 6e20 696e 2074 6865 2063  Or even in the c
+00001670: 6173 6520 6f66 0a6f 7468 6572 2061 7574  ase of.other aut
+00001680: 6865 6e74 6963 6174 696f 6e20 6d65 6368  hentication mech
+00001690: 616e 6973 6d73 2c20 6120 7573 6572 2077  anisms, a user w
+000016a0: 6173 2065 6974 6865 7220 6175 7468 656e  as either authen
+000016b0: 7469 6361 7465 6420 6f72 206e 6f74 0a28  ticated or not.(
+000016c0: 616e 6f6e 796d 6f75 7320 696e 2044 6a61  anonymous in Dja
+000016d0: 6e67 6f27 7320 7465 726d 696e 6f6c 6f67  ngo's terminolog
+000016e0: 7929 2e20 5468 656e 2074 6865 7265 2077  y). Then there w
+000016f0: 6173 2074 776f 2d66 6163 746f 7220 6175  as two-factor au
+00001700: 7468 656e 7469 6361 7469 6f6e 2c0a 7768  thentication,.wh
+00001710: 6963 6820 636f 756c 6420 7369 6d70 6c79  ich could simply
+00001720: 2062 6520 616e 2069 6d70 6c65 6d65 6e74   be an implement
+00001730: 6174 696f 6e20 6465 7461 696c 2069 6e20  ation detail in 
+00001740: 6120 6269 6e61 7279 2061 7574 6865 6e74  a binary authent
+00001750: 6963 6174 696f 6e20 7374 6174 652c 0a62  ication state,.b
+00001760: 7574 2063 6f75 6c64 2061 6c73 6f20 696d  ut could also im
+00001770: 706c 7920 6c65 7665 6c73 206f 7220 6465  ply levels or de
+00001780: 6772 6565 7320 6f66 2061 7574 6865 6e74  grees of authent
+00001790: 6963 6174 696f 6e2e 0a0a 5468 6573 6520  ication...These 
+000017a0: 6461 7973 2c20 6974 2773 2069 6e63 7265  days, it's incre
+000017b0: 6173 696e 676c 7920 636f 6d6d 6f6e 2074  asingly common t
+000017c0: 6f20 7365 6520 7369 7465 7320 7769 7468  o see sites with
+000017d0: 206d 6f72 6520 6e75 616e 6365 640a 6175   more nuanced.au
+000017e0: 7468 656e 7469 6361 7469 6f6e 2073 7461  thentication sta
+000017f0: 7465 2e20 4120 7369 7465 206d 6967 6874  te. A site might
+00001800: 2072 656d 656d 6265 7220 7768 6f20 796f   remember who yo
+00001810: 7520 6172 6520 666f 7265 7665 72e2 8094  u are forever...
+00001820: 736f 2079 6f75 2772 6520 6e6f 740a 616e  so you're not.an
+00001830: 6f6e 796d 6f75 73e2 8094 6275 7420 6966  onymous...but if
+00001840: 2079 6f75 2074 7279 2074 6f20 646f 2061   you try to do a
+00001850: 6e79 7468 696e 6720 7072 6976 6174 652c  nything private,
+00001860: 2079 6f75 2068 6176 6520 746f 2072 652d   you have to re-
+00001870: 6175 7468 656e 7469 6361 7465 2e0a 596f  authenticate..Yo
+00001880: 7520 6d61 7920 6265 2061 626c 6520 746f  u may be able to
+00001890: 2063 686f 6f73 6520 6672 6f6d 2061 6d6f   choose from amo
+000018a0: 6e67 2061 6c6c 206f 6620 7468 6520 6175  ng all of the au
+000018b0: 7468 656e 7469 6361 7469 6f6e 206d 6563  thentication mec
+000018c0: 6861 6e69 736d 7320 796f 750a 6861 7665  hanisms you.have
+000018d0: 2063 6f6e 6669 6775 7265 642c 206f 7220   configured, or 
+000018e0: 6f6e 6c79 2066 726f 6d20 736f 6d65 206f  only from some o
+000018f0: 6620 7468 656d 2e20 5370 6563 6966 6963  f them. Specific
+00001900: 206d 6563 6861 6e69 736d 7320 6d61 7920   mechanisms may 
+00001910: 6265 2072 6571 7569 7265 640a 666f 7220  be required.for 
+00001920: 7370 6563 6966 6963 2061 6374 696f 6e73  specific actions
+00001930: 2c20 7375 6368 2061 7320 7573 696e 6720  , such as using 
+00001940: 796f 7572 2055 3246 2064 6576 6963 6520  your U2F device 
+00001950: 746f 2061 6363 6573 7320 796f 7572 2055  to access your U
+00001960: 3246 2073 6574 7469 6e67 732e 0a0a 496e  2F settings...In
+00001970: 2073 686f 7274 2c20 7468 6520 776f 726c   short, the worl
+00001980: 6420 7365 656d 7320 746f 2062 6520 6d6f  d seems to be mo
+00001990: 7669 6e67 2062 6579 6f6e 6420 7468 6520  ving beyond the 
+000019a0: 6173 7375 6d70 7469 6f6e 7320 7468 6174  assumptions that
+000019b0: 206f 7269 6769 6e61 6c6c 790a 696e 666f   originally.info
+000019c0: 726d 6564 2044 6a61 6e67 6f27 7320 6573  rmed Django's es
+000019d0: 7365 6e74 6961 6c20 6175 7468 656e 7469  sential authenti
+000019e0: 6361 7469 6f6e 2064 6573 6967 6e2e 2049  cation design. I
+000019f0: 6620 4920 7765 7265 2073 7469 6c6c 2069  f I were still i
+00001a00: 6e76 6573 7469 6e67 2069 6e0a 446a 616e  nvesting in.Djan
+00001a10: 676f 2067 656e 6572 616c 6c79 2c20 4920  go generally, I 
+00001a20: 776f 756c 6420 7072 6f62 6162 6c79 2073  would probably s
+00001a30: 7461 7274 2061 206e 6577 206d 756c 7469  tart a new multi
+00001a40: 2d66 6163 746f 7220 6175 7468 656e 7469  -factor authenti
+00001a50: 6361 7469 6f6e 0a70 726f 6a65 6374 2074  cation.project t
+00001a60: 6861 7420 776f 756c 6420 7265 666c 6563  hat would reflec
+00001a70: 7420 7468 6573 6520 6368 616e 6765 732e  t these changes.
+00001a80: 2049 7420 776f 756c 6420 696e 636f 7270   It would incorp
+00001a90: 6f72 6174 6520 7468 6520 6964 6561 2074  orate the idea t
+00001aa0: 6861 7420 610a 7573 6572 206d 6179 2062  hat a.user may b
+00001ab0: 6520 6175 7468 656e 7469 6361 7465 6420  e authenticated 
+00001ac0: 6279 2076 6172 696f 7573 2063 6f6d 6269  by various combi
+00001ad0: 6e61 7469 6f6e 7320 6f66 206d 6563 6861  nations of mecha
+00001ae0: 6e69 736d 7320 6174 2061 6e79 2074 696d  nisms at any tim
+00001af0: 6520 616e 640a 7468 6174 2064 6966 6665  e and.that diffe
+00001b00: 7265 6e74 2063 6f6d 6269 6e61 7469 6f6e  rent combination
+00001b10: 7320 6d61 7920 6265 2072 6571 7569 7265  s may be require
+00001b20: 6420 746f 2073 6174 6973 6679 2064 6976  d to satisfy div
+00001b30: 6572 7365 2061 7574 686f 7269 7a61 7469  erse authorizati
+00001b40: 6f6e 0a72 6571 7569 7265 6d65 6e74 7320  on.requirements 
+00001b50: 6163 726f 7373 2074 6865 2073 6974 652e  across the site.
+00001b60: 2049 7420 776f 756c 6420 6d6f 7374 206c   It would most l
+00001b70: 696b 656c 7920 7472 7920 746f 2064 6973  ikely try to dis
+00001b80: 656e 7461 6e67 6c65 0a61 7574 6865 6e74  entangle.authent
+00001b90: 6963 6174 696f 6e20 7065 7273 6973 7465  ication persiste
+00001ba0: 6e63 6520 6672 6f6d 2073 6573 7369 6f6e  nce from session
+00001bb0: 732c 2061 7420 6c65 6173 7420 746f 2073  s, at least to s
+00001bc0: 6f6d 6520 6578 7465 6e74 2e20 4d61 6e79  ome extent. Many
+00001bd0: 2073 6974 6573 0a77 6f75 6c64 206e 6f74   sites.would not
+00001be0: 2072 6571 7569 7265 2061 6c6c 206f 6620   require all of 
+00001bf0: 7468 6973 2066 6c65 7869 6269 6c69 7479  this flexibility
+00001c00: 2c20 6275 7420 6974 2077 6f75 6c64 206f  , but it would o
+00001c10: 7065 6e20 7570 2070 6f73 7369 6269 6c69  pen up possibili
+00001c20: 7469 6573 0a66 6f72 2062 6574 7465 7220  ties.for better 
+00001c30: 6578 7065 7269 656e 6365 7320 6279 206e  experiences by n
+00001c40: 6f74 2061 736b 696e 6720 7573 6572 7320  ot asking users 
+00001c50: 666f 7220 6d6f 7265 2074 6861 6e20 7765  for more than we
+00001c60: 2072 6571 7569 7265 2061 7420 616e 790a   require at any.
+00001c70: 706f 696e 742e 0a0a 4966 2061 6e79 6f6e  point...If anyon
+00001c80: 6520 6861 7320 6120 6d69 6e64 2074 6f20  e has a mind to 
+00001c90: 7461 6b65 206f 6e20 6120 7072 6f6a 6563  take on a projec
+00001ca0: 7420 6c69 6b65 2074 6869 732c 2049 2764  t like this, I'd
+00001cb0: 2062 6520 6861 7070 7920 746f 206f 6666   be happy to off
+00001cc0: 6572 0a77 6861 7465 7665 7220 6164 7669  er.whatever advi
+00001cd0: 6365 206f 7220 6c65 7373 6f6e 7320 6c65  ce or lessons le
+00001ce0: 6172 6e65 6420 7468 6174 2049 2063 616e  arned that I can
+00001cf0: 2e0a 0a0a 2e2e 205f 6861 7463 683a 2068  ...... _hatch: h
+00001d00: 7474 7073 3a2f 2f68 6174 6368 2e70 7970  ttps://hatch.pyp
+00001d10: 612e 696f 2f0a 2e2e 205f 7069 7078 3a20  a.io/... _pipx: 
+00001d20: 6874 7470 733a 2f2f 7079 7061 2e67 6974  https://pypa.git
+00001d30: 6875 622e 696f 2f70 6970 782f 0a         hub.io/pipx/.
```

### Comparing `django-otp-1.1.6/docs/Makefile` & `django_otp-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/docs/source/auth.rst` & `django_otp-1.2.0/docs/source/auth.rst`

 * *Files 1% similar despite different names*

```diff
@@ -152,17 +152,14 @@
 .. autofunction:: django_otp.match_token
 
 .. autofunction:: django_otp.login
 
 .. autoclass:: django_otp.models.Device
     :members: is_interactive, generate_challenge, verify_token, verify_is_allowed, persistent_id, from_persistent_id
 
-.. autoclass:: django_otp.models.SideChannelDevice
-    :members: generate_token, verify_token
-
 .. autoclass:: django_otp.models.DeviceManager
     :members: devices_for_user
 
 .. autoclass:: django_otp.models.VerifyNotAllowed
 
 
 Authorizing Users
```

### Comparing `django-otp-1.1.6/docs/source/conf.py` & `django_otp-1.2.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import os.path
 import sys
 
 import django
 import django.conf
 
+
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('../ext'))
 
 # -- General configuration -----------------------------------------------------
 
@@ -59,16 +60,16 @@
     ],
     SECRET_KEY='properly-configured',
 )
 django.setup()
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
-    'django': ('https://docs.djangoproject.com/en/2.2/',
-               'https://docs.djangoproject.com/en/2.2/_objects/'),
+    'django': ('https://docs.djangoproject.com/en/4.2/',
+               'https://docs.djangoproject.com/en/4.2/_objects/'),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
@@ -77,22 +78,22 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'django-otp'
-copyright = '2012, Peter Sagerson'
+#  copyright = ''
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '1.1.6'
+release = '1.2.0'
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
@@ -190,15 +191,15 @@
 # If true, links to the reST sources are added to the pages.
 # html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
 # html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-# html_show_copyright = True
+html_show_copyright = False
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
```

### Comparing `django-otp-1.1.6/docs/source/extend.rst` & `django_otp-1.2.0/docs/source/extend.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. vim: tw=80 lbr
+
 Extending Django-OTP
 ====================
 
 A django-otp plugin is defined as a Django app that includes at least one model
 derived from :class:`django_otp.models.Device`. All Device-derived model objects
 will be detected by the framework and included in the standard forms and APIs.
 
@@ -56,23 +58,27 @@
 
 If a device uses a challenge-response algorithm or requires some other kind of
 user interaction, it should implement an additional method:
 
 .. automethod:: django_otp.models.Device.generate_challenge
     :noindex:
 
-For devices that send a token via a separate channel, like the
-:class:`~django_otp.plugins.otp_email.models.EmailDevice` example, a generic
-:class:`~django_otp.models.SideChannelDevice` is provided. This abstract subclass of
-:class:`~django_otp.models.Device` provides
-:meth:`~django_otp.models.SideChannelDevice.generate_token` and implements
-:meth:`~django_otp.models.SideChannelDevice.verify_token` for concrete devices, which
-then only have to implement :meth:`~django_otp.models.Device.generate_challenge` to
-actually deliver the token to the user.
 
+Helpers
+-------
+
+:mod:`django_otp.models` also provides a few mixins and other helpers for
+common functionality. These are entirely optional, but can be helpful for common
+functionality.
+
+.. autoclass:: django_otp.models.SideChannelDevice
+    :members: generate_token, verify_token
+
+.. autoclass:: django_otp.models.ThrottlingMixin
+   :members: get_throttle_factor, verify_is_allowed, throttle_reset, throttle_increment
 
 .. _utilities:
 
 Utilities
 ---------
 
 django_otp provides several low-level utilities as a convenience to plugin
```

### Comparing `django-otp-1.1.6/docs/source/overview.rst` & `django_otp-1.2.0/docs/source/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -311,14 +311,26 @@
 
 Default: ``None``
 
 The ``issuer`` parameter for the otpauth URL generated by
 :attr:`~django_otp.plugins.otp_totp.models.TOTPDevice.config_url`.
 This can be a string or a callable to dynamically set the value.
 
+.. setting:: OTP_TOTP_IMAGE
+
+**OTP_TOTP_IMAGE**
+
+Default: ``None``
+
+The ``image`` parameter for the otpauth URL generated by
+:attr:`~django_otp.plugins.otp_totp.models.TOTPDevice.config_url`.
+It should be a HTTPS URL pointing to a square PNG image.
+This will be read and displayed by some authenticator applications, e.g. FreeOTP.
+This can be a string or a callable to dynamically set the value.
+
 .. setting:: OTP_TOTP_SYNC
 
 **OTP_TOTP_SYNC**
 
 Default: ``True``
 
 If true, then TOTP devices will keep track of the difference between the
```

### Comparing `django-otp-1.1.6/src/django_otp/__init__.py` & `django_otp-1.2.0/src/django_otp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from django.contrib.auth.signals import user_logged_in
 from django.db import transaction
 
-
 DEVICE_ID_SESSION_KEY = 'otp_device_id'
 
 
 def login(request, device):
     """
     Persist the given OTP device in the current session. The device will be
     rejected if it does not belong to ``request.user``.
@@ -60,15 +59,19 @@
 
     """
     from django_otp.models import Device
 
     verified = None
     with transaction.atomic():
         device = Device.from_persistent_id(device_id, for_verify=True)
-        if (device is not None) and (device.user_id == user.pk) and device.verify_token(token):
+        if (
+            (device is not None)
+            and (device.user_id == user.pk)
+            and device.verify_token(token)
+        ):
             verified = device
 
     return verified
 
 
 def match_token(user, token):
     """
@@ -154,14 +157,14 @@
     return has_device
 
 
 def device_classes():
     """
     Returns an iterable of all loaded device models.
     """
-    from django.apps import apps           # isort: skip
+    from django.apps import apps  # isort: skip
     from django_otp.models import Device
 
     for config in apps.get_app_configs():
         for model in config.get_models():
             if issubclass(model, Device):
                 yield model
```

### Comparing `django-otp-1.1.6/src/django_otp/admin.py` & `django_otp-1.2.0/src/django_otp/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class OTPAdminAuthenticationForm(AdminAuthenticationForm, OTPAuthenticationFormMixin):
     """
     An :class:`~django.contrib.admin.forms.AdminAuthenticationForm` subclass
     that solicits an OTP token. This has the same behavior as
     :class:`~django_otp.forms.OTPAuthenticationForm`.
     """
+
     otp_device = forms.CharField(required=False, widget=forms.Select)
     otp_token = forms.CharField(required=False)
 
     # This is a placeholder field that allows us to detect when the user clicks
     # the otp_challenge submit button.
     otp_challenge = forms.CharField(required=False)
 
@@ -40,14 +41,15 @@
     """
     This is an :class:`~django.contrib.admin.AdminSite` subclass that requires
     two-factor authentication. Only users that can be verified by a registered
     OTP device will be authorized for this admin site. Unverified users will be
     treated as if :attr:`~django.contrib.auth.models.User.is_staff` is
     ``False``.
     """
+
     #: The default instance name of this admin site. You should instantiate
     #: this class as ``OTPAdminSite(OTPAdminSite.name)`` to make sure the admin
     #: templates render the correct URLs.
     name = 'otpadmin'
 
     login_form = OTPAdminAuthenticationForm
```

### Comparing `django-otp-1.1.6/src/django_otp/conf.py` & `django_otp-1.2.0/src/django_otp/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import django.conf
+from django.utils.functional import cached_property
 
 
 class Settings:
     """
     This is a simple class to take the place of the global settings object. An
     instance will contain all of our settings as attributes, with default values
     if they are not specified by the configuration.
     """
-    defaults = {
-        'OTP_LOGIN_URL': django.conf.settings.LOGIN_URL,
-        'OTP_ADMIN_HIDE_SENSITIVE_DATA': False,
-    }
+
+    @cached_property
+    def defaults(self):
+        return {
+            'OTP_LOGIN_URL': django.conf.settings.LOGIN_URL,
+            'OTP_ADMIN_HIDE_SENSITIVE_DATA': False,
+        }
 
     def __getattr__(self, name):
         if name in self.defaults:
             return getattr(django.conf.settings, name, self.defaults[name])
         else:
             return getattr(django.conf.settings, name)
```

### Comparing `django-otp-1.1.6/src/django_otp/decorators.py` & `django_otp-1.2.0/src/django_otp/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from django.contrib.auth.decorators import user_passes_test
 
 from django_otp import user_has_device
 from django_otp.conf import settings
 
 
-def otp_required(view=None, redirect_field_name='next', login_url=None, if_configured=False):
+def otp_required(
+    view=None, redirect_field_name='next', login_url=None, if_configured=False
+):
     """
     Similar to :func:`~django.contrib.auth.decorators.login_required`, but
     requires the user to be :term:`verified`. By default, this redirects users
     to :setting:`OTP_LOGIN_URL`.
 
     :param if_configured: If ``True``, an authenticated user with no confirmed
         OTP devices will be allowed. Default is ``False``.
     :type if_configured: bool
     """
     if login_url is None:
         login_url = settings.OTP_LOGIN_URL
 
     def test(user):
-        return user.is_verified() or (if_configured and user.is_authenticated and not user_has_device(user))
-
-    decorator = user_passes_test(test, login_url=login_url, redirect_field_name=redirect_field_name)
+        return user.is_verified() or (
+            if_configured and user.is_authenticated and not user_has_device(user)
+        )
+
+    decorator = user_passes_test(
+        test, login_url=login_url, redirect_field_name=redirect_field_name
+    )
 
     return decorator if (view is None) else decorator(view)
```

### Comparing `django-otp-1.1.6/src/django_otp/forms.py` & `django_otp-1.2.0/src/django_otp/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,25 +51,31 @@
         class CustomAuthForm(OTPAuthenticationFormMixin, AuthenticationForm):
             otp_error_messages = dict(OTPAuthenticationFormMixin.otp_error_messages,
                 token_required=_('Please enter your authentication code.'),
                 invalid_token=_('Incorrect authentication code. Please try again.'),
             )
 
     """
+
     otp_error_messages = {
         'token_required': _('Please enter your OTP token.'),
         'challenge_exception': _('Error generating challenge: {0}'),
         'not_interactive': _('The selected OTP device is not interactive'),
         'challenge_message': _('OTP Challenge: {0}'),
-        'invalid_token': _('Invalid token. Please make sure you have entered it correctly.'),
+        'invalid_token': _(
+            'Invalid token. Please make sure you have entered it correctly.'
+        ),
         'n_failed_attempts': ngettext_lazy(
             "Verification temporarily disabled because of %(failure_count)d failed attempt, please try again soon.",
             "Verification temporarily disabled because of %(failure_count)d failed attempts, please try again soon.",
-            "failure_count"),
-        'verification_not_allowed': _("Verification of the token is currently disabled"),
+            "failure_count",
+        ),
+        'verification_not_allowed': _(
+            "Verification of the token is currently disabled"
+        ),
     }
 
     def clean_otp(self, user):
         """
         Processes the ``otp_*`` fields.
 
         :param user: A user that has been authenticated by the first factor
@@ -91,15 +97,18 @@
 
                 try:
                     if self.cleaned_data.get('otp_challenge'):
                         self._handle_challenge(device)
                     elif token:
                         user.otp_device = self._verify_token(user, token, device)
                     else:
-                        raise forms.ValidationError(self.otp_error_messages['token_required'], code='token_required')
+                        raise forms.ValidationError(
+                            self.otp_error_messages['token_required'],
+                            code='token_required',
+                        )
                 finally:
                     if user.otp_device is None:
                         self._update_form(user)
             except forms.ValidationError as e:
                 # Validation errors shouldn't abort the transaction, so we have
                 # to carefully transport them out.
                 validation_error = e
@@ -125,42 +134,55 @@
         return device
 
     def _handle_challenge(self, device):
         try:
             challenge = device.generate_challenge() if (device is not None) else None
         except Exception as e:
             raise forms.ValidationError(
-                self.otp_error_messages['challenge_exception'].format(e), code='challenge_exception'
+                self.otp_error_messages['challenge_exception'].format(e),
+                code='challenge_exception',
             )
         else:
             if challenge is None:
-                raise forms.ValidationError(self.otp_error_messages['not_interactive'], code='not_interactive')
+                raise forms.ValidationError(
+                    self.otp_error_messages['not_interactive'], code='not_interactive'
+                )
             else:
                 raise forms.ValidationError(
-                    self.otp_error_messages['challenge_message'].format(challenge), code='challenge_message'
+                    self.otp_error_messages['challenge_message'].format(challenge),
+                    code='challenge_message',
                 )
 
     def _verify_token(self, user, token, device=None):
         if device is not None:
             verify_is_allowed, extra = device.verify_is_allowed()
             if not verify_is_allowed:
                 # Try to match specific conditions we know about.
-                if ('reason' in extra and extra['reason'] == VerifyNotAllowed.N_FAILED_ATTEMPTS):
-                    raise forms.ValidationError(self.otp_error_messages['n_failed_attempts'] % extra)
+                if (
+                    'reason' in extra
+                    and extra['reason'] == VerifyNotAllowed.N_FAILED_ATTEMPTS
+                ):
+                    raise forms.ValidationError(
+                        self.otp_error_messages['n_failed_attempts'] % extra
+                    )
                 if 'error_message' in extra:
                     raise forms.ValidationError(extra['error_message'])
                 # Fallback to generic message otherwise.
-                raise forms.ValidationError(self.otp_error_messages['verification_not_allowed'])
+                raise forms.ValidationError(
+                    self.otp_error_messages['verification_not_allowed']
+                )
 
             device = device if device.verify_token(token) else None
         else:
             device = match_token(user, token)
 
         if device is None:
-            raise forms.ValidationError(self.otp_error_messages['invalid_token'], code='invalid_token')
+            raise forms.ValidationError(
+                self.otp_error_messages['invalid_token'], code='invalid_token'
+            )
 
         return device
 
     def _update_form(self, user):
         if 'otp_device' in self.fields:
             self.fields['otp_device'].widget.choices = self.device_choices(user)
 
@@ -232,16 +254,19 @@
           the chosen device. When that succeeds, authentication and
           verification are successful and the user is logged in.
 
     Error messages can be customized in subclasses; see
     :class:`OTPAuthenticationFormMixin`.
 
     """
+
     otp_device = forms.CharField(required=False, widget=forms.Select)
-    otp_token = forms.CharField(required=False, widget=forms.TextInput(attrs={'autocomplete': 'off'}))
+    otp_token = forms.CharField(
+        required=False, widget=forms.TextInput(attrs={'autocomplete': 'off'})
+    )
 
     # This is a placeholder field that allows us to detect when the user clicks
     # the otp_challenge submit button.
     otp_challenge = forms.CharField(required=False)
 
     def clean(self):
         self.cleaned_data = super().clean()
@@ -269,16 +294,19 @@
     :param user: An authenticated user.
     :type user: :class:`~django.contrib.auth.models.User`
 
     :param request: The current request.
     :type request: :class:`~django.http.HttpRequest`
 
     """
+
     otp_device = forms.ChoiceField(choices=[])
-    otp_token = forms.CharField(required=False, widget=forms.TextInput(attrs={'autocomplete': 'off'}))
+    otp_token = forms.CharField(
+        required=False, widget=forms.TextInput(attrs={'autocomplete': 'off'})
+    )
     otp_challenge = forms.CharField(required=False)
 
     def __init__(self, user, request=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.user = user
         self.fields['otp_device'].choices = self.device_choices(user)
```

### Comparing `django-otp-1.1.6/src/django_otp/locale/de/LC_MESSAGES/django.mo` & `django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/locale/de/LC_MESSAGES/django.po` & `django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/locale/es/LC_MESSAGES/django.mo` & `django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/locale/es/LC_MESSAGES/django.po` & `django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/locale/fr/LC_MESSAGES/django.mo` & `django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/locale/fr/LC_MESSAGES/django.po` & `django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/middleware.py` & `django_otp-1.2.0/src/django_otp/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,34 +17,41 @@
     performs an analogous function. Just as AuthenticationMiddleware populates
     ``request.user`` based on session data, OTPMiddleware populates
     ``request.user.otp_device`` to the :class:`~django_otp.models.Device`
     object that has verified the user, or ``None`` if the user has not been
     verified.  As a convenience, this also installs ``user.is_verified()``,
     which returns ``True`` if ``user.otp_device`` is not ``None``.
     """
+
     def __init__(self, get_response=None):
         self.get_response = get_response
 
     def __call__(self, request):
         user = getattr(request, 'user', None)
         if user is not None:
-            request.user = SimpleLazyObject(functools.partial(self._verify_user, request, user))
+            request.user = SimpleLazyObject(
+                functools.partial(self._verify_user, request, user)
+            )
 
         return self.get_response(request)
 
     def _verify_user(self, request, user):
         """
         Sets OTP-related fields on an authenticated user.
         """
         user.otp_device = None
         user.is_verified = functools.partial(is_verified, user)
 
         if user.is_authenticated:
             persistent_id = request.session.get(DEVICE_ID_SESSION_KEY)
-            device = self._device_from_persistent_id(persistent_id) if persistent_id else None
+            device = (
+                self._device_from_persistent_id(persistent_id)
+                if persistent_id
+                else None
+            )
 
             if (device is not None) and (device.user_id != user.pk):
                 device = None
 
             if (device is None) and (DEVICE_ID_SESSION_KEY in request.session):
                 del request.session[DEVICE_ID_SESSION_KEY]
```

### Comparing `django-otp-1.1.6/src/django_otp/models.py` & `django_otp-1.2.0/src/django_otp/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 class DeviceManager(models.Manager):
     """
     The :class:`~django.db.models.Manager` object installed as
     ``Device.objects``.
     """
+
     def devices_for_user(self, user, confirmed=None):
         """
         Returns a queryset for all devices of this class that belong to the
         given user.
 
         :param user: The user.
         :type user: :class:`~django.contrib.auth.models.User`
@@ -67,17 +68,28 @@
         a device and then ask the user for confirmation. As a rule, built-in
         APIs that enumerate devices will only include those that are confirmed.
 
     .. attribute:: objects
 
         A :class:`~django_otp.models.DeviceManager`.
     """
-    user = models.ForeignKey(getattr(settings, 'AUTH_USER_MODEL', 'auth.User'), help_text="The user that this device belongs to.", on_delete=models.CASCADE)
-    name = models.CharField(max_length=64, help_text="The human-readable name of this device.")
-    confirmed = models.BooleanField(default=True, help_text="Is this device ready for use?")
+
+    user = models.ForeignKey(
+        getattr(settings, 'AUTH_USER_MODEL', 'auth.User'),
+        help_text="The user that this device belongs to.",
+        on_delete=models.CASCADE,
+    )
+
+    name = models.CharField(
+        max_length=64, help_text="The human-readable name of this device."
+    )
+
+    confirmed = models.BooleanField(
+        default=True, help_text="Is this device ready for use?"
+    )
 
     objects = DeviceManager()
 
     class Meta:
         abstract = True
 
     def __str__(self):
@@ -160,14 +172,15 @@
             return ``None`` if this device is not interactive.
         :rtype: string or ``None``
 
         :raises: Any :exc:`~exceptions.Exception` is permitted. Callers should
             trap ``Exception`` and report it to the user.
         """
         return None
+
     generate_challenge.stub = True
 
     def verify_is_allowed(self):
         """
         Checks whether it is permissible to call :meth:`verify_token`. If it is
         allowed, returns ``(True, None)``. Otherwise returns ``(False,
         data_dict)``, where ``data_dict`` contains extra information, defined
@@ -205,18 +218,20 @@
     """
     Abstract base model for a side-channel :term:`device` attached to a user.
 
     This model implements token generation, verification and expiration, so the
     concrete devices only have to implement delivery.
 
     """
+
     token = models.CharField(max_length=16, blank=True, null=True)
+
     valid_until = models.DateTimeField(
         default=timezone.now,
-        help_text="The timestamp of the moment of expiry of the saved token."
+        help_text="The timestamp of the moment of expiry of the saved token.",
     )
 
     class Meta:
         abstract = True
 
     def generate_token(self, length=6, valid_secs=300, commit=True):
         """
@@ -243,15 +258,19 @@
 
         :param str token: The OTP token provided by the user.
         :rtype: bool
 
         """
         _now = timezone.now()
 
-        if (self.token is not None) and (token == self.token) and (_now < self.valid_until):
+        if (
+            (self.token is not None)
+            and (token == self.token)
+            and (_now < self.valid_until)
+        ):
             self.token = None
             self.valid_until = _now
             self.save()
 
             return True
         else:
             return False
@@ -266,61 +285,80 @@
     .. data:: N_FAILED_ATTEMPTS
 
        Indicates that verification is disallowed because of ``n`` successive
        failed attempts. The data dictionary should include the value of ``n``
        in member ``failure_count``
 
     """
+
     N_FAILED_ATTEMPTS = 'N_FAILED_ATTEMPTS'
 
 
 class ThrottlingMixin(models.Model):
     """
-    Mixin class for models that need throttling behaviour. Implements
-    exponential back-off.
+    Mixin class for models that want throttling behaviour.
+
+    This implements exponential back-off for verifying tokens. Subclasses must
+    implement :meth:`get_throttle_factor`, and must use the
+    :meth:`verify_is_allowed`, :meth:`throttle_reset` and
+    :meth:`throttle_increment` methods from within their verify_token() method.
+
+    See the implementation of
+    :class:`~django_otp.plugins.otp_email.models.EmailDevice` for an example.
+
     """
-    # This mixin is not publicly documented, but is used internally to avoid
-    # code duplication. Subclasses must implement get_throttle_factor(), and
-    # must use the verify_is_allowed(), throttle_reset() and
-    # throttle_increment() methods from within their verify_token() method.
+
     throttling_failure_timestamp = models.DateTimeField(
-        null=True, blank=True, default=None,
-        help_text="A timestamp of the last failed verification attempt. Null if last attempt succeeded."
+        null=True,
+        blank=True,
+        default=None,
+        help_text="A timestamp of the last failed verification attempt. Null if last attempt succeeded.",
     )
+
     throttling_failure_count = models.PositiveIntegerField(
         default=0, help_text="Number of successive failed attempts."
     )
 
     def verify_is_allowed(self):
         """
         If verification is allowed, returns ``(True, None)``.
         Otherwise, returns ``(False, data_dict)``.
 
         ``data_dict`` contains further information. Currently it can be::
 
-            {'reason': VerifyNotAllowed.N_FAILED_ATTEMPTS,
-             'failure_count': n
+            {
+                'reason': VerifyNotAllowed.N_FAILED_ATTEMPTS,
+                'failure_count': n
             }
 
         where ``n`` is the number of successive failures. See
         :class:`~django_otp.models.VerifyNotAllowed`.
+
         """
-        if (self.throttling_enabled and
-                self.throttling_failure_count > 0 and
-                self.throttling_failure_timestamp is not None):
+        if (
+            self.throttling_enabled
+            and self.throttling_failure_count > 0
+            and self.throttling_failure_timestamp is not None
+        ):
             now = timezone.now()
             delay = (now - self.throttling_failure_timestamp).total_seconds()
             # Required delays should be 1, 2, 4, 8 ...
-            delay_required = self.get_throttle_factor() * (2 ** (self.throttling_failure_count - 1))
+            delay_required = self.get_throttle_factor() * (
+                2 ** (self.throttling_failure_count - 1)
+            )
             if delay < delay_required:
-                return (False,
-                        {'reason': VerifyNotAllowed.N_FAILED_ATTEMPTS,
-                         'failure_count': self.throttling_failure_count,
-                         'locked_until': self.throttling_failure_timestamp + timedelta(seconds=delay_required)}
-                        )
+                return (
+                    False,
+                    {
+                        'reason': VerifyNotAllowed.N_FAILED_ATTEMPTS,
+                        'failure_count': self.throttling_failure_count,
+                        'locked_until': self.throttling_failure_timestamp
+                        + timedelta(seconds=delay_required),
+                    },
+                )
 
         return super().verify_is_allowed()
 
     def throttle_reset(self, commit=True):
         """
         Call this method to reset throttling (normally when a verify attempt
         succeeded).
@@ -347,11 +385,23 @@
             self.save()
 
     @cached_property
     def throttling_enabled(self):
         return self.get_throttle_factor() > 0
 
     def get_throttle_factor(self):  # pragma: no cover
+        """
+        This must be implemented to return the throttle factor.
+
+        The number of seconds required between verification attempts will be
+        :math:`c2^{n-1}` where `c` is this factor and `n` is the number of
+        previous failures. A factor of 1 translates to delays of 1, 2, 4, 8,
+        etc. seconds. A factor of 0 disables the throttling.
+
+        Normally this is just a wrapper for a plugin-specific setting like
+        :setting:`OTP_EMAIL_THROTTLE_FACTOR`.
+
+        """
         raise NotImplementedError()
 
     class Meta:
         abstract = True
```

### Comparing `django-otp-1.1.6/src/django_otp/oath.py` & `django_otp-1.2.0/src/django_otp/oath.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,21 @@
     399871
     520489
     """
     msg = pack(b'>Q', counter)
     hs = hmac.new(key, msg, sha1).digest()
     hs = list(iter(hs))
 
-    offset = hs[19] & 0x0f
-    bin_code = (hs[offset] & 0x7f) << 24 | hs[offset + 1] << 16 | hs[offset + 2] << 8 | hs[offset + 3]
+    offset = hs[19] & 0x0F
+    bin_code = (
+        (hs[offset] & 0x7F) << 24
+        | hs[offset + 1] << 16
+        | hs[offset + 2] << 8
+        | hs[offset + 3]
+    )
     hotp = bin_code % pow(10, digits)
 
     return hotp
 
 
 def totp(key, step=30, t0=0, digits=6, drift=0):
     """
@@ -121,28 +126,29 @@
     >>> del totp.time
     >>> totp.t0 = int(time()) - 60
     >>> totp.t()
     2
     >>> totp.token()
     359152
     """
+
     def __init__(self, key, step=30, t0=0, digits=6, drift=0):
         self.key = key
         self.step = step
         self.t0 = t0
         self.digits = digits
         self.drift = drift
         self._time = None
 
     def token(self):
-        """ The computed TOTP token. """
+        """The computed TOTP token."""
         return hotp(self.key, self.t(), digits=self.digits)
 
     def t(self):
-        """ The computed time step. """
+        """The computed time step."""
         return ((int(self.time) - self.t0) // self.step) + self.drift
 
     @property
     def time(self):
         """
         The current time.
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_email/admin.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_email/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,28 @@
 
 
 class EmailDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~django_otp.plugins.otp_email.models.EmailDevice`.
     """
+
     fieldsets = [
-        ('Identity', {
-            'fields': ['user', 'name', 'confirmed'],
-        }),
-        ('Configuration', {
-            'fields': ['email'],
-        }),
+        (
+            'Identity',
+            {
+                'fields': ['user', 'name', 'confirmed'],
+            },
+        ),
+        (
+            'Configuration',
+            {
+                'fields': ['email'],
+            },
+        ),
     ]
     raw_id_fields = ['user']
 
 
 # Somehow this is getting imported twice, triggering a useless exception.
 try:
     admin.site.register(EmailDevice, EmailDeviceAdmin)
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_email/conf.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_email/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     """
     This is a simple class to take the place of the global settings object.
 
     An instance will contain all of our settings as attributes, with default
     values if they are not specified by the configuration.
 
     """
+
     defaults = {
         'OTP_EMAIL_SENDER': None,
         'OTP_EMAIL_SUBJECT': 'OTP token',
         'OTP_EMAIL_BODY_TEMPLATE': None,
         'OTP_EMAIL_BODY_TEMPLATE_PATH': 'otp/email/token.txt',
         'OTP_EMAIL_TOKEN_VALIDITY': 300,
         'OTP_EMAIL_THROTTLE_FACTOR': 1,
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/0001_initial.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_email/migrations/0004_throttling.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_email/models.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_email/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from django_otp.models import SideChannelDevice, ThrottlingMixin
 from django_otp.util import hex_validator, random_hex
 
 from .conf import settings
 
 
 def default_key():  # pragma: no cover
-    """ Obsolete code here for migrations. """
+    """Obsolete code here for migrations."""
     return random_hex(20)
 
 
 def key_validator(value):  # pragma: no cover
-    """ Obsolete code here for migrations. """
+    """Obsolete code here for migrations."""
     return hex_validator()(value)
 
 
 class EmailDevice(ThrottlingMixin, SideChannelDevice):
     """
     A :class:`~django_otp.models.SideChannelDevice` that delivers a token to
     the email address saved in this object or alternatively to the user's
@@ -33,19 +33,20 @@
     e.g., requiring the user to re-verify their email address on new devices.
 
     .. attribute:: email
 
         *EmailField*: An alternative email address to send the tokens to.
 
     """
+
     email = models.EmailField(
         max_length=254,
         blank=True,
         null=True,
-        help_text='Optional alternative email address to send tokens to'
+        help_text='Optional alternative email address to send tokens to',
     )
 
     def get_throttle_factor(self):
         return settings.OTP_EMAIL_THROTTLE_FACTOR
 
     def generate_challenge(self, extra_context=None):
         """
@@ -60,18 +61,20 @@
 
         context = {'token': self.token, **(extra_context or {})}
         if settings.OTP_EMAIL_BODY_TEMPLATE:
             body = Template(settings.OTP_EMAIL_BODY_TEMPLATE).render(Context(context))
         else:
             body = get_template(settings.OTP_EMAIL_BODY_TEMPLATE_PATH).render(context)
 
-        send_mail(str(settings.OTP_EMAIL_SUBJECT),
-                  body,
-                  settings.OTP_EMAIL_SENDER,
-                  [self.email or self.user.email])
+        send_mail(
+            str(settings.OTP_EMAIL_SUBJECT),
+            body,
+            settings.OTP_EMAIL_SENDER,
+            [self.email or self.user.email],
+        )
 
         message = "sent by email"
 
         return message
 
     def verify_token(self, token):
         verify_allowed, _ = self.verify_is_allowed()
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_email/tests.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_email/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,17 @@
         self.assertEqual(len(mail.outbox), 1)
 
         msg = mail.outbox[0]
 
         with self.subTest(field='from_email'):
             self.assertEqual(msg.from_email, "root@localhost")
         with self.subTest(field='body'):
-            self.assertEqual(msg.body, "Test template 1: {}\n".format(self.device.token))
+            self.assertEqual(
+                msg.body, "Test template 1: {}\n".format(self.device.token)
+            )
 
     @override_settings(
         OTP_EMAIL_SENDER="webmaster@example.com",
         OTP_EMAIL_SUBJECT="Test subject",
         OTP_EMAIL_BODY_TEMPLATE="Test template 2: {{token}}",
     )
     def test_settings(self):
@@ -126,15 +128,17 @@
         msg = mail.outbox[0]
 
         with self.subTest(field='from_email'):
             self.assertEqual(msg.from_email, "webmaster@example.com")
         with self.subTest(field='subject'):
             self.assertEqual(msg.subject, "Test subject")
         with self.subTest(field='body'):
-            self.assertEqual(msg.body, "Test template 3: {}\n".format(self.device.token))
+            self.assertEqual(
+                msg.body, "Test template 3: {}\n".format(self.device.token)
+            )
 
     @override_settings(
         OTP_EMAIL_SENDER="webmaster@example.com",
         OTP_EMAIL_SUBJECT="Test subject",
         OTP_EMAIL_BODY_TEMPLATE="Test template 4: {{token}} {{foo}} {{bar}}",
     )
     def test_settings_extra_template_options(self):
@@ -148,15 +152,17 @@
         with self.subTest(field='from_email'):
             self.assertEqual(msg.from_email, "webmaster@example.com")
         with self.subTest(field='subject'):
             self.assertEqual(msg.subject, "Test subject")
         with self.subTest(field='body'):
             self.assertEqual(
                 msg.body,
-                "Test template 4: {} {} {}".format(self.device.token, extra_context["foo"], extra_context["bar"])
+                "Test template 4: {} {} {}".format(
+                    self.device.token, extra_context["foo"], extra_context["bar"]
+                ),
             )
 
     def test_alternative_email(self):
         self.device.email = 'alice2@example.com'
         self.device.save()
 
         self.device.generate_challenge()
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_hotp/admin.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 class HOTPDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~django_otp.plugins.otp_hotp.models.HOTPDevice`.
     """
+
     list_display = ['user', 'name', 'confirmed']
 
     raw_id_fields = ['user']
     readonly_fields = ['qrcode_link']
     radio_fields = {'digits': admin.HORIZONTAL}
 
     def get_list_display(self, request):
@@ -32,34 +33,52 @@
         # Show the key value only for adding new objects or when sensitive data
         # is not hidden.
         if settings.OTP_ADMIN_HIDE_SENSITIVE_DATA and obj:
             configuration_fields = ['digits', 'tolerance']
         else:
             configuration_fields = ['key', 'digits', 'tolerance']
         fieldsets = [
-            ('Identity', {
-                'fields': ['user', 'name', 'confirmed'],
-            }),
-            ('Configuration', {
-                'fields': configuration_fields,
-            }),
-            ('State', {
-                'fields': ['counter'],
-            }),
-            ('Throttling', {
-                'fields': ['throttling_failure_timestamp', 'throttling_failure_count'],
-            }),
+            (
+                'Identity',
+                {
+                    'fields': ['user', 'name', 'confirmed'],
+                },
+            ),
+            (
+                'Configuration',
+                {
+                    'fields': configuration_fields,
+                },
+            ),
+            (
+                'State',
+                {
+                    'fields': ['counter'],
+                },
+            ),
+            (
+                'Throttling',
+                {
+                    'fields': [
+                        'throttling_failure_timestamp',
+                        'throttling_failure_count',
+                    ],
+                },
+            ),
         ]
         # Show the QR code link only for existing objects when sensitive data
         # is not hidden.
         if not settings.OTP_ADMIN_HIDE_SENSITIVE_DATA and obj:
             fieldsets.append(
-                (None, {
-                    'fields': ['qrcode_link'],
-                }),
+                (
+                    None,
+                    {
+                        'fields': ['qrcode_link'],
+                    },
+                ),
             )
         return fieldsets
 
     def get_queryset(self, request):
         queryset = super().get_queryset(request)
         queryset = queryset.select_related('user')
 
@@ -73,24 +92,33 @@
         try:
             href = reverse('admin:otp_hotp_hotpdevice_config', kwargs={'pk': device.pk})
             link = format_html('<a href="{}">qrcode</a>', href)
         except Exception:
             link = ''
 
         return link
+
     qrcode_link.short_description = "QR Code"
 
     #
     # Custom views
     #
 
     def get_urls(self):
         urls = [
-            path('<int:pk>/config/', self.admin_site.admin_view(self.config_view), name='otp_hotp_hotpdevice_config'),
-            path('<int:pk>/qrcode/', self.admin_site.admin_view(self.qrcode_view), name='otp_hotp_hotpdevice_qrcode'),
+            path(
+                '<int:pk>/config/',
+                self.admin_site.admin_view(self.config_view),
+                name='otp_hotp_hotpdevice_config',
+            ),
+            path(
+                '<int:pk>/qrcode/',
+                self.admin_site.admin_view(self.qrcode_view),
+                name='otp_hotp_hotpdevice_qrcode',
+            ),
         ] + super().get_urls()
 
         return urls
 
     def config_view(self, request, pk):
         if settings.OTP_ADMIN_HIDE_SENSITIVE_DATA:
             raise PermissionDenied()
@@ -114,15 +142,17 @@
         if not self.has_view_or_change_permission(request, device):
             raise PermissionDenied()
 
         try:
             import qrcode
             import qrcode.image.svg
 
-            img = qrcode.make(device.config_url, image_factory=qrcode.image.svg.SvgImage)
+            img = qrcode.make(
+                device.config_url, image_factory=qrcode.image.svg.SvgImage
+            )
             response = HttpResponse(content_type='image/svg+xml')
             img.save(response)
         except ImportError:
             response = HttpResponse('', status=503)
 
         return response
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_hotp/models.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,18 +40,32 @@
         (Default: 5)
 
     .. attribute:: counter
 
         *BigIntegerField*: The next counter value to expect. (Initial: 0)
 
     """
-    key = models.CharField(max_length=80, validators=[key_validator], default=default_key, help_text="A hex-encoded secret key of up to 40 bytes.")
-    digits = models.PositiveSmallIntegerField(choices=[(6, 6), (8, 8)], default=6, help_text="The number of digits to expect in a token.")
-    tolerance = models.PositiveSmallIntegerField(default=5, help_text="The number of missed tokens to tolerate.")
-    counter = models.BigIntegerField(default=0, help_text="The next counter value to expect.")
+
+    key = models.CharField(
+        max_length=80,
+        validators=[key_validator],
+        default=default_key,
+        help_text="A hex-encoded secret key of up to 40 bytes.",
+    )
+    digits = models.PositiveSmallIntegerField(
+        choices=[(6, 6), (8, 8)],
+        default=6,
+        help_text="The number of digits to expect in a token.",
+    )
+    tolerance = models.PositiveSmallIntegerField(
+        default=5, help_text="The number of missed tokens to tolerate."
+    )
+    counter = models.BigIntegerField(
+        default=0, help_text="The next counter value to expect."
+    )
 
     class Meta(Device.Meta):
         verbose_name = "HOTP device"
 
     @property
     def bin_key(self):
         """
@@ -109,12 +123,14 @@
 
         issuer = getattr(settings, 'OTP_HOTP_ISSUER', None)
         if callable(issuer):
             issuer = issuer(self)
         if isinstance(issuer, str) and (issuer != ''):
             issuer = issuer.replace(':', '')
             label = '{}:{}'.format(issuer, label)
-            urlencoded_params += '&issuer={}'.format(quote(issuer))  # encode issuer as per RFC 3986, not quote_plus
+            urlencoded_params += '&issuer={}'.format(
+                quote(issuer)
+            )  # encode issuer as per RFC 3986, not quote_plus
 
         url = 'otpauth://hotp/{}?{}'.format(quote(label), urlencoded_params)
 
         return url
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html` & `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_hotp/tests.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,27 @@
 from .models import HOTPDevice
 
 
 class HOTPDeviceMixin:
     """
     A TestCase helper that gives us a HOTPDevice to work with.
     """
+
     # The next three tokens
     tokens = [782373, 313268, 307722]
     key = 'd2e8a68036f68960b1c30532bb6c56da5934d879'
 
     def setUp(self):
         try:
-            alice = self.create_user(
-                'alice', 'password', email='alice@example.com')
+            alice = self.create_user('alice', 'password', email='alice@example.com')
         except IntegrityError:
             self.skipTest("Unable to create test user.")
         else:
             self.device = alice.hotpdevice_set.create(
-                key=self.key, digits=6,
-                tolerance=1, counter=0
+                key=self.key, digits=6, tolerance=1, counter=0
             )
 
 
 @override_settings(
     OTP_HOTP_THROTTLE_FACTOR=0,
 )
 class HOTPTest(HOTPDeviceMixin, TestCase):
@@ -124,26 +123,26 @@
         self.assertEqual(params['issuer'][0], 'alice@example.com')
 
 
 class AuthFormTest(TestCase):
     """
     Test auth form with HOTP tokens
     """
+
     tokens = HOTPTest.tokens
     key = HOTPTest.key
 
     def setUp(self):
         try:
             alice = self.create_user('alice', 'password')
         except IntegrityError:
             self.skipTest("Unable to create test user.")
         else:
             self.device = alice.hotpdevice_set.create(
-                key=self.key, digits=6,
-                tolerance=1, counter=0
+                key=self.key, digits=6, tolerance=1, counter=0
             )
 
     def test_no_token(self):
         data = {
             'username': 'alice',
             'password': 'password',
             'otp_device': self.device.persistent_id,
@@ -190,87 +189,102 @@
         with freeze_time() as frozen_time:
             form1 = OTPAuthenticationForm(None, bad_data)
             self.assertFalse(form1.is_valid())
 
             # Should fail even with good data:
             form2 = OTPAuthenticationForm(None, good_data)
             self.assertFalse(form2.is_valid())
-            self.assertIn('Verification temporarily disabled because of 1 failed attempt', form2.errors['__all__'][0])
+            self.assertIn(
+                'Verification temporarily disabled because of 1 failed attempt',
+                form2.errors['__all__'][0],
+            )
 
             # Fail again after throttling expired:
             frozen_time.tick(timedelta(seconds=1.1))
             form3 = OTPAuthenticationForm(None, bad_data)
             self.assertFalse(form3.is_valid())
             self.assertIn('Invalid token', form3.errors['__all__'][0])
 
             # Test n=2 error message:
             form4 = OTPAuthenticationForm(None, bad_data)
             self.assertFalse(form4.is_valid())
-            self.assertIn('Verification temporarily disabled because of 2 failed attempts', form4.errors['__all__'][0])
+            self.assertIn(
+                'Verification temporarily disabled because of 2 failed attempts',
+                form4.errors['__all__'][0],
+            )
 
             # Pass this time:
             frozen_time.tick(timedelta(seconds=2.1))
             form5 = OTPAuthenticationForm(None, good_data)
             self.assertTrue(form5.is_valid())
 
 
 class HOTPAdminTest(TestCase):
     def setUp(self):
         """
         Create a device at the fourth time step. The current token is 154567.
         """
         try:
             self.admin = self.create_user(
-                'admin', 'password', email='admin@example.com',
-                is_staff=True
+                'admin', 'password', email='admin@example.com', is_staff=True
             )
         except IntegrityError:
             self.skipTest("Unable to create test user.")
         else:
             self.device = self.admin.hotpdevice_set.create(
-                key='d2e8a68036f68960b1c30532bb6c56da5934d879', digits=6,
-                tolerance=1, counter=0
+                key='d2e8a68036f68960b1c30532bb6c56da5934d879',
+                digits=6,
+                tolerance=1,
+                counter=0,
             )
         self.device_admin = HOTPDeviceAdmin(HOTPDevice, AdminSite())
         self.get_request = RequestFactory().get('/')
         self.get_request.user = self.admin
 
     def test_anonymous(self):
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 302)
 
     def test_unauthorized(self):
         self.client.login(username='admin', password='password')
 
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 403)
 
     def test_view_perm(self):
         self._add_device_perms('view_hotpdevice')
         self.client.login(username='admin', password='password')
 
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 200)
 
     def test_change_perm(self):
         self._add_device_perms('change_hotpdevice')
         self.client.login(username='admin', password='password')
 
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_hotp_hotpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 200)
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=True)
     def test_sensitive_information_hidden_while_adding_device(self):
         fields = self._get_fields(device=None)
         self.assertIn('key', fields)
@@ -345,15 +359,17 @@
         ]
 
         self.admin.user_permissions.add(*perms)
 
     def _get_fields(self, device):
         return {
             field
-            for fieldset in self.device_admin.get_fieldsets(self.get_request, obj=device)
+            for fieldset in self.device_admin.get_fieldsets(
+                self.get_request, obj=device
+            )
             for field in fieldset[1]['fields']
         }
 
 
 @override_settings(
     OTP_HOTP_THROTTLE_FACTOR=1,
 )
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_static/admin.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_static/admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 
 
 class StaticDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~django_otp.plugins.otp_static.models.StaticDevice`.
     """
+
     fieldsets = [
-        ('Identity', {
-            'fields': ['user', 'name', 'confirmed'],
-        }),
+        (
+            'Identity',
+            {
+                'fields': ['user', 'name', 'confirmed'],
+            },
+        ),
     ]
     raw_id_fields = ['user']
 
     inlines = [
         StaticTokenInline,
     ]
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_static/lib.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_static/lib.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     This is the implementation for the management command of a similar name.
     Returns the StaticToken object created.
 
     """
     user = get_user_model().objects.get_by_natural_key(username)
 
-    device = next(StaticDevice.objects.filter(user=user).iterator(), None)
+    device = StaticDevice.objects.filter(user=user).first()
     if device is None:
         device = StaticDevice.objects.create(user=user, name='Backup Code')
 
     if token is None:
         token = StaticToken.random_token()
 
     return device.token_set.create(token=token)
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,31 @@
 from django.core.management.base import BaseCommand, CommandError
 from django.utils.encoding import force_str
 
 from django_otp.plugins.otp_static.lib import add_static_token, get_user_model
 
 
 class Command(BaseCommand):
-    help = fill('Adds a single static OTP token to the given user. '
-                'The token will be added to an arbitrary static device '
-                'attached to the user, creating one if necessary.', width=78)
+    help = fill(
+        'Adds a single static OTP token to the given user. '
+        'The token will be added to an arbitrary static device '
+        'attached to the user, creating one if necessary.',
+        width=78,
+    )
 
     def add_arguments(self, parser):
-        parser.add_argument('-t', '--token', dest='token', help='The token to add. If omitted, one will be randomly generated.')
-        parser.add_argument('username', help='The user to which the token will be assigned.')
+        parser.add_argument(
+            '-t',
+            '--token',
+            dest='token',
+            help='The token to add. If omitted, one will be randomly generated.',
+        )
+        parser.add_argument(
+            'username', help='The user to which the token will be assigned.'
+        )
 
     def handle(self, *args, **options):
         username = options['username']
 
         try:
             statictoken = add_static_token(username, options.get('token'))
         except get_user_model().DoesNotExist:
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_static/migrations/0001_initial.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_static/migrations/0002_throttling.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_static/models.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_static/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     :class:`StaticToken` objects.
 
     .. attribute:: token_set
 
         The RelatedManager for our tokens.
 
     """
+
     def get_throttle_factor(self):
         return getattr(settings, 'OTP_STATIC_THROTTLE_FACTOR', 1)
 
     def verify_token(self, token):
         verify_allowed, _ = self.verify_is_allowed()
         if verify_allowed:
             match = self.token_set.filter(token=token).first()
@@ -35,30 +36,33 @@
                 match.delete()
                 self.throttle_reset()
             else:
                 self.throttle_increment()
         else:
             match = None
 
-        return (match is not None)
+        return match is not None
 
 
 class StaticToken(models.Model):
     """
     A single token belonging to a :class:`StaticDevice`.
 
     .. attribute:: device
 
         *ForeignKey*: A foreign key to :class:`StaticDevice`.
 
     .. attribute:: token
 
         *CharField*: A random string up to 16 characters.
     """
-    device = models.ForeignKey(StaticDevice, related_name='token_set', on_delete=models.CASCADE)
+
+    device = models.ForeignKey(
+        StaticDevice, related_name='token_set', on_delete=models.CASCADE
+    )
     token = models.CharField(max_length=16, db_index=True)
 
     @staticmethod
     def random_token():
         """
         Returns a new random string that can be used as a static token.
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_static/tests.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_static/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from .admin import StaticDeviceAdmin, StaticTokenInline
 from .lib import add_static_token
 from .models import StaticDevice, StaticToken
 
 
 class DeviceTest(TestCase):
-    """ A few generic tests to get us started. """
+    """A few generic tests to get us started."""
+
     def setUp(self):
         try:
             self.user = self.create_user('alice', 'password')
         except Exception:
             self.skipTest("Unable to create the test user.")
 
     def test_str(self):
@@ -32,14 +33,15 @@
         str(device)
 
 
 class LibTest(TestCase):
     """
     Test miscellaneous library functions.
     """
+
     def setUp(self):
         try:
             self.user = self.create_user('alice', 'password')
         except Exception:
             self.skipTest("Unable to create the test user.")
 
     def test_add_static_token(self):
@@ -69,14 +71,15 @@
 class AuthFormTest(TestCase):
     """
     Test the auth form with static tokens.
 
     We try to honor custom user models, but if we can't create users, we'll
     skip the tests.
     """
+
     def setUp(self):
         for device_id, username in enumerate(['alice', 'bob']):
             try:
                 user = self.create_user(username, 'password')
             except IntegrityError:
                 self.skipTest("Unable to create a test user.")
             else:
@@ -211,22 +214,26 @@
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=True)
     def test_inline_instances_when_sensitive_information_hidden(self):
         self._add_device_perms('change_statictoken')
         instances = self.device_admin.get_inline_instances(self.get_request, obj=None)
         self.assertIsInstance(instances, list)
         self.assertEqual(len(instances), 1)
         self.assertIsInstance(instances[0], StaticTokenInline)
-        instances = self.device_admin.get_inline_instances(self.get_request, obj=self.device)
+        instances = self.device_admin.get_inline_instances(
+            self.get_request, obj=self.device
+        )
         self.assertEqual(instances, [])
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=False)
     def test_inline_instances_when_sensitive_information_shown(self):
         self._add_device_perms('change_statictoken')
         for obj in (None, self.device):
-            instances = self.device_admin.get_inline_instances(self.get_request, obj=obj)
+            instances = self.device_admin.get_inline_instances(
+                self.get_request, obj=obj
+            )
             self.assertIsInstance(instances, list)
             self.assertEqual(len(instances), 1)
 
     #
     # Helpers
     #
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_totp/admin.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_totp/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 class TOTPDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~django_otp.plugins.otp_totp.models.TOTPDevice`.
     """
+
     list_display = ['user', 'name', 'confirmed']
 
     raw_id_fields = ['user']
     readonly_fields = ['qrcode_link']
     radio_fields = {'digits': admin.HORIZONTAL}
 
     def get_list_display(self, request):
@@ -32,34 +33,52 @@
         # Show the key value only for adding new objects or when sensitive data
         # is not hidden.
         if settings.OTP_ADMIN_HIDE_SENSITIVE_DATA and obj:
             configuration_fields = ['step', 't0', 'digits', 'tolerance']
         else:
             configuration_fields = ['key', 'step', 't0', 'digits', 'tolerance']
         fieldsets = [
-            ('Identity', {
-                'fields': ['user', 'name', 'confirmed'],
-            }),
-            ('Configuration', {
-                'fields': configuration_fields,
-            }),
-            ('State', {
-                'fields': ['drift'],
-            }),
-            ('Throttling', {
-                'fields': ['throttling_failure_timestamp', 'throttling_failure_count'],
-            }),
+            (
+                'Identity',
+                {
+                    'fields': ['user', 'name', 'confirmed'],
+                },
+            ),
+            (
+                'Configuration',
+                {
+                    'fields': configuration_fields,
+                },
+            ),
+            (
+                'State',
+                {
+                    'fields': ['drift'],
+                },
+            ),
+            (
+                'Throttling',
+                {
+                    'fields': [
+                        'throttling_failure_timestamp',
+                        'throttling_failure_count',
+                    ],
+                },
+            ),
         ]
         # Show the QR code link only for existing objects when sensitive data
         # is not hidden.
         if not settings.OTP_ADMIN_HIDE_SENSITIVE_DATA and obj:
             fieldsets.append(
-                (None, {
-                    'fields': ['qrcode_link'],
-                }),
+                (
+                    None,
+                    {
+                        'fields': ['qrcode_link'],
+                    },
+                ),
             )
         return fieldsets
 
     def get_queryset(self, request):
         queryset = super().get_queryset(request)
         queryset = queryset.select_related('user')
 
@@ -73,24 +92,33 @@
         try:
             href = reverse('admin:otp_totp_totpdevice_config', kwargs={'pk': device.pk})
             link = format_html('<a href="{}">qrcode</a>', href)
         except Exception:
             link = ''
 
         return link
+
     qrcode_link.short_description = "QR Code"
 
     #
     # Custom views
     #
 
     def get_urls(self):
         urls = [
-            path('<int:pk>/config/', self.admin_site.admin_view(self.config_view), name='otp_totp_totpdevice_config'),
-            path('<int:pk>/qrcode/', self.admin_site.admin_view(self.qrcode_view), name='otp_totp_totpdevice_qrcode'),
+            path(
+                '<int:pk>/config/',
+                self.admin_site.admin_view(self.config_view),
+                name='otp_totp_totpdevice_config',
+            ),
+            path(
+                '<int:pk>/qrcode/',
+                self.admin_site.admin_view(self.qrcode_view),
+                name='otp_totp_totpdevice_qrcode',
+            ),
         ] + super().get_urls()
 
         return urls
 
     def config_view(self, request, pk):
         if settings.OTP_ADMIN_HIDE_SENSITIVE_DATA:
             raise PermissionDenied()
@@ -114,15 +142,17 @@
         if not self.has_view_or_change_permission(request, device):
             raise PermissionDenied()
 
         try:
             import qrcode
             import qrcode.image.svg
 
-            img = qrcode.make(device.config_url, image_factory=qrcode.image.svg.SvgImage)
+            img = qrcode.make(
+                device.config_url, image_factory=qrcode.image.svg.SvgImage
+            )
             response = HttpResponse(content_type='image/svg+xml')
             img.save(response)
         except ImportError:
             response = HttpResponse('', status=503)
 
         return response
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_totp/migrations/0001_initial.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_totp/models.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_totp/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,21 +62,43 @@
 
         *BigIntegerField*: The time step of the last verified token. To avoid
         verifying the same token twice, this will be updated on each successful
         verification. Only tokens at a higher time step will be verified
         subsequently. (Default: -1)
 
     """
-    key = models.CharField(max_length=80, validators=[key_validator], default=default_key, help_text="A hex-encoded secret key of up to 40 bytes.")
-    step = models.PositiveSmallIntegerField(default=30, help_text="The time step in seconds.")
-    t0 = models.BigIntegerField(default=0, help_text="The Unix time at which to begin counting steps.")
-    digits = models.PositiveSmallIntegerField(choices=[(6, 6), (8, 8)], default=6, help_text="The number of digits to expect in a token.")
-    tolerance = models.PositiveSmallIntegerField(default=1, help_text="The number of time steps in the past or future to allow.")
-    drift = models.SmallIntegerField(default=0, help_text="The number of time steps the prover is known to deviate from our clock.")
-    last_t = models.BigIntegerField(default=-1, help_text="The t value of the latest verified token. The next token must be at a higher time step.")
+
+    key = models.CharField(
+        max_length=80,
+        validators=[key_validator],
+        default=default_key,
+        help_text="A hex-encoded secret key of up to 40 bytes.",
+    )
+    step = models.PositiveSmallIntegerField(
+        default=30, help_text="The time step in seconds."
+    )
+    t0 = models.BigIntegerField(
+        default=0, help_text="The Unix time at which to begin counting steps."
+    )
+    digits = models.PositiveSmallIntegerField(
+        choices=[(6, 6), (8, 8)],
+        default=6,
+        help_text="The number of digits to expect in a token.",
+    )
+    tolerance = models.PositiveSmallIntegerField(
+        default=1, help_text="The number of time steps in the past or future to allow."
+    )
+    drift = models.SmallIntegerField(
+        default=0,
+        help_text="The number of time steps the prover is known to deviate from our clock.",
+    )
+    last_t = models.BigIntegerField(
+        default=-1,
+        help_text="The t value of the latest verified token. The next token must be at a higher time step.",
+    )
 
     class Meta(Device.Meta):
         verbose_name = "TOTP device"
 
     @property
     def bin_key(self):
         """
@@ -120,29 +142,42 @@
     @property
     def config_url(self):
         """
         A URL for configuring Google Authenticator or similar.
 
         See https://github.com/google/google-authenticator/wiki/Key-Uri-Format.
         The issuer is taken from :setting:`OTP_TOTP_ISSUER`, if available.
+        The image (for e.g. FreeOTP) is taken from :setting:`OTP_TOTP_IMAGE`, if available.
 
         """
         label = str(self.user.get_username())
         params = {
             'secret': b32encode(self.bin_key),
             'algorithm': 'SHA1',
             'digits': self.digits,
             'period': self.step,
         }
         urlencoded_params = urlencode(params)
 
-        issuer = getattr(settings, 'OTP_TOTP_ISSUER', None)
-        if callable(issuer):
-            issuer = issuer(self)
-        if isinstance(issuer, str) and (issuer != ''):
+        issuer = self._read_str_from_settings('OTP_TOTP_ISSUER')
+        if issuer:
             issuer = issuer.replace(':', '')
             label = '{}:{}'.format(issuer, label)
-            urlencoded_params += '&issuer={}'.format(quote(issuer))  # encode issuer as per RFC 3986, not quote_plus
+            urlencoded_params += '&issuer={}'.format(
+                quote(issuer)
+            )  # encode issuer as per RFC 3986, not quote_plus
+
+        image = self._read_str_from_settings('OTP_TOTP_IMAGE')
+        if image:
+            urlencoded_params += "&image={}".format(quote(image, safe=':/'))
 
         url = 'otpauth://totp/{}?{}'.format(quote(label), urlencoded_params)
 
         return url
+
+    def _read_str_from_settings(self, key):
+        val = getattr(settings, key, None)
+        if callable(val):
+            val = val(self)
+        if isinstance(val, str) and (val != ''):
+            return val
+        return None
```

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html` & `django_otp-1.2.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/plugins/otp_totp/tests.py` & `django_otp-1.2.0/src/django_otp/plugins/otp_totp/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,47 @@
 from .models import TOTPDevice
 
 
 class TOTPDeviceMixin:
     """
     A TestCase helper that gives us a TOTPDevice to work with.
     """
+
     # The next ten tokens
-    tokens = [179225, 656163, 839400, 154567, 346912, 471576, 45675, 101397, 491039, 784503]
+    tokens = [
+        179225,
+        656163,
+        839400,
+        154567,
+        346912,
+        471576,
+        45675,
+        101397,
+        491039,
+        784503,
+    ]
 
     def setUp(self):
         """
         Create a device at the fourth time step. The current token is 154567.
         """
         try:
             self.alice = self.create_user(
-                'alice', 'password', email='alice@example.com')
+                'alice', 'password', email='alice@example.com'
+            )
         except IntegrityError:
             self.skipTest("Unable to create the test user.")
         else:
             self.device = self.alice.totpdevice_set.create(
-                key='2a2bbba1092ffdd25a328ad1a0a5f5d61d7aacc4', step=30,
-                t0=int(time() - (30 * 3)), digits=6, tolerance=0, drift=0
+                key='2a2bbba1092ffdd25a328ad1a0a5f5d61d7aacc4',
+                step=30,
+                t0=int(time() - (30 * 3)),
+                digits=6,
+                tolerance=0,
+                drift=0,
             )
 
 
 @override_settings(
     OTP_TOTP_SYNC=False,
     OTP_TOTP_THROTTLE_FACTOR=0,
 )
@@ -135,69 +152,95 @@
         self.assertEqual(parsed.scheme, 'otpauth')
         self.assertEqual(parsed.netloc, 'totp')
         self.assertEqual(parsed.path, '/alice%40example.com%3Aalice')
         self.assertIn('secret', params)
         self.assertIn('issuer', params)
         self.assertEqual(params['issuer'][0], 'alice@example.com')
 
+    def test_config_url_image(self):
+        image_url = "https://test.invalid/square.png"
+
+        with override_settings(OTP_TOTP_ISSUER=None, OTP_TOTP_IMAGE=image_url):
+            url = self.device.config_url
+
+        parsed = urlsplit(url)
+        params = parse_qs(parsed.query)
+
+        self.assertEqual(parsed.scheme, 'otpauth')
+        self.assertEqual(parsed.netloc, 'totp')
+        self.assertEqual(parsed.path, '/alice')
+        self.assertIn('secret', params)
+        self.assertEqual(params['image'][0], image_url)
+
 
 class TOTPAdminTest(TestCase):
     def setUp(self):
         """
         Create a device at the fourth time step. The current token is 154567.
         """
         try:
             self.admin = self.create_user(
-                'admin', 'password', email='admin@example.com',
-                is_staff=True
+                'admin', 'password', email='admin@example.com', is_staff=True
             )
         except IntegrityError:
             self.skipTest("Unable to create the test user.")
         else:
             self.device = self.admin.totpdevice_set.create(
-                key='2a2bbba1092ffdd25a328ad1a0a5f5d61d7aacc4', step=30,
-                t0=int(time() - (30 * 3)), digits=6, tolerance=0, drift=0
+                key='2a2bbba1092ffdd25a328ad1a0a5f5d61d7aacc4',
+                step=30,
+                t0=int(time() - (30 * 3)),
+                digits=6,
+                tolerance=0,
+                drift=0,
             )
         self.device_admin = TOTPDeviceAdmin(TOTPDevice, AdminSite())
         self.get_request = RequestFactory().get('/')
         self.get_request.user = self.admin
 
     def test_anonymous(self):
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 302)
 
     def test_unauthorized(self):
         self.client.login(username='admin', password='password')
 
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 403)
 
     def test_view_perm(self):
         self._add_device_perms('view_totpdevice')
         self.client.login(username='admin', password='password')
 
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 200)
 
     def test_change_perm(self):
         self._add_device_perms('change_totpdevice')
         self.client.login(username='admin', password='password')
 
         for suffix in ['config', 'qrcode']:
             with self.subTest(view=suffix):
-                url = reverse('admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk})
+                url = reverse(
+                    'admin:otp_totp_totpdevice_' + suffix, kwargs={'pk': self.device.pk}
+                )
                 response = self.client.get(url)
                 self.assertEqual(response.status_code, 200)
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=True)
     def test_sensitive_information_hidden_while_adding_device(self):
         fields = self._get_fields(device=None)
         self.assertIn('key', fields)
@@ -272,15 +315,17 @@
         ]
 
         self.admin.user_permissions.add(*perms)
 
     def _get_fields(self, device):
         return {
             field
-            for fieldset in self.device_admin.get_fieldsets(self.get_request, obj=device)
+            for fieldset in self.device_admin.get_fieldsets(
+                self.get_request, obj=device
+            )
             for field in fieldset[1]['fields']
         }
 
 
 @override_settings(
     OTP_TOTP_THROTTLE_FACTOR=1,
 )
```

### Comparing `django-otp-1.1.6/src/django_otp/templates/otp/admin111/login.html` & `django_otp-1.2.0/src/django_otp/templates/otp/admin111/login.html`

 * *Files identical despite different names*

### Comparing `django-otp-1.1.6/src/django_otp/tests.py` & `django_otp-1.2.0/src/django_otp/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 from datetime import timedelta
 from doctest import DocTestSuite
+from io import StringIO
 import pickle
 from threading import Thread
 import unittest
 
 from freezegun import freeze_time
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AnonymousUser
+from django.core.management import call_command
+from django.core.management.base import CommandError
 from django.db import IntegrityError, connection
 from django.test import RequestFactory
 from django.test import TestCase as DjangoTestCase
 from django.test import TransactionTestCase as DjangoTransactionTestCase
 from django.test import skipUnlessDBFeature
 from django.test.utils import override_settings
 from django.urls import reverse
 from django.utils import timezone
 
-from django_otp import DEVICE_ID_SESSION_KEY, match_token, oath, user_has_device, util, verify_token
+from django_otp import (
+    DEVICE_ID_SESSION_KEY,
+    match_token,
+    oath,
+    user_has_device,
+    util,
+    verify_token,
+)
 from django_otp.forms import OTPTokenForm
 from django_otp.middleware import OTPMiddleware
 from django_otp.models import VerifyNotAllowed
-from django_otp.plugins.otp_static.models import StaticDevice
+from django_otp.plugins.otp_static.models import StaticDevice, StaticToken
 
 
 def load_tests(loader, tests, pattern):
     suite = unittest.TestSuite()
 
     suite.addTests(tests)
     suite.addTest(DocTestSuite(util))
     suite.addTest(DocTestSuite(oath))
 
     return suite
 
 
 class TestThread(Thread):
     "Django testing quirk: threads have to close their DB connections."
+
     def run(self):
         super().run()
         connection.close()
 
 
 class OTPTestCaseMixin:
     """
     Utilities for dealing with custom user models.
     """
+
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
 
         cls.User = get_user_model()
         cls.USERNAME_FIELD = cls.User.USERNAME_FIELD
 
@@ -78,23 +90,24 @@
     TestCase subclass that includes this as a base class. This will help verify
     a correct integration of ThrottlingMixin.
 
     Subclasses are responsible for populating self.device with a device to test
     as well as implementing methods to generate tokens to test with.
 
     """
+
     def setUp(self):
         self.device = None
 
     def valid_token(self):
-        """ Returns a valid token to pass to our device under test. """
+        """Returns a valid token to pass to our device under test."""
         raise NotImplementedError()
 
     def invalid_token(self):
-        """ Returns an invalid token to pass to our device under test. """
+        """Returns an invalid token to pass to our device under test."""
         raise NotImplementedError()
 
     #
     # Tests
     #
 
     def test_delay_imposed_after_fail(self):
@@ -128,18 +141,22 @@
         self.assertEqual(data1, None)
 
         # After failure, verify is not allowed
         with freeze_time():
             self.device.verify_token(self.invalid_token())
             verify_is_allowed2, data2 = self.device.verify_is_allowed()
             self.assertEqual(verify_is_allowed2, False)
-            self.assertEqual(data2, {'reason': VerifyNotAllowed.N_FAILED_ATTEMPTS,
-                                     'failure_count': 1,
-                                     'locked_until': timezone.now() + timezone.timedelta(seconds=1)
-                                     })
+            self.assertEqual(
+                data2,
+                {
+                    'reason': VerifyNotAllowed.N_FAILED_ATTEMPTS,
+                    'failure_count': 1,
+                    'locked_until': timezone.now() + timezone.timedelta(seconds=1),
+                },
+            )
 
         # After a successful attempt, should be allowed again
         with freeze_time() as frozen_time:
             frozen_time.tick(delta=timedelta(seconds=1.1))
             self.device.verify_token(self.valid_token())
 
             verify_is_allowed3, data3 = self.device.verify_is_allowed()
@@ -199,17 +216,15 @@
 
         self.middleware = OTPMiddleware(lambda r: None)
 
     def test_verified(self):
         request = self.factory.get('/')
         request.user = self.alice
         device = self.alice.staticdevice_set.get()
-        request.session = {
-            DEVICE_ID_SESSION_KEY: device.persistent_id
-        }
+        request.session = {DEVICE_ID_SESSION_KEY: device.persistent_id}
 
         self.middleware(request)
 
         self.assertTrue(request.user.is_verified())
 
     def test_verified_legacy_device_id(self):
         request = self.factory.get('/')
@@ -256,29 +271,25 @@
 
         self.assertFalse(request.user.is_verified())
 
     def test_wrong_user(self):
         request = self.factory.get('/')
         request.user = self.alice
         device = self.bob.staticdevice_set.get()
-        request.session = {
-            DEVICE_ID_SESSION_KEY: device.persistent_id
-        }
+        request.session = {DEVICE_ID_SESSION_KEY: device.persistent_id}
 
         self.middleware(request)
 
         self.assertFalse(request.user.is_verified())
 
     def test_pickling(self):
         request = self.factory.get('/')
         request.user = self.alice
         device = self.alice.staticdevice_set.get()
-        request.session = {
-            DEVICE_ID_SESSION_KEY: device.persistent_id
-        }
+        request.session = {DEVICE_ID_SESSION_KEY: device.persistent_id}
 
         self.middleware(request)
 
         # Should not raise an exception.
         pickle.dumps(request.user)
 
 
@@ -296,69 +307,81 @@
 
     def test_admin_login_template(self):
         response = self.client.get(reverse('otpadmin:login'))
         self.assertContains(response, 'Username:')
         self.assertContains(response, 'Password:')
         self.assertNotContains(response, 'OTP Device:')
         self.assertContains(response, 'OTP Token:')
-        response = self.client.post(reverse('otpadmin:login'), data={
-            'username': self.bob.get_username(),
-            'password': 'password',
-        })
+        response = self.client.post(
+            reverse('otpadmin:login'),
+            data={
+                'username': self.bob.get_username(),
+                'password': 'password',
+            },
+        )
         self.assertContains(response, 'Username:')
         self.assertContains(response, 'Password:')
         self.assertContains(response, 'OTP Device:')
         self.assertContains(response, 'OTP Token:')
 
         device = self.bob.staticdevice_set.get()
         token = device.token_set.get()
-        response = self.client.post(reverse('otpadmin:login'), data={
-            'username': self.bob.get_username(),
-            'password': 'password',
-            'otp_device': device.persistent_id,
-            'otp_token': token.token,
-            'next': '/',
-        })
+        response = self.client.post(
+            reverse('otpadmin:login'),
+            data={
+                'username': self.bob.get_username(),
+                'password': 'password',
+                'otp_device': device.persistent_id,
+                'otp_token': token.token,
+                'next': '/',
+            },
+        )
         self.assertRedirects(response, '/')
 
     def test_authenticate(self):
         device = self.alice.staticdevice_set.get()
         token = device.token_set.get()
 
         params = {
             'username': self.alice.get_username(),
             'password': 'password',
             'otp_device': device.persistent_id,
             'otp_token': token.token,
             'next': '/',
         }
 
-        response = self.client.post('/login/', params)
+        response = self.client.post(reverse('login'), params)
         self.assertRedirects(response, '/')
 
         response = self.client.get('/')
-        self.assertContains(response, self.alice.get_username())
+        self.assertInHTML(
+            f'<span id="username">{self.alice.get_username()}</span>',
+            response.content.decode(response.charset),
+        )
 
     def test_verify(self):
         device = self.alice.staticdevice_set.get()
         token = device.token_set.get()
 
         params = {
             'otp_device': device.persistent_id,
             'otp_token': token.token,
             'next': '/',
         }
 
         self.client.login(username=self.alice.get_username(), password='password')
 
-        response = self.client.post('/login/', params)
+        response = self.client.post(reverse('login-otp'), params)
         self.assertRedirects(response, '/')
 
         response = self.client.get('/')
-        self.assertContains(response, self.alice.get_username())
+        self.assertInHTML(
+            f'<span id="username">{self.alice.get_username()}</span>',
+            response.content.decode(response.charset),
+        )
 
 
 @skipUnlessDBFeature('has_select_for_update')
 @override_settings(OTP_STATIC_THROTTLE_FACTOR=0)
 class ConcurrencyTestCase(TransactionTestCase):
     def setUp(self):
         try:
@@ -383,15 +406,17 @@
                 self.verified = None
 
             def run(self):
                 self.verified = verify_token(self.user, self.device_id, self.token)
                 connection.close()
 
         device = self.alice.staticdevice_set.get()
-        threads = [VerifyThread(device.user, device.persistent_id, 'valid') for _ in range(10)]
+        threads = [
+            VerifyThread(device.user, device.persistent_id, 'valid') for _ in range(10)
+        ]
         for thread in threads:
             thread.start()
         for thread in threads:
             thread.join()
 
         self.assertEqual(sum(1 for t in threads if t.verified is not None), 1)
 
@@ -424,21 +449,73 @@
     def test_serialized_throttling(self):
         # After the first failure, verification will be skipped and the count
         # will not be incremented.
         self._test_throttling_concurrency(thread_count=10, expected_failures=1)
 
     def _test_throttling_concurrency(self, thread_count, expected_failures):
         forms = (
-            OTPTokenForm(device.user, None, {'otp_device': device.persistent_id, 'otp_token': 'bogus'})
+            OTPTokenForm(
+                device.user,
+                None,
+                {'otp_device': device.persistent_id, 'otp_token': 'bogus'},
+            )
             for _ in range(thread_count)
             for device in StaticDevice.objects.all()
         )
 
         threads = [TestThread(target=form.is_valid) for form in forms]
         for thread in threads:
             thread.start()
         for thread in threads:
             thread.join()
 
         for device in StaticDevice.objects.all():
             with self.subTest(user=device.user.get_username()):
                 self.assertEqual(device.throttling_failure_count, expected_failures)
+
+
+class AddStaticTokenTestCase(TestCase):
+    def setUp(self):
+        try:
+            self.alice = self.create_user('alice', 'password')
+            self.bob = self.create_user('bob', 'password', is_staff=True)
+        except IntegrityError:
+            self.skipTest("Unable to create a test user.")
+
+    def test_no_user(self):
+        with self.assertRaises(CommandError):
+            call_command('addstatictoken', 'bogus')
+
+    def test_new_device(self):
+        out = StringIO()
+        call_command('addstatictoken', 'alice', stdout=out)
+        token = out.getvalue().strip()
+
+        static_token = StaticToken.objects.select_related('device__user').get(
+            token=token
+        )
+        self.assertEqual(static_token.device.user, self.alice)
+
+    def test_existing_device(self):
+        device = self.alice.staticdevice_set.create()
+
+        out = StringIO()
+        call_command('addstatictoken', 'alice', stdout=out)
+        token = out.getvalue().strip()
+
+        static_token = StaticToken.objects.select_related('device__user').get(
+            token=token
+        )
+        self.assertEqual(static_token.device, device)
+
+    def test_explicit_token(self):
+        device = self.alice.staticdevice_set.create()
+
+        out = StringIO()
+        call_command('addstatictoken', 'alice', '-t', 'secret-token', stdout=out)
+        token = out.getvalue().strip()
+
+        static_token = StaticToken.objects.select_related('device__user').get(
+            token=token
+        )
+        self.assertEqual(token, 'secret-token')
+        self.assertEqual(static_token.device, device)
```

### Comparing `django-otp-1.1.6/src/django_otp/util.py` & `django_otp-1.2.0/src/django_otp/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,28 @@
         ...
     ValidationError: ['phlebotinum is not valid hex-encoded data.']
     >>> hex_validator(9)('0123456789abcdef')    # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     ValidationError: ['0123456789abcdef does not represent exactly 9 bytes.']
     """
+
     def _validator(value):
         try:
             if isinstance(value, str):
                 value = value.encode()
 
             unhexlify(value)
         except Exception:
             raise ValidationError('{0} is not valid hex-encoded data.'.format(value))
 
         if (length > 0) and (len(value) != length * 2):
-            raise ValidationError('{0} does not represent exactly {1} bytes.'.format(value, length))
+            raise ValidationError(
+                '{0} does not represent exactly {1} bytes.'.format(value, length)
+            )
 
     return _validator
 
 
 def random_hex(length=20):
     """
     Returns a string of random bytes encoded as hex.
```

### Comparing `django-otp-1.1.6/src/django_otp/views.py` & `django_otp-1.2.0/src/django_otp/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     device, it will use the full username/password/token form. In order to use
     this, you must supply a template that is compatible with both
     :class:`~django_otp.forms.OTPAuthenticationForm` and
     :class:`~django_otp.forms.OTPTokenForm`. This is a good view for
     :setting:`OTP_LOGIN_URL`.
 
     """
+
     otp_authentication_form = OTPAuthenticationForm
     otp_token_form = OTPTokenForm
 
     @cached_property
     def authentication_form(self):
         user = self.request.user
         if user.is_anonymous or user.is_verified():
```


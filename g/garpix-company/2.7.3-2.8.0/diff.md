# Comparing `tmp/garpix_company-2.7.3.tar.gz` & `tmp/garpix_company-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.7.3.tar", last modified: Thu May 11 09:19:56 2023, max compression
+gzip compressed data, was "garpix_company-2.8.0.tar", last modified: Thu May 11 10:44:32 2023, max compression
```

## Comparing `garpix_company-2.7.3.tar` & `garpix_company-2.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.186044 garpix_company-2.7.3/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-11 09:19:56.000000 garpix_company-2.7.3/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-11 09:19:56.185890 garpix_company-2.7.3/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.156556 garpix_company-2.7.3/garpix_company/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2441 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3323 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.157565 garpix_company-2.7.3/garpix_company/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/admin/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.7.3/garpix_company/admin/company_invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/helpers.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.157876 garpix_company-2.7.3/garpix_company/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/managers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/managers/invite.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.157992 garpix_company-2.7.3/garpix_company/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.158082 garpix_company-2.7.3/garpix_company/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.158287 garpix_company-2.7.3/garpix_company/mixins/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/mixins/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.7.3/garpix_company/mixins/views/company_mixin.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.158865 garpix_company-2.7.3/garpix_company/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-05-05 07:20:15.000000 garpix_company-2.7.3/garpix_company/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6079 2023-05-11 09:19:51.000000 garpix_company-2.7.3/garpix_company/models/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/models/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4133 2023-05-10 09:40:57.000000 garpix_company-2.7.3/garpix_company/models/user_company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.7.3/garpix_company/models/user_role.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.184080 garpix_company-2.7.3/garpix_company/permissions/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.7.3/garpix_company/permissions/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/permissions/company_admin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.7.3/garpix_company/permissions/company_owner.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.7.3/garpix_company/permissions/company_user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      420 2022-12-09 14:51:29.000000 garpix_company-2.7.3/garpix_company/permissions/invite_receiver.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.184877 garpix_company-2.7.3/garpix_company/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.7.3/garpix_company/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/serializers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5620 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/serializers/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.7.3/garpix_company/serializers/role.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.7.3/garpix_company/serializers/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      851 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/serializers/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.185088 garpix_company-2.7.3/garpix_company/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.7.3/garpix_company/services/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.7.3/garpix_company/services/role_service.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.7.3/garpix_company/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-11 09:19:31.000000 garpix_company-2.7.3/garpix_company/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.7.3/garpix_company/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.7.3/garpix_company/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.185683 garpix_company-2.7.3/garpix_company/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.7.3/garpix_company/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5446 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/views/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2127 2023-02-06 10:05:38.000000 garpix_company-2.7.3/garpix_company/views/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3588 2023-05-04 14:33:02.000000 garpix_company-2.7.3/garpix_company/views/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 09:19:56.157220 garpix_company-2.7.3/garpix_company.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-11 09:19:56.000000 garpix_company-2.7.3/garpix_company.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-11 09:19:56.000000 garpix_company-2.7.3/garpix_company.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-11 09:19:56.000000 garpix_company-2.7.3/garpix_company.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-11 09:19:56.000000 garpix_company-2.7.3/garpix_company.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-11 09:19:56.000000 garpix_company-2.7.3/garpix_company.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-11 09:19:56.000000 garpix_company-2.7.3/garpix_company.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-11 09:19:56.186102 garpix_company-2.7.3/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-11 09:19:56.000000 garpix_company-2.7.3/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.144485 garpix_company-2.8.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-11 10:44:32.000000 garpix_company-2.8.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-11 10:44:32.144315 garpix_company-2.8.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.138732 garpix_company-2.8.0/garpix_company/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2533 2023-05-11 10:44:26.000000 garpix_company-2.8.0/garpix_company/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3508 2023-05-11 10:44:26.000000 garpix_company-2.8.0/garpix_company/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.140321 garpix_company-2.8.0/garpix_company/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-11 10:08:25.000000 garpix_company-2.8.0/garpix_company/admin/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.8.0/garpix_company/admin/company_invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/helpers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.140699 garpix_company-2.8.0/garpix_company/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/managers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/managers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/managers/invite.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.140823 garpix_company-2.8.0/garpix_company/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.140921 garpix_company-2.8.0/garpix_company/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.141139 garpix_company-2.8.0/garpix_company/mixins/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/mixins/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.8.0/garpix_company/mixins/views/company_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.141907 garpix_company-2.8.0/garpix_company/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-05-05 07:20:15.000000 garpix_company-2.8.0/garpix_company/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6079 2023-05-11 09:19:51.000000 garpix_company-2.8.0/garpix_company/models/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.8.0/garpix_company/models/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4133 2023-05-10 09:40:57.000000 garpix_company-2.8.0/garpix_company/models/user_company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.8.0/garpix_company/models/user_role.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.142513 garpix_company-2.8.0/garpix_company/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.8.0/garpix_company/permissions/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.8.0/garpix_company/permissions/company_admin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.8.0/garpix_company/permissions/company_owner.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.8.0/garpix_company/permissions/company_user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      410 2023-05-11 10:44:26.000000 garpix_company-2.8.0/garpix_company/permissions/invite_receiver.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.143198 garpix_company-2.8.0/garpix_company/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.8.0/garpix_company/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.8.0/garpix_company/serializers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5728 2023-05-11 10:44:26.000000 garpix_company-2.8.0/garpix_company/serializers/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.8.0/garpix_company/serializers/role.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.8.0/garpix_company/serializers/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      851 2023-05-04 14:33:02.000000 garpix_company-2.8.0/garpix_company/serializers/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.143477 garpix_company-2.8.0/garpix_company/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.8.0/garpix_company/services/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.8.0/garpix_company/services/role_service.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.8.0/garpix_company/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-11 10:44:26.000000 garpix_company-2.8.0/garpix_company/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.8.0/garpix_company/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.8.0/garpix_company/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.143938 garpix_company-2.8.0/garpix_company/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.8.0/garpix_company/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5446 2023-05-04 14:33:02.000000 garpix_company-2.8.0/garpix_company/views/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3409 2023-05-11 10:44:26.000000 garpix_company-2.8.0/garpix_company/views/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3588 2023-05-04 14:33:02.000000 garpix_company-2.8.0/garpix_company/views/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-11 10:44:32.139551 garpix_company-2.8.0/garpix_company.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-11 10:44:32.000000 garpix_company-2.8.0/garpix_company.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-11 10:44:32.000000 garpix_company-2.8.0/garpix_company.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-11 10:44:32.000000 garpix_company-2.8.0/garpix_company.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-11 10:44:32.000000 garpix_company-2.8.0/garpix_company.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-11 10:44:32.000000 garpix_company-2.8.0/garpix_company.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-11 10:44:32.000000 garpix_company-2.8.0/garpix_company.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-11 10:44:32.144533 garpix_company-2.8.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-11 10:44:32.000000 garpix_company-2.8.0/setup.py
```

### Comparing `garpix_company-2.7.3/PKG-INFO` & `garpix_company-2.8.0/garpix_company/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: garpix_company
-Version: 2.7.3
-Home-page: https://github.com/garpixcms/garpix_company
-Author: Garpix LTD
-Author-email: info@garpix.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
 # Garpix Company
 
 Company module for Django/DRF projects.
 
 
 ## Quickstart
 
@@ -146,26 +129,29 @@
 # settings.py
 
 GARPIX_COMPANY_USER_SERIALIZER = 'app.serializers.UserSerializer'
 GARPIX_COMPANY_ROLE_SERIALIZER = 'app.serializers.CompanyRoleSerializer'
 
 ```
 
+You can also set `GARPIX_COMPANY_INVITE_NOT_USERS` setting to True (False is default) to allow to invite not registered users
+
 ## Companies count limit
 
 If you need to add some limitations on companies count the user can be a part of, you can override `check_user_companies_limit` class method of `Company` class:
 
 ```python
-from garpix_company.models import AbstractCompany, UserCompany
+from garpix_company.models import AbstractCompany, get_user_company_model
 
 
 class Company(AbstractCompany):
 
     @classmethod
     def check_user_companies_limit(cls, user):
+        UserCompany = get_user_company_model()
         return UserCompany.objects.filter(user=user).count() < 1
 
 ```
 
 See `garpix_company/tests/test_company.py` for examples.
 
 # Changelog
@@ -178,8 +164,8 @@
 
 # License
 
 [MIT](LICENSE)
 
 ---
 
-Developed by Garpix / [https://garpix.com](https://garpix.com)
+Developed by Garpix / [https://garpix.com](https://garpix.com)
```

### Comparing `garpix_company-2.7.3/garpix_company/CHANGELOG.md` & `garpix_company-2.8.0/garpix_company/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 2.8.0 (11.05.2023)
+
+- `GARPIX_COMPANY_INVITE_NOT_USERS` setting added (see `Readme.md)
+
 ### 2.7.0 (04.05.2023)
 
 - `GARPIX_USER_COMPANY_MODEL` setting added
 - `role` and `stay_in_company` fields added to `change_owner` endpoint
 
 ### 2.6.1 (27.04.2023)
```

### Comparing `garpix_company-2.7.3/garpix_company/CONTRIBUTING.md` & `garpix_company-2.8.0/garpix_company/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/README.md` & `garpix_company-2.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: garpix_company
+Version: 2.8.0
+Home-page: https://github.com/garpixcms/garpix_company
+Author: Garpix LTD
+Author-email: info@garpix.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+
 # Garpix Company
 
 Company module for Django/DRF projects.
 
 
 ## Quickstart
 
@@ -129,26 +146,29 @@
 # settings.py
 
 GARPIX_COMPANY_USER_SERIALIZER = 'app.serializers.UserSerializer'
 GARPIX_COMPANY_ROLE_SERIALIZER = 'app.serializers.CompanyRoleSerializer'
 
 ```
 
+You can also set `GARPIX_COMPANY_INVITE_NOT_USERS` setting to True (False is default) to allow to invite not registered users
+
 ## Companies count limit
 
 If you need to add some limitations on companies count the user can be a part of, you can override `check_user_companies_limit` class method of `Company` class:
 
 ```python
-from garpix_company.models import AbstractCompany, UserCompany
+from garpix_company.models import AbstractCompany, get_user_company_model
 
 
 class Company(AbstractCompany):
 
     @classmethod
     def check_user_companies_limit(cls, user):
+        UserCompany = get_user_company_model()
         return UserCompany.objects.filter(user=user).count() < 1
 
 ```
 
 See `garpix_company/tests/test_company.py` for examples.
 
 # Changelog
@@ -161,8 +181,8 @@
 
 # License
 
 [MIT](LICENSE)
 
 ---
 
-Developed by Garpix / [https://garpix.com](https://garpix.com)
+Developed by Garpix / [https://garpix.com](https://garpix.com)
```

### Comparing `garpix_company-2.7.3/garpix_company/helpers.py` & `garpix_company-2.8.0/garpix_company/helpers.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/models/company.py` & `garpix_company-2.8.0/garpix_company/models/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/models/invite.py` & `garpix_company-2.8.0/garpix_company/models/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/models/user_company.py` & `garpix_company-2.8.0/garpix_company/models/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/models/user_role.py` & `garpix_company-2.8.0/garpix_company/models/user_role.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/permissions/company_admin.py` & `garpix_company-2.8.0/garpix_company/permissions/company_admin.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/permissions/company_owner.py` & `garpix_company-2.8.0/garpix_company/permissions/company_owner.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/serializers/company.py` & `garpix_company-2.8.0/garpix_company/serializers/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/serializers/invite.py` & `garpix_company-2.8.0/garpix_company/serializers/invite.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,23 @@
             'role': {'required': True},
         }
 
     def validate_email(self, value):
         User = get_user_model()
         Company = get_company_model()
         company_id = self.context.get("company_id")
-        try:
-            user = User.objects.get(email=value)
-            if not Company.check_user_companies_limit(user):
-                raise ValidationError(_('У пользователя с указанным email превышен лимит количества компаний'))
-            if UserCompany.active_objects.filter(user=user, company_id=company_id).exists():
-                raise ValidationError(_('Указанный пользователь уже является сотрудником компании'))
-        except User.DoesNotExist:
-            raise ValidationError(_('Пользователь с указанным email не зарегистрирован'))
+        if not getattr(settings, 'GARPIX_COMPANY_INVITE_NOT_USERS', False):
+            try:
+                user = User.objects.get(email=value)
+                if not Company.check_user_companies_limit(user):
+                    raise ValidationError(_('У пользователя с указанным email превышен лимит количества компаний'))
+                if UserCompany.active_objects.filter(user=user, company_id=company_id).exists():
+                    raise ValidationError(_('Указанный пользователь уже является сотрудником компании'))
+            except User.DoesNotExist:
+                raise ValidationError(_('Пользователь с указанным email не зарегистрирован'))
         return value
 
     def validate_user(self, value):
         Company = get_company_model()
         company_id = self.context.get("company_id")
         if not Company.check_user_companies_limit(value):
             raise ValidationError(_('У пользователя с указанным id превышен лимит количества компаний'))
```

### Comparing `garpix_company-2.7.3/garpix_company/serializers/user_company.py` & `garpix_company-2.8.0/garpix_company/serializers/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/services/role_service.py` & `garpix_company-2.8.0/garpix_company/services/role_service.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/settings.py` & `garpix_company-2.8.0/garpix_company/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/setup.py` & `garpix_company-2.8.0/garpix_company/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.7.3',
+    version='2.8.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_company-2.7.3/garpix_company/urls.py` & `garpix_company-2.8.0/garpix_company/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/views/company.py` & `garpix_company-2.8.0/garpix_company/views/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company/views/invite.py` & `garpix_company-2.8.0/garpix_company/views/invite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from rest_framework import mixins, permissions, status
 from rest_framework.decorators import action
+from rest_framework.generics import get_object_or_404
 from rest_framework.response import Response
 from rest_framework.viewsets import GenericViewSet
 
 from garpix_company.mixins.views import GarpixCompanyViewSetMixin
 from garpix_company.models.invite import InviteToCompany
 from garpix_company.permissions import CompanyAdminOnly, CompanyOwnerOnly
 from garpix_company.permissions.invite_receiver import CompanyInviteReceiverOnly
@@ -17,15 +18,15 @@
     queryset = InviteToCompany.created_objects.all()
     serializer_class = InviteToCompanySerializer
     permission_classes = [permissions.IsAdminUser | CompanyAdminOnly | CompanyOwnerOnly | CompanyInviteReceiverOnly]
 
     # lookup_field = 'token'  # TODO сделать вариант инвайта по токену
 
     def get_serializer_class(self):
-        if self.action == 'retrieve':
+        if self.action in ('retrieve', 'token_retrieve'):
             return InviteToCompanySerializer
         return None
 
     def retrieve(self, request, *args, **kwargs):
         instance = self.get_object()
         self.check_object_permissions(request, instance)
         serializer = self.get_serializer(instance)
@@ -44,7 +45,32 @@
     @action(methods=['post'], detail=True)
     def decline(self, request, pk):
         invite = self.get_object()
         self.check_object_permissions(request, invite)
         invite.decline()
         serializer = InviteToCompanySerializer(invite)
         return Response(serializer.data)
+
+    @action(methods=['get'], detail=False, url_path='(?P<token>[^/.]+)')
+    def token_retrieve(self, request, token):
+        instance = get_object_or_404(self.get_queryset(), token=token)
+        self.check_object_permissions(request, instance)
+        serializer = self.get_serializer(instance)
+        return Response(serializer.data)
+
+    @action(methods=['post'], detail=False, url_path='(?P<token>[^/.]+)/accept')
+    def accept(self, request, token):
+        invite = get_object_or_404(self.get_queryset(), token=token)
+        self.check_object_permissions(request, invite)
+        result, message = invite.accept()
+        if result:
+            serializer = InviteToCompanySerializer(invite)
+            return Response(serializer.data)
+        return Response({'non_field_error': [message]}, status=status.HTTP_400_BAD_REQUEST)
+
+    @action(methods=['post'], detail=False, url_path='(?P<token>[^/.]+)/decline')
+    def decline(self, request, token):
+        invite = get_object_or_404(self.get_queryset(), token=token)
+        self.check_object_permissions(request, invite)
+        invite.decline()
+        serializer = InviteToCompanySerializer(invite)
+        return Response(serializer.data)
```

### Comparing `garpix_company-2.7.3/garpix_company/views/user_company.py` & `garpix_company-2.8.0/garpix_company/views/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/garpix_company.egg-info/PKG-INFO` & `garpix_company-2.8.0/garpix_company.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-company
-Version: 2.7.3
+Version: 2.8.0
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -146,26 +146,29 @@
 # settings.py
 
 GARPIX_COMPANY_USER_SERIALIZER = 'app.serializers.UserSerializer'
 GARPIX_COMPANY_ROLE_SERIALIZER = 'app.serializers.CompanyRoleSerializer'
 
 ```
 
+You can also set `GARPIX_COMPANY_INVITE_NOT_USERS` setting to True (False is default) to allow to invite not registered users
+
 ## Companies count limit
 
 If you need to add some limitations on companies count the user can be a part of, you can override `check_user_companies_limit` class method of `Company` class:
 
 ```python
-from garpix_company.models import AbstractCompany, UserCompany
+from garpix_company.models import AbstractCompany, get_user_company_model
 
 
 class Company(AbstractCompany):
 
     @classmethod
     def check_user_companies_limit(cls, user):
+        UserCompany = get_user_company_model()
         return UserCompany.objects.filter(user=user).count() < 1
 
 ```
 
 See `garpix_company/tests/test_company.py` for examples.
 
 # Changelog
```

### Comparing `garpix_company-2.7.3/garpix_company.egg-info/SOURCES.txt` & `garpix_company-2.8.0/garpix_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.3/setup.py` & `garpix_company-2.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.7.3',
+    version='2.8.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```


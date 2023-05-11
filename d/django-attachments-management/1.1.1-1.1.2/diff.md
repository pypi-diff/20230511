# Comparing `tmp/django_attachments_management-1.1.1.tar.gz` & `tmp/django_attachments_management-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_attachments_management-1.1.1.tar", last modified: Wed May 10 11:24:44 2023, max compression
+gzip compressed data, was "django_attachments_management-1.1.2.tar", last modified: Thu May 11 04:30:40 2023, max compression
```

## Comparing `django_attachments_management-1.1.1.tar` & `django_attachments_management-1.1.2.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.702454 django_attachments_management-1.1.1/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      101 2022-12-11 15:20:12.000000 django_attachments_management-1.1.1/.cz.toml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      129 2022-12-11 15:16:56.000000 django_attachments_management-1.1.1/.editorconfig
--rw-r--r--   0 mirec     (1000) mirec     (1000)      157 2022-12-11 15:26:57.000000 django_attachments_management-1.1.1/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-11-30 13:28:53.000000 django_attachments_management-1.1.1/AUTHORS
--rw-r--r--   0 mirec     (1000) mirec     (1000)      728 2023-05-10 11:24:36.000000 django_attachments_management-1.1.1/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-11 15:13:56.000000 django_attachments_management-1.1.1/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)      246 2018-01-17 13:30:39.000000 django_attachments_management-1.1.1/MANIFEST.in
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2360 2023-05-10 11:24:44.702454 django_attachments_management-1.1.1/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1669 2022-12-11 15:40:10.000000 django_attachments_management-1.1.1/README.rst
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.696454 django_attachments_management-1.1.1/django_attachments/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      106 2021-06-01 10:32:36.000000 django_attachments_management-1.1.1/django_attachments/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2428 2021-03-25 07:42:43.000000 django_attachments_management-1.1.1/django_attachments/admin.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      379 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/django_attachments/apps.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1667 2020-01-23 06:48:52.000000 django_attachments_management-1.1.1/django_attachments/cleanup.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      715 2021-03-25 07:05:36.000000 django_attachments_management-1.1.1/django_attachments/fields.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1159 2021-03-25 07:05:36.000000 django_attachments_management-1.1.1/django_attachments/forms.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.671454 django_attachments_management-1.1.1/django_attachments/locale/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.671454 django_attachments_management-1.1.1/django_attachments/locale/sk_SK/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.696454 django_attachments_management-1.1.1/django_attachments/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1266 2018-07-27 08:03:41.000000 django_attachments_management-1.1.1/django_attachments/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1412 2018-07-27 08:03:35.000000 django_attachments_management-1.1.1/django_attachments/locale/sk_SK/LC_MESSAGES/django.po
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.697454 django_attachments_management-1.1.1/django_attachments/migrations/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2492 2020-01-23 06:52:23.000000 django_attachments_management-1.1.1/django_attachments/migrations/0001_initial.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      598 2018-07-27 08:04:58.000000 django_attachments_management-1.1.1/django_attachments/migrations/0002_auto_20180727_0804.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      364 2020-05-22 13:47:18.000000 django_attachments_management-1.1.1/django_attachments/migrations/0003_attachment_options.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-11-30 17:02:36.000000 django_attachments_management-1.1.1/django_attachments/migrations/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4567 2022-10-15 06:26:46.000000 django_attachments_management-1.1.1/django_attachments/models.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.672454 django_attachments_management-1.1.1/django_attachments/static/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.672454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.697454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/css/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1974 2017-12-07 15:53:15.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/css/attachments.css
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.697454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       18 2017-12-07 21:17:13.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/.gitattributes
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.672454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.697454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      806 2017-12-07 20:41:12.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.png
--rw-r--r--   0 mirec     (1000) mirec     (1000)     7945 2017-08-06 16:25:08.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.svg
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1199 2017-12-07 20:41:13.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/pdf.png
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2680 2017-08-06 16:25:08.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/pdf.svg
--rw-r--r--   0 mirec     (1000) mirec     (1000)      126 2015-06-13 17:13:07.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/trashcan.png
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2426 2015-12-05 11:50:14.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/upload.png
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.698454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/js/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2452 2023-02-04 12:37:47.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/js/admin_attachments.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)    24312 2022-07-27 15:16:29.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/js/attachments.js
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.672454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.698454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1151 2017-12-01 17:30:40.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)      751 2017-12-01 17:30:27.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/basic.min.css
--rw-r--r--   0 mirec     (1000) mirec     (1000)     9717 2017-12-01 17:30:12.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.css
--rw-r--r--   0 mirec     (1000) mirec     (1000)    42790 2017-12-02 15:04:54.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.js
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.698454 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/sortable/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        4 2017-12-03 14:16:41.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/sortable/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)    15369 2017-12-03 14:16:53.000000 django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/sortable/Sortable.min.js
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.672454 django_attachments_management-1.1.1/django_attachments/templates/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.672454 django_attachments_management-1.1.1/django_attachments/templates/admin/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.699454 django_attachments_management-1.1.1/django_attachments/templates/admin/attachments/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      238 2017-12-07 12:42:29.000000 django_attachments_management-1.1.1/django_attachments/templates/admin/attachments/library_create.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      807 2017-12-07 11:15:37.000000 django_attachments_management-1.1.1/django_attachments/templates/admin/attachments/library_edit.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.672454 django_attachments_management-1.1.1/django_attachments/templates/django_attachments/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.699454 django_attachments_management-1.1.1/django_attachments/templates/django_attachments/widgets/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      308 2017-12-07 19:18:07.000000 django_attachments_management-1.1.1/django_attachments/templates/django_attachments/widgets/admin_attachments.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4433 2020-01-23 06:50:50.000000 django_attachments_management-1.1.1/django_attachments/tests.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2170 2022-09-09 13:49:10.000000 django_attachments_management-1.1.1/django_attachments/utils.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5622 2023-05-10 11:24:32.000000 django_attachments_management-1.1.1/django_attachments/views.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1245 2021-03-25 07:05:36.000000 django_attachments_management-1.1.1/django_attachments/widgets.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.699454 django_attachments_management-1.1.1/django_attachments_management.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2360 2023-05-10 11:24:44.000000 django_attachments_management-1.1.1/django_attachments_management.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3162 2023-05-10 11:24:44.000000 django_attachments_management-1.1.1/django_attachments_management.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-05-10 11:24:44.000000 django_attachments_management-1.1.1/django_attachments_management.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       72 2023-05-10 11:24:44.000000 django_attachments_management-1.1.1/django_attachments_management.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       19 2023-05-10 11:24:44.000000 django_attachments_management-1.1.1/django_attachments_management.egg-info/top_level.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1119 2023-05-10 11:24:36.000000 django_attachments_management-1.1.1/pyproject.toml
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.700454 django_attachments_management-1.1.1/sample_project/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.700454 django_attachments_management-1.1.1/sample_project/example/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/example/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      310 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/example/admin.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      667 2021-03-25 07:05:36.000000 django_attachments_management-1.1.1/sample_project/example/admin_forms.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      127 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/example/apps.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.701454 django_attachments_management-1.1.1/sample_project/example/migrations/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      984 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/example/migrations/0001_initial.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-12-01 13:16:12.000000 django_attachments_management-1.1.1/sample_project/example/migrations/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      491 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/example/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1664 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/example/views.py
--rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2022-12-11 15:26:16.000000 django_attachments_management-1.1.1/sample_project/manage.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       23 2023-01-24 05:58:06.000000 django_attachments_management-1.1.1/sample_project/requirements.txt
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.701454 django_attachments_management-1.1.1/sample_project/templates/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      715 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/templates/base.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-12-07 07:51:48.000000 django_attachments_management-1.1.1/sample_project/templates/gallery_upload.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      303 2017-12-07 07:50:57.000000 django_attachments_management-1.1.1/sample_project/templates/index.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1082 2017-12-07 15:25:33.000000 django_attachments_management-1.1.1/sample_project/templates/live_upload_attachments.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1642 2017-12-07 18:11:20.000000 django_attachments_management-1.1.1/sample_project/templates/on_save_upload_attachments.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.702454 django_attachments_management-1.1.1/sample_project/web/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-11-30 13:50:34.000000 django_attachments_management-1.1.1/sample_project/web/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1888 2022-12-11 11:58:20.000000 django_attachments_management-1.1.1/sample_project/web/settings.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      112 2022-12-11 14:32:48.000000 django_attachments_management-1.1.1/sample_project/web/settings_local.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      712 2021-03-25 07:05:36.000000 django_attachments_management-1.1.1/sample_project/web/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2017-11-30 13:50:34.000000 django_attachments_management-1.1.1/sample_project/web/wsgi.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1730 2022-12-11 14:32:48.000000 django_attachments_management-1.1.1/sample_project/web/wsgi_werkzeug.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-05-10 11:24:44.702454 django_attachments_management-1.1.1/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)      591 2022-12-11 15:17:36.000000 django_attachments_management-1.1.1/setup.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-10 11:24:44.702454 django_attachments_management-1.1.1/static_assets/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-11 15:18:55.000000 django_attachments_management-1.1.1/static_assets/.keep
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.195829 django_attachments_management-1.1.2/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      101 2022-12-11 15:20:12.000000 django_attachments_management-1.1.2/.cz.toml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      129 2022-12-11 15:16:56.000000 django_attachments_management-1.1.2/.editorconfig
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      157 2022-12-11 15:26:57.000000 django_attachments_management-1.1.2/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-11-30 13:28:53.000000 django_attachments_management-1.1.2/AUTHORS
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      728 2023-05-10 12:39:00.000000 django_attachments_management-1.1.2/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-11 15:13:56.000000 django_attachments_management-1.1.2/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      246 2018-01-17 13:30:39.000000 django_attachments_management-1.1.2/MANIFEST.in
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2360 2023-05-11 04:30:40.194829 django_attachments_management-1.1.2/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1669 2022-12-11 15:40:10.000000 django_attachments_management-1.1.2/README.rst
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.188829 django_attachments_management-1.1.2/django_attachments/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      805 2023-05-11 04:30:01.000000 django_attachments_management-1.1.2/django_attachments/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      106 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2428 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/admin.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      379 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/apps.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1667 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/cleanup.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      715 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/fields.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1159 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/forms.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.184829 django_attachments_management-1.1.2/django_attachments/locale/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.184829 django_attachments_management-1.1.2/django_attachments/locale/sk_SK/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.188829 django_attachments_management-1.1.2/django_attachments/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1266 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1412 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/locale/sk_SK/LC_MESSAGES/django.po
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.189829 django_attachments_management-1.1.2/django_attachments/migrations/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2492 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/migrations/0001_initial.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      598 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/migrations/0002_auto_20180727_0804.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      364 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/migrations/0003_attachment_options.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      358 2023-05-11 04:29:53.000000 django_attachments_management-1.1.2/django_attachments/migrations/0004_rename_attachment_library_rank_django_atta_library_9d0164_idx.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/migrations/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4586 2023-05-11 04:29:53.000000 django_attachments_management-1.1.2/django_attachments/models.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.184829 django_attachments_management-1.1.2/django_attachments/static/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.184829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.189829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/css/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1974 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/css/attachments.css
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.189829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       18 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/.gitattributes
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.184829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.190829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      806 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.png
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     7945 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.svg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1199 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/pdf.png
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2680 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/pdf.svg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      126 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/trashcan.png
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2426 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/upload.png
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.190829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/js/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2452 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/js/admin_attachments.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    24312 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/js/attachments.js
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.185829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.190829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1151 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      751 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/basic.min.css
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     9717 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.css
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    42790 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.js
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.191829 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/sortable/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        4 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/sortable/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    15369 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/sortable/Sortable.min.js
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.185829 django_attachments_management-1.1.2/django_attachments/templates/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.185829 django_attachments_management-1.1.2/django_attachments/templates/admin/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.191829 django_attachments_management-1.1.2/django_attachments/templates/admin/attachments/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      238 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/templates/admin/attachments/library_create.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      807 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/templates/admin/attachments/library_edit.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.185829 django_attachments_management-1.1.2/django_attachments/templates/django_attachments/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.191829 django_attachments_management-1.1.2/django_attachments/templates/django_attachments/widgets/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      308 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/templates/django_attachments/widgets/admin_attachments.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4433 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/tests.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2170 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/utils.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     5622 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/views.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1245 2023-05-10 15:53:40.000000 django_attachments_management-1.1.2/django_attachments/widgets.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.191829 django_attachments_management-1.1.2/django_attachments_management.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2360 2023-05-11 04:30:40.000000 django_attachments_management-1.1.2/django_attachments_management.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     3294 2023-05-11 04:30:40.000000 django_attachments_management-1.1.2/django_attachments_management.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-05-11 04:30:40.000000 django_attachments_management-1.1.2/django_attachments_management.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       72 2023-05-11 04:30:40.000000 django_attachments_management-1.1.2/django_attachments_management.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       19 2023-05-11 04:30:40.000000 django_attachments_management-1.1.2/django_attachments_management.egg-info/top_level.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1119 2023-05-11 04:30:01.000000 django_attachments_management-1.1.2/pyproject.toml
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.192829 django_attachments_management-1.1.2/sample_project/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.193829 django_attachments_management-1.1.2/sample_project/example/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/example/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      310 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/example/admin.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      667 2021-03-25 07:05:36.000000 django_attachments_management-1.1.2/sample_project/example/admin_forms.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      127 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/example/apps.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.193829 django_attachments_management-1.1.2/sample_project/example/migrations/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      984 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/example/migrations/0001_initial.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-12-01 13:16:12.000000 django_attachments_management-1.1.2/sample_project/example/migrations/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      491 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/example/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1664 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/example/views.py
+-rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2022-12-11 15:26:16.000000 django_attachments_management-1.1.2/sample_project/manage.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       23 2023-01-24 05:58:06.000000 django_attachments_management-1.1.2/sample_project/requirements.txt
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.193829 django_attachments_management-1.1.2/sample_project/templates/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      715 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/templates/base.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-12-07 07:51:48.000000 django_attachments_management-1.1.2/sample_project/templates/gallery_upload.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      303 2017-12-07 07:50:57.000000 django_attachments_management-1.1.2/sample_project/templates/index.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1082 2017-12-07 15:25:33.000000 django_attachments_management-1.1.2/sample_project/templates/live_upload_attachments.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1642 2017-12-07 18:11:20.000000 django_attachments_management-1.1.2/sample_project/templates/on_save_upload_attachments.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.194829 django_attachments_management-1.1.2/sample_project/web/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-11-30 13:50:34.000000 django_attachments_management-1.1.2/sample_project/web/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1888 2022-12-11 11:58:20.000000 django_attachments_management-1.1.2/sample_project/web/settings.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      112 2022-12-11 14:32:48.000000 django_attachments_management-1.1.2/sample_project/web/settings_local.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      712 2021-03-25 07:05:36.000000 django_attachments_management-1.1.2/sample_project/web/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2017-11-30 13:50:34.000000 django_attachments_management-1.1.2/sample_project/web/wsgi.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1730 2022-12-11 14:32:48.000000 django_attachments_management-1.1.2/sample_project/web/wsgi_werkzeug.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-05-11 04:30:40.195829 django_attachments_management-1.1.2/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      591 2022-12-11 15:17:36.000000 django_attachments_management-1.1.2/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-11 04:30:40.194829 django_attachments_management-1.1.2/static_assets/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-11 15:18:55.000000 django_attachments_management-1.1.2/static_assets/.keep
```

### Comparing `django_attachments_management-1.1.1/CHANGELOG.md` & `django_attachments_management-1.1.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/LICENSE` & `django_attachments_management-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/PKG-INFO` & `django_attachments_management-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_attachments_management
-Version: 1.1.1
+Version: 1.1.2
 Summary: Attachments management app for django
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-attachments
 Project-URL: documentation, https://github.com/mireq/django-attachments
 Project-URL: repository, https://github.com/mireq/django-attachments
 Project-URL: changelog, https://github.com/mireq/django-attachments/blob/master/CHANGELOG.md
```

### Comparing `django_attachments_management-1.1.1/README.rst` & `django_attachments_management-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/admin.py` & `django_attachments_management-1.1.2/django_attachments/admin.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/cleanup.py` & `django_attachments_management-1.1.2/django_attachments/cleanup.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/fields.py` & `django_attachments_management-1.1.2/django_attachments/fields.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/forms.py` & `django_attachments_management-1.1.2/django_attachments/forms.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/locale/sk_SK/LC_MESSAGES/django.mo` & `django_attachments_management-1.1.2/django_attachments/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/locale/sk_SK/LC_MESSAGES/django.po` & `django_attachments_management-1.1.2/django_attachments/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/migrations/0001_initial.py` & `django_attachments_management-1.1.2/django_attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/migrations/0002_auto_20180727_0804.py` & `django_attachments_management-1.1.2/django_attachments/migrations/0002_auto_20180727_0804.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/models.py` & `django_attachments_management-1.1.2/django_attachments/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,17 @@
 		blank=True
 	)
 
 	class Meta:
 		verbose_name = _("Attachment")
 		verbose_name_plural = _("Attachments")
 		ordering = ('-library', 'rank')
-		index_together = (('library', 'rank',),)
+		indexes = [
+			models.Index(fields=['library', 'rank'])
+		]
 
 	def __str__(self):
 		return self.original_name
 
 	@property
 	def is_image(self):
 		return self.image_width is not None
```

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/css/attachments.css` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/css/attachments.css`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.png` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.png`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.svg` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.svg`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/pdf.png` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/pdf.png`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/mimetypes/application/pdf.svg` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/mimetypes/application/pdf.svg`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/img/upload.png` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/img/upload.png`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/js/admin_attachments.js` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/js/admin_attachments.js`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/js/attachments.js` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/js/attachments.js`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/LICENSE` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/LICENSE`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/basic.min.css` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/basic.min.css`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.css` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.js` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/dropzone/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/static/django_attachments/vendor/sortable/Sortable.min.js` & `django_attachments_management-1.1.2/django_attachments/static/django_attachments/vendor/sortable/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/templates/admin/attachments/library_edit.html` & `django_attachments_management-1.1.2/django_attachments/templates/admin/attachments/library_edit.html`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/tests.py` & `django_attachments_management-1.1.2/django_attachments/tests.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/utils.py` & `django_attachments_management-1.1.2/django_attachments/utils.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/views.py` & `django_attachments_management-1.1.2/django_attachments/views.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments/widgets.py` & `django_attachments_management-1.1.2/django_attachments/widgets.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/django_attachments_management.egg-info/PKG-INFO` & `django_attachments_management-1.1.2/django_attachments_management.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-attachments-management
-Version: 1.1.1
+Version: 1.1.2
 Summary: Attachments management app for django
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-attachments
 Project-URL: documentation, https://github.com/mireq/django-attachments
 Project-URL: repository, https://github.com/mireq/django-attachments
 Project-URL: changelog, https://github.com/mireq/django-attachments/blob/master/CHANGELOG.md
```

### Comparing `django_attachments_management-1.1.1/django_attachments_management.egg-info/SOURCES.txt` & `django_attachments_management-1.1.2/django_attachments_management.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 AUTHORS
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
+django_attachments/CHANGELOG.md
 django_attachments/__init__.py
 django_attachments/admin.py
 django_attachments/apps.py
 django_attachments/cleanup.py
 django_attachments/fields.py
 django_attachments/forms.py
 django_attachments/models.py
@@ -20,14 +21,15 @@
 django_attachments/views.py
 django_attachments/widgets.py
 django_attachments/locale/sk_SK/LC_MESSAGES/django.mo
 django_attachments/locale/sk_SK/LC_MESSAGES/django.po
 django_attachments/migrations/0001_initial.py
 django_attachments/migrations/0002_auto_20180727_0804.py
 django_attachments/migrations/0003_attachment_options.py
+django_attachments/migrations/0004_rename_attachment_library_rank_django_atta_library_9d0164_idx.py
 django_attachments/migrations/__init__.py
 django_attachments/static/django_attachments/css/attachments.css
 django_attachments/static/django_attachments/img/.gitattributes
 django_attachments/static/django_attachments/img/trashcan.png
 django_attachments/static/django_attachments/img/upload.png
 django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.png
 django_attachments/static/django_attachments/img/mimetypes/application/octet-stream.svg
```

### Comparing `django_attachments_management-1.1.1/pyproject.toml` & `django_attachments_management-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,9 +38,9 @@
 where = ["."]
 include = ["django_attachments*"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.1"
+version = "1.1.2"
 tag_format = "$version"
```

### Comparing `django_attachments_management-1.1.1/sample_project/example/admin_forms.py` & `django_attachments_management-1.1.2/sample_project/example/admin_forms.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/example/migrations/0001_initial.py` & `django_attachments_management-1.1.2/sample_project/example/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/example/views.py` & `django_attachments_management-1.1.2/sample_project/example/views.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/manage.py` & `django_attachments_management-1.1.2/sample_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/templates/base.html` & `django_attachments_management-1.1.2/sample_project/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/templates/live_upload_attachments.html` & `django_attachments_management-1.1.2/sample_project/templates/live_upload_attachments.html`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/templates/on_save_upload_attachments.html` & `django_attachments_management-1.1.2/sample_project/templates/on_save_upload_attachments.html`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/web/settings.py` & `django_attachments_management-1.1.2/sample_project/web/settings.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/web/urls.py` & `django_attachments_management-1.1.2/sample_project/web/urls.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/sample_project/web/wsgi_werkzeug.py` & `django_attachments_management-1.1.2/sample_project/web/wsgi_werkzeug.py`

 * *Files identical despite different names*

### Comparing `django_attachments_management-1.1.1/setup.py` & `django_attachments_management-1.1.2/setup.py`

 * *Files identical despite different names*


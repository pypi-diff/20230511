# Comparing `tmp/django-admin-interface-0.9.2.tar.gz` & `tmp/django-admin-interface-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-admin-interface-0.9.2.tar", last modified: Thu Feb  7 09:53:42 2019, max compression
+gzip compressed data, was "dist/django-admin-interface-0.9.3.tar", last modified: Thu Feb 21 17:05:51 2019, max compression
```

## Comparing `django-admin-interface-0.9.2.tar` & `django-admin-interface-0.9.3.tar`

### file list

```diff
@@ -1,112 +1,117 @@
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       90 2017-09-29 09:17:20.000000 django-admin-interface-0.9.2/admin_interface/__init__.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3087 2019-01-04 10:07:12.000000 django-admin-interface-0.9.2/admin_interface/admin.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      517 2019-01-04 10:54:08.000000 django-admin-interface-0.9.2/admin_interface/apps.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/fixtures/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1595 2017-05-24 08:59:52.000000 django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_bootstrap.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1591 2017-05-24 08:58:39.000000 django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_django.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1596 2017-05-24 08:59:00.000000 django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_foundation.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1592 2018-01-31 14:02:16.000000 django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_uswds.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1132 2017-05-24 10:01:48.000000 django-admin-interface-0.9.2/admin_interface/fixtures/initial_data.json
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/locale/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/locale/es/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/locale/es/LC_MESSAGES/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2562 2019-01-11 10:19:38.000000 django-admin-interface-0.9.2/admin_interface/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3728 2019-01-11 10:19:38.000000 django-admin-interface-0.9.2/admin_interface/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/locale/fr/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/locale/fr/LC_MESSAGES/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2503 2019-01-11 10:19:38.000000 django-admin-interface-0.9.2/admin_interface/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3695 2019-01-11 10:19:38.000000 django-admin-interface-0.9.2/admin_interface/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/locale/it/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/locale/it/LC_MESSAGES/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2468 2019-01-11 10:19:38.000000 django-admin-interface-0.9.2/admin_interface/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3600 2019-01-11 10:19:38.000000 django-admin-interface-0.9.2/admin_interface/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/migrations/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7501 2017-11-23 11:05:23.000000 django-admin-interface-0.9.2/admin_interface/migrations/0001_initial.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1824 2017-11-23 11:01:09.000000 django-admin-interface-0.9.2/admin_interface/migrations/0002_add_related_modal.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      898 2017-11-23 11:01:14.000000 django-admin-interface-0.9.2/admin_interface/migrations/0003_add_logo_color.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      404 2017-11-23 11:01:19.000000 django-admin-interface-0.9.2/admin_interface/migrations/0004_rename_title_color.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      483 2017-11-23 11:01:23.000000 django-admin-interface-0.9.2/admin_interface/migrations/0005_add_recent_actions_visible.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     8878 2017-11-23 11:01:27.000000 django-admin-interface-0.9.2/admin_interface/migrations/0006_bytes_to_str.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      574 2017-11-23 11:01:31.000000 django-admin-interface-0.9.2/admin_interface/migrations/0007_add_favicon.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      791 2017-11-23 11:01:34.000000 django-admin-interface-0.9.2/admin_interface/migrations/0008_change_related_modal_background_opacity_type.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      782 2019-01-11 13:56:02.000000 django-admin-interface-0.9.2/admin_interface/migrations/0009_add_enviroment.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1590 2019-01-11 13:56:05.000000 django-admin-interface-0.9.2/admin_interface/migrations/0010_add_localization.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        0 2016-02-24 09:01:09.000000 django-admin-interface-0.9.2/admin_interface/migrations/__init__.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7852 2019-02-06 13:20:08.000000 django-admin-interface-0.9.2/admin_interface/models.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1289 2019-01-04 10:07:12.000000 django-admin-interface-0.9.2/admin_interface/settings.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/admin/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/admin/js/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      705 2019-02-06 15:57:16.000000 django-admin-interface-0.9.2/admin_interface/static/admin/js/cancel.js
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1903 2018-10-24 15:24:41.000000 django-admin-interface-0.9.2/admin_interface/static/admin/js/popup_response.js
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/admin_interface/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/admin_interface/magnific-popup/
--rwxr-xr-x   0 fabiocaccamo   (501) staff       (20)    60830 2017-05-11 13:43:47.000000 django-admin-interface-0.9.2/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js
--rwxr-xr-x   0 fabiocaccamo   (501) staff       (20)     6951 2017-04-12 14:38:26.000000 django-admin-interface-0.9.2/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/admin_interface/related-modal/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5018 2018-11-13 09:13:28.000000 django-admin-interface-0.9.2/admin_interface/static/admin_interface/related-modal/related-modal.js
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      265 2015-11-10 16:13:09.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/bower.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    15856 2015-11-10 16:13:10.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    36243 2015-11-10 16:13:12.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    34639 2015-11-10 16:13:10.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    36187 2015-11-10 16:13:11.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    38212 2015-11-10 16:13:11.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    36362 2015-11-10 16:13:11.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    22758 2015-11-10 16:13:13.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    33069 2015-11-10 16:13:13.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      261 2015-11-10 16:13:14.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/arrow.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      824 2015-11-10 16:13:14.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1792 2015-11-10 16:13:14.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1503 2015-11-10 16:13:14.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1616 2015-11-10 16:13:15.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2320 2015-11-10 16:13:15.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      736 2015-11-10 16:13:15.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      728 2015-11-10 16:13:16.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      953 2015-11-10 16:13:16.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1072 2015-11-10 16:13:16.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       42 2015-11-10 16:13:16.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/README.md
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    14994 2015-11-10 16:13:17.000000 django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/templates/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/templates/admin/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3333 2018-02-06 09:57:44.000000 django-admin-interface-0.9.2/admin_interface/templates/admin/base_site.html
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      659 2017-09-23 12:19:32.000000 django-admin-interface-0.9.2/admin_interface/templates/admin/filter.html
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      603 2017-07-13 15:13:19.000000 django-admin-interface-0.9.2/admin_interface/templates/admin/popup_response.html
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7855 2018-02-06 14:24:38.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/admin-interface-fix.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    13267 2018-01-31 11:13:53.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/admin-interface.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2719 2017-10-03 15:02:28.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/ckeditor.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5289 2018-02-06 09:41:30.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      232 2017-05-19 10:43:38.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/list-filter-dropdown.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      356 2018-02-05 11:06:20.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/modeltranslation.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      215 2017-05-23 15:50:20.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/recent-actions.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2077 2017-05-23 13:07:55.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/related-modal.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1451 2017-05-19 10:51:15.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/sorl-thumbnail.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      853 2018-02-06 14:27:44.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/tabbed-admin.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       77 2017-05-19 10:43:47.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/tinymce.css
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      504 2017-09-23 12:19:27.000000 django-admin-interface-0.9.2/admin_interface/templates/admin_interface/dropdown_filter.html
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/admin_interface/templatetags/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        0 2016-02-24 09:00:39.000000 django-admin-interface-0.9.2/admin_interface/templatetags/__init__.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      738 2018-02-01 13:52:26.000000 django-admin-interface-0.9.2/admin_interface/templatetags/admin_interface_tags.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       47 2019-02-06 13:21:00.000000 django-admin-interface-0.9.2/admin_interface/version.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/django_admin_interface.egg-info/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/django_admin_interface.egg-info/dependency_links.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7637 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/django_admin_interface.egg-info/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       89 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/django_admin_interface.egg-info/requires.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     4374 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/django_admin_interface.egg-info/SOURCES.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       16 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/django_admin_interface.egg-info/top_level.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1106 2016-02-24 09:12:19.000000 django-admin-interface-0.9.2/LICENSE.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      121 2017-09-29 10:17:14.000000 django-admin-interface-0.9.2/MANIFEST.in
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7637 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5082 2018-10-11 10:05:59.000000 django-admin-interface-0.9.2/README.md
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     4912 2018-10-10 13:49:57.000000 django-admin-interface-0.9.2/README.rst
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       79 2019-02-07 09:53:42.000000 django-admin-interface-0.9.2/setup.cfg
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2364 2018-10-10 13:04:02.000000 django-admin-interface-0.9.2/setup.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       90 2017-09-29 09:17:20.000000 django-admin-interface-0.9.3/admin_interface/__init__.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3087 2019-02-21 10:54:07.000000 django-admin-interface-0.9.3/admin_interface/admin.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      517 2019-01-04 10:54:08.000000 django-admin-interface-0.9.3/admin_interface/apps.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/fixtures/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1595 2017-05-24 08:59:52.000000 django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_bootstrap.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1591 2017-05-24 08:58:39.000000 django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_django.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1596 2017-05-24 08:59:00.000000 django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_foundation.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1592 2018-01-31 14:02:16.000000 django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_uswds.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1132 2017-05-24 10:01:48.000000 django-admin-interface-0.9.3/admin_interface/fixtures/initial_data.json
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/locale/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/locale/es/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/locale/es/LC_MESSAGES/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2562 2019-01-11 10:19:38.000000 django-admin-interface-0.9.3/admin_interface/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3728 2019-01-11 10:19:38.000000 django-admin-interface-0.9.3/admin_interface/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/locale/fr/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2503 2019-01-11 10:19:38.000000 django-admin-interface-0.9.3/admin_interface/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3695 2019-01-11 10:19:38.000000 django-admin-interface-0.9.3/admin_interface/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/locale/it/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/locale/it/LC_MESSAGES/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2468 2019-01-11 10:19:38.000000 django-admin-interface-0.9.3/admin_interface/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3600 2019-01-11 10:19:38.000000 django-admin-interface-0.9.3/admin_interface/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/migrations/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7501 2017-11-23 11:05:23.000000 django-admin-interface-0.9.3/admin_interface/migrations/0001_initial.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1824 2017-11-23 11:01:09.000000 django-admin-interface-0.9.3/admin_interface/migrations/0002_add_related_modal.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      898 2017-11-23 11:01:14.000000 django-admin-interface-0.9.3/admin_interface/migrations/0003_add_logo_color.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      404 2017-11-23 11:01:19.000000 django-admin-interface-0.9.3/admin_interface/migrations/0004_rename_title_color.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      483 2017-11-23 11:01:23.000000 django-admin-interface-0.9.3/admin_interface/migrations/0005_add_recent_actions_visible.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     8878 2017-11-23 11:01:27.000000 django-admin-interface-0.9.3/admin_interface/migrations/0006_bytes_to_str.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      574 2017-11-23 11:01:31.000000 django-admin-interface-0.9.3/admin_interface/migrations/0007_add_favicon.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      791 2017-11-23 11:01:34.000000 django-admin-interface-0.9.3/admin_interface/migrations/0008_change_related_modal_background_opacity_type.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      782 2019-01-11 13:56:02.000000 django-admin-interface-0.9.3/admin_interface/migrations/0009_add_enviroment.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1590 2019-01-11 13:56:05.000000 django-admin-interface-0.9.3/admin_interface/migrations/0010_add_localization.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        0 2016-02-24 09:01:09.000000 django-admin-interface-0.9.3/admin_interface/migrations/__init__.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     8169 2019-02-21 13:08:46.000000 django-admin-interface-0.9.3/admin_interface/models.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1289 2019-01-04 10:07:12.000000 django-admin-interface-0.9.3/admin_interface/settings.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/admin/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/admin/js/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      705 2019-02-06 15:52:53.000000 django-admin-interface-0.9.3/admin_interface/static/admin/js/cancel.js
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1903 2018-10-24 15:24:41.000000 django-admin-interface-0.9.3/admin_interface/static/admin/js/popup_response.js
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/favico/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    30766 2019-02-21 11:58:10.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.js
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     9302 2019-02-21 11:57:07.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.min.js
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/magnific-popup/
+-rwxr-xr-x   0 fabiocaccamo   (501) staff       (20)    60830 2017-05-11 13:43:47.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js
+-rwxr-xr-x   0 fabiocaccamo   (501) staff       (20)     6951 2017-04-12 14:38:26.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/related-modal/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5018 2018-11-13 09:13:28.000000 django-admin-interface-0.9.3/admin_interface/static/admin_interface/related-modal/related-modal.js
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      265 2015-11-10 16:13:09.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/bower.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    15856 2015-11-10 16:13:10.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    36243 2015-11-10 16:13:12.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    34639 2015-11-10 16:13:10.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    36187 2015-11-10 16:13:11.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    38212 2015-11-10 16:13:11.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    36362 2015-11-10 16:13:11.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    22758 2015-11-10 16:13:13.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    33069 2015-11-10 16:13:13.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      261 2015-11-10 16:13:14.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/arrow.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      824 2015-11-10 16:13:14.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1792 2015-11-10 16:13:14.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1503 2015-11-10 16:13:14.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1616 2015-11-10 16:13:15.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2320 2015-11-10 16:13:15.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      736 2015-11-10 16:13:15.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      728 2015-11-10 16:13:16.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      953 2015-11-10 16:13:16.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1072 2015-11-10 16:13:16.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       42 2015-11-10 16:13:16.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/README.md
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    14994 2015-11-10 16:13:17.000000 django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/templates/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/templates/admin/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2870 2019-02-21 13:13:19.000000 django-admin-interface-0.9.3/admin_interface/templates/admin/base_site.html
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      659 2017-09-23 12:19:32.000000 django-admin-interface-0.9.3/admin_interface/templates/admin/filter.html
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      603 2017-07-13 15:13:19.000000 django-admin-interface-0.9.3/admin_interface/templates/admin/popup_response.html
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7855 2018-02-06 14:24:38.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/admin-interface-fix.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    13368 2019-02-20 17:01:41.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/admin-interface.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2719 2017-10-03 15:02:28.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/ckeditor.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5289 2018-02-06 09:41:30.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      232 2017-05-19 10:43:38.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/list-filter-dropdown.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      356 2018-02-05 11:06:20.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/modeltranslation.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      215 2017-05-23 15:50:20.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/recent-actions.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2077 2017-05-23 13:07:55.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/related-modal.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1451 2017-05-19 10:51:15.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/sorl-thumbnail.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      853 2018-02-06 14:27:44.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/tabbed-admin.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       77 2017-05-19 10:43:47.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/tinymce.css
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      503 2019-02-21 13:14:39.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/dropdown_filter.html
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      509 2019-02-21 13:13:57.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/favicon.html
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      456 2019-02-21 13:13:47.000000 django-admin-interface-0.9.3/admin_interface/templates/admin_interface/related-modal.html
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/admin_interface/templatetags/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        0 2016-02-24 09:00:39.000000 django-admin-interface-0.9.3/admin_interface/templatetags/__init__.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      738 2018-02-01 13:52:26.000000 django-admin-interface-0.9.3/admin_interface/templatetags/admin_interface_tags.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       47 2019-02-21 13:16:08.000000 django-admin-interface-0.9.3/admin_interface/version.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/django_admin_interface.egg-info/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/django_admin_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7757 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/django_admin_interface.egg-info/PKG-INFO
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       89 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/django_admin_interface.egg-info/requires.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     4636 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/django_admin_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       16 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/django_admin_interface.egg-info/top_level.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1106 2016-02-24 09:12:19.000000 django-admin-interface-0.9.3/LICENSE.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      121 2017-09-29 10:17:14.000000 django-admin-interface-0.9.3/MANIFEST.in
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7757 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/PKG-INFO
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5220 2019-02-08 11:00:41.000000 django-admin-interface-0.9.3/README.md
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5016 2019-02-08 10:59:51.000000 django-admin-interface-0.9.3/README.rst
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       79 2019-02-21 17:05:51.000000 django-admin-interface-0.9.3/setup.cfg
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2364 2018-10-10 13:04:02.000000 django-admin-interface-0.9.3/setup.py
```

### Comparing `django-admin-interface-0.9.2/admin_interface/admin.py` & `django-admin-interface-0.9.3/admin_interface/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/apps.py` & `django-admin-interface-0.9.3/admin_interface/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_bootstrap.json` & `django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_bootstrap.json`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_django.json` & `django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_django.json`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_foundation.json` & `django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_foundation.json`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/fixtures/admin_interface_theme_uswds.json` & `django-admin-interface-0.9.3/admin_interface/fixtures/admin_interface_theme_uswds.json`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/fixtures/initial_data.json` & `django-admin-interface-0.9.3/admin_interface/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/locale/es/LC_MESSAGES/django.mo` & `django-admin-interface-0.9.3/admin_interface/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/locale/es/LC_MESSAGES/django.po` & `django-admin-interface-0.9.3/admin_interface/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/locale/fr/LC_MESSAGES/django.mo` & `django-admin-interface-0.9.3/admin_interface/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/locale/fr/LC_MESSAGES/django.po` & `django-admin-interface-0.9.3/admin_interface/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/locale/it/LC_MESSAGES/django.mo` & `django-admin-interface-0.9.3/admin_interface/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/locale/it/LC_MESSAGES/django.po` & `django-admin-interface-0.9.3/admin_interface/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0001_initial.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0002_add_related_modal.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0002_add_related_modal.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0003_add_logo_color.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0003_add_logo_color.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0006_bytes_to_str.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0006_bytes_to_str.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0007_add_favicon.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0007_add_favicon.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0008_change_related_modal_background_opacity_type.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0008_change_related_modal_background_opacity_type.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0009_add_enviroment.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0009_add_enviroment.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/migrations/0010_add_localization.py` & `django-admin-interface-0.9.3/admin_interface/migrations/0010_add_localization.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/models.py` & `django-admin-interface-0.9.3/admin_interface/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,28 +89,43 @@
 
     favicon = models.FileField(
         upload_to='admin-interface/favicon/',
         blank=True,
         help_text=_('(.ico|.png|.gif - 16x16|32x32 px)'),
         verbose_name=_('favicon'))
 
+    envs = (
+        'development',
+        'testing',
+        'staging',
+        'production',
+    )
     env_choices = (
-        ('development', _('Development'), ),
-        ('testing', _('Testing'), ),
-        ('staging', _('Staging'), ),
-        ('production', _('Production'), ),
+        (envs[0], _('Development'), ),
+        (envs[1], _('Testing'), ),
+        (envs[2], _('Staging'), ),
+        (envs[3], _('Production'), ),
     )
     env = models.CharField(
         max_length=50,
         choices=env_choices,
-        default='development',
+        default=env_choices[0][0],
         verbose_name=_('environment'))
     env_visible = models.BooleanField(
         default=True,
         verbose_name=_('visible'))
+    env_colors = {
+        envs[0]: '#e74c3c',
+        envs[1]: '#e67e22',
+        envs[2]: '#f1c40f',
+        envs[3]: '#2ecc71',
+    }
+    @property
+    def env_color(self):
+        return Theme.env_colors.get(self.env, '')
 
     css_header_background_color = ColorField(
         blank=True,
         default='#0C4B33',
         help_text='#0C4B33',
         max_length=10,
         verbose_name=_('background color'))
```

### Comparing `django-admin-interface-0.9.2/admin_interface/settings.py` & `django-admin-interface-0.9.3/admin_interface/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/admin/js/cancel.js` & `django-admin-interface-0.9.3/admin_interface/static/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/admin/js/popup_response.js` & `django-admin-interface-0.9.3/admin_interface/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js` & `django-admin-interface-0.9.3/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css` & `django-admin-interface-0.9.3/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/admin_interface/related-modal/related-modal.js` & `django-admin-interface-0.9.3/admin_interface/static/admin_interface/related-modal/related-modal.js`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js` & `django-admin-interface-0.9.3/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin/base_site.html` & `django-admin-interface-0.9.3/admin_interface/templates/admin/base_site.html`

 * *Files 10% similar despite different names*

```diff
@@ -36,22 +36,16 @@
 {% block blockbots %}
 {{ block.super }}
 {% get_admin_interface_theme as theme %}
 {% get_admin_interface_version as version %}
 {# https://github.com/elky/django-flat-responsive#important-note #}
 <meta name="viewport" content="user-scalable=no, width=device-width, initial-scale=1.0, maximum-scale=1.0">
 <link rel="stylesheet" type="text/css" href="{% static 'admin/css/responsive.css' %}?v={{ version }}" />
-{% if theme.favicon %}
-<link rel="icon" type="image/x-icon" href="{{ theme.favicon.url }}?v={{ version }}" />
-{% endif %}
-{% if theme.related_modal_active %}
-<link rel="stylesheet" type="text/css" href="{% static 'admin_interface/magnific-popup/magnific-popup.css' %}?v={{ version }}" />
-<script type="text/javascript" src="{% static 'admin_interface/magnific-popup/jquery.magnific-popup.js' %}?v={{ version }}"></script>
-<script type="text/javascript" src="{% static 'admin_interface/related-modal/related-modal.js' %}?v={{ version }}"></script>
-{% endif %}
+{% include "admin_interface/favicon.html" %}
+{% include "admin_interface/related-modal.html" %}
 {% endblock %}
 
 {% block bodyclass %}admin-interface flat-theme {% get_admin_interface_theme as theme %}{% if theme.name %}{{ theme.name|slugify }}-theme{% endif %}{% endblock %}
 
 {% block branding %}
 {% get_admin_interface_theme as theme %}
 <h1 id="site-name">
```

#### html2text {}

```diff
@@ -4,19 +4,18 @@
 { site_title|default:_('Django administration') }}{% endif %} {% endblock %} {%
 block extrastyle %} {% get_admin_interface_theme as theme %} {%
 get_admin_interface_version as version %}
  {% endblock %} {% block blockbots %} {{ block.super }} {%
 get_admin_interface_theme as theme %} {% get_admin_interface_version as version
 %} {# https://github.com/elky/django-flat-responsive#important-note #}
 
- {% if theme.favicon %}
- {% endif %} {% if theme.related_modal_active %}
- {% endif %} {% endblock %} {% block bodyclass %}admin-interface flat-theme {%
-get_admin_interface_theme as theme %}{% if theme.name %}{{ theme.name|slugify
-}}-theme{% endif %}{% endblock %} {% block branding %} {%
+ {% include "admin_interface/favicon.html" %} {% include "admin_interface/
+related-modal.html" %} {% endblock %} {% block bodyclass %}admin-interface
+flat-theme {% get_admin_interface_theme as theme %}{% if theme.name %}{
+{ theme.name|slugify }}-theme{% endif %}{% endblock %} {% block branding %} {%
 get_admin_interface_theme as theme %}
 ****** {% if theme.logo_visible %} {% if theme.logo %} % if theme.logo.width
 %}width="{{ theme.logo.width }}"{% endif %} {% if theme.logo.height %}height="{
 { theme.logo.height }}"{% endif %} /> {% else %} [data:image/
 gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7] {% endif
 %} {% endif %} {% if theme.title_visible %} {% if theme.title %}{% trans
 theme.title %}{% else %}{% trans 'Django administration' %}{% endif %} {% endif
```

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin/filter.html` & `django-admin-interface-0.9.3/admin_interface/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin/popup_response.html` & `django-admin-interface-0.9.3/admin_interface/templates/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/admin-interface-fix.css` & `django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/admin-interface-fix.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/admin-interface.css` & `django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/admin-interface.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .admin-interface #header {
-    background:{{ theme.css_header_background_color }};
-    color:{{ theme.css_header_text_color }};
+    background: {{ theme.css_header_background_color }};
+    color: {{ theme.css_header_text_color }};
 }
 
 .admin-interface .enviroment-label {
 }
 
 .admin-interface .enviroment-label::before {
     content: "";
@@ -16,27 +16,27 @@
     margin-right: 6px;
     box-sizing: border-box;
     -moz-box-sizing: border-box;
     -webkit-box-sizing: border-box;
 }
 
 .admin-interface .enviroment-label.development::before {
-    background-color: #e74c3c;
+    background-color: {{ theme.env_colors.development }};
 }
 
 .admin-interface .enviroment-label.testing::before {
-    background-color: #e67e22;
+    background-color: {{ theme.env_colors.testing }};
 }
 
 .admin-interface .enviroment-label.staging::before {
-    background-color: #f1c40f;
+    background-color: {{ theme.env_colors.staging }};
 }
 
 .admin-interface .enviroment-label.production::before {
-    background-color: #2ecc71;
+    background-color: {{ theme.env_colors.production }};
 }
 
 .admin-interface .enviroment-label::after {
     content: "";
 }
 
 .admin-interface .enviroment-label.development::after {
```

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/ckeditor.css` & `django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/ckeditor.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css` & `django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/related-modal.css` & `django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/related-modal.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/sorl-thumbnail.css` & `django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/sorl-thumbnail.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templates/admin_interface/css/tabbed-admin.css` & `django-admin-interface-0.9.3/admin_interface/templates/admin_interface/css/tabbed-admin.css`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/admin_interface/templatetags/admin_interface_tags.py` & `django-admin-interface-0.9.3/admin_interface/templatetags/admin_interface_tags.py`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/django_admin_interface.egg-info/PKG-INFO` & `django-admin-interface-0.9.3/django_admin_interface.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: django-admin-interface
-Version: 0.9.2
+Version: 0.9.3
 Summary: django-admin-interface is a modern responsive flat admin interface customizable by the admin itself.
 Home-page: https://github.com/fabiocaccamo/django-admin-interface
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/django-admin-interface/archive/0.9.2.tar.gz
-Description: |Build Status| |codecov| |Code Health| |PyPI version| |Py versions| |License|
+Download-URL: https://github.com/fabiocaccamo/django-admin-interface/archive/0.9.3.tar.gz
+Description: |Build Status| |codecov| |Code Health| |PyPI version| |PyPI downloads| |Py versions| |License|
         
         django-admin-interface
         ======================
         
         django-admin-interface is a modern **responsive flat admin interface
         customizable by the admin itself**.
         
@@ -142,14 +142,16 @@
         
         .. |codecov| image:: https://codecov.io/gh/fabiocaccamo/django-admin-interface/branch/master/graph/badge.svg
         
         .. |Code Health| image:: https://landscape.io/github/fabiocaccamo/django-admin-interface/master/landscape.svg?style=flat
         
         .. |PyPI version| image:: https://badge.fury.io/py/django-admin-interface.svg
         
+        .. |PyPI downloads| image:: https://img.shields.io/pypi/dm/django-admin-interface.svg
+        
         .. |Py versions| image:: https://img.shields.io/pypi/pyversions/django-admin-interface.svg
         
         .. |License| image:: https://img.shields.io/pypi/l/django-admin-interface.svg
         
         .. |django-admin-interface_preview| image:: https://user-images.githubusercontent.com/1035294/35631521-64b0cab8-06a4-11e8-8f57-c04fdfbb7e8b.gif
         
         .. |django-admin-interface_login| image:: https://cloud.githubusercontent.com/assets/1035294/11240233/55c8d4ba-8df1-11e5-9568-00fdc987ede8.gif
```

### Comparing `django-admin-interface-0.9.2/django_admin_interface.egg-info/SOURCES.txt` & `django-admin-interface-0.9.3/django_admin_interface.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 admin_interface/migrations/0007_add_favicon.py
 admin_interface/migrations/0008_change_related_modal_background_opacity_type.py
 admin_interface/migrations/0009_add_enviroment.py
 admin_interface/migrations/0010_add_localization.py
 admin_interface/migrations/__init__.py
 admin_interface/static/admin/js/cancel.js
 admin_interface/static/admin/js/popup_response.js
+admin_interface/static/admin_interface/favico/favico-0.3.10-patched.js
+admin_interface/static/admin_interface/favico/favico-0.3.10-patched.min.js
 admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js
 admin_interface/static/admin_interface/magnific-popup/magnific-popup.css
 admin_interface/static/admin_interface/related-modal/related-modal.js
 admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE
 admin_interface/static/ckeditor/ckeditor/skins/light/README.md
 admin_interface/static/ckeditor/ckeditor/skins/light/bower.json
 admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css
@@ -58,14 +60,16 @@
 admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png
 admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png
 admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png
 admin_interface/templates/admin/base_site.html
 admin_interface/templates/admin/filter.html
 admin_interface/templates/admin/popup_response.html
 admin_interface/templates/admin_interface/dropdown_filter.html
+admin_interface/templates/admin_interface/favicon.html
+admin_interface/templates/admin_interface/related-modal.html
 admin_interface/templates/admin_interface/css/admin-interface-fix.css
 admin_interface/templates/admin_interface/css/admin-interface.css
 admin_interface/templates/admin_interface/css/ckeditor.css
 admin_interface/templates/admin_interface/css/jquery.ui.tabs.css
 admin_interface/templates/admin_interface/css/list-filter-dropdown.css
 admin_interface/templates/admin_interface/css/modeltranslation.css
 admin_interface/templates/admin_interface/css/recent-actions.css
```

### Comparing `django-admin-interface-0.9.2/LICENSE.txt` & `django-admin-interface-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-admin-interface-0.9.2/PKG-INFO` & `django-admin-interface-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: django-admin-interface
-Version: 0.9.2
+Version: 0.9.3
 Summary: django-admin-interface is a modern responsive flat admin interface customizable by the admin itself.
 Home-page: https://github.com/fabiocaccamo/django-admin-interface
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/django-admin-interface/archive/0.9.2.tar.gz
-Description: |Build Status| |codecov| |Code Health| |PyPI version| |Py versions| |License|
+Download-URL: https://github.com/fabiocaccamo/django-admin-interface/archive/0.9.3.tar.gz
+Description: |Build Status| |codecov| |Code Health| |PyPI version| |PyPI downloads| |Py versions| |License|
         
         django-admin-interface
         ======================
         
         django-admin-interface is a modern **responsive flat admin interface
         customizable by the admin itself**.
         
@@ -142,14 +142,16 @@
         
         .. |codecov| image:: https://codecov.io/gh/fabiocaccamo/django-admin-interface/branch/master/graph/badge.svg
         
         .. |Code Health| image:: https://landscape.io/github/fabiocaccamo/django-admin-interface/master/landscape.svg?style=flat
         
         .. |PyPI version| image:: https://badge.fury.io/py/django-admin-interface.svg
         
+        .. |PyPI downloads| image:: https://img.shields.io/pypi/dm/django-admin-interface.svg
+        
         .. |Py versions| image:: https://img.shields.io/pypi/pyversions/django-admin-interface.svg
         
         .. |License| image:: https://img.shields.io/pypi/l/django-admin-interface.svg
         
         .. |django-admin-interface_preview| image:: https://user-images.githubusercontent.com/1035294/35631521-64b0cab8-06a4-11e8-8f57-c04fdfbb7e8b.gif
         
         .. |django-admin-interface_login| image:: https://cloud.githubusercontent.com/assets/1035294/11240233/55c8d4ba-8df1-11e5-9568-00fdc987ede8.gif
```

### Comparing `django-admin-interface-0.9.2/README.md` & `django-admin-interface-0.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![Build Status](https://travis-ci.org/fabiocaccamo/django-admin-interface.svg?branch=master)](https://travis-ci.org/fabiocaccamo/django-admin-interface)
 [![codecov](https://codecov.io/gh/fabiocaccamo/django-admin-interface/branch/master/graph/badge.svg)](https://codecov.io/gh/fabiocaccamo/django-admin-interface)
 [![Code Health](https://landscape.io/github/fabiocaccamo/django-admin-interface/master/landscape.svg?style=flat)](https://landscape.io/github/fabiocaccamo/django-admin-interface/master)
 [![PyPI version](https://badge.fury.io/py/django-admin-interface.svg)](https://badge.fury.io/py/django-admin-interface)
+[![PyPI downloads](https://img.shields.io/pypi/dm/django-admin-interface.svg)](https://img.shields.io/pypi/dm/django-admin-interface.svg)
 [![Py versions](https://img.shields.io/pypi/pyversions/django-admin-interface.svg)](https://img.shields.io/pypi/pyversions/django-admin-interface.svg)
 [![License](https://img.shields.io/pypi/l/django-admin-interface.svg)](https://img.shields.io/pypi/l/django-admin-interface.svg)
 
 # django-admin-interface
 django-admin-interface is a modern **responsive flat admin interface customizable by the admin itself**.
 
 ![django-admin-interface-preview](https://user-images.githubusercontent.com/1035294/35631521-64b0cab8-06a4-11e8-8f57-c04fdfbb7e8b.gif)
```

### Comparing `django-admin-interface-0.9.2/README.rst` & `django-admin-interface-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|Build Status| |codecov| |Code Health| |PyPI version| |Py versions| |License|
+|Build Status| |codecov| |Code Health| |PyPI version| |PyPI downloads| |Py versions| |License|
 
 django-admin-interface
 ======================
 
 django-admin-interface is a modern **responsive flat admin interface
 customizable by the admin itself**.
 
@@ -133,14 +133,16 @@
 
 .. |codecov| image:: https://codecov.io/gh/fabiocaccamo/django-admin-interface/branch/master/graph/badge.svg
 
 .. |Code Health| image:: https://landscape.io/github/fabiocaccamo/django-admin-interface/master/landscape.svg?style=flat
 
 .. |PyPI version| image:: https://badge.fury.io/py/django-admin-interface.svg
 
+.. |PyPI downloads| image:: https://img.shields.io/pypi/dm/django-admin-interface.svg
+
 .. |Py versions| image:: https://img.shields.io/pypi/pyversions/django-admin-interface.svg
 
 .. |License| image:: https://img.shields.io/pypi/l/django-admin-interface.svg
 
 .. |django-admin-interface_preview| image:: https://user-images.githubusercontent.com/1035294/35631521-64b0cab8-06a4-11e8-8f57-c04fdfbb7e8b.gif
 
 .. |django-admin-interface_login| image:: https://cloud.githubusercontent.com/assets/1035294/11240233/55c8d4ba-8df1-11e5-9568-00fdc987ede8.gif
```

### Comparing `django-admin-interface-0.9.2/setup.py` & `django-admin-interface-0.9.3/setup.py`

 * *Files identical despite different names*


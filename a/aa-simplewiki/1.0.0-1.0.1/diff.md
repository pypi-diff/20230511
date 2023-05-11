# Comparing `tmp/aa-simplewiki-1.0.0.tar.gz` & `tmp/aa-simplewiki-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-simplewiki-1.0.0.tar", last modified: Sat Apr 29 20:16:46 2023, max compression
+gzip compressed data, was "aa-simplewiki-1.0.1.tar", last modified: Thu May 11 04:40:44 2023, max compression
```

## Comparing `aa-simplewiki-1.0.0.tar` & `aa-simplewiki-1.0.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/LICENSE
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/MANIFEST.in
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4701 2023-04-29 20:02:43.000000 aa-simplewiki-1.0.0/README.md
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.033726 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/SOURCES.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/dependency_links.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-29 20:14:32.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/not-zip-safe
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/requires.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/top_level.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/pyproject.toml
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/setup.cfg
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1205 2023-04-29 20:16:39.000000 aa-simplewiki-1.0.0/setup.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.033726 aa-simplewiki-1.0.0/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       48 2023-04-29 20:15:23.000000 aa-simplewiki-1.0.0/simplewiki/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/admin.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11877 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/admin_helper_menus.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/admin_helper_sections.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/app_settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/apps.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/auth_hooks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/migrations/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0001_initial.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0002_pageitem_page_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0003_menuitem_icon.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0010_rename_path_menuitem_name.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0011_rename_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0012_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0013_alter_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0018_rename_group_menuitem_groups.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0019_alter_general_options.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0020_menuitem_parent.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/models.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.029726 aa-simplewiki-1.0.0/simplewiki/static/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/static/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/static/simplewiki/.gitkeep
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/static/simplewiki/custom.css
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/tasks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.029726 aa-simplewiki-1.0.0/simplewiki/templates/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/base.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/dynamic_page.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6552 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_menus.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-04-29 19:49:06.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_sections.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2311 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2345 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/error.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/index.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/search.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templatetags/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2121 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templatetags/custom_filters.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templatetags/markdown_filters.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/tests/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/tests/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/tests/test_example.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12689 2023-04-29 20:15:58.000000 aa-simplewiki-1.0.0/simplewiki/views.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/testauth/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/celery.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/wsgi.py
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)    35164 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/LICENSE
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      123 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/MANIFEST.in
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     5719 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/PKG-INFO
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     4701 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/README.md
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.724061 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     5719 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/PKG-INFO
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2607 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        1 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        1 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/not-zip-safe
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       24 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/requires.txt
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       20 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/top_level.txt
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      104 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/pyproject.toml
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1462 2023-05-11 04:40:44.740062 aa-simplewiki-1.0.1/setup.cfg
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1205 2023-05-11 04:38:56.000000 aa-simplewiki-1.0.1/setup.py
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.728061 aa-simplewiki-1.0.1/simplewiki/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       48 2023-05-11 04:39:37.000000 aa-simplewiki-1.0.1/simplewiki/__init__.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      231 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/admin.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)    11877 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/admin_helper_menus.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     8956 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/admin_helper_sections.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      169 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/app_settings.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      284 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/apps.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1076 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/auth_hooks.py
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.732061 aa-simplewiki-1.0.1/simplewiki/migrations/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1489 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0001_initial.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      395 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0002_pageitem_page_title.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      401 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0003_menuitem_icon.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1532 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1522 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      374 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      392 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1657 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      658 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      381 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0010_rename_path_menuitem_name.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      372 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0011_rename_name_menuitem_path.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      576 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0012_menuitem_group.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      579 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0013_alter_menuitem_group.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     3030 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      685 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      407 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      831 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      399 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0018_rename_group_menuitem_groups.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      492 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0019_alter_general_options.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      538 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0020_menuitem_parent.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        0 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/__init__.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     4236 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/models.py
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.724061 aa-simplewiki-1.0.1/simplewiki/static/
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.732061 aa-simplewiki-1.0.1/simplewiki/static/simplewiki/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        0 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/static/simplewiki/.gitkeep
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      199 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/static/simplewiki/custom.css
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      226 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/tasks.py
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.724061 aa-simplewiki-1.0.1/simplewiki/templates/
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.732061 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     6324 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/base.html
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1076 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/dynamic_page.html
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     6630 2023-05-11 04:36:11.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_menus.html
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     9500 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_sections.html
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2320 2023-05-10 23:16:59.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2468 2023-05-10 23:16:44.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      593 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/error.html
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      460 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/index.html
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1578 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/search.html
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/templatetags/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2121 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templatetags/custom_filters.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      407 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templatetags/markdown_filters.py
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/tests/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       27 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/tests/__init__.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      448 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/tests/test_example.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      488 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/urls.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)    12689 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/views.py
+drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/testauth/
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       52 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/__init__.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      654 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/celery.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     9481 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/settings.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      167 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/urls.py
+-rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      425 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/wsgi.py
```

### Comparing `aa-simplewiki-1.0.0/LICENSE` & `aa-simplewiki-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/PKG-INFO` & `aa-simplewiki-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `aa-simplewiki-1.0.0/README.md` & `aa-simplewiki-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/aa_simplewiki.egg-info/PKG-INFO` & `aa-simplewiki-1.0.1/aa_simplewiki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `aa-simplewiki-1.0.0/aa_simplewiki.egg-info/SOURCES.txt` & `aa-simplewiki-1.0.1/aa_simplewiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/setup.cfg` & `aa-simplewiki-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/setup.py` & `aa-simplewiki-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/admin_helper_menus.py` & `aa-simplewiki-1.0.1/simplewiki/admin_helper_menus.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/admin_helper_sections.py` & `aa-simplewiki-1.0.1/simplewiki/admin_helper_sections.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/auth_hooks.py` & `aa-simplewiki-1.0.1/simplewiki/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0001_initial.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0012_menuitem_group.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0012_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0013_alter_menuitem_group.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0013_alter_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/migrations/0020_menuitem_parent.py` & `aa-simplewiki-1.0.1/simplewiki/migrations/0020_menuitem_parent.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/models.py` & `aa-simplewiki-1.0.1/simplewiki/models.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/base.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/base.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/dynamic_page.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/dynamic_page.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_menus.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_menus.html`

 * *Files 8% similar despite different names*

```diff
@@ -139,34 +139,40 @@
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
 {% if user_action == 'edit' %}
 {# groupInput needs to be seperated, otherwise it won't find the input #}
 <script>
-  document.getElementById("groupInput").value = '{{ selectedMenu.groups|escapejs }}';
-</script>
-<script>
-  document.getElementById("indexInput").value = '{{ selectedMenu.index|escapejs }}';
-  document.getElementById("titleInput").value = '{{ selectedMenu.title|escapejs }}';
-  document.getElementById("iconInput").value = '{{ selectedMenu.icon|escapejs }}';
-  document.getElementById("parentInput").value = '{{ selectedMenu.parent|escapejs }}';
-  document.getElementById("pathInput").value = '{{ selectedMenu.path|escapejs }}';
-</script>
-<script>
+  const selectElement = document.getElementById("menuParentSelect");
+  const selectedPath = "{{ selectedMenu.menu_path }}";
+
+  for (let i = 0; i < menuParentSelect.options.length; i++) {
+          if (menuParentSelect.options[i].value == selectedPath) {
+              menuParentSelect.options[i].selected = true;
+              break;
+          }
+      }
+
   document.addEventListener('DOMContentLoaded', function() {
       const menuParentSelect = document.getElementById('menuParentSelect');
-      const selectedPath = "{{ selectedMenu.menu_path }}";
+      const selectedPath = "{{ selectedMenu.parent }}";
 
       for (let i = 0; i < menuParentSelect.options.length; i++) {
           if (menuParentSelect.options[i].value == selectedPath) {
               menuParentSelect.options[i].selected = true;
               break;
           }
       }
   });
 </script>
+<script>
+  document.getElementById("indexInput").value = '{{ selectedMenu.index|escapejs }}';
+  document.getElementById("titleInput").value = '{{ selectedMenu.title|escapejs }}';
+  document.getElementById("iconInput").value = '{{ selectedMenu.icon|escapejs }}';
+</script>
+
 {% endif %}
 {% endblock %}
 
 {% block extra_script %}
 {% endblock %}
```

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_sections.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_sections.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_create_menu.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_create_menu.html`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       {% endfor %}
     </select>
     <p class="help-block">Optional: Select the parent menu here. If you leave it at 'None' it will be the parent. For example: welcome</p>
   </div>
   <div class="form-group">
     <label for="menuPathSelect">Groups:</label>
     <select multiple class="form-control" name="group_select" id="menuGroupSelect">
-      <option value="none">None</option>
+      <option value="none" selected>None</option>
       {% for group_item in all_groups %}
         <option value="{{ group_item.name }}">{{ group_item.name }}</option>
       {% endfor %}
     </select>
     <p class="help-block">Optional: Select the groups who are able to access this menu. You can select multiple.</p>
   </div>
   <button type="submit" name="confirm_create" value="0" class="btn btn-default">Cancel</button>
```

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
       {% endfor %}
     </select>
     <p class="help-block">Optional: Select the parent menu here. If you leave it at 'None' it will be the parent. For example: welcome</p>
   </div>
   <div class="form-group">
     <label for="menuPathSelect">Groups:</label>
     <select multiple class="form-control" name="group_select" id="menuGroupSelect">
-      <option value="none">None</option>
+      <option value="none" {% if selectedMenu.groups == "" %}selected{% endif %} >None</option>
       {% for group_item in all_groups %}
-        <option value="{{ group_item.name }}">{{ group_item.name }}</option>
+        <option value="{{ group_item.name }}" {% if group_item.name in selectedMenu.groups %} selected{% endif %}>{{ group_item.name }}</option>
       {% endfor %}
     </select>
     <p class="help-block">Optional: Select the groups who are able to access this menu. You can select multiple.</p>
   </div>
   <button type="submit" name="confirm_edit" value="0" class="btn btn-default">Cancel</button>
   <div class="pull-right">
     <button type="submit" name="confirm_edit" value="1" class="btn btn-success">Save</button>
```

#### html2text {}

```diff
@@ -8,14 +8,16 @@
 icons. We only support free icons. Format example: fas fa-hand-spock
 {% for menu_item in menu_items %} {% if not menu_item.parent and
 selectedMenu.path != menu_item.path %}
 {{ menu_item.title }}
 {% endif %} {% endfor %}
 Optional: Select the parent menu here. If you leave it at 'None' it will be the
 parent. For example: welcome
+% if selectedMenu.groups == "" %}selected{% endif %} >None
 {% for group_item in all_groups %}
-{{ group_item.name }}
+% if group_item.name in selectedMenu.groups %} selected{% endif %}>{
+{ group_item.name }}
 {% endfor %}
 Optional: Select the groups who are able to access this menu. You can select
 multiple.
 Cancel
 Save
```

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/error.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/error.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/search.html` & `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/search.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/templatetags/custom_filters.py` & `aa-simplewiki-1.0.1/simplewiki/templatetags/custom_filters.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/simplewiki/views.py` & `aa-simplewiki-1.0.1/simplewiki/views.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/testauth/celery.py` & `aa-simplewiki-1.0.1/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.0/testauth/settings.py` & `aa-simplewiki-1.0.1/testauth/settings.py`

 * *Files identical despite different names*


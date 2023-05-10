# Comparing `tmp/wagtail_sb_socialnetworks-0.6.0.tar.gz` & `tmp/wagtail_sb_socialnetworks-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_socialnetworks-0.6.0.tar", max compression
+gzip compressed data, was "wagtail_sb_socialnetworks-0.7.0.tar", max compression
```

## Comparing `wagtail_sb_socialnetworks-0.6.0.tar` & `wagtail_sb_socialnetworks-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      817 2023-04-29 21:57:06.429894 wagtail_sb_socialnetworks-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2022-12-12 01:51:13.643284 wagtail_sb_socialnetworks-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1661 2023-04-15 13:45:43.322506 wagtail_sb_socialnetworks-0.6.0/README.md
--rw-r--r--   0        0        0     1996 2023-04-29 21:57:06.421894 wagtail_sb_socialnetworks-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       88 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/admin.py
--rw-r--r--   0        0        0      180 2023-04-17 03:43:34.273612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/apps.py
--rw-r--r--   0        0        0     1069 2023-04-29 21:48:38.016239 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/compat.py
--rw-r--r--   0        0        0     1204 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4536 2023-04-17 03:43:34.289612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py
--rw-r--r--   0        0        0      684 2023-04-17 03:43:34.289612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py
--rw-r--r--   0        0        0      574 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py
--rw-r--r--   0        0        0        0 2023-04-17 03:43:34.293612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/__init__.py
--rw-r--r--   0        0        0     3177 2023-04-29 21:55:17.869551 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/models.py
--rw-r--r--   0        0        0        0 2023-04-17 03:43:34.265612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/tests.py
--rw-r--r--   0        0        0       20 2023-04-29 21:57:06.433894 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/version.py
--rw-r--r--   0        0        0        0 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/views.py
--rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 wagtail_sb_socialnetworks-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      873 2023-05-10 23:16:34.484356 wagtail_sb_socialnetworks-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2022-12-12 01:51:13.643284 wagtail_sb_socialnetworks-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1661 2023-04-15 13:45:43.322506 wagtail_sb_socialnetworks-0.7.0/README.md
+-rw-r--r--   0        0        0     1996 2023-05-10 23:16:34.472356 wagtail_sb_socialnetworks-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/admin.py
+-rw-r--r--   0        0        0      180 2023-04-17 03:43:34.273612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/apps.py
+-rw-r--r--   0        0        0     1069 2023-04-29 21:57:57.382065 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/compat.py
+-rw-r--r--   0        0        0     1204 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4536 2023-04-17 03:43:34.289612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py
+-rw-r--r--   0        0        0      684 2023-04-17 03:43:34.289612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py
+-rw-r--r--   0        0        0      574 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.293612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/migrations/__init__.py
+-rw-r--r--   0        0        0     3177 2023-04-29 21:57:57.382065 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/models.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.265612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/tests.py
+-rw-r--r--   0        0        0       20 2023-05-10 23:16:34.500356 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/version.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/views.py
+-rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 wagtail_sb_socialnetworks-0.7.0/PKG-INFO
```

### Comparing `wagtail_sb_socialnetworks-0.6.0/CHANGELOG.md` & `wagtail_sb_socialnetworks-0.7.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.7.0] - 2023-05-10
+
+* Add support for Wagtail 5.x
+
 ## [0.6.0] - 2023-04-29
 
 * Move compatibility handling to `compat` module
 ## [0.5.0] - 2023-04-15
 
 - Drop support for python 3.8.0
 - Drop codecov from development dependencies
```

### Comparing `wagtail_sb_socialnetworks-0.6.0/LICENSE.txt` & `wagtail_sb_socialnetworks-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/README.md` & `wagtail_sb_socialnetworks-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/pyproject.toml` & `wagtail_sb_socialnetworks-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtail-sb-socialnetworks"
-version = "0.6.0"
+version = "0.7.0"
 description = "Social Networks settings for wagtail sites."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -28,22 +28,22 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.6.0/wagtail-sb-socialnetworks-v0.6.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.7.0/wagtail-sb-socialnetworks-v0.7.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">= 3.8.1, < 4.0.0"
 Django = "< 5.0"
-wagtail = "< 5.0"
+wagtail = "< 6.0"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
 bandit = "^1.7.4"
 black = "^23.1.0"
 coverage = "^7.1.0"
 flake8 = "^6.0.0"
```

### Comparing `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/compat.py` & `wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/compat.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po` & `wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py` & `wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py` & `wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py` & `wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/models.py` & `wagtail_sb_socialnetworks-0.7.0/src/wagtail_sb_socialnetworks/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.6.0/PKG-INFO` & `wagtail_sb_socialnetworks-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-sb-socialnetworks
-Version: 0.6.0
+Version: 0.7.0
 Summary: Social Networks settings for wagtail sites.
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -18,18 +18,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (<5.0)
-Requires-Dist: wagtail (<5.0)
+Requires-Dist: wagtail (<6.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.6.0/wagtail-sb-socialnetworks-v0.6.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.7.0/wagtail-sb-socialnetworks-v0.7.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-socialnetworks)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-socialnetworks)
```


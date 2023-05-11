# Comparing `tmp/odoo_image_changelog-0.1.3.tar.gz` & `tmp/odoo_image_changelog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_image_changelog-0.1.3.tar", last modified: Fri Apr 28 08:48:45 2023, max compression
+gzip compressed data, was "odoo_image_changelog-0.2.0.tar", last modified: Thu May 11 09:56:46 2023, max compression
```

## Comparing `odoo_image_changelog-0.1.3.tar` & `odoo_image_changelog-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 08:48:45.985286 odoo_image_changelog-0.1.3/
--rw-r--r--   0 vrenaville  (1110) docker     (998)     1799 2023-04-20 08:54:35.000000 odoo_image_changelog-0.1.3/.gitignore
--rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 08:48:45.985286 odoo_image_changelog-0.1.3/PKG-INFO
--rw-r--r--   0 vrenaville  (1110) docker     (998)        0 2023-04-20 09:33:13.000000 odoo_image_changelog-0.1.3/README.rst
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 08:48:45.985286 odoo_image_changelog-0.1.3/odoo_image_changelog/
--rw-r--r--   0 vrenaville  (1110) docker     (998)      132 2023-04-28 08:48:20.000000 odoo_image_changelog-0.1.3/odoo_image_changelog/__init__.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)     4902 2023-04-20 09:36:51.000000 odoo_image_changelog-0.1.3/odoo_image_changelog/github_helpers.py
--rw-r--r--   0 vrenaville  (1110) docker     (998)     4812 2023-04-28 08:46:09.000000 odoo_image_changelog-0.1.3/odoo_image_changelog/main.py
-drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-04-28 08:48:45.985286 odoo_image_changelog-0.1.3/odoo_image_changelog.egg-info/
--rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-04-28 08:48:45.000000 odoo_image_changelog-0.1.3/odoo_image_changelog.egg-info/PKG-INFO
--rw-r--r--   0 vrenaville  (1110) docker     (998)      397 2023-04-28 08:48:45.000000 odoo_image_changelog-0.1.3/odoo_image_changelog.egg-info/SOURCES.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)        1 2023-04-28 08:48:45.000000 odoo_image_changelog-0.1.3/odoo_image_changelog.egg-info/dependency_links.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       71 2023-04-28 08:48:45.000000 odoo_image_changelog-0.1.3/odoo_image_changelog.egg-info/entry_points.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 08:48:45.000000 odoo_image_changelog-0.1.3/odoo_image_changelog.egg-info/requires.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-04-28 08:48:45.000000 odoo_image_changelog-0.1.3/odoo_image_changelog.egg-info/top_level.txt
--rw-r--r--   0 vrenaville  (1110) docker     (998)       38 2023-04-28 08:48:45.985286 odoo_image_changelog-0.1.3/setup.cfg
--rw-r--r--   0 vrenaville  (1110) docker     (998)      619 2023-04-28 08:48:17.000000 odoo_image_changelog-0.1.3/setup.py
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-05-11 09:56:46.740257 odoo_image_changelog-0.2.0/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     1799 2023-04-20 08:54:35.000000 odoo_image_changelog-0.2.0/.gitignore
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-05-11 09:56:46.740257 odoo_image_changelog-0.2.0/PKG-INFO
+-rw-r--r--   0 vrenaville  (1110) docker     (998)        0 2023-04-20 09:33:13.000000 odoo_image_changelog-0.2.0/README.rst
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-05-11 09:56:46.740257 odoo_image_changelog-0.2.0/odoo_image_changelog/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      132 2023-05-11 09:56:40.000000 odoo_image_changelog-0.2.0/odoo_image_changelog/__init__.py
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     4902 2023-04-20 09:36:51.000000 odoo_image_changelog-0.2.0/odoo_image_changelog/github_helpers.py
+-rw-r--r--   0 vrenaville  (1110) docker     (998)     4842 2023-05-11 09:56:40.000000 odoo_image_changelog-0.2.0/odoo_image_changelog/main.py
+drwxr-xr-x   0 vrenaville  (1110) docker     (998)        0 2023-05-11 09:56:46.740257 odoo_image_changelog-0.2.0/odoo_image_changelog.egg-info/
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      355 2023-05-11 09:56:46.000000 odoo_image_changelog-0.2.0/odoo_image_changelog.egg-info/PKG-INFO
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      397 2023-05-11 09:56:46.000000 odoo_image_changelog-0.2.0/odoo_image_changelog.egg-info/SOURCES.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)        1 2023-05-11 09:56:46.000000 odoo_image_changelog-0.2.0/odoo_image_changelog.egg-info/dependency_links.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       71 2023-05-11 09:56:46.000000 odoo_image_changelog-0.2.0/odoo_image_changelog.egg-info/entry_points.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-05-11 09:56:46.000000 odoo_image_changelog-0.2.0/odoo_image_changelog.egg-info/requires.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       21 2023-05-11 09:56:46.000000 odoo_image_changelog-0.2.0/odoo_image_changelog.egg-info/top_level.txt
+-rw-r--r--   0 vrenaville  (1110) docker     (998)       38 2023-05-11 09:56:46.740257 odoo_image_changelog-0.2.0/setup.cfg
+-rw-r--r--   0 vrenaville  (1110) docker     (998)      619 2023-05-11 09:56:40.000000 odoo_image_changelog-0.2.0/setup.py
```

### Comparing `odoo_image_changelog-0.1.3/.gitignore` & `odoo_image_changelog-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `odoo_image_changelog-0.1.3/odoo_image_changelog/github_helpers.py` & `odoo_image_changelog-0.2.0/odoo_image_changelog/github_helpers.py`

 * *Files identical despite different names*

### Comparing `odoo_image_changelog-0.1.3/odoo_image_changelog/main.py` & `odoo_image_changelog-0.2.0/odoo_image_changelog/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,18 +59,20 @@
     if changelog_array:
         if stable:
             change_log_file = f"{current_running_build}/CHANGELOG.md"
         else:
             change_log_file = f"{current_running_build}/CHANGELOG_UNSTABLE.md"
 
         with open(f"local_repo/{change_log_file}") as file:
-            while line := file.readline().rstrip():
-                content_array.append(line)
+            for line in file:
+                content_array.append(f"{line.rstrip()}\n")
         previous_hash = hash_yaml["previous_hash"]
-        title_change_log = f"\nChangelog: from {previous_hash} to {current_hash}\n"
+        title_change_log = (
+            f"\nChangelog: from {hash_yaml['current_hash']} to {current_hash}\n"
+        )
         line = len(title_change_log) * "-"
         content_array.append(title_change_log)
         content_array.append("\n")
         content_array.append(line)
         content_array.append("\n\n")
         content_array = content_array + changelog_array
         changelog_string = "".join(content_array)
```

### Comparing `odoo_image_changelog-0.1.3/setup.py` & `odoo_image_changelog-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="odoo_image_changelog",
-    version="0.1.3",
+    version="0.2.0",
     description="a odoo changelog generator",
     url="https://github.com/camptocamp/odoo-image-changelog",
     author="Camptocamp (Vincent Renaville)",
     author_email="vincent.renaville@camptocamp.com",
     packages=["odoo_image_changelog"],
     install_requires=[
         "PyGithub",
```


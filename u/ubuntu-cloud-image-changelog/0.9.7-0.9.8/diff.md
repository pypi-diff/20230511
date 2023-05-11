# Comparing `tmp/ubuntu-cloud-image-changelog-0.9.7.tar.gz` & `tmp/ubuntu-cloud-image-changelog-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubuntu-cloud-image-changelog-0.9.7.tar", last modified: Tue Feb 22 10:26:49 2022, max compression
+gzip compressed data, was "ubuntu-cloud-image-changelog-0.9.8.tar", last modified: Tue Feb 22 12:22:37 2022, max compression
```

## Comparing `ubuntu-cloud-image-changelog-0.9.7.tar` & `ubuntu-cloud-image-changelog-0.9.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 10:26:49.032951 ubuntu-cloud-image-changelog-0.9.7/
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      162 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/AUTHORS.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     3779 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/CONTRIBUTING.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      948 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/HISTORY.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     1585 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/LICENSE
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      262 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/MANIFEST.in
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     3365 2022-02-22 10:26:49.032951 ubuntu-cloud-image-changelog-0.9.7/PKG-INFO
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     1504 2022-02-22 10:19:39.000000 ubuntu-cloud-image-changelog-0.9.7/README.rst
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 10:26:49.028951 ubuntu-cloud-image-changelog-0.9.7/docs/
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      629 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/Makefile
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       28 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/authors.rst
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)     5158 2020-10-12 17:56:38.000000 ubuntu-cloud-image-changelog-0.9.7/docs/conf.py
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       33 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/contributing.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       28 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/history.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      325 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/index.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     1286 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/installation.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      790 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/make.bat
--rw-rw-r--   0 philroche  (1000) philroche  (1000)       27 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/readme.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      111 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.7/docs/usage.rst
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      527 2022-02-22 10:26:49.032951 ubuntu-cloud-image-changelog-0.9.7/setup.cfg
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     1604 2022-02-22 10:26:38.000000 ubuntu-cloud-image-changelog-0.9.7/setup.py
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 10:26:49.028951 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/
--rw-rw-r--   0 philroche  (1000) philroche  (1000)      152 2022-02-22 10:26:38.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/__init__.py
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     9292 2022-02-22 10:19:39.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/cli.py
--rw-rw-r--   0 philroche  (1000) philroche  (1000)     2931 2022-02-22 10:19:39.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/launchpadagent.py
--rw-rw-r--   0 philroche  (1000) philroche  (1000)    10898 2022-02-22 10:19:44.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/lib.py
-drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 10:26:49.032951 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)     3365 2022-02-22 10:26:48.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/PKG-INFO
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)      780 2022-02-22 10:26:48.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/SOURCES.txt
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)        1 2022-02-22 10:26:48.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/dependency_links.txt
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)       88 2022-02-22 10:26:48.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/entry_points.txt
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)        1 2020-10-12 17:25:14.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/not-zip-safe
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)       38 2022-02-22 10:26:48.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/requires.txt
--rwxr-xr-x   0 philroche  (1000) philroche  (1000)       29 2022-02-22 10:26:48.000000 ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/top_level.txt
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 12:22:37.780777 ubuntu-cloud-image-changelog-0.9.8/
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      162 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/AUTHORS.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     3779 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/CONTRIBUTING.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      948 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/HISTORY.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     1585 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/LICENSE
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      262 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/MANIFEST.in
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     3365 2022-02-22 12:22:37.780777 ubuntu-cloud-image-changelog-0.9.8/PKG-INFO
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     1504 2022-02-22 10:19:39.000000 ubuntu-cloud-image-changelog-0.9.8/README.rst
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 12:22:37.780777 ubuntu-cloud-image-changelog-0.9.8/docs/
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      629 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/Makefile
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)       28 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/authors.rst
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)     5158 2020-10-12 17:56:38.000000 ubuntu-cloud-image-changelog-0.9.8/docs/conf.py
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)       33 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/contributing.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)       28 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/history.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      325 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/index.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     1286 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/installation.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      790 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/make.bat
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)       27 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/readme.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      111 2022-02-21 18:07:36.000000 ubuntu-cloud-image-changelog-0.9.8/docs/usage.rst
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      527 2022-02-22 12:22:37.780777 ubuntu-cloud-image-changelog-0.9.8/setup.cfg
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     1604 2022-02-22 12:22:28.000000 ubuntu-cloud-image-changelog-0.9.8/setup.py
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 12:22:37.780777 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)      152 2022-02-22 12:22:28.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/__init__.py
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     9385 2022-02-22 12:21:40.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/cli.py
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)     2931 2022-02-22 10:19:39.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/launchpadagent.py
+-rw-rw-r--   0 philroche  (1000) philroche  (1000)    11048 2022-02-22 12:21:47.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/lib.py
+drwxrwxr-x   0 philroche  (1000) philroche  (1000)        0 2022-02-22 12:22:37.780777 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)     3365 2022-02-22 12:22:37.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/PKG-INFO
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)      780 2022-02-22 12:22:37.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/SOURCES.txt
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)        1 2022-02-22 12:22:37.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/dependency_links.txt
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)       88 2022-02-22 12:22:37.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/entry_points.txt
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)        1 2020-10-12 17:25:14.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/not-zip-safe
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)       38 2022-02-22 12:22:37.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/requires.txt
+-rwxr-xr-x   0 philroche  (1000) philroche  (1000)       29 2022-02-22 12:22:37.000000 ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/top_level.txt
```

### Comparing `ubuntu-cloud-image-changelog-0.9.7/CONTRIBUTING.rst` & `ubuntu-cloud-image-changelog-0.9.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/HISTORY.rst` & `ubuntu-cloud-image-changelog-0.9.8/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/LICENSE` & `ubuntu-cloud-image-changelog-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/PKG-INFO` & `ubuntu-cloud-image-changelog-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubuntu-cloud-image-changelog
-Version: 0.9.7
+Version: 0.9.8
 Summary: Helpful utility to generate package changelog between two cloud images
 Home-page: https://github.com/CanonicalLtd/ubuntu_cloud_image_changelog
 Author: Philip Roche
 Author-email: phil.roche@canonical.com
 License: GNU General Public License v3
 Keywords: ubuntu_cloud_image_changelog
 Platform: UNKNOWN
```

### Comparing `ubuntu-cloud-image-changelog-0.9.7/README.rst` & `ubuntu-cloud-image-changelog-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/docs/Makefile` & `ubuntu-cloud-image-changelog-0.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/docs/conf.py` & `ubuntu-cloud-image-changelog-0.9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/docs/installation.rst` & `ubuntu-cloud-image-changelog-0.9.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/docs/make.bat` & `ubuntu-cloud-image-changelog-0.9.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/setup.cfg` & `ubuntu-cloud-image-changelog-0.9.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.7
+current_version = 0.9.8
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `ubuntu-cloud-image-changelog-0.9.7/setup.py` & `ubuntu-cloud-image-changelog-0.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     include_package_data=True,
     keywords="ubuntu_cloud_image_changelog",
     name="ubuntu-cloud-image-changelog",
     packages=find_packages(
         include=["ubuntu_cloud_image_changelog", "ubuntu_cloud_image_changelog.*"]
     ),
     url="https://github.com/CanonicalLtd/ubuntu_cloud_image_changelog",
-    version="0.9.7",
+    version="0.9.8",
     zip_safe=False,
 )
```

### Comparing `ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/cli.py` & `ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,21 +170,23 @@
             click.echo(
                 "{} changed from version '{}' to version '{}'".format(
                     package, from_to["from"], from_to["to"]
                 )
             )
             click.echo()
 
-    if deb_package_diffs:
+    if deb_package_diffs or added_deb_packages:
 
         click.echo("\n** Changelogs for added and changed deb packages " "below: **\n")
 
         # for each of the deb package diffs and new packages download the
         # changelog
-        with tempfile.TemporaryDirectory(prefix="ubuntu-cloud-image-changelog") as tmp_cache_directory:
+        with tempfile.TemporaryDirectory(
+            prefix="ubuntu-cloud-image-changelog"
+        ) as tmp_cache_directory:
             launchpad = launchpadagent.get_launchpad(
                 launchpadlib_dir=tmp_cache_directory,
                 lp_credentials_store=lp_credentials_store,
             )
             ubuntu = launchpad.distributions["ubuntu"]
             lp_series = ubuntu.getSeries(name_or_version=series)
             lp_arch_series = lp_series.getDistroArchSeries(archtag=image_architecture)
@@ -199,15 +201,15 @@
                     package,
                     to_deb_packages[package],
                     ppas,
                 )
 
                 # get the most recent changelog entry
                 version_diff_changelog = lib.parse_changelog(
-                    package_changelog_file, count=1
+                    package_changelog_file, to_version=to_deb_packages[package], count=1
                 )
 
                 click.echo(
                     "==========================================================="
                     "==========================================================="
                 )
                 click.echo(
@@ -229,15 +231,15 @@
                     package,
                     from_to["to"],
                     ppas,
                 )
 
                 # get changelog just between the from and to version
                 version_diff_changelog = lib.parse_changelog(
-                    package_changelog_file, from_to["from"], from_to["to"]
+                    package_changelog_file, from_to["from"], from_to["to"], count=None
                 )
 
                 click.echo(
                     "==========================================================="
                     "==========================================================="
                 )
                 click.echo(
```

### Comparing `ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/launchpadagent.py` & `ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/launchpadagent.py`

 * *Files identical despite different names*

### Comparing `ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog/lib.py` & `ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,26 @@
         )
         all_package_version_variants.append(package_version_without_epoch)
     # shim-signed is a special package as it appends the version of the
     # binary shim from Microsoft. This full version will not appear in
     # the manifest so we can safely remove anything after the binary
     # shim version.
     if "+" in package_version:
-        all_package_version_variants.append(package_version[0: package_version.index("+")])
+        all_package_version_variants.append(
+            package_version[0 : package_version.index("+")]
+        )
     # An Ubuntu version might have ~ suffix. Remove this as it might not
     # always appear in the changelog
     if "~" in package_version:
-        all_package_version_variants.append(package_version[0: package_version.index("~")])
+        all_package_version_variants.append(
+            package_version[0 : package_version.index("~")]
+        )
     return all_package_version_variants
 
+
 def arch_independent_package_name(package_name):
     # packages ending with ':amd64' or ':arm64' are special
     if package_name.endswith(":amd64") or package_name.endswith(":arm64"):
         package_name = package_name[:-6]
     return package_name
 
 
@@ -45,53 +50,59 @@
     list of changelog entries the result will be incomplete and
     a non-empty error message is returned to indicate the issue.
     """
     changelog = ""
     # Set max_blocks to none if we know the versions we want changelog for
     from_versions = []
     to_versions = []
-    if from_version and to_version:
+
+    if from_version:
         from_versions = package_version_variants(from_version)
+    if to_version:
         to_versions = package_version_variants(to_version)
-        count = None
 
     with open(changelog_filename, "r") as fileptr:
-        parsed_changelog = Changelog(fileptr.read(), max_blocks=count)
+        parsed_changelog = Changelog(fileptr.read())
         start = False
         end = False
         try:
             changelog += "Source: {}\n".format(parsed_changelog.get_package())
             changelog += "Version: {}\n".format(parsed_changelog.version)
             changelog += "Distribution: {}\n".format(parsed_changelog.distributions)
             changelog += "Urgency: {}\n".format(parsed_changelog.urgency)
             changelog += "Maintainer: {}\n".format(parsed_changelog.author)
             changelog += "Date: {}\n".format(parsed_changelog.date)
 
             # The changelog blocks are in reverse order; we'll see high|to before low|from.
             change_blocks = []
             launchpad_bugs_fixed = []
             for changelog_block in parsed_changelog:
-                changelog_block_versions = package_version_variants(changelog_block.version.full_version)
+                changelog_block_versions = package_version_variants(
+                    changelog_block.version.full_version
+                )
                 for to_version in to_versions:
                     if to_version in changelog_block_versions:
                         start = True
                         break
                 for from_version in from_versions:
                     if from_version in changelog_block_versions:
                         end = True
                         break
-                if (not from_versions and not to_versions) or (start and not end):
+                if start and not end:
                     launchpad_bugs_fixed += changelog_block.lp_bugs_closed
                     changeblock_summary = "{} ({}) {}; urgency={}".format(
                         changelog_block.package,
                         changelog_block.version,
                         changelog_block.distributions,
                         changelog_block.urgency,
                     )
                     change_blocks.append((changeblock_summary, changelog_block))
+                if count and len(change_blocks) == count:
+                    end = True
+                    break  # we have enough blocks now
 
             changelog += "Launchpad-Bugs-Fixed: {}\n".format(launchpad_bugs_fixed)
             changelog += "Changes:\n"
             for changeblock_summary, change_block in change_blocks:
                 changelog += "{}\n".format(changeblock_summary)
                 for change in change_block.changes():
                     changelog += "{}\n".format(change)
```

### Comparing `ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/PKG-INFO` & `ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubuntu-cloud-image-changelog
-Version: 0.9.7
+Version: 0.9.8
 Summary: Helpful utility to generate package changelog between two cloud images
 Home-page: https://github.com/CanonicalLtd/ubuntu_cloud_image_changelog
 Author: Philip Roche
 Author-email: phil.roche@canonical.com
 License: GNU General Public License v3
 Keywords: ubuntu_cloud_image_changelog
 Platform: UNKNOWN
```

### Comparing `ubuntu-cloud-image-changelog-0.9.7/ubuntu_cloud_image_changelog.egg-info/SOURCES.txt` & `ubuntu-cloud-image-changelog-0.9.8/ubuntu_cloud_image_changelog.egg-info/SOURCES.txt`

 * *Files identical despite different names*


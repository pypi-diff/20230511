# Comparing `tmp/llvm-installer-1.3.1.tar.gz` & `tmp/llvm-installer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvm-installer-1.3.1.tar", last modified: Mon May  1 16:00:57 2023, max compression
+gzip compressed data, was "llvm-installer-1.3.2.tar", last modified: Thu May 11 18:19:50 2023, max compression
```

## Comparing `llvm-installer-1.3.1.tar` & `llvm-installer-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-01 16:00:57.329468 llvm-installer-1.3.1/
--rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm-installer-1.3.1/LICENSE
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-05-01 16:00:57.329329 llvm-installer-1.3.1/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm-installer-1.3.1/README.md
--rw-r--r--   0 mikhail    (503) staff       (20)       38 2023-05-01 16:00:57.329536 llvm-installer-1.3.1/setup.cfg
--rw-r--r--   0 mikhail    (503) staff       (20)     2235 2023-05-01 16:00:26.000000 llvm-installer-1.3.1/setup.py
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-01 16:00:57.326230 llvm-installer-1.3.1/src/
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-01 16:00:57.327781 llvm-installer-1.3.1/src/llvm_installer/
--rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm-installer-1.3.1/src/llvm_installer/__init__.py
--rw-r--r--   0 mikhail    (503) staff       (20)     1641 2022-07-07 03:54:15.000000 llvm-installer-1.3.1/src/llvm_installer/__main__.py
--rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm-installer-1.3.1/src/llvm_installer/py.typed
--rw-r--r--   0 mikhail    (503) staff       (20)    79197 2023-05-01 16:00:10.000000 llvm-installer-1.3.1/src/llvm_installer/release_tags.json
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-01 16:00:57.329100 llvm-installer-1.3.1/src/llvm_installer.egg-info/
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-05-01 16:00:57.000000 llvm-installer-1.3.1/src/llvm_installer.egg-info/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      407 2023-05-01 16:00:57.000000 llvm-installer-1.3.1/src/llvm_installer.egg-info/SOURCES.txt
--rw-r--r--   0 mikhail    (503) staff       (20)        1 2023-05-01 16:00:57.000000 llvm-installer-1.3.1/src/llvm_installer.egg-info/dependency_links.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       64 2023-05-01 16:00:57.000000 llvm-installer-1.3.1/src/llvm_installer.egg-info/entry_points.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       86 2023-05-01 16:00:57.000000 llvm-installer-1.3.1/src/llvm_installer.egg-info/requires.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       15 2023-05-01 16:00:57.000000 llvm-installer-1.3.1/src/llvm_installer.egg-info/top_level.txt
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.693847 llvm-installer-1.3.2/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm-installer-1.3.2/LICENSE
+-rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-05-11 18:19:50.693715 llvm-installer-1.3.2/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm-installer-1.3.2/README.md
+-rw-r--r--   0 mikhail    (503) staff       (20)       38 2023-05-11 18:19:50.693926 llvm-installer-1.3.2/setup.cfg
+-rw-r--r--   0 mikhail    (503) staff       (20)     2235 2023-05-11 18:19:27.000000 llvm-installer-1.3.2/setup.py
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.690242 llvm-installer-1.3.2/src/
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.692015 llvm-installer-1.3.2/src/llvm_installer/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm-installer-1.3.2/src/llvm_installer/__init__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)     1641 2022-07-07 03:54:15.000000 llvm-installer-1.3.2/src/llvm_installer/__main__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm-installer-1.3.2/src/llvm_installer/py.typed
+-rw-r--r--   0 mikhail    (503) staff       (20)    84030 2023-05-11 18:18:08.000000 llvm-installer-1.3.2/src/llvm_installer/release_tags.json
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.693503 llvm-installer-1.3.2/src/llvm_installer.egg-info/
+-rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      407 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)        1 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       64 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/entry_points.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       86 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/requires.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       15 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/top_level.txt
```

### Comparing `llvm-installer-1.3.1/LICENSE` & `llvm-installer-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.1/PKG-INFO` & `llvm-installer-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.3.1
+Version: 1.3.2
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `llvm-installer-1.3.1/README.md` & `llvm-installer-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.1/setup.py` & `llvm-installer-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from os import path
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as readme_file:
         long_description = readme_file.read()
 
     setup(
         name='llvm-installer',
-        version='1.3.1',
+        version='1.3.2',
         url='https://github.com/yugabyte/llvm-installer',
         author='Mikhail Bautin',
         author_email='mbautin@users.noreply.github.com',
         description='Allows installing pre-built LLVM packages for various operating systems',
         packages=find_packages(where='src'),
         package_dir={"": "src"},
         package_data={'llvm_installer': ['py.typed', 'release_tags.json']},
```

### Comparing `llvm-installer-1.3.1/src/llvm_installer/__init__.py` & `llvm-installer-1.3.2/src/llvm_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.1/src/llvm_installer/__main__.py` & `llvm-installer-1.3.2/src/llvm_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.1/src/llvm_installer/release_tags.json` & `llvm-installer-1.3.2/src/llvm_installer/release_tags.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9713541666666667%*

 * *Differences: {"'parsed_tags'": "{insert: [(151, OrderedDict([('architecture', 'aarch64'), "*

 * *                  "('is_old_tag_without_os_and_arch', False), ('major_version', 16), "*

 * *                  "('minor_version', 0), ('patch_version', 3), ('sha1_prefix', 'c8b432af'), "*

 * *                  "('short_os_name_and_version', 'almalinux8'), ('tag', "*

 * *                  "'v16.0.3-yb-1-1683790678-c8b432af-almalinux8-aarch64'), ('timestamp', "*

 * *                  "'1683790678'), ('version', '16.0.3'), ('version_suffix', 'yb-1'), "*

 * * […]*

```diff
@@ -2111,14 +2111,28 @@
             "tag": "v16.0.2-yb-1-1682894421-7886e0ac-almalinux8-aarch64",
             "timestamp": "1682894421",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v16.0.3-yb-1-1683790678-c8b432af-almalinux8-aarch64",
+            "timestamp": "1683790678",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "almalinux8",
@@ -2157,14 +2171,28 @@
             "yb_suffix_version": 1
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v16.0.3-yb-1-1683786200-c8b432af-almalinux8-x86_64",
+            "timestamp": "1683786200",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
             "patch_version": 1,
             "sha1_prefix": "58dbb949",
             "short_os_name_and_version": "almalinux9",
             "tag": "v16.0.1-yb-1-1680849004-58dbb949-almalinux9-x86_64",
             "timestamp": "1680849004",
             "version": "16.0.1",
             "version_suffix": "yb-1",
@@ -2195,14 +2223,28 @@
             "tag": "v16.0.2-yb-1-1682631493-7886e0ac-almalinux9-x86_64",
             "timestamp": "1682631493",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v16.0.3-yb-1-1683787641-c8b432af-almalinux9-x86_64",
+            "timestamp": "1683787641",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "centos7",
@@ -2223,14 +2265,28 @@
             "tag": "v16.0.2-yb-1-1682888906-7886e0ac-centos7-aarch64",
             "timestamp": "1682888906",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "centos7",
+            "tag": "v16.0.3-yb-1-1683785203-c8b432af-centos7-aarch64",
+            "timestamp": "1683785203",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "centos7",
@@ -2293,14 +2349,28 @@
             "tag": "v16.0.2-yb-1-1682627241-7886e0ac-centos7-x86_64",
             "timestamp": "1682627241",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "centos7",
+            "tag": "v16.0.3-yb-1-1683784713-c8b432af-centos7-x86_64",
+            "timestamp": "1683784713",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "arm64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "macos",
@@ -2349,14 +2419,28 @@
             "tag": "v16.0.2-yb-1-1682667271-7886e0ac-macos-arm64",
             "timestamp": "1682667271",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "arm64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "macos",
+            "tag": "v16.0.3-yb-1-1683785495-c8b432af-macos-arm64",
+            "timestamp": "1683785495",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 1,
             "sha1_prefix": "58dbb949",
             "short_os_name_and_version": "macos",
@@ -2391,14 +2475,28 @@
             "tag": "v16.0.1-yb-1-1682021461-58dbb949-macos-x86_64",
             "timestamp": "1682021461",
             "version": "16.0.1",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "macos",
+            "tag": "v16.0.3-yb-1-1683817162-c8b432af-macos-x86_64",
+            "timestamp": "1683817162",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu20.04",
@@ -2419,14 +2517,28 @@
             "tag": "v16.0.2-yb-1-1682668230-7886e0ac-ubuntu20.04-aarch64",
             "timestamp": "1682668230",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "ubuntu20.04",
+            "tag": "v16.0.3-yb-1-1683796047-c8b432af-ubuntu20.04-aarch64",
+            "timestamp": "1683796047",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu20.04",
@@ -2461,14 +2573,28 @@
             "tag": "v16.0.2-yb-1-1682632928-7886e0ac-ubuntu20.04-x86_64",
             "timestamp": "1682632928",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "ubuntu20.04",
+            "tag": "v16.0.3-yb-1-1683789090-c8b432af-ubuntu20.04-x86_64",
+            "timestamp": "1683789090",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu22.04",
@@ -2489,14 +2615,28 @@
             "tag": "v16.0.2-yb-1-1682673575-7886e0ac-ubuntu22.04-aarch64",
             "timestamp": "1682673575",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v16.0.3-yb-1-1683801442-c8b432af-ubuntu22.04-aarch64",
+            "timestamp": "1683801442",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu22.04",
@@ -2529,10 +2669,24 @@
             "sha1_prefix": "7886e0ac",
             "short_os_name_and_version": "ubuntu22.04",
             "tag": "v16.0.2-yb-1-1682634395-7886e0ac-ubuntu22.04-x86_64",
             "timestamp": "1682634395",
             "version": "16.0.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 3,
+            "sha1_prefix": "c8b432af",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v16.0.3-yb-1-1683790564-c8b432af-ubuntu22.04-x86_64",
+            "timestamp": "1683790564",
+            "version": "16.0.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
         }
     ]
 }
```

### Comparing `llvm-installer-1.3.1/src/llvm_installer.egg-info/PKG-INFO` & `llvm-installer-1.3.2/src/llvm_installer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.3.1
+Version: 1.3.2
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```


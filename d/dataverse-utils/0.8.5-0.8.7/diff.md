# Comparing `tmp/dataverse_utils-0.8.5.tar.gz` & `tmp/dataverse_utils-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_utils-0.8.5.tar", last modified: Thu May  4 22:04:12 2023, max compression
+gzip compressed data, was "dataverse_utils-0.8.7.tar", last modified: Thu May 11 17:29:21 2023, max compression
```

## Comparing `dataverse_utils-0.8.5.tar` & `dataverse_utils-0.8.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.733716 dataverse_utils-0.8.5/
--rw-r--r--   0 paul       (501) staff       (20)      144 2023-05-01 17:26:53.000000 dataverse_utils-0.8.5/.gitignore
--rw-r--r--   0 paul       (501) staff       (20)     1103 2021-06-17 22:51:24.000000 dataverse_utils-0.8.5/LICENCE.md
--rw-r--r--   0 paul       (501) staff       (20)     2052 2023-05-04 22:04:12.732785 dataverse_utils-0.8.5/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1163 2023-05-04 18:36:40.000000 dataverse_utils-0.8.5/README.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.704946 dataverse_utils-0.8.5/docs/
--rw-r--r--   0 paul       (501) staff       (20)    10917 2022-04-26 15:29:23.000000 dataverse_utils-0.8.5/docs/api_ref.md
--rw-r--r--   0 paul       (501) staff       (20)      383 2023-05-03 22:01:24.000000 dataverse_utils-0.8.5/docs/credits.md
--rw-r--r--   0 paul       (501) staff       (20)     2932 2021-08-09 17:51:55.000000 dataverse_utils-0.8.5/docs/faq.md
--rw-r--r--   0 paul       (501) staff       (20)     5840 2023-05-04 21:45:19.000000 dataverse_utils-0.8.5/docs/index.md
--rw-r--r--   0 paul       (501) staff       (20)    17965 2023-05-04 20:54:58.000000 dataverse_utils-0.8.5/docs/scripts.md
--rw-r--r--   0 paul       (501) staff       (20)     5748 2023-05-04 21:33:02.000000 dataverse_utils-0.8.5/docs/windows.md
--rw-r--r--   0 paul       (501) staff       (20)      396 2023-05-04 21:38:25.000000 dataverse_utils-0.8.5/mkdocs.yml
--rw-r--r--   0 paul       (501) staff       (20)     2538 2023-05-04 20:33:51.000000 dataverse_utils-0.8.5/pyproject.toml
--rw-r--r--   0 paul       (501) staff       (20)      240 2023-05-04 21:31:12.000000 dataverse_utils-0.8.5/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-05-04 22:04:12.733920 dataverse_utils-0.8.5/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)       84 2023-04-28 20:29:51.000000 dataverse_utils-0.8.5/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.690109 dataverse_utils-0.8.5/src/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.708457 dataverse_utils-0.8.5/src/dataverse_utils/
--rw-r--r--   0 paul       (501) staff       (20)      155 2023-05-04 20:40:04.000000 dataverse_utils-0.8.5/src/dataverse_utils/__init__.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.715876 dataverse_utils-0.8.5/src/dataverse_utils/data/
--rw-r--r--   0 paul       (501) staff       (20)     1545 2021-06-17 22:51:24.000000 dataverse_utils-0.8.5/src/dataverse_utils/data/LDC_EULA_general.md
--rw-r--r--   0 paul       (501) staff       (20)    17269 2022-09-28 16:03:47.000000 dataverse_utils-0.8.5/src/dataverse_utils/dataverse_utils.py
--rw-r--r--   0 paul       (501) staff       (20)    16047 2023-01-24 22:34:17.000000 dataverse_utils-0.8.5/src/dataverse_utils/ldc.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.726431 dataverse_utils-0.8.5/src/dataverse_utils/scripts/
--rw-r--r--   0 paul       (501) staff       (20)     4965 2023-01-26 23:32:25.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_del.py
--rw-r--r--   0 paul       (501) staff       (20)     5348 2023-01-24 22:05:28.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_ldc_uploader.py
--rw-r--r--   0 paul       (501) staff       (20)     5366 2022-04-26 15:29:23.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_manifest_gen.py
--rw-r--r--   0 paul       (501) staff       (20)     9076 2023-05-04 17:20:02.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_pg_facet_date.py
--rw-r--r--   0 paul       (501) staff       (20)     4349 2023-04-26 22:53:03.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_record_copy.py
--rw-r--r--   0 paul       (501) staff       (20)     8071 2021-08-09 17:51:55.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_release.py
--rw-r--r--   0 paul       (501) staff       (20)     4566 2023-05-04 20:36:54.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_replace_licence.py
--rw-r--r--   0 paul       (501) staff       (20)     2975 2021-10-20 23:02:56.000000 dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_upload_tsv.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.715137 dataverse_utils-0.8.5/src/dataverse_utils.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     2052 2023-05-04 22:04:12.000000 dataverse_utils-0.8.5/src/dataverse_utils.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1022 2023-05-04 22:04:12.000000 dataverse_utils-0.8.5/src/dataverse_utils.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-04 22:04:12.000000 dataverse_utils-0.8.5/src/dataverse_utils.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)      576 2023-05-04 22:04:12.000000 dataverse_utils-0.8.5/src/dataverse_utils.egg-info/entry_points.txt
--rw-r--r--   0 paul       (501) staff       (20)      266 2023-05-04 22:04:12.000000 dataverse_utils-0.8.5/src/dataverse_utils.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       16 2023-05-04 22:04:12.000000 dataverse_utils-0.8.5/src/dataverse_utils.egg-info/top_level.txt
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.728284 dataverse_utils-0.8.5/tests/
--rw-r--r--   0 paul       (501) staff       (20)        0 2021-08-09 17:51:55.000000 dataverse_utils-0.8.5/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     1124 2021-08-09 17:51:55.000000 dataverse_utils-0.8.5/tests/tests_dataverse_utils.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-04 22:04:12.730987 dataverse_utils-0.8.5/tmp/
--rw-r--r--   0 paul       (501) staff       (20)      324 2021-09-17 20:10:42.000000 dataverse_utils-0.8.5/tmp/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)     2493 2023-02-14 19:51:38.000000 dataverse_utils-0.8.5/tmp/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.888426 dataverse_utils-0.8.7/
+-rw-r--r--   0 paul       (501) staff       (20)      144 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/.gitignore
+-rw-r--r--   0 paul       (501) staff       (20)     1103 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/LICENCE.md
+-rw-r--r--   0 paul       (501) staff       (20)     2052 2023-05-11 17:29:21.887614 dataverse_utils-0.8.7/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1163 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.853564 dataverse_utils-0.8.7/docs/
+-rw-r--r--   0 paul       (501) staff       (20)    10917 2022-04-26 15:29:23.000000 dataverse_utils-0.8.7/docs/api_ref.md
+-rw-r--r--   0 paul       (501) staff       (20)      383 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/docs/credits.md
+-rw-r--r--   0 paul       (501) staff       (20)     2932 2021-08-09 17:51:55.000000 dataverse_utils-0.8.7/docs/faq.md
+-rw-r--r--   0 paul       (501) staff       (20)     5840 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/docs/index.md
+-rw-r--r--   0 paul       (501) staff       (20)    18831 2023-05-11 15:44:20.000000 dataverse_utils-0.8.7/docs/scripts.md
+-rw-r--r--   0 paul       (501) staff       (20)     5748 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/docs/windows.md
+-rw-r--r--   0 paul       (501) staff       (20)      396 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/mkdocs.yml
+-rw-r--r--   0 paul       (501) staff       (20)     2536 2023-05-11 15:42:55.000000 dataverse_utils-0.8.7/pyproject.toml
+-rw-r--r--   0 paul       (501) staff       (20)      240 2023-05-11 15:55:17.000000 dataverse_utils-0.8.7/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-05-11 17:29:21.888603 dataverse_utils-0.8.7/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)       84 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.841640 dataverse_utils-0.8.7/src/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.856538 dataverse_utils-0.8.7/src/dataverse_utils/
+-rw-r--r--   0 paul       (501) staff       (20)      155 2023-05-11 15:54:33.000000 dataverse_utils-0.8.7/src/dataverse_utils/__init__.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.872144 dataverse_utils-0.8.7/src/dataverse_utils/data/
+-rw-r--r--   0 paul       (501) staff       (20)     1545 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/data/LDC_EULA_general.md
+-rw-r--r--   0 paul       (501) staff       (20)    17269 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/dataverse_utils.py
+-rw-r--r--   0 paul       (501) staff       (20)    16047 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/ldc.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.881112 dataverse_utils-0.8.7/src/dataverse_utils/scripts/
+-rw-r--r--   0 paul       (501) staff       (20)     4965 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_del.py
+-rw-r--r--   0 paul       (501) staff       (20)     5348 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_ldc_uploader.py
+-rw-r--r--   0 paul       (501) staff       (20)     5366 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_manifest_gen.py
+-rw-r--r--   0 paul       (501) staff       (20)     9076 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_pg_facet_date.py
+-rw-r--r--   0 paul       (501) staff       (20)     4349 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_record_copy.py
+-rw-r--r--   0 paul       (501) staff       (20)     8071 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_release.py
+-rw-r--r--   0 paul       (501) staff       (20)     4566 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_replace_licence.py
+-rw-r--r--   0 paul       (501) staff       (20)     2975 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_upload_tsv.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.871100 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     2052 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1022 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)      574 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/entry_points.txt
+-rw-r--r--   0 paul       (501) staff       (20)      266 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       16 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/top_level.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.882809 dataverse_utils-0.8.7/tests/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2021-08-09 17:51:55.000000 dataverse_utils-0.8.7/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     1124 2021-08-09 17:51:55.000000 dataverse_utils-0.8.7/tests/tests_dataverse_utils.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.886306 dataverse_utils-0.8.7/tmp/
+-rw-r--r--   0 paul       (501) staff       (20)      324 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/tmp/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)     2493 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/tmp/setup.py
```

### Comparing `dataverse_utils-0.8.5/LICENCE.md` & `dataverse_utils-0.8.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/PKG-INFO` & `dataverse_utils-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse_utils
-Version: 0.8.5
+Version: 0.8.7
 Summary: Utilities for the Dataverse data respository system
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dataverse_utils
 Project-URL: Repository, https://github.com/ubc-library-rc/dataverse_utils.git
 Project-URL: Issue Tracker, https://github.com/ubc-library-rc/dataverse_utils/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataverse_utils-0.8.5/README.md` & `dataverse_utils-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/docs/api_ref.md` & `dataverse_utils-0.8.7/docs/api_ref.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/docs/faq.md` & `dataverse_utils-0.8.7/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/docs/index.md` & `dataverse_utils-0.8.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/docs/scripts.md` & `dataverse_utils-0.8.7/docs/scripts.md`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,30 @@
 ```
 
 ##dv_replace_licen[cs]e
 
 This will replace the text in a record with the text Markdown file. Text is converted to HTML. Optionally, the record can be republished without incrementing the version (ie, with `type=updatecurrent`.
 
 ```nohighlight
+usage: dv_replace_licence [-h] [-u URL] -l LIC -k KEY [-r] [--version] studies [studies ...]
+
+Replaces the licence text in a Dataverse study and [optionally] republishes it as the same version. Superuser privileges are required for republishing as the version is not incremented.
+This software requires the Dataverse installation to be running Dataverse software version >= 5.6.
+
+positional arguments:
+  studies               Persistent IDs of studies
+
+options:
+  -h, --help            show this help message and exit
+  -u URL, --url URL     Base URL of Dataverse installation. Defaults to "https://abacus.library.ubc.ca"
+  -l LIC, --licence LIC
+                        Licence file in Markdown format
+  -k KEY, --key KEY     Dataverse API key
+  -r, --republish       Republish study without incrementing version
+  --version             Show version number and exit
 ``` 
 
 ## dv_upload_tsv
 
 Now that you have a tsv full of nicely described data, you can easily upload it to an existing study if you know the persistent ID and have an API key.
 
 For the best metadata, you should probably edit it manually to add correct descriptive metadata, notably the "Description" and "Tags". Tags are split separated by commas, so it's possible to have multiple tags for each data item, like "Data, SPSS, June 2021".
```

#### html2text {}

```diff
@@ -180,15 +180,25 @@
 run Only output a list of studies to be released -d DV, --dv DV Short name of
 Dataverse collection to process (eg: statcan) -p PID [PID ...], --pid PID [PID
 ...] Handles or DOIs to release in format hdl:11272.1/FK2/12345 or doi:
 10.80240/FK2/NWRABI. Multiple values OK --version Show version number and exit
 ``` ##dv_replace_licen[cs]e This will replace the text in a record with the
 text Markdown file. Text is converted to HTML. Optionally, the record can be
 republished without incrementing the version (ie, with `type=updatecurrent`.
-```nohighlight ``` ## dv_upload_tsv Now that you have a tsv full of nicely
+```nohighlight usage: dv_replace_licence [-h] [-u URL] -l LIC -k KEY [-r] [--
+version] studies [studies ...] Replaces the licence text in a Dataverse study
+and [optionally] republishes it as the same version. Superuser privileges are
+required for republishing as the version is not incremented. This software
+requires the Dataverse installation to be running Dataverse software version >=
+5.6. positional arguments: studies Persistent IDs of studies options: -h, --
+help show this help message and exit -u URL, --url URL Base URL of Dataverse
+installation. Defaults to "https://abacus.library.ubc.ca" -l LIC, --licence LIC
+Licence file in Markdown format -k KEY, --key KEY Dataverse API key -r, --
+republish Republish study without incrementing version --version Show version
+number and exit ``` ## dv_upload_tsv Now that you have a tsv full of nicely
 described data, you can easily upload it to an existing study if you know the
 persistent ID and have an API key. For the best metadata, you should probably
 edit it manually to add correct descriptive metadata, notably the "Description"
 and "Tags". Tags are split separated by commas, so it's possible to have
 multiple tags for each data item, like "Data, SPSS, June 2021". File paths are
 automatically generated from the "file" column. Because of this, you should
 probably use relative paths rather than absolute paths unless you want to have
```

### Comparing `dataverse_utils-0.8.5/docs/windows.md` & `dataverse_utils-0.8.7/docs/windows.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/pyproject.toml` & `dataverse_utils-0.8.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,10 +50,10 @@
 #This should be restructured one day
 dv_del = 'dataverse_utils.scripts.dv_del:main'
 dv_ldc_uploader = 'dataverse_utils.scripts.dv_ldc_uploader:main'
 dv_manifest_gen = 'dataverse_utils.scripts.dv_manifest_gen:main'
 dv_pg_facet_date = 'dataverse_utils.scripts.dv_pg_facet_date:main [server]'
 dv_record_copy = 'dataverse_utils.scripts.dv_record_copy:main'
 dv_release = 'dataverse_utils.scripts.dv_release:main'
-dv_replace_licence = 'dataverse_utils.scripts.dv_replace_licences:main'
-dv_replace_license = 'dataverse_utils.scripts.dv_replace_licences:main'
+dv_replace_licence = 'dataverse_utils.scripts.dv_replace_licence:main'
+dv_replace_license = 'dataverse_utils.scripts.dv_replace_licence:main'
 dv_upload_tsv = 'dataverse_utils.scripts.dv_upload_tsv:main'
```

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/data/LDC_EULA_general.md` & `dataverse_utils-0.8.7/src/dataverse_utils/data/LDC_EULA_general.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/dataverse_utils.py` & `dataverse_utils-0.8.7/src/dataverse_utils/dataverse_utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/ldc.py` & `dataverse_utils-0.8.7/src/dataverse_utils/ldc.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_del.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_del.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_ldc_uploader.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_ldc_uploader.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_manifest_gen.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_manifest_gen.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_pg_facet_date.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_pg_facet_date.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_record_copy.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_record_copy.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_release.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_release.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_replace_licence.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_replace_licence.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils/scripts/dv_upload_tsv.py` & `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_upload_tsv.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils.egg-info/PKG-INFO` & `dataverse_utils-0.8.7/src/dataverse_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-utils
-Version: 0.8.5
+Version: 0.8.7
 Summary: Utilities for the Dataverse data respository system
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dataverse_utils
 Project-URL: Repository, https://github.com/ubc-library-rc/dataverse_utils.git
 Project-URL: Issue Tracker, https://github.com/ubc-library-rc/dataverse_utils/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils.egg-info/SOURCES.txt` & `dataverse_utils-0.8.7/src/dataverse_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/src/dataverse_utils.egg-info/entry_points.txt` & `dataverse_utils-0.8.7/src/dataverse_utils.egg-info/entry_points.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [console_scripts]
 dv_del = dataverse_utils.scripts.dv_del:main
 dv_ldc_uploader = dataverse_utils.scripts.dv_ldc_uploader:main
 dv_manifest_gen = dataverse_utils.scripts.dv_manifest_gen:main
 dv_pg_facet_date = dataverse_utils.scripts.dv_pg_facet_date:main [server]
 dv_record_copy = dataverse_utils.scripts.dv_record_copy:main
 dv_release = dataverse_utils.scripts.dv_release:main
-dv_replace_licence = dataverse_utils.scripts.dv_replace_licences:main
-dv_replace_license = dataverse_utils.scripts.dv_replace_licences:main
+dv_replace_licence = dataverse_utils.scripts.dv_replace_licence:main
+dv_replace_license = dataverse_utils.scripts.dv_replace_licence:main
 dv_upload_tsv = dataverse_utils.scripts.dv_upload_tsv:main
```

### Comparing `dataverse_utils-0.8.5/tests/tests_dataverse_utils.py` & `dataverse_utils-0.8.7/tests/tests_dataverse_utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.5/tmp/setup.py` & `dataverse_utils-0.8.7/tmp/setup.py`

 * *Files identical despite different names*


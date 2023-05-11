# Comparing `tmp/NikeCA-0.2.5a0.tar.gz` & `tmp/NikeCA-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.5a0.tar", last modified: Wed May 10 20:48:54 2023, max compression
+gzip compressed data, was "NikeCA-0.2.6.tar", last modified: Thu May 11 05:42:37 2023, max compression
```

## Comparing `NikeCA-0.2.5a0.tar` & `NikeCA-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:48:54.041913 NikeCA-0.2.5a0/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.5a0/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-10 20:48:54.041476 NikeCA-0.2.5a0/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.5a0/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 20:48:54.042031 NikeCA-0.2.5a0/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2487 2023-05-10 20:48:46.000000 NikeCA-0.2.5a0/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:48:54.032454 NikeCA-0.2.5a0/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:48:54.033750 NikeCA-0.2.5a0/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.5a0/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:48:54.035377 NikeCA-0.2.5a0/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.5a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:46:33.000000 NikeCA-0.2.5a0/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:48:54.038175 NikeCA-0.2.5a0/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.5a0/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.5a0/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.5a0/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.5a0/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:48:54.040792 NikeCA-0.2.5a0/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-10 20:48:53.000000 NikeCA-0.2.5a0/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 20:48:53.000000 NikeCA-0.2.5a0/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:48:53.000000 NikeCA-0.2.5a0/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 20:48:53.000000 NikeCA-0.2.5a0/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:48:53.000000 NikeCA-0.2.5a0/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:48:35.000000 NikeCA-0.2.5a0/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19225 2023-05-10 19:50:52.000000 NikeCA-0.2.5a0/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14091 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.5a0/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:43:36.000000 NikeCA-0.2.5a0/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 05:42:37.274029 NikeCA-0.2.6/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.6/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-11 05:42:37.273562 NikeCA-0.2.6/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.6/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-11 05:42:37.274180 NikeCA-0.2.6/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2486 2023-05-11 05:42:02.000000 NikeCA-0.2.6/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 05:42:37.264426 NikeCA-0.2.6/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 05:42:37.266196 NikeCA-0.2.6/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.6/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 05:42:37.267681 NikeCA-0.2.6/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.6/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:46:33.000000 NikeCA-0.2.6/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 05:42:37.269882 NikeCA-0.2.6/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.6/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.6/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.6/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.6/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 05:42:37.272948 NikeCA-0.2.6/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-11 05:42:37.000000 NikeCA-0.2.6/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-11 05:42:37.000000 NikeCA-0.2.6/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-11 05:42:37.000000 NikeCA-0.2.6/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-11 05:42:37.000000 NikeCA-0.2.6/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-11 05:42:37.000000 NikeCA-0.2.6/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:48:35.000000 NikeCA-0.2.6/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.6/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19225 2023-05-10 19:50:52.000000 NikeCA-0.2.6/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.6/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13660 2023-05-11 05:36:47.000000 NikeCA-0.2.6/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.6/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.6/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14091 2023-05-10 19:40:28.000000 NikeCA-0.2.6/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-10 19:40:28.000000 NikeCA-0.2.6/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.6/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:43:36.000000 NikeCA-0.2.6/src/__init__.py
```

### Comparing `NikeCA-0.2.5a0/LICENSE` & `NikeCA-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/PKG-INFO` & `NikeCA-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.5a0
+Version: 0.2.6
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.5a0/README.md` & `NikeCA-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/setup.py` & `NikeCA-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.5a',
+	version='0.2.6',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"_BuildSearchQuery",
 		"_GitHub",
 		"_SearchFiles",
 		"_SnowflakeData",
```

### Comparing `NikeCA-0.2.5a0/src/Dashboards/Dashboards.py` & `NikeCA-0.2.6/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.6/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.6/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.2.6/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.6/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.5a0
+Version: 0.2.6
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.5a0/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.6/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.6/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/NikeQA.py` & `NikeCA-0.2.6/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/NikeSF.py` & `NikeCA-0.2.6/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/_BuildSearchQuery.py` & `NikeCA-0.2.6/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/_GitHub.py` & `NikeCA-0.2.6/src/_GitHub.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,16 +248,17 @@
             if linkheads:
                 linkheads_parsed = links_from_header.extract(linkheads)
                 nexturl = linkheads_parsed.get('next', None)
             else:
                 nexturl = None
             respcon = json.loads(resp.content)
 
+            respcon = json.loads(resp.content)
             with open(repo_list_filename, 'w+') as fh:
-                fh.writelines([f'{respconi["full_name"]}\n' for respconi in respcon])
+                fh.writelines([f'{respconi.get("full_name")}\n' for respconi in respcon])
 
     def get_clone(self, git_username: str = None, pat: str = None, filename: str = None, org_name: str = None,
                   repo_name: str = None, repo_list_filename: str = None, repo_directory_name: str | None = None):
         """
         This function clones a repository from GitHub using the username, password/Personal Acess Token (PAT), and
         either a filename or org_name and repo_name. The repository is saved in the savepath directory.
```

### Comparing `NikeCA-0.2.5a0/src/_QA.py` & `NikeCA-0.2.6/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/_SearchFiles.py` & `NikeCA-0.2.6/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/_SnowflakeData.py` & `NikeCA-0.2.6/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/_SnowflakeDependencies.py` & `NikeCA-0.2.6/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.5a0/src/_SnowflakePull.py` & `NikeCA-0.2.6/src/_SnowflakePull.py`

 * *Files identical despite different names*


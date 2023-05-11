# Comparing `tmp/NikeCA-0.2.7.tar.gz` & `tmp/NikeCA-0.2.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.7.tar", last modified: Thu May 11 20:36:55 2023, max compression
+gzip compressed data, was "NikeCA-0.2.7a0.tar", last modified: Thu May 11 20:42:44 2023, max compression
```

## Comparing `NikeCA-0.2.7.tar` & `NikeCA-0.2.7a0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:36:55.908395 NikeCA-0.2.7/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.7/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-11 20:36:55.907921 NikeCA-0.2.7/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.7/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-11 20:36:55.908517 NikeCA-0.2.7/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2539 2023-05-11 20:36:42.000000 NikeCA-0.2.7/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:36:55.897738 NikeCA-0.2.7/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:36:55.899989 NikeCA-0.2.7/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.7/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:36:55.901711 NikeCA-0.2.7/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.7/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:46:33.000000 NikeCA-0.2.7/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:36:55.904280 NikeCA-0.2.7/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.7/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.7/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.7/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.7/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:36:55.907326 NikeCA-0.2.7/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-11 20:36:55.000000 NikeCA-0.2.7/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-11 20:36:55.000000 NikeCA-0.2.7/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-11 20:36:55.000000 NikeCA-0.2.7/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-11 20:36:55.000000 NikeCA-0.2.7/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      394 2023-05-11 20:36:55.000000 NikeCA-0.2.7/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:48:35.000000 NikeCA-0.2.7/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.7/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19225 2023-05-11 20:09:22.000000 NikeCA-0.2.7/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.7/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13660 2023-05-11 05:36:47.000000 NikeCA-0.2.7/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.7/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.7/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14091 2023-05-11 20:09:10.000000 NikeCA-0.2.7/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-11 20:09:00.000000 NikeCA-0.2.7/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.7/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:43:36.000000 NikeCA-0.2.7/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:44.358332 NikeCA-0.2.7a0/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.7a0/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-11 20:42:44.357879 NikeCA-0.2.7a0/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.7a0/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-11 20:42:44.358449 NikeCA-0.2.7a0/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2540 2023-05-11 20:42:38.000000 NikeCA-0.2.7a0/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:44.347684 NikeCA-0.2.7a0/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:44.349304 NikeCA-0.2.7a0/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.7a0/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:44.350493 NikeCA-0.2.7a0/src/Dashboards/IMP/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4387 2023-05-11 20:42:04.000000 NikeCA-0.2.7a0/src/Dashboards/IMP/IMP.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:04.000000 NikeCA-0.2.7a0/src/Dashboards/IMP/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:44.351992 NikeCA-0.2.7a0/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.7a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:46:33.000000 NikeCA-0.2.7a0/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:44.354518 NikeCA-0.2.7a0/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.7a0/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.7a0/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.7a0/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-10 20:43:36.000000 NikeCA-0.2.7a0/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-11 20:42:44.357168 NikeCA-0.2.7a0/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-11 20:42:44.000000 NikeCA-0.2.7a0/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      729 2023-05-11 20:42:44.000000 NikeCA-0.2.7a0/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-11 20:42:44.000000 NikeCA-0.2.7a0/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-11 20:42:44.000000 NikeCA-0.2.7a0/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      394 2023-05-11 20:42:44.000000 NikeCA-0.2.7a0/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:48:35.000000 NikeCA-0.2.7a0/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.7a0/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19225 2023-05-11 20:09:22.000000 NikeCA-0.2.7a0/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.7a0/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13660 2023-05-11 05:36:47.000000 NikeCA-0.2.7a0/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.7a0/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.7a0/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14091 2023-05-11 20:09:10.000000 NikeCA-0.2.7a0/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-11 20:09:00.000000 NikeCA-0.2.7a0/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.7a0/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:43:36.000000 NikeCA-0.2.7a0/src/__init__.py
```

### Comparing `NikeCA-0.2.7/LICENSE` & `NikeCA-0.2.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/PKG-INFO` & `NikeCA-0.2.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.7
+Version: 0.2.7a0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.7/README.md` & `NikeCA-0.2.7a0/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/setup.py` & `NikeCA-0.2.7a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.7',
+	version='0.2.7a',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"_BuildSearchQuery",
 		"_GitHub",
 		"_SearchFiles",
 		"_SnowflakeData",
```

### Comparing `NikeCA-0.2.7/src/Dashboards/Dashboards.py` & `NikeCA-0.2.7a0/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.7a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.7a0/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.2.7a0/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.7a0/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.7
+Version: 0.2.7a0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.7/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.7a0/src/NikeCA.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 src/_SearchFiles.py
 src/_SnowflakeData.py
 src/_SnowflakeDependencies.py
 src/_SnowflakePull.py
 src/__init__.py
 src/Dashboards/Dashboards.py
 src/Dashboards/__init__.py
+src/Dashboards/IMP/IMP.py
+src/Dashboards/IMP/__init__.py
 src/Dashboards/InclusionExclusion/InclusionExclusion.py
 src/Dashboards/InclusionExclusion/__init__.py
 src/Dashboards/Telemetry/ProductUsage.py
 src/Dashboards/Telemetry/Telemetry.py
 src/Dashboards/Telemetry/__init__.py
 src/NikeCA.egg-info/PKG-INFO
 src/NikeCA.egg-info/SOURCES.txt
```

### Comparing `NikeCA-0.2.7/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.7a0/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/NikeQA.py` & `NikeCA-0.2.7a0/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/NikeSF.py` & `NikeCA-0.2.7a0/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/_BuildSearchQuery.py` & `NikeCA-0.2.7a0/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/_GitHub.py` & `NikeCA-0.2.7a0/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/_QA.py` & `NikeCA-0.2.7a0/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/_SearchFiles.py` & `NikeCA-0.2.7a0/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/_SnowflakeData.py` & `NikeCA-0.2.7a0/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/_SnowflakeDependencies.py` & `NikeCA-0.2.7a0/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.7/src/_SnowflakePull.py` & `NikeCA-0.2.7a0/src/_SnowflakePull.py`

 * *Files identical despite different names*


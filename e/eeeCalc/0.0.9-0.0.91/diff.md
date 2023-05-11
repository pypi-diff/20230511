# Comparing `tmp/eeecalc-0.0.9.tar.gz` & `tmp/eeecalc-0.0.91.tar.gz`

## Comparing `eeecalc-0.0.9.tar` & `eeecalc-0.0.91.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/base-eeeCalc.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/vcs.xml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/.DS_Store
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/__init__.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/dBtoRatio.py
--rwxr-xr-x   0        0        0     4721 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/filter.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/general.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/phasors.py
--rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/secondDegreeDiffEq.py
--rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/signalFunctions.py
--rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/transferFunctionPlot.py
--rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/trigFunc.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/eeeCalc.iml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/modules.xml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eeecalc-0.0.9/tests/filterTest.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.9/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.9/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/base-eeeCalc.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/vcs.xml
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/.DS_Store
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/__init__.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/dBtoRatio.py
+-rwxr-xr-x   0        0        0     4721 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/filter.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/general.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/phasors.py
+-rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/secondDegreeDiffEq.py
+-rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/signalFunctions.py
+-rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/transferFunctionPlot.py
+-rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/trigFunc.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/eeeCalc.iml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/modules.xml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eeecalc-0.0.91/tests/filterTest.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.91/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.91/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 eeecalc-0.0.91/pyproject.toml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 eeecalc-0.0.91/PKG-INFO
```

### Comparing `eeecalc-0.0.9/.DS_Store` & `eeecalc-0.0.91/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/.idea/workspace.xml` & `eeecalc-0.0.91/.idea/workspace.xml`

 * *Files 12% similar despite different names*

#### Comparing `eeecalc-0.0.9/.idea/workspace.xml` & `eeecalc-0.0.91/.idea/workspace.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="b760d63e-7a17-4aba-ba56-d8314c16af6d" name="Changes" comment="refined .gitignore and some api stuff"/>
+    <list default="true" id="b760d63e-7a17-4aba-ba56-d8314c16af6d" name="Changes" comment="name change"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
@@ -136,15 +136,57 @@
     <task id="LOCAL-00002" summary="refined .gitignore and some api stuff">
       <created>1683662179010</created>
       <option name="number" value="00002"/>
       <option name="presentableId" value="LOCAL-00002"/>
       <option name="project" value="LOCAL"/>
       <updated>1683662179010</updated>
     </task>
-    <option name="localTasksCounter" value="3"/>
+    <task id="LOCAL-00003" summary="changed version number from 0.0.8 to 0.0.9">
+      <created>1683760193811</created>
+      <option name="number" value="00003"/>
+      <option name="presentableId" value="LOCAL-00003"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683760193811</updated>
+    </task>
+    <task id="LOCAL-00004" summary="changed version number from 0.0.8 to 0.0.9">
+      <created>1683768181443</created>
+      <option name="number" value="00004"/>
+      <option name="presentableId" value="LOCAL-00004"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683768181443</updated>
+    </task>
+    <task id="LOCAL-00005" summary="changed version number from 0.0.8 to 0.0.9">
+      <created>1683768641368</created>
+      <option name="number" value="00005"/>
+      <option name="presentableId" value="LOCAL-00005"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683768641368</updated>
+    </task>
+    <task id="LOCAL-00006" summary="rewrote diffeq function name">
+      <created>1683769238602</created>
+      <option name="number" value="00006"/>
+      <option name="presentableId" value="LOCAL-00006"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683769238602</updated>
+    </task>
+    <task id="LOCAL-00007" summary="Merge remote-tracking branch 'origin/transferFunction'">
+      <created>1683769335747</created>
+      <option name="number" value="00007"/>
+      <option name="presentableId" value="LOCAL-00007"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683769335747</updated>
+    </task>
+    <task id="LOCAL-00008" summary="name change">
+      <created>1683769439669</created>
+      <option name="number" value="00008"/>
+      <option name="presentableId" value="LOCAL-00008"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683769439669</updated>
+    </task>
+    <option name="localTasksCounter" value="9"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
@@ -165,10 +207,14 @@
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="transfer function refined with comments and better more accurate experience, specifically with differences between Hz and rad/s"/>
     <MESSAGE value="refined .gitignore and some api stuff"/>
-    <option name="LAST_COMMIT_MESSAGE" value="refined .gitignore and some api stuff"/>
+    <MESSAGE value="changed version number from 0.0.8 to 0.0.9"/>
+    <MESSAGE value="rewrote diffeq function name"/>
+    <MESSAGE value="Merge remote-tracking branch 'origin/transferFunction'"/>
+    <MESSAGE value="name change"/>
+    <option name="LAST_COMMIT_MESSAGE" value="name change"/>
   </component>
 </project>
```

### Comparing `eeecalc-0.0.9/src/.DS_Store` & `eeecalc-0.0.91/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/src/eeeCalc/dBtoRatio.py` & `eeecalc-0.0.91/src/eeeCalc/dBtoRatio.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/src/eeeCalc/filter.py` & `eeecalc-0.0.91/src/eeeCalc/filter.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/src/eeeCalc/general.py` & `eeecalc-0.0.91/src/eeeCalc/general.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/src/eeeCalc/phasors.py` & `eeecalc-0.0.91/src/eeeCalc/phasors.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/src/eeeCalc/secondDegreeDiffEq.py` & `eeecalc-0.0.91/src/eeeCalc/secondDegreeDiffEq.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/src/eeeCalc/transferFunctionPlot.py` & `eeecalc-0.0.91/src/eeeCalc/transferFunctionPlot.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/src/eeeCalc/.idea/workspace.xml` & `eeecalc-0.0.91/src/eeeCalc/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/.gitignore` & `eeecalc-0.0.91/.gitignore`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/LICENSE` & `eeecalc-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.9/pyproject.toml` & `eeecalc-0.0.91/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "eeeCalc"
-version = "0.0.9"
+version = "0.0.91"
 authors = [
   { name="Kevin Johnson", email="john2003.kjj@gmail.com" },
 ]
 description = "Package to aid electrical engineering calculations"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 #[project.urls]
```


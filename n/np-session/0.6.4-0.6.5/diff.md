# Comparing `tmp/np-session-0.6.4.tar.gz` & `tmp/np-session-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.6.4.tar", last modified: Thu May  4 22:53:13 2023, max compression
+gzip compressed data, was "np-session-0.6.5.tar", last modified: Thu May 11 17:08:22 2023, max compression
```

## Comparing `np-session-0.6.4.tar` & `np-session-0.6.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2289 2023-05-04 22:53:06.521398 np-session-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.4/README.md
--rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.4/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.4/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.4/src/np_session/components/info.py
--rw-r--r--   0        0        0     9191 2023-05-02 22:17:19.176981 np-session-0.6.4/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.4/src/np_session/components/mixins.py
--rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.4/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.4/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.4/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.4/src/np_session/components/state.py
--rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.4/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.4/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.4/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.4/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.4/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.4/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.4/src/np_session/exceptions.py
--rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.4/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.4/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.4/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.4/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0     8942 2023-05-04 00:08:23.244576 np-session-0.6.4/src/np_session/session.py
--rw-r--r--   0        0        0      279 2023-05-04 19:21:42.017380 np-session-0.6.4/src/np_session/subclasses/__init__.py
--rw-r--r--   0        0        0     4954 2023-05-04 02:16:46.922126 np-session-0.6.4/src/np_session/subclasses/dynamic_routing_pilot.py
--rw-r--r--   0        0        0    21567 2023-05-04 02:17:18.728472 np-session-0.6.4/src/np_session/subclasses/pipeline.py
--rw-r--r--   0        0        0     8047 2023-05-04 22:52:29.098852 np-session-0.6.4/src/np_session/subclasses/templeton_pilot.py
--rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.4/src/np_session/tasks.py
--rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.4/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.4/tests/__init__.py
--rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.4/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.4/tests/test_platform_json.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     2289 2023-05-11 17:08:16.970420 np-session-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.5/README.md
+-rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.5/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.5/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.5/src/np_session/components/info.py
+-rw-r--r--   0        0        0     9199 2023-05-11 17:07:49.659610 np-session-0.6.5/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.5/src/np_session/components/mixins.py
+-rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.5/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.5/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.5/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.5/src/np_session/components/state.py
+-rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.5/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.5/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.5/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.5/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.5/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.5/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.5/src/np_session/exceptions.py
+-rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.5/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.5/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.5/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.5/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0     8942 2023-05-04 00:08:23.244576 np-session-0.6.5/src/np_session/session.py
+-rw-r--r--   0        0        0      279 2023-05-04 19:21:42.017380 np-session-0.6.5/src/np_session/subclasses/__init__.py
+-rw-r--r--   0        0        0     4954 2023-05-04 02:16:46.922126 np-session-0.6.5/src/np_session/subclasses/dynamic_routing_pilot.py
+-rw-r--r--   0        0        0    21567 2023-05-04 02:17:18.728472 np-session-0.6.5/src/np_session/subclasses/pipeline.py
+-rw-r--r--   0        0        0     8047 2023-05-04 22:52:29.098852 np-session-0.6.5/src/np_session/subclasses/templeton_pilot.py
+-rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.5/src/np_session/tasks.py
+-rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.5/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.5/tests/__init__.py
+-rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.5/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.5/tests/test_platform_json.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.5/PKG-INFO
```

### Comparing `np-session-0.6.4/pyproject.toml` & `np-session-0.6.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.6.4"
+version = "0.6.5"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np-session-0.6.4/README.md` & `np-session-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/components/info.py` & `np-session-0.6.5/src/np_session/components/info.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/components/lims_manifests.py` & `np-session-0.6.5/src/np_session/components/lims_manifests.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 
         for _ in SESSION_TYPES:
             if _ in (*args, *kwargs.values()):
                 self.session_type = _
                 break
 
         for _ in (*args, *kwargs.values()):
-            if _ in np_session.session.Projects.__members__:
+            if _ in np_session.components.info.Projects.__members__:
                 self.project = _
                 break
 
     def assign_props_from_session(self) -> None:
         if self.project is None:
             self.project = self.session.project.parent.name
             logger.debug(
```

### Comparing `np-session-0.6.4/src/np_session/components/mixins.py` & `np-session-0.6.5/src/np_session/components/mixins.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/components/paths.py` & `np-session-0.6.5/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/components/platform_json.py` & `np-session-0.6.5/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/components/settings_xml.py` & `np-session-0.6.5/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/components/state.py` & `np-session-0.6.5/src/np_session/components/state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/databases/data_getters.py` & `np-session-0.6.5/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/databases/firebase_state.py` & `np-session-0.6.5/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/databases/lims2.py` & `np-session-0.6.5/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/databases/mtrain.py` & `np-session-0.6.5/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/databases/redis_state.py` & `np-session-0.6.5/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/jobs/lims_upload.py` & `np-session-0.6.5/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/jobs/sessions.json` & `np-session-0.6.5/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/jobs/sync_states.py` & `np-session-0.6.5/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/session.py` & `np-session-0.6.5/src/np_session/session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/subclasses/dynamic_routing_pilot.py` & `np-session-0.6.5/src/np_session/subclasses/dynamic_routing_pilot.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/subclasses/pipeline.py` & `np-session-0.6.5/src/np_session/subclasses/pipeline.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/subclasses/templeton_pilot.py` & `np-session-0.6.5/src/np_session/subclasses/templeton_pilot.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/tasks.py` & `np-session-0.6.5/src/np_session/tasks.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/src/np_session/utils.py` & `np-session-0.6.5/src/np_session/utils.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/tests/test_np_session.py` & `np-session-0.6.5/tests/test_np_session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/tests/test_platform_json.py` & `np-session-0.6.5/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.4/PKG-INFO` & `np-session-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.6.4
+Version: 0.6.5
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```


# Comparing `tmp/recon_lw-2.0.0.dev4936886767.tar.gz` & `tmp/recon_lw-2.0.0.dev4937169816.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4936886767.tar", last modified: Wed May 10 12:19:00 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4937169816.tar", last modified: Wed May 10 12:48:21 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4936886767.tar` & `recon_lw-2.0.0.dev4937169816.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-10 12:18:38.000000 recon_lw-2.0.0.dev4936886767/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    21366 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    13987 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-10 12:47:58.000000 recon_lw-2.0.0.dev4937169816/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21366 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14594 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:48:21.000000 recon_lw-2.0.0.dev4937169816/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-10 12:47:52.000000 recon_lw-2.0.0.dev4937169816/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4936886767/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4937169816/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936886767/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4937169816/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936886767/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4937169816/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936886767/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4937169816/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4937169816/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4937169816/recon_lw/recon_ob_cross_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,73 +106,80 @@
     return None, None, None
 
 
 def ob_compare_interpret_match_aggr(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_aggr(match[0]["body"], match[1]["body"])
         if len(comp_res) > 0:
-            error_event = create_event("StreamMismatch",
-                                       "StreamMismatch",
+            error_event = create_event("StreamMismatchAggr",
+                                       "StreamMismatchAggr",
                                        False,
                                        {"full_book_event": match[0]["eventId"],
                                         "aggr_book_event": match[1]["eventId"],
                                         "book_id": match[0]["body"]["book_id"],
-                                        "version": match[0]["body"]["aggr_seq"]["limit_v"],
+                                        "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
+                                        "top_v": match[0]["body"]["aggr_seq"]["top_v"],
                                         "errors": comp_res})
             save_events([error_event])
     elif match[0] is not None:
         tech_info = ob_compare_get_timestamp_key1_key2_aggr(match[0], custom_settings)
         error_event = create_event("StreamMismatchNoAggr",
                                    "StreamMismatchNoAggr",
                                    False,
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
-                                    "version": match[0]["body"]["aggr_seq"]["limit_v"],
+                                    "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
+                                    "top_v": match[0]["body"]["aggr_seq"]["top_v"],
                                     "sessionId": match[0]["body"]["sessionId"],
                                     "tech_info": tech_info})
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "version": match[1]["body"]["aggr_seq"]["limit_v"],
+                                    "limit_v": match[1]["body"]["aggr_seq"]["limit_v"],
+                                   "top_v": match[1]["body"]["aggr_seq"]["top_v"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def ob_compare_interpret_match_top(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_top(match[0]["body"], match[1]["body"])
         if len(comp_res) > 0:
-            error_event = create_event("StreamMismatch",
-                                       "StreamMismatch",
+            error_event = create_event("StreamMismatchTop",
+                                       "StreamMismatchTop",
                                        False,
                                        {"full_book_event": match[0]["eventId"],
                                         "top_book_event": match[1]["eventId"],
                                         "book_id": match[0]["body"]["book_id"],
-                                        "version": match[0]["body"]["aggr_seq"]["limit_v"],
+                                        "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
+                                        "top_v": match[0]["body"]["aggr_seq"]["top_v"],
                                         "errors": comp_res})
             save_events([error_event])
     elif match[0] is not None:
         error_event = create_event("StreamMismatchNoTop",
                                    "StreamMismatchNoTop",
                                    False,
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
-                                    "version": match[0]["body"]["aggr_seq"]["limit_v"]})
+                                    "limit_v": match[0]["body"]["aggr_seq"]["limit_v"],
+                                    "top_v": match[0]["body"]["aggr_seq"]["top_v"],
+                                    "sessionId": match[0]["body"]["sessionId"]})
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"top_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "version": match[1]["body"]["aggr_seq"]["limit_v"],
+                                    "limit_v": match[1]["body"]["aggr_seq"]["limit_v"],
+                                    "top_v": match[1]["body"]["aggr_seq"]["limit_v"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def split_every(n, data):
     iterable = iter(data)
     while 1:
```

### Comparing `recon_lw-2.0.0.dev4936886767/setup.py` & `recon_lw-2.0.0.dev4937169816/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936886767/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4937169816/test/test_recon_ob.py`

 * *Files identical despite different names*


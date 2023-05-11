# Comparing `tmp/recon_lw-2.0.0.dev4945863409.tar.gz` & `tmp/recon_lw-2.0.0.dev4946478922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4945863409.tar", last modified: Thu May 11 08:46:34 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4946478922.tar", last modified: Thu May 11 09:51:47 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4945863409.tar` & `recon_lw-2.0.0.dev4946478922.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-11 08:46:17.000000 recon_lw-2.0.0.dev4945863409/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    23046 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14757 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 08:46:34.000000 recon_lw-2.0.0.dev4945863409/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-11 08:46:11.000000 recon_lw-2.0.0.dev4945863409/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-11 09:51:22.000000 recon_lw-2.0.0.dev4946478922/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23051 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14757 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4945863409/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4946478922/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4945863409/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4946478922/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4945863409/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4946478922/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4945863409/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4946478922/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4945863409/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,23 +144,23 @@
                 skip_aggr = 0
                 for i in range(len(obs)-1):
                     if obs[i]["body"]["aggr_seq"]["top_delta"] == 1:
                         skip_top += 1
                     obs[i]["body"]["aggr_seq"]["top_delta"] = 0
                     obs[i]["body"]["aggr_seq"]["top_v"] = -1
                     if same_level:
-                        if obs[i]["body"]["aggr_seq"]["aggr_delta"] == 1:
+                        if obs[i]["body"]["aggr_seq"]["limit_delta"] == 1:
                             skip_aggr += 1
-                        obs[i]["body"]["aggr_seq"]["aggr_delta"] = 0
-                        obs[i]["body"]["aggr_seq"]["aggr_v"] = -1
+                        obs[i]["body"]["aggr_seq"]["limit_delta"] = 0
+                        obs[i]["body"]["aggr_seq"]["limit_v"] = -1
                 obs[-1]["body"]["aggr_seq"]["top_delta"] = 1
                 obs[-1]["body"]["aggr_seq"]["top_v"] -= skip_top
                 if same_level:
-                    obs[-1]["body"]["aggr_seq"]["aggr_delta"] = 1
-                    obs[-1]["body"]["aggr_seq"]["aggr_v"] -= skip_aggr
+                    obs[-1]["body"]["aggr_seq"]["limit_delta"] = 1
+                    obs[-1]["body"]["aggr_seq"]["limit_v"] -= skip_aggr
 
         events.extend(obs)
 
 
 def process_ob_rules(sequenced_batch: SortedKeyList, books_cache: dict, get_book_id_func,
                      update_book_rule,
                      check_book_rule, event_sequence: dict, send_events_func, parent_event: dict,
```

### Comparing `recon_lw-2.0.0.dev4945863409/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4945863409/setup.py` & `recon_lw-2.0.0.dev4946478922/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4945863409/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4946478922/test/test_recon_ob.py`

 * *Files identical despite different names*


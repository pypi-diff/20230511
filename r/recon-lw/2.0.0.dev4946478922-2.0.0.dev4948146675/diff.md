# Comparing `tmp/recon_lw-2.0.0.dev4946478922.tar.gz` & `tmp/recon_lw-2.0.0.dev4948146675.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4946478922.tar", last modified: Thu May 11 09:51:47 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4948146675.tar", last modified: Thu May 11 12:51:54 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4946478922.tar` & `recon_lw-2.0.0.dev4948146675.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-11 09:51:22.000000 recon_lw-2.0.0.dev4946478922/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    23051 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14757 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 09:51:47.000000 recon_lw-2.0.0.dev4946478922/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-11 09:51:14.000000 recon_lw-2.0.0.dev4946478922/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-11 12:51:32.000000 recon_lw-2.0.0.dev4948146675/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23298 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14757 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:51:54.000000 recon_lw-2.0.0.dev4948146675/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-11 12:51:25.000000 recon_lw-2.0.0.dev4948146675/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4946478922/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4948146675/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4946478922/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4948146675/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4946478922/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4948146675/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4946478922/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4948146675/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4948146675/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,21 @@
                         r["body"]["initial_book"] = initial_book
                     r["body"]["operation"] = operation.__name__
                     r["body"]["book_id"] = book_id
                     r["parentEventId"] = parent_event["eventId"]
                     r["attachedMessageIds"] = [mess["messageId"]]
                     events.append(r)
 
-        if len(obs) >0 and aggregate_batch_updates:
+        if len(obs) >1 and aggregate_batch_updates:
             same_side = all(obs[i]["body"]["aggr_seq"]["affected_side"] == obs[0]["body"]["aggr_seq"]["affected_side"] for i in range(1, len(obs)))
             same_level = all(obs[i]["body"]["aggr_seq"]["affected_level"] == obs[0]["body"]["aggr_seq"]["affected_level"] for i in range(1, len(obs)))
+            obs[0]["body"]["debug_batch_updates"] = len(obs)
+            obs[0]["body"]["debug_same_side"] = same_side
+            obs[0]["body"]["debug_same_level"] = same_level
+
             if same_side:
                 skip_top = 0
                 skip_aggr = 0
                 for i in range(len(obs)-1):
                     if obs[i]["body"]["aggr_seq"]["top_delta"] == 1:
                         skip_top += 1
                     obs[i]["body"]["aggr_seq"]["top_delta"] = 0
@@ -239,14 +243,18 @@
     flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book: dict) -> None:
     order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0}
 
 
+def reset_aggr_seq(order_book):
+    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0, "affected_side": "na", "affected_level": -1})
+
+
 def reflect_price_update_in_version(side: str, price: float, order_book: dict):
     level = get_price_level(side, price, order_book)
     order_book["aggr_seq"]["affected_side"] = side
     order_book["aggr_seq"]["affected_level"] = level
 
     max_levels = order_book["aggr_max_levels"]
     if level <= max_levels:
@@ -256,15 +264,16 @@
         order_book["aggr_seq"]["top_v"] += 1
         order_book["aggr_seq"]["top_delta"] = 1
 
 
 def ob_add_order(order_id: str, price: float, size: int, side: str, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
 
     if find_order_position(order_id, order_book)[0] is not None:
         return {"error": order_id + " already exists"}, []
     if price not in order_book[side]:
         order_book[side][price] = {order_id: size}
     else:
         order_book[side][price][order_id] = size
@@ -272,15 +281,16 @@
     reflect_price_update_in_version(side, price, order_book)
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_update_order(order_id: str, price: float, size: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
         return {"error": order_id + " not found"}, []
 
     log = []
     if price == old_price:
@@ -302,15 +312,16 @@
 
     return {}, log
 
 
 def ob_delete_order(order_id: str, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
         return {"error": order_id + " not found"}, []
 
     log = []
     reflect_price_update_in_version(old_side, old_price, order_book)
@@ -329,15 +340,17 @@
 
     return {}, log
 
 
 def ob_trade_order(order_id: str, traded_size: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
+
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     log = []
     if old_side is None:
         return {"error": order_id + " not found"}, []
     if traded_size > old_size:
         return {"error": "traded size > resting size"}, []
     elif traded_size == old_size:
@@ -360,28 +373,33 @@
         log.append(copy.deepcopy(order_book))
     return {}, log
 
 
 def ob_clean_book(order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
+
     for side_key in ["ask", "bid"]:
         if side_key in order_book:
             order_book[side_key].clear()
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_change_status(new_status: str, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
+    else:
+        reset_aggr_seq(order_book)
+
     order_book["status"] = new_status
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
@@ -403,15 +421,17 @@
     return levels.index(p) + 1 if side == "ask" else len(levels) - levels.index(p)
 
 
 def ob_aggr_add_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
                       impl_num_orders: int, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
+
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     new_index = level - 1
     if not 0 <= new_index <= len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
@@ -425,15 +445,17 @@
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_delete_level(side: str, level: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
+
     result_body = {}
     side_key = side + "_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
 
@@ -444,15 +466,17 @@
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_update_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
                          impl_num_orders: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
+
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     update_index = level - 1
     if not 0 <= update_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body, []
@@ -465,26 +489,30 @@
 
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_clean_book(order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
+    else:
+        reset_aggr_seq(order_book)
+
     for side_key in ["ask_aggr", "bid_aggr"]:
         if side_key in order_book:
             order_book[side_key].clear()
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_top_clean_book(order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
+    else:
+        reset_aggr_seq(order_book)
 
     order_book["ask_price"] = 0
     order_book["ask_real_qty"] = 0
     order_book["ask_impl_qty"] = 0
     order_book["ask_real_n_orders"] = 0
     order_book["ask_impl_n_orders"] = 0
     order_book["bid_price"] = 0
@@ -500,14 +528,17 @@
 
 
 def ob_top_update(ask_price: str, ask_real_qty: str, ask_impl_qty: str, ask_real_n_orders: str, ask_impl_n_orders: str,
                   bid_price: int, bid_real_qty: str, bid_impl_qty: str, bid_real_n_orders: int, bid_impl_n_orders: str,
                   order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
+    else:
+        reset_aggr_seq(order_book)
+
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
     order_book["ask_real_n_orders"] = ask_real_n_orders
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
     order_book["bid_real_qty"] = bid_real_qty
```

### Comparing `recon_lw-2.0.0.dev4946478922/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4948146675/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4946478922/setup.py` & `recon_lw-2.0.0.dev4948146675/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4946478922/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4948146675/test/test_recon_ob.py`

 * *Files identical despite different names*


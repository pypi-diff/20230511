# Comparing `tmp/polygon-sdk-client-1.0.1.tar.gz` & `tmp/polygon-sdk-client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon-sdk-client-1.0.1.tar", last modified: Thu May 11 21:19:19 2023, max compression
+gzip compressed data, was "polygon-sdk-client-1.1.1.tar", last modified: Thu May 11 21:32:48 2023, max compression
```

## Comparing `polygon-sdk-client-1.0.1.tar` & `polygon-sdk-client-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 21:19:19.533702 polygon-sdk-client-1.0.1/
--rw-rw-rw-   0        0        0       89 2023-05-11 21:19:19.533702 polygon-sdk-client-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 21:19:19.514980 polygon-sdk-client-1.0.1/polygon_sdk/
--rw-rw-rw-   0        0        0        0 2023-05-05 01:43:16.000000 polygon-sdk-client-1.0.1/polygon_sdk/__init__.py
--rw-rw-rw-   0        0        0     1398 2023-05-07 06:11:03.000000 polygon-sdk-client-1.0.1/polygon_sdk/aggregates.py
--rw-rw-rw-   0        0        0    41119 2023-05-11 20:20:03.000000 polygon-sdk-client-1.0.1/polygon_sdk/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     1730 2023-05-06 02:03:07.000000 polygon-sdk-client-1.0.1/polygon_sdk/company_info.py
--rw-rw-rw-   0        0        0     2086 2023-05-09 20:29:16.000000 polygon-sdk-client-1.0.1/polygon_sdk/conditions.py
--rw-rw-rw-   0        0        0      723 2023-03-26 14:45:02.000000 polygon-sdk-client-1.0.1/polygon_sdk/daily_open_close.py
--rw-rw-rw-   0        0        0    24263 2023-05-09 13:03:23.000000 polygon-sdk-client-1.0.1/polygon_sdk/dictionaries.py
--rw-rw-rw-   0        0        0     1869 2023-03-24 22:11:15.000000 polygon-sdk-client-1.0.1/polygon_sdk/ema.py
--rw-rw-rw-   0        0        0      910 2023-04-08 14:08:49.000000 polygon-sdk-client-1.0.1/polygon_sdk/embeddings.py
--rw-rw-rw-   0        0        0     1041 2023-05-09 20:53:09.000000 polygon-sdk-client-1.0.1/polygon_sdk/extra_data.py
--rw-rw-rw-   0        0        0    15262 2023-05-07 17:43:52.000000 polygon-sdk-client-1.0.1/polygon_sdk/financials.py
--rw-rw-rw-   0        0        0      753 2023-03-25 21:04:05.000000 polygon-sdk-client-1.0.1/polygon_sdk/helpers.py
--rw-rw-rw-   0        0        0     1005 2023-05-07 18:14:26.000000 polygon-sdk-client-1.0.1/polygon_sdk/indices_snapshot.py
--rw-rw-rw-   0        0        0        6 2023-05-11 20:19:22.000000 polygon-sdk-client-1.0.1/polygon_sdk/logo.py
--rw-rw-rw-   0        0        0      340 2023-04-17 19:09:47.000000 polygon-sdk-client-1.0.1/polygon_sdk/macd.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:19:19.515981 polygon-sdk-client-1.0.1/polygon_sdk/mapping/
--rw-rw-rw-   0        0        0    24838 2023-05-06 13:11:03.000000 polygon-sdk-client-1.0.1/polygon_sdk/mapping/mapping_dicts.py
--rw-rw-rw-   0        0        0     3287 2023-04-27 13:19:35.000000 polygon-sdk-client-1.0.1/polygon_sdk/models.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:19:19.520630 polygon-sdk-client-1.0.1/polygon_sdk/options_market/
--rw-rw-rw-   0        0        0    19097 2023-05-11 20:26:14.000000 polygon-sdk-client-1.0.1/polygon_sdk/options_market/async_options_sdk.py
--rw-rw-rw-   0        0        0      416 2023-05-10 03:00:32.000000 polygon-sdk-client-1.0.1/polygon_sdk/options_market/daily_oc.py
--rw-rw-rw-   0        0        0     9147 2023-05-11 20:31:17.000000 polygon-sdk-client-1.0.1/polygon_sdk/options_market/get_all_options.py
--rw-rw-rw-   0        0        0      842 2023-03-30 22:00:34.000000 polygon-sdk-client-1.0.1/polygon_sdk/options_market/option_aggs.py
--rw-rw-rw-   0        0        0     3525 2023-05-04 04:04:43.000000 polygon-sdk-client-1.0.1/polygon_sdk/options_market/option_snapshot.py
--rw-rw-rw-   0        0        0      587 2023-05-10 03:15:58.000000 polygon-sdk-client-1.0.1/polygon_sdk/options_market/option_trades.py
--rw-rw-rw-   0        0        0      556 2023-04-17 13:14:22.000000 polygon-sdk-client-1.0.1/polygon_sdk/pivot_points.py
--rw-rw-rw-   0        0        0      710 2023-04-14 17:39:56.000000 polygon-sdk-client-1.0.1/polygon_sdk/quote.py
--rw-rw-rw-   0        0        0     9408 2023-05-11 20:13:25.000000 polygon-sdk-client-1.0.1/polygon_sdk/snapshot.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:19:19.521630 polygon-sdk-client-1.0.1/polygon_sdk/test_events/
--rw-rw-rw-   0        0        0     2490 2023-05-02 06:27:35.000000 polygon-sdk-client-1.0.1/polygon_sdk/test_events/test_stock.py
--rw-rw-rw-   0        0        0     7511 2023-05-11 20:22:47.000000 polygon-sdk-client-1.0.1/polygon_sdk/tickernews.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:19:19.532703 polygon-sdk-client-1.0.1/polygon_sdk_client.egg-info/
--rw-rw-rw-   0        0        0       89 2023-05-11 21:19:19.000000 polygon-sdk-client-1.0.1/polygon_sdk_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-11 21:19:19.000000 polygon-sdk-client-1.0.1/polygon_sdk_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 21:19:19.000000 polygon-sdk-client-1.0.1/polygon_sdk_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1984 2023-05-11 21:19:19.000000 polygon-sdk-client-1.0.1/polygon_sdk_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 21:19:19.000000 polygon-sdk-client-1.0.1/polygon_sdk_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 21:19:19.533702 polygon-sdk-client-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3821 2023-05-11 21:19:05.000000 polygon-sdk-client-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:32:48.368106 polygon-sdk-client-1.1.1/
+-rw-rw-rw-   0        0        0       89 2023-05-11 21:32:48.368106 polygon-sdk-client-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 21:32:48.351016 polygon-sdk-client-1.1.1/polygon_sdk/
+-rw-rw-rw-   0        0        0        0 2023-05-05 01:43:16.000000 polygon-sdk-client-1.1.1/polygon_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1398 2023-05-07 06:11:03.000000 polygon-sdk-client-1.1.1/polygon_sdk/aggregates.py
+-rw-rw-rw-   0        0        0    41119 2023-05-11 20:20:03.000000 polygon-sdk-client-1.1.1/polygon_sdk/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0     1730 2023-05-06 02:03:07.000000 polygon-sdk-client-1.1.1/polygon_sdk/company_info.py
+-rw-rw-rw-   0        0        0     2086 2023-05-09 20:29:16.000000 polygon-sdk-client-1.1.1/polygon_sdk/conditions.py
+-rw-rw-rw-   0        0        0      723 2023-03-26 14:45:02.000000 polygon-sdk-client-1.1.1/polygon_sdk/daily_open_close.py
+-rw-rw-rw-   0        0        0    24263 2023-05-09 13:03:23.000000 polygon-sdk-client-1.1.1/polygon_sdk/dictionaries.py
+-rw-rw-rw-   0        0        0     1869 2023-03-24 22:11:15.000000 polygon-sdk-client-1.1.1/polygon_sdk/ema.py
+-rw-rw-rw-   0        0        0      910 2023-04-08 14:08:49.000000 polygon-sdk-client-1.1.1/polygon_sdk/embeddings.py
+-rw-rw-rw-   0        0        0     1041 2023-05-09 20:53:09.000000 polygon-sdk-client-1.1.1/polygon_sdk/extra_data.py
+-rw-rw-rw-   0        0        0    15262 2023-05-07 17:43:52.000000 polygon-sdk-client-1.1.1/polygon_sdk/financials.py
+-rw-rw-rw-   0        0        0      753 2023-03-25 21:04:05.000000 polygon-sdk-client-1.1.1/polygon_sdk/helpers.py
+-rw-rw-rw-   0        0        0     1005 2023-05-07 18:14:26.000000 polygon-sdk-client-1.1.1/polygon_sdk/indices_snapshot.py
+-rw-rw-rw-   0        0        0        6 2023-05-11 20:19:22.000000 polygon-sdk-client-1.1.1/polygon_sdk/logo.py
+-rw-rw-rw-   0        0        0      340 2023-04-17 19:09:47.000000 polygon-sdk-client-1.1.1/polygon_sdk/macd.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:32:48.352016 polygon-sdk-client-1.1.1/polygon_sdk/mapping/
+-rw-rw-rw-   0        0        0    24838 2023-05-06 13:11:03.000000 polygon-sdk-client-1.1.1/polygon_sdk/mapping/mapping_dicts.py
+-rw-rw-rw-   0        0        0     3287 2023-04-27 13:19:35.000000 polygon-sdk-client-1.1.1/polygon_sdk/models.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:32:48.356016 polygon-sdk-client-1.1.1/polygon_sdk/options_market/
+-rw-rw-rw-   0        0        0    19097 2023-05-11 20:26:14.000000 polygon-sdk-client-1.1.1/polygon_sdk/options_market/async_options_sdk.py
+-rw-rw-rw-   0        0        0      416 2023-05-10 03:00:32.000000 polygon-sdk-client-1.1.1/polygon_sdk/options_market/daily_oc.py
+-rw-rw-rw-   0        0        0     9147 2023-05-11 20:31:17.000000 polygon-sdk-client-1.1.1/polygon_sdk/options_market/get_all_options.py
+-rw-rw-rw-   0        0        0      842 2023-03-30 22:00:34.000000 polygon-sdk-client-1.1.1/polygon_sdk/options_market/option_aggs.py
+-rw-rw-rw-   0        0        0     3525 2023-05-04 04:04:43.000000 polygon-sdk-client-1.1.1/polygon_sdk/options_market/option_snapshot.py
+-rw-rw-rw-   0        0        0      587 2023-05-10 03:15:58.000000 polygon-sdk-client-1.1.1/polygon_sdk/options_market/option_trades.py
+-rw-rw-rw-   0        0        0      556 2023-04-17 13:14:22.000000 polygon-sdk-client-1.1.1/polygon_sdk/pivot_points.py
+-rw-rw-rw-   0        0        0      710 2023-04-14 17:39:56.000000 polygon-sdk-client-1.1.1/polygon_sdk/quote.py
+-rw-rw-rw-   0        0        0     9408 2023-05-11 20:13:25.000000 polygon-sdk-client-1.1.1/polygon_sdk/snapshot.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:32:48.357016 polygon-sdk-client-1.1.1/polygon_sdk/test_events/
+-rw-rw-rw-   0        0        0     2490 2023-05-02 06:27:35.000000 polygon-sdk-client-1.1.1/polygon_sdk/test_events/test_stock.py
+-rw-rw-rw-   0        0        0     7511 2023-05-11 20:22:47.000000 polygon-sdk-client-1.1.1/polygon_sdk/tickernews.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:32:48.367106 polygon-sdk-client-1.1.1/polygon_sdk_client.egg-info/
+-rw-rw-rw-   0        0        0       89 2023-05-11 21:32:48.000000 polygon-sdk-client-1.1.1/polygon_sdk_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-05-11 21:32:48.000000 polygon-sdk-client-1.1.1/polygon_sdk_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 21:32:48.000000 polygon-sdk-client-1.1.1/polygon_sdk_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      769 2023-05-11 21:32:48.000000 polygon-sdk-client-1.1.1/polygon_sdk_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 21:32:48.000000 polygon-sdk-client-1.1.1/polygon_sdk_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 21:32:48.368106 polygon-sdk-client-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1490 2023-05-11 21:32:37.000000 polygon-sdk-client-1.1.1/setup.py
```

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/aggregates.py` & `polygon-sdk-client-1.1.1/polygon_sdk/aggregates.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/async_polygon_sdk.py` & `polygon-sdk-client-1.1.1/polygon_sdk/async_polygon_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/company_info.py` & `polygon-sdk-client-1.1.1/polygon_sdk/company_info.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/conditions.py` & `polygon-sdk-client-1.1.1/polygon_sdk/conditions.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/daily_open_close.py` & `polygon-sdk-client-1.1.1/polygon_sdk/daily_open_close.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/dictionaries.py` & `polygon-sdk-client-1.1.1/polygon_sdk/dictionaries.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/ema.py` & `polygon-sdk-client-1.1.1/polygon_sdk/ema.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/embeddings.py` & `polygon-sdk-client-1.1.1/polygon_sdk/embeddings.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/extra_data.py` & `polygon-sdk-client-1.1.1/polygon_sdk/extra_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/financials.py` & `polygon-sdk-client-1.1.1/polygon_sdk/financials.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/helpers.py` & `polygon-sdk-client-1.1.1/polygon_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/indices_snapshot.py` & `polygon-sdk-client-1.1.1/polygon_sdk/indices_snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/mapping/mapping_dicts.py` & `polygon-sdk-client-1.1.1/polygon_sdk/mapping/mapping_dicts.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/models.py` & `polygon-sdk-client-1.1.1/polygon_sdk/models.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/options_market/async_options_sdk.py` & `polygon-sdk-client-1.1.1/polygon_sdk/options_market/async_options_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/options_market/get_all_options.py` & `polygon-sdk-client-1.1.1/polygon_sdk/options_market/get_all_options.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/options_market/option_aggs.py` & `polygon-sdk-client-1.1.1/polygon_sdk/options_market/option_aggs.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/options_market/option_snapshot.py` & `polygon-sdk-client-1.1.1/polygon_sdk/options_market/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/options_market/option_trades.py` & `polygon-sdk-client-1.1.1/polygon_sdk/options_market/option_trades.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/pivot_points.py` & `polygon-sdk-client-1.1.1/polygon_sdk/pivot_points.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/quote.py` & `polygon-sdk-client-1.1.1/polygon_sdk/quote.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/snapshot.py` & `polygon-sdk-client-1.1.1/polygon_sdk/snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/test_events/test_stock.py` & `polygon-sdk-client-1.1.1/polygon_sdk/test_events/test_stock.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk/tickernews.py` & `polygon-sdk-client-1.1.1/polygon_sdk/tickernews.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-client-1.0.1/polygon_sdk_client.egg-info/SOURCES.txt` & `polygon-sdk-client-1.1.1/polygon_sdk_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/spotON_sdk-0.0.3.6.tar.gz` & `tmp/spotON_sdk-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.3.6.tar", last modified: Wed May 10 15:34:44 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.3.7.tar", last modified: Thu May 11 09:14:46 2023, max compression
```

## Comparing `spotON_sdk-0.0.3.6.tar` & `spotON_sdk-0.0.3.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.6/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.6/LICENSE
--rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.6/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-10 15:34:37.424455 spotON_sdk-0.0.3.6/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.6/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4640 2023-05-10 15:34:03.631538 spotON_sdk-0.0.3.6/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2215 2023-05-09 22:15:15.648490 spotON_sdk-0.0.3.6/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.6/spotON_sdk/logic/BestHour.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.6/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.6/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.6/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0       94 2023-05-09 21:55:38.975092 spotON_sdk-0.0.3.6/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.7/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.7/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-11 09:12:35.474099 spotON_sdk-0.0.3.7/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.7/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4640 2023-05-11 09:12:50.539688 spotON_sdk-0.0.3.7/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2309 2023-05-11 09:13:15.250068 spotON_sdk-0.0.3.7/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.7/spotON_sdk/logic/BestHour.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.7/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.7/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.7/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0       94 2023-05-09 21:55:38.975092 spotON_sdk-0.0.3.7/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.7/PKG-INFO
```

### Comparing `spotON_sdk-0.0.3.6/.gitignore` & `spotON_sdk-0.0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.6/LICENSE` & `spotON_sdk-0.0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.6/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.3.7/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.6/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.3.7/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.6/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.3.7/spotON_sdk/constants/markets.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,18 +48,20 @@
     #luxembourg = Market(Area.DE_LU,Luxembourg)
     sweden1 = Market(Area.SE_1,Sweden)
     #sweden2 = Market(Area.SE_2,Sweden)
     #sweden3 = Market(Area.SE_3,Sweden)
     #sweden4 = Market(Area.SE_4,Sweden)
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
     merged_Markets = []
+
     @staticmethod
     def get_Market_by_area_code(area_code: str) -> Optional[Market]:
         for country in Markets.markets_List:
-            if country.country_code == area_code:
+            #print (f"Try to find {area_code =} in {country}")
+            if country.country_code == area_code or country.alias == area_code:
                 return country
 
         return None
 
 
 def return_All_Areas(filterstring:str ="MBA"):
```

### Comparing `spotON_sdk-0.0.3.6/spotON_sdk/logic/BestHour.py` & `spotON_sdk-0.0.3.7/spotON_sdk/logic/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.6/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.3.7/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.6/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.3.7/spotON_sdk/logic/Entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.6/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.3.7/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*


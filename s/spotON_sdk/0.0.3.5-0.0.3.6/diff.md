# Comparing `tmp/spotON_sdk-0.0.3.5.tar.gz` & `tmp/spotON_sdk-0.0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.3.5.tar", last modified: Tue May  9 22:15:45 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.3.6.tar", last modified: Wed May 10 15:34:44 2023, max compression
```

## Comparing `spotON_sdk-0.0.3.5.tar` & `spotON_sdk-0.0.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.5/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.5/LICENSE
--rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.5/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-09 22:15:41.320706 spotON_sdk-0.0.3.5/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.5/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.5/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2215 2023-05-09 22:15:15.648490 spotON_sdk-0.0.3.5/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.5/spotON_sdk/logic/BestHour.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.5/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.5/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.5/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0       94 2023-05-09 21:55:38.975092 spotON_sdk-0.0.3.5/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.6/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.6/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-10 15:34:37.424455 spotON_sdk-0.0.3.6/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.6/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4640 2023-05-10 15:34:03.631538 spotON_sdk-0.0.3.6/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2215 2023-05-09 22:15:15.648490 spotON_sdk-0.0.3.6/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.6/spotON_sdk/logic/BestHour.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.6/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.6/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.6/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0       94 2023-05-09 21:55:38.975092 spotON_sdk-0.0.3.6/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.6/PKG-INFO
```

### Comparing `spotON_sdk-0.0.3.5/.gitignore` & `spotON_sdk-0.0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.5/LICENSE` & `spotON_sdk-0.0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.5/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.3.6/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.5/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.3.6/spotON_sdk/constants/countries.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,31 +16,32 @@
     capital: str
     country_code: str
     country_name: str
     UTC_time_difference: int = field(init=False)
     
     def calculate_utc_time_difference(self) -> Optional[pd.Timedelta]:
         try:
-            #print ("calculating timezone differecne")
             timezone = f"Europe/{self.capital}"
             local_tz = pytz.timezone(timezone)
             utc_dt = pd.Timestamp.utcnow().to_pydatetime()
             local_dt = utc_dt.astimezone(local_tz)
             UTC_time_difference = (local_dt.utcoffset().total_seconds()) // 3600
             delta = pd.Timedelta(hours=UTC_time_difference)
-            return delta,UTC_time_difference
-        
+            return delta, UTC_time_difference
+
         except:
             print(f"{self.capital} not found in European capitals.")
-            return None
+            default_delta = pd.Timedelta(hours=0)
+            default_UTC_time_difference = 0
+            return default_delta, default_UTC_time_difference
 
-    def __post_init__(self: Any) -> None:
+    def __post_init__(self) -> None:
         self.delta,self.UTC_time_difference = self.calculate_utc_time_difference()
         self.emoji = _country_code_to_emoji(self.country_code)
-
+        
 def get_country_by_code(countries: List[Country], country_code: str) -> Optional[Country]:
     """
     Returns the country object that matches the given country code.
     If no such object is found, returns None.
     """
     for country in countries:
         if country.country_code == country_code:
```

### Comparing `spotON_sdk-0.0.3.5/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.3.6/spotON_sdk/constants/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.5/spotON_sdk/logic/BestHour.py` & `spotON_sdk-0.0.3.6/spotON_sdk/logic/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.5/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.3.6/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.5/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.3.6/spotON_sdk/logic/Entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.5/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.3.6/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*


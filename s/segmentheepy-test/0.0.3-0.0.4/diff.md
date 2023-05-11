# Comparing `tmp/segmentheepy_test-0.0.3-py3-none-any.whl.zip` & `tmp/segmentheepy_test-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10122 bytes, number of entries: 9
--rw-rw-r--  2.0 unx        0 b- defN 23-May-09 16:01 segmenthee/__init__.py
--rw-rw-r--  2.0 unx    24731 b- defN 23-May-09 18:18 segmenthee/cart_api.py
--rw-rw-r--  2.0 unx      766 b- defN 23-May-09 16:01 segmenthee/config.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-May-09 16:01 segmenthee/parser_api.py
--rw-rw-r--  2.0 unx     7932 b- defN 23-May-09 16:02 segmenthee/shop.py
--rw-rw-r--  2.0 unx      308 b- defN 23-May-09 18:20 segmentheepy_test-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-09 18:20 segmentheepy_test-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-09 18:20 segmentheepy_test-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      725 b- defN 23-May-09 18:20 segmentheepy_test-0.0.3.dist-info/RECORD
-9 files, 36588 bytes uncompressed, 8868 bytes compressed:  75.8%
+Zip file size: 10448 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-26 09:11 segmenthee/__init__.py
+-rw-rw-r--  2.0 unx    25660 b- defN 23-May-11 12:16 segmenthee/cart_api.py
+-rw-rw-r--  2.0 unx      766 b- defN 23-Apr-26 09:11 segmenthee/config.py
+-rw-rw-r--  2.0 unx     2023 b- defN 23-Apr-26 09:11 segmenthee/parser_api.py
+-rw-rw-r--  2.0 unx     7932 b- defN 23-Apr-26 09:12 segmenthee/shop.py
+-rw-rw-r--  2.0 unx      288 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      725 b- defN 23-May-11 12:28 segmentheepy_test-0.0.4.dist-info/RECORD
+9 files, 37497 bytes uncompressed, 9194 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: segmenthee/parser_api.py
 Comment: 
 
 Filename: segmenthee/shop.py
 Comment: 
 
-Filename: segmentheepy_test-0.0.3.dist-info/METADATA
+Filename: segmentheepy_test-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: segmentheepy_test-0.0.3.dist-info/WHEEL
+Filename: segmentheepy_test-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: segmentheepy_test-0.0.3.dist-info/top_level.txt
+Filename: segmentheepy_test-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: segmentheepy_test-0.0.3.dist-info/RECORD
+Filename: segmentheepy_test-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## segmenthee/cart_api.py

```diff
@@ -2,14 +2,15 @@
 import copy
 import json
 from typing import Union, Tuple, List, Dict, Any
 import numpy as np
 import xgboost
 from segmenthee.config import Config
 from segmenthee import parser_api
+import statsmodels.api as sm
 
 ABANDONER = 1
 BUYER = 0
 
 FILE_NAME = 'xgbm.sav'
 SCORE_THRESHOLD = Config.SCORE_THRESHOLD
 FRUSTRATION_TOLERANCE = Config.FRUSTRATION_TOLERANCE
@@ -141,14 +142,37 @@
 def GetCoefficients(coeffs, params, delta_time):
     ''' exp(-lambda * delta_time) '''
     for key in params:
         if not isinstance(params[key],list):
             continue
         coeffs[key][1] = np.exp(-params[key][1] * delta_time)
 
+def CalculateUnalikeability(list):
+    n = len(list)
+    if n == 1:
+        return 0 # may be better to return 1
+    s = 0
+    for i in range(n-1):
+        for j in range(i+1,n):
+            if list[i] != list[j]:
+                s += 1
+    u = 2*s/(n**2 - n)
+    return u
+
+def CalculateAutocorrelation(list):
+    if len(list) == 1 or CalculateUnalikeability(list) == 0:
+        return 0
+    s = set()
+    for i in list:
+        s.add(i)
+    enc = {value:idx for idx,value in enumerate(s)}
+    list = [enc[val] for val in list]    
+    autocorr = sm.tsa.acf(list, nlags = len(list)-1)[1:]
+    return max(autocorr, key=abs)
+
 class SessionBodyEvent:
     def __init__(self, time: int):
         self.time = time
 
     def Update(self,prevstate):
         retval = copy.deepcopy(prevstate)
         retval["lastbodyeventtime"] = self.time
@@ -305,14 +329,17 @@
         retval = super().Update(prevstate)
         retval["lastcategory"] = self.category_id
         category = self.category_id
         LogCategory(retval,self.coeffs,category)
         retval["lastprice"] = self.price
         UpdateAttribute(retval, self.coeffs, "lastpriceviewedtrend", self.price)
         retval["producteverviewed"] = 1
+        retval["product_ids"].append(self.product_id)
+        retval["autocorr"] = CalculateAutocorrelation(retval["product_ids"])
+        retval["u_product"] = CalculateUnalikeability(retval["product_ids"])
         return retval
 
 class CartBrowsingEvent(BrowsingEvent):
 
     cindex = nextclassindex()
     classnames[cindex] = "CartBrowsingEvent"
 
@@ -535,23 +562,25 @@
         "tabtypetrend" : [0.0] * len(params["tabtypetrend"]),
         "navigationtrend": [0.0] * len(params["navigationtrend"]),
         "referrertrend": [0.0] * len(params["referrertrend"]),
         "sorttrend": [0.0] * len(params["sorttrend"]),
         "pagetrend": [0.0] * len(params["pagetrend"]),
         "producteverviewed": 0,
         "highwatermark": 0,
-        #"productdict": dict()
+        "product_ids": [],
+        "u_product": -1,
+        "autocorr": 0
     }
 
     return Update(original_state,firstbodyevent,newparams)
 
 def RowOfState(state):
     row ={k:state[k] for k in ["actioncount","origin","device","os","lang","carttotal","cartcount", "producteverviewed","couponstatus","clickrate_avg",
                                #"clickrate_squares",
-                               "clickrate_var","z_score"]}                  
+                               "clickrate_var","z_score", "u_product", "autocorr"]}                  
     row["sessionage"] = state["lastbodyeventtime"] - state["sessionstart"]
     lastbodyeventtime = datetime.datetime.fromtimestamp(state["lastbodyeventtime"])
     row["hourofday"] = lastbodyeventtime.hour
     row["dayofweek"] = lastbodyeventtime.weekday()
     row["dayofmonth"] = lastbodyeventtime.day
     row["cartaverageprice"] = state["carttotal"]/state["cartcount"] if state["cartcount"] != 0 else 0.0
     # row["highwatermark"] = state["highwatermark"]
```

## Comparing `segmentheepy_test-0.0.3.dist-info/RECORD` & `segmentheepy_test-0.0.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 segmenthee/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-segmenthee/cart_api.py,sha256=vMuGM4y10HKGiYVq8AYFC5sYCKP7Vhbz8vH00AqK5Ps,24731
+segmenthee/cart_api.py,sha256=ExPwGSJ5oy2C_OyXiEmRz72Jt6F9ZpYvBOOm2a9o7r0,25660
 segmenthee/config.py,sha256=lXea6JINCK44eZP38JaQOlfgVerzFx0e9wDxObuw54c,766
 segmenthee/parser_api.py,sha256=TB-Q8roqNAV_wwYSrdJYchNoC3zTGRKI0die0sN-K-8,2023
 segmenthee/shop.py,sha256=RlKZfL1vebVw6JOxUthPfzgzkcU7MaAYE96Wc4EYDJQ,7932
-segmentheepy_test-0.0.3.dist-info/METADATA,sha256=_tstasHRBbNfN-P35N_gknUu_ONuEr1aHWSkCesJuk0,308
-segmentheepy_test-0.0.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-segmentheepy_test-0.0.3.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
-segmentheepy_test-0.0.3.dist-info/RECORD,,
+segmentheepy_test-0.0.4.dist-info/METADATA,sha256=NhMAS2iF_jTov3JZLu4KjF2raOWe0Emuk7k5TuzeGOw,288
+segmentheepy_test-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+segmentheepy_test-0.0.4.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
+segmentheepy_test-0.0.4.dist-info/RECORD,,
```


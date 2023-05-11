# Comparing `tmp/atlantic-1.0.55-py3-none-any.whl.zip` & `tmp/atlantic-1.0.60-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18666 bytes, number of entries: 12
+Zip file size: 18667 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 atlantic/__init__.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-17 10:17 atlantic/atl_feat_eng.py
+-rw-rw-rw-  2.0 fat     5500 b- defN 23-May-11 19:39 atlantic/atl_feat_eng.py
 -rw-rw-rw-  2.0 fat     8704 b- defN 23-Apr-17 10:49 atlantic/atl_feat_selection.py
 -rw-rw-rw-  2.0 fat     1563 b- defN 23-Apr-17 09:56 atlantic/atl_metrics.py
 -rw-rw-rw-  2.0 fat     2862 b- defN 23-May-06 15:26 atlantic/atl_performance.py
 -rw-rw-rw-  2.0 fat     8541 b- defN 23-Apr-17 10:17 atlantic/atl_pipeline.py
 -rw-rw-rw-  2.0 fat    20571 b- defN 23-May-06 15:42 atlantic/atl_processing.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12316 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      969 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/RECORD
-12 files, 62604 bytes uncompressed, 17046 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-May-11 19:43 atlantic-1.0.60.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12317 b- defN 23-May-11 19:43 atlantic-1.0.60.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-11 19:43 atlantic-1.0.60.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-11 19:43 atlantic-1.0.60.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      969 b- defN 23-May-11 19:43 atlantic-1.0.60.dist-info/RECORD
+12 files, 62595 bytes uncompressed, 17047 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: atlantic/atl_pipeline.py
 Comment: 
 
 Filename: atlantic/atl_processing.py
 Comment: 
 
-Filename: atlantic-1.0.55.dist-info/LICENSE
+Filename: atlantic-1.0.60.dist-info/LICENSE
 Comment: 
 
-Filename: atlantic-1.0.55.dist-info/METADATA
+Filename: atlantic-1.0.60.dist-info/METADATA
 Comment: 
 
-Filename: atlantic-1.0.55.dist-info/WHEEL
+Filename: atlantic-1.0.60.dist-info/WHEEL
 Comment: 
 
-Filename: atlantic-1.0.55.dist-info/top_level.txt
+Filename: atlantic-1.0.60.dist-info/top_level.txt
 Comment: 
 
-Filename: atlantic-1.0.55.dist-info/RECORD
+Filename: atlantic-1.0.60.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atlantic/atl_feat_eng.py

```diff
@@ -37,15 +37,15 @@
     y_test = test.iloc[:, (len(sel_cols)-1)].values
     
     return X_train,X_test,y_train,y_test
 
 def slice_timestamp(dataset:pd.DataFrame):
     
     df=dataset.copy()
-    datetime_cols=list_date=list(df.select_dtypes(include=['datetime','datetime64[ns]']))
+    datetime_cols=list(df.select_dtypes(include=['datetime','datetime64[ns]']))
     for date_col in datetime_cols:
             df[date_col] = df[date_col].astype(str)
             df[date_col] = df[date_col].str.slice(0,19)
             df[date_col] = pd.to_datetime(df[date_col])
             
     return df
```

## Comparing `atlantic-1.0.55.dist-info/LICENSE` & `atlantic-1.0.60.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atlantic-1.0.55.dist-info/METADATA` & `atlantic-1.0.60.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlantic
-Version: 1.0.55
+Version: 1.0.60
 Summary: Atlantic is an automated preprocessing framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/Atlantic
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,predictive modeling,data preprocessing,automated data preprocessing,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -88,15 +88,15 @@
 * encoding_fs: You can choose if you want to encond your features in order to reduce loading time in "H2O AutoML feature selection" step. If in "True" mode label encoding is applied to categorical features.
 * vif_ratio: This value defines the minimal 'threshold' for Variance Inflation Factor filtering (default value=10).
  
 Importante Notes:
     
 * Default predictive evaluation metric for regression contexts is MAE (Mean Absolute Error) and classification is AUC (Accuracy).
 * Although functional, `Atlantic` data processing is not optimized for big data purposes yet.
-* Major update is now available in **versions>=1.0.5**
+* Major update is now available in **versions>=1.0.50**
     
 ```py
     
 import atlantic as atl
 import pandas as pd   
     
 data = pd.read_csv('csv_directory_path', encoding='latin', delimiter=',') # Dataframe Loading Example
```

## Comparing `atlantic-1.0.55.dist-info/RECORD` & `atlantic-1.0.60.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 atlantic/__init__.py,sha256=aJxiUy0U6d3cxOQQo5m4ATN4A3xAGwAFCqCl21JTvhM,389
-atlantic/atl_feat_eng.py,sha256=qTxn3NxyT_GRR4gdmlLCIrNfL5xViqZEQ29iQpo8cug,5510
+atlantic/atl_feat_eng.py,sha256=Xio6qpJLszw59TkKEgvf9ry-jnODwZAY7O3PxvN-22g,5500
 atlantic/atl_feat_selection.py,sha256=r1H8N7DEbbNgo8jUT9kA-5JRmc9v1WVZ3Bf1zU-ACAI,8704
 atlantic/atl_metrics.py,sha256=ZbP98YCmgf0UTiCtozQDRzVARP4EWy9GvzqbQ1XcJ_s,1563
 atlantic/atl_performance.py,sha256=1O9718eY3Ppko1COIYO8MKMS7eaH0xP5fc2CKX0Hlaw,2862
 atlantic/atl_pipeline.py,sha256=Fn77_CUA09jZNXkgUJc3yqGWBu7KNBXmcC6eLJU-7qc,8541
 atlantic/atl_processing.py,sha256=R97TbF5_4p8XyilGFhWzViIHbwRd4XscXzbC8yBKRvs,20571
-atlantic-1.0.55.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
-atlantic-1.0.55.dist-info/METADATA,sha256=mCnocJuRSSHO4nFyP6jmtKtw1ocz74z0UqyQ35i99jo,12316
-atlantic-1.0.55.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-atlantic-1.0.55.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
-atlantic-1.0.55.dist-info/RECORD,,
+atlantic-1.0.60.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
+atlantic-1.0.60.dist-info/METADATA,sha256=WpkqyX2JyFGUPzDhTyBK-50-T0BGuacr3M8oDIks-9E,12317
+atlantic-1.0.60.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+atlantic-1.0.60.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
+atlantic-1.0.60.dist-info/RECORD,,
```


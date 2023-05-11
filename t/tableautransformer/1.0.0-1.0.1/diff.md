# Comparing `tmp/tableautransformer-1.0.0.tar.gz` & `tmp/tableautransformer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableautransformer-1.0.0.tar", last modified: Wed May 10 14:27:38 2023, max compression
+gzip compressed data, was "tableautransformer-1.0.1.tar", last modified: Thu May 11 13:30:43 2023, max compression
```

## Comparing `tableautransformer-1.0.0.tar` & `tableautransformer-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/
--rw-rw-rw-   0        0        0     1091 2022-12-21 16:48:30.000000 tableautransformer-1.0.0/LICENCE
--rw-rw-rw-   0        0        0     8204 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7854 2023-05-10 14:18:05.000000 tableautransformer-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-05-10 14:18:21.000000 tableautransformer-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:27:38.826856 tableautransformer-1.0.0/tableautransformer/
--rw-rw-rw-   0        0        0        0 2022-12-22 15:23:56.000000 tableautransformer-1.0.0/tableautransformer/__init__.py
--rw-rw-rw-   0        0        0      189 2022-12-22 15:56:40.000000 tableautransformer-1.0.0/tableautransformer/backbone.py
--rw-rw-rw-   0        0        0     4541 2023-05-10 13:52:34.000000 tableautransformer-1.0.0/tableautransformer/datawrangling.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/tableautransformer.egg-info/
--rw-rw-rw-   0        0        0     8204 2023-05-10 14:27:37.000000 tableautransformer-1.0.0/tableautransformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-10 14:27:38.000000 tableautransformer-1.0.0/tableautransformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:27:37.000000 tableautransformer-1.0.0/tableautransformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-10 14:27:38.000000 tableautransformer-1.0.0/tableautransformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2022-12-21 16:48:30.000000 tableautransformer-1.0.1/LICENCE
+-rw-rw-rw-   0        0        0     8485 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8135 2023-05-11 13:29:50.000000 tableautransformer-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-05-11 13:30:23.000000 tableautransformer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:30:43.362043 tableautransformer-1.0.1/tableautransformer/
+-rw-rw-rw-   0        0        0        0 2022-12-22 15:23:56.000000 tableautransformer-1.0.1/tableautransformer/__init__.py
+-rw-rw-rw-   0        0        0      189 2022-12-22 15:56:40.000000 tableautransformer-1.0.1/tableautransformer/backbone.py
+-rw-rw-rw-   0        0        0     4590 2023-05-11 13:27:31.000000 tableautransformer-1.0.1/tableautransformer/datawrangling.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/tableautransformer.egg-info/
+-rw-rw-rw-   0        0        0     8485 2023-05-11 13:30:42.000000 tableautransformer-1.0.1/tableautransformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-11 13:30:43.000000 tableautransformer-1.0.1/tableautransformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 13:30:42.000000 tableautransformer-1.0.1/tableautransformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 13:30:42.000000 tableautransformer-1.0.1/tableautransformer.egg-info/top_level.txt
```

### Comparing `tableautransformer-1.0.0/LICENCE` & `tableautransformer-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tableautransformer-1.0.0/PKG-INFO` & `tableautransformer-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableautransformer
-Version: 1.0.0
+Version: 1.0.1
 Summary: ETL tooling for tableau seed data
 Home-page: https://pypi.org/project/tableautransformer
 Author: Josh Teixeira
 Author-email: jteixeira@cppib.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -182,15 +182,32 @@
 
 ```
 force_string(df)
 ```
 
 ##### Description
 
-Force all scalar data to be strings in a given dataframe.
+Force all scalar data to be strings in a given dataframe, mitigates float percision error for database upload.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+***
+
+### Force_Object()
+
+```
+force_object(df)
+```
+
+##### Description
+
+Force all series to be of type object, mitigates merge fail.
 
 ##### Inputs
 
 > **df**: *dataframe*
 >> The DataFrame you want to loop through
 
 ***
```

### Comparing `tableautransformer-1.0.0/README.md` & `tableautransformer-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,32 @@
 
 ```
 force_string(df)
 ```
 
 ##### Description
 
-Force all scalar data to be strings in a given dataframe.
+Force all scalar data to be strings in a given dataframe, mitigates float percision error for database upload.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+***
+
+### Force_Object()
+
+```
+force_object(df)
+```
+
+##### Description
+
+Force all series to be of type object, mitigates merge fail.
 
 ##### Inputs
 
 > **df**: *dataframe*
 >> The DataFrame you want to loop through
 
 ***
```

### Comparing `tableautransformer-1.0.0/tableautransformer/datawrangling.py` & `tableautransformer-1.0.1/tableautransformer/datawrangling.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,28 +57,30 @@
     return df_basic_table
 
 def find_dtypes(df):
     for col in df.columns:
         datatypes = set(df[col].dtype for i in df[col])
         print(f'{col}: {list(datatypes)}')
 
-# this is new, add md
 def find_dups(df, name):
     duplicated = df.duplicated(subset=df.columns)
     print('-----------------------------------------------')
     print(f"Your duplicated inside {name} are:")
     print(df[duplicated])
     print('-----------------------------------------------')
 
-# this is new, add md
 def force_string(df):
     for col in df.columns:
         df[col] = df[col].astype(str)
         df[col] = df[col].replace(0,'')
 
+def force_object(df):
+    for col in df.columns:
+        df[col] = df[col].astype(object)
+
 def is_in(df, target_col, isin_list):
     df = df[df[target_col].isin(isin_list)]
     return df
 
 def cast(df, target_col, value):
     df[target_col] = value
     return df
```

### Comparing `tableautransformer-1.0.0/tableautransformer.egg-info/PKG-INFO` & `tableautransformer-1.0.1/tableautransformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableautransformer
-Version: 1.0.0
+Version: 1.0.1
 Summary: ETL tooling for tableau seed data
 Home-page: https://pypi.org/project/tableautransformer
 Author: Josh Teixeira
 Author-email: jteixeira@cppib.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -182,15 +182,32 @@
 
 ```
 force_string(df)
 ```
 
 ##### Description
 
-Force all scalar data to be strings in a given dataframe.
+Force all scalar data to be strings in a given dataframe, mitigates float percision error for database upload.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+***
+
+### Force_Object()
+
+```
+force_object(df)
+```
+
+##### Description
+
+Force all series to be of type object, mitigates merge fail.
 
 ##### Inputs
 
 > **df**: *dataframe*
 >> The DataFrame you want to loop through
 
 ***
```


# Comparing `tmp/KaggleToDatabricks-0.5.tar.gz` & `tmp/KaggleToDatabricks-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\KaggleToDatabricks-0.5.tar", last modified: Thu May 11 18:40:48 2023, max compression
+gzip compressed data, was "dist\KaggleToDatabricks-0.6.tar", last modified: Thu May 11 18:53:32 2023, max compression
```

## Comparing `KaggleToDatabricks-0.5.tar` & `KaggleToDatabricks-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:40:48.622027 KaggleToDatabricks-0.5/
-drwxrwxrwx   0        0        0        0 2023-05-11 18:40:48.616026 KaggleToDatabricks-0.5/KaggleToDatabricks/
--rw-rw-rw-   0        0        0      302 2023-05-11 17:53:32.000000 KaggleToDatabricks-0.5/KaggleToDatabricks/Authenticate.py
--rw-rw-rw-   0        0        0      748 2023-05-11 18:39:41.000000 KaggleToDatabricks-0.5/KaggleToDatabricks/TranfsformDataset.py
--rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.5/KaggleToDatabricks/__innit__.py
--rw-rw-rw-   0        0        0        0 2023-05-11 17:48:04.000000 KaggleToDatabricks-0.5/KaggleToDatabricks/test_Authenticate.py
--rw-rw-rw-   0        0        0        0 2023-05-11 18:39:26.000000 KaggleToDatabricks-0.5/KaggleToDatabricks/test_TransformDataset.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:40:48.621028 KaggleToDatabricks-0.5/KaggleToDatabricks.egg-info/
--rw-rw-rw-   0        0        0      898 2023-05-11 18:40:48.000000 KaggleToDatabricks-0.5/KaggleToDatabricks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-11 18:40:48.000000 KaggleToDatabricks-0.5/KaggleToDatabricks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:40:48.000000 KaggleToDatabricks-0.5/KaggleToDatabricks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-11 18:40:48.000000 KaggleToDatabricks-0.5/KaggleToDatabricks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 18:40:48.000000 KaggleToDatabricks-0.5/KaggleToDatabricks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      898 2023-05-11 18:40:48.622027 KaggleToDatabricks-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-05-11 17:15:30.000000 KaggleToDatabricks-0.5/README.md
--rw-rw-rw-   0        0        0       86 2023-05-11 18:40:48.623029 KaggleToDatabricks-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1842 2023-05-11 18:40:26.000000 KaggleToDatabricks-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:53:32.497855 KaggleToDatabricks-0.6/
+drwxrwxrwx   0        0        0        0 2023-05-11 18:53:32.491210 KaggleToDatabricks-0.6/KaggleToDatabricks/
+-rw-rw-rw-   0        0        0      302 2023-05-11 17:53:32.000000 KaggleToDatabricks-0.6/KaggleToDatabricks/Authenticate.py
+-rw-rw-rw-   0        0        0      763 2023-05-11 18:53:03.000000 KaggleToDatabricks-0.6/KaggleToDatabricks/TranfsformDataset.py
+-rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.6/KaggleToDatabricks/__innit__.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 17:48:04.000000 KaggleToDatabricks-0.6/KaggleToDatabricks/test_Authenticate.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 18:39:26.000000 KaggleToDatabricks-0.6/KaggleToDatabricks/test_TransformDataset.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:53:32.496855 KaggleToDatabricks-0.6/KaggleToDatabricks.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-05-11 18:53:32.000000 KaggleToDatabricks-0.6/KaggleToDatabricks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-11 18:53:32.000000 KaggleToDatabricks-0.6/KaggleToDatabricks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:53:32.000000 KaggleToDatabricks-0.6/KaggleToDatabricks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-11 18:53:32.000000 KaggleToDatabricks-0.6/KaggleToDatabricks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 18:53:32.000000 KaggleToDatabricks-0.6/KaggleToDatabricks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      898 2023-05-11 18:53:32.497855 KaggleToDatabricks-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2023-05-11 17:15:30.000000 KaggleToDatabricks-0.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-11 18:53:32.497855 KaggleToDatabricks-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2023-05-11 18:53:13.000000 KaggleToDatabricks-0.6/setup.py
```

### Comparing `KaggleToDatabricks-0.5/KaggleToDatabricks/TranfsformDataset.py` & `KaggleToDatabricks-0.6/KaggleToDatabricks/TranfsformDataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 class TransformDataset:
     import pandas as pd
     from pyspark.sql import SparkSession
 
-    spark = SparkSession.builder.appName("pandas to spark").getOrCreate()
+    spark = self.SparkSession.builder.appName("pandas to spark").getOrCreate()
 
     def df_from_dataset(input_path,dataset_file):
-        df = pd.read_csv(f'{input_path}/{dataset_file}')
+        df = self.pd.read_csv(f'{input_path}/{dataset_file}')
         return df
 
     def filter_dataset(df,dataset_file,col_list_to_drop):
         df2 = df.drop(columns=col_list_to_drop)
         return df2
 
     def get_max_from_dataset(df,col_list_to_groupby,col_get_max):
         df2 = df.groupby(col_list_to_groupby)[col_get_max].max().reset_index()
         return(df2)
     
     def write_df_to_parquet(df,output_path):
-        sdf = spark.createDataFrame(df)
+        sdf = self.spark.createDataFrame(df)
         sdf.write.mode("overwrite").parquet(output_path)
```

### Comparing `KaggleToDatabricks-0.5/KaggleToDatabricks.egg-info/PKG-INFO` & `KaggleToDatabricks-0.6/KaggleToDatabricks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.5
+Version: 0.6
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.5/LICENSE.txt` & `KaggleToDatabricks-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KaggleToDatabricks-0.5/PKG-INFO` & `KaggleToDatabricks-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.5
+Version: 0.6
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.5/setup.py` & `KaggleToDatabricks-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'KaggleToDatabricks',         # How you named your package folder (MyLib)
   packages = ['KaggleToDatabricks'],   # Chose the same as "name"
-  version = '0.5',      # Start with a small number and increase it with every change you make
+  version = '0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Package created for recruitment task',   # Give a short description about your library
   author = 'Artur Woźniak',                   # Type in your name
   author_email = 'arturwn39@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/Teneb/kaggle_to_databricks',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz',    # I explain this later on
   keywords = ['pls', 'hire', 'me'],   # Keywords that define your package best
```


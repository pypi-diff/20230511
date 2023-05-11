# Comparing `tmp/KaggleToDatabricks-0.7.tar.gz` & `tmp/KaggleToDatabricks-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\KaggleToDatabricks-0.7.tar", last modified: Thu May 11 18:55:54 2023, max compression
+gzip compressed data, was "dist\KaggleToDatabricks-0.8.tar", last modified: Thu May 11 18:57:50 2023, max compression
```

## Comparing `KaggleToDatabricks-0.7.tar` & `KaggleToDatabricks-0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:55:54.697101 KaggleToDatabricks-0.7/
-drwxrwxrwx   0        0        0        0 2023-05-11 18:55:54.690101 KaggleToDatabricks-0.7/KaggleToDatabricks/
--rw-rw-rw-   0        0        0      302 2023-05-11 17:53:32.000000 KaggleToDatabricks-0.7/KaggleToDatabricks/Authenticate.py
--rw-rw-rw-   0        0        0      783 2023-05-11 18:55:39.000000 KaggleToDatabricks-0.7/KaggleToDatabricks/TranfsformDataset.py
--rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.7/KaggleToDatabricks/__innit__.py
--rw-rw-rw-   0        0        0        0 2023-05-11 17:48:04.000000 KaggleToDatabricks-0.7/KaggleToDatabricks/test_Authenticate.py
--rw-rw-rw-   0        0        0        0 2023-05-11 18:39:26.000000 KaggleToDatabricks-0.7/KaggleToDatabricks/test_TransformDataset.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:55:54.695100 KaggleToDatabricks-0.7/KaggleToDatabricks.egg-info/
--rw-rw-rw-   0        0        0      898 2023-05-11 18:55:54.000000 KaggleToDatabricks-0.7/KaggleToDatabricks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-11 18:55:54.000000 KaggleToDatabricks-0.7/KaggleToDatabricks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:55:54.000000 KaggleToDatabricks-0.7/KaggleToDatabricks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-11 18:55:54.000000 KaggleToDatabricks-0.7/KaggleToDatabricks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 18:55:54.000000 KaggleToDatabricks-0.7/KaggleToDatabricks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      898 2023-05-11 18:55:54.697101 KaggleToDatabricks-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-05-11 17:15:30.000000 KaggleToDatabricks-0.7/README.md
--rw-rw-rw-   0        0        0       86 2023-05-11 18:55:54.697101 KaggleToDatabricks-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1842 2023-05-11 18:55:43.000000 KaggleToDatabricks-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:57:50.579011 KaggleToDatabricks-0.8/
+drwxrwxrwx   0        0        0        0 2023-05-11 18:57:50.573009 KaggleToDatabricks-0.8/KaggleToDatabricks/
+-rw-rw-rw-   0        0        0      302 2023-05-11 17:53:32.000000 KaggleToDatabricks-0.8/KaggleToDatabricks/Authenticate.py
+-rw-rw-rw-   0        0        0      778 2023-05-11 18:57:24.000000 KaggleToDatabricks-0.8/KaggleToDatabricks/TranfsformDataset.py
+-rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.8/KaggleToDatabricks/__innit__.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 17:48:04.000000 KaggleToDatabricks-0.8/KaggleToDatabricks/test_Authenticate.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 18:39:26.000000 KaggleToDatabricks-0.8/KaggleToDatabricks/test_TransformDataset.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:57:50.578011 KaggleToDatabricks-0.8/KaggleToDatabricks.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-05-11 18:57:50.000000 KaggleToDatabricks-0.8/KaggleToDatabricks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-11 18:57:50.000000 KaggleToDatabricks-0.8/KaggleToDatabricks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:57:50.000000 KaggleToDatabricks-0.8/KaggleToDatabricks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-11 18:57:50.000000 KaggleToDatabricks-0.8/KaggleToDatabricks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 18:57:50.000000 KaggleToDatabricks-0.8/KaggleToDatabricks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      898 2023-05-11 18:57:50.579011 KaggleToDatabricks-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2023-05-11 17:15:30.000000 KaggleToDatabricks-0.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-11 18:57:50.580010 KaggleToDatabricks-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2023-05-11 18:57:42.000000 KaggleToDatabricks-0.8/setup.py
```

### Comparing `KaggleToDatabricks-0.7/KaggleToDatabricks/TranfsformDataset.py` & `KaggleToDatabricks-0.8/KaggleToDatabricks/TranfsformDataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class TransformDataset:
     import pandas as pd
     from pyspark.sql import SparkSession
 
-    spark = self.SparkSession.builder.appName("pandas to spark").getOrCreate()
+    spark = SparkSession.builder.appName("pandas to spark").getOrCreate()
 
     def df_from_dataset(self,input_path,dataset_file):
         df = self.pd.read_csv(f'{input_path}/{dataset_file}')
         return df
 
     def filter_dataset(self,df,dataset_file,col_list_to_drop):
         df2 = df.drop(columns=col_list_to_drop)
```

### Comparing `KaggleToDatabricks-0.7/KaggleToDatabricks.egg-info/PKG-INFO` & `KaggleToDatabricks-0.8/KaggleToDatabricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.7
+Version: 0.8
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.7/LICENSE.txt` & `KaggleToDatabricks-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KaggleToDatabricks-0.7/PKG-INFO` & `KaggleToDatabricks-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.7
+Version: 0.8
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.7/setup.py` & `KaggleToDatabricks-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'KaggleToDatabricks',         # How you named your package folder (MyLib)
   packages = ['KaggleToDatabricks'],   # Chose the same as "name"
-  version = '0.7',      # Start with a small number and increase it with every change you make
+  version = '0.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Package created for recruitment task',   # Give a short description about your library
   author = 'Artur Woźniak',                   # Type in your name
   author_email = 'arturwn39@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/Teneb/kaggle_to_databricks',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz',    # I explain this later on
   keywords = ['pls', 'hire', 'me'],   # Keywords that define your package best
```


# Comparing `tmp/discotoolkit-1.0.2.tar.gz` & `tmp/discotoolkit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.2.tar", last modified: Thu May 11 01:29:03 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.3.tar", last modified: Thu May 11 01:52:20 2023, max compression
```

## Comparing `discotoolkit-1.0.2.tar` & `discotoolkit-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:28:52.264664 discotoolkit-1.0.2/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.2/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-11 01:28:52.264664 discotoolkit-1.0.2/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     1162 2023-05-11 01:27:16.000000 discotoolkit-1.0.2/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:28:52.224665 discotoolkit-1.0.2/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-10 16:37:16.000000 discotoolkit-1.0.2/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.2/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-03 17:04:16.000000 discotoolkit-1.0.2/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     6958 2023-05-05 07:03:35.000000 discotoolkit-1.0.2/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-03 17:04:16.000000 discotoolkit-1.0.2/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-10 07:17:57.000000 discotoolkit-1.0.2/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      107 2023-05-10 06:00:24.000000 discotoolkit-1.0.2/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:28:52.256664 discotoolkit-1.0.2/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)      104 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-11 01:28:52.268664 discotoolkit-1.0.2/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-11 01:28:23.000000 discotoolkit-1.0.2/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:52:09.022427 discotoolkit-1.0.3/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.3/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-11 01:52:09.022427 discotoolkit-1.0.3/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1433 2023-05-11 01:51:49.000000 discotoolkit-1.0.3/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:52:08.990427 discotoolkit-1.0.3/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-11 01:50:32.000000 discotoolkit-1.0.3/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.3/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-03 17:04:16.000000 discotoolkit-1.0.3/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     6958 2023-05-11 01:51:05.000000 discotoolkit-1.0.3/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-03 17:04:16.000000 discotoolkit-1.0.3/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.3/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      107 2023-05-10 06:00:24.000000 discotoolkit-1.0.3/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:52:09.014427 discotoolkit-1.0.3/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-11 01:52:08.000000 discotoolkit-1.0.3/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-11 01:52:08.000000 discotoolkit-1.0.3/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-11 01:52:08.000000 discotoolkit-1.0.3/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      128 2023-05-11 01:52:08.000000 discotoolkit-1.0.3/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-11 01:52:08.000000 discotoolkit-1.0.3/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-11 01:52:09.022427 discotoolkit-1.0.3/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-11 01:51:35.000000 discotoolkit-1.0.3/setup.py
```

### Comparing `discotoolkit-1.0.2/PKG-INFO` & `discotoolkit-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.2
+Version: 1.0.3
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
 Description: 
             DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
```

### Comparing `discotoolkit-1.0.2/README.md` & `discotoolkit-1.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * @Descripttion: 
  * @version: 
  * @Author: Mengwei Li
  * @Date: 2023-04-16 21:20:42
  * @LastEditors: Mengwei Li
  * @LastEditTime: 2023-04-16 21:22:03
 -->
-# DISCOtoolkit 1.0.1
+# DISCOtoolkit 1.0.3
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). It provides the following functions:
 
 - Filter and download DISCO data based on sample metadata and cell type information
 - CELLiD: cell type annotation
 - scEnrichment: geneset enrichment using DISCO DEGs
 - CellMapper: project data into DISCO atlas
@@ -19,17 +19,28 @@
 - Numpy 1.21.6
 - Pandas 1.4.2
 - Scanpy 1.9.3
 - Scipy 1.8.0
 - joblib 1.1.0
 - pandarallel 1.6.5
 
+Installation guide:
+
+we recommend to install miniconda first and install discotoolkit in virtual env
+
+```
+conda create --name disco python=3.8
+conda install pip
+conda install ipykernel
+python -m ipykernel install --user --name disco --display-name "disco"
+```
+
 Installation using pip:
 ``` 
-pip install discotoolkit
+python -m pip install discotoolkit
 ```
 
 ## Basic Usage
 Example in Jupyter notebook
 
 ### [Filter and download DISCO data](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/download_data.ipynb)
```

### Comparing `discotoolkit-1.0.2/discotoolkit/CELLiD.py` & `discotoolkit-1.0.3/discotoolkit/CELLiD.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.2/discotoolkit/DiscoClass.py` & `discotoolkit-1.0.3/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.2/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.0.3/discotoolkit/DownloadDiscoData.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.2/discotoolkit/GetMetadata.py` & `discotoolkit-1.0.3/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.2/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.3/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.2/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.3/discotoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.2
+Version: 1.0.3
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
 Description: 
             DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
```

### Comparing `discotoolkit-1.0.2/setup.py` & `discotoolkit-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='discotoolkit',
-    version='1.0.2',
+    version='1.0.3',
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
     python_requires = '>=3.8.10',
```


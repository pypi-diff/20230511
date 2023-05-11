# Comparing `tmp/discotoolkit-1.0.1.tar.gz` & `tmp/discotoolkit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.1.tar", last modified: Wed May 10 16:28:50 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.2.tar", last modified: Thu May 11 01:29:03 2023, max compression
```

## Comparing `discotoolkit-1.0.1.tar` & `discotoolkit-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-10 16:28:39.538223 discotoolkit-1.0.1/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.1/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-10 16:28:39.534222 discotoolkit-1.0.1/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     1163 2023-05-10 16:28:04.000000 discotoolkit-1.0.1/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-10 16:28:39.494223 discotoolkit-1.0.1/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-10 16:21:34.000000 discotoolkit-1.0.1/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.1/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-03 17:04:16.000000 discotoolkit-1.0.1/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     6958 2023-05-05 07:03:35.000000 discotoolkit-1.0.1/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-03 17:04:16.000000 discotoolkit-1.0.1/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-10 07:17:57.000000 discotoolkit-1.0.1/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      107 2023-05-10 06:00:24.000000 discotoolkit-1.0.1/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-10 16:28:39.526223 discotoolkit-1.0.1/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-10 16:28:39.000000 discotoolkit-1.0.1/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       89 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-10 16:28:39.538223 discotoolkit-1.0.1/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-10 16:28:17.000000 discotoolkit-1.0.1/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:28:52.264664 discotoolkit-1.0.2/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.2/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-11 01:28:52.264664 discotoolkit-1.0.2/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1162 2023-05-11 01:27:16.000000 discotoolkit-1.0.2/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:28:52.224665 discotoolkit-1.0.2/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-10 16:37:16.000000 discotoolkit-1.0.2/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.2/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-03 17:04:16.000000 discotoolkit-1.0.2/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     6958 2023-05-05 07:03:35.000000 discotoolkit-1.0.2/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-03 17:04:16.000000 discotoolkit-1.0.2/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-10 07:17:57.000000 discotoolkit-1.0.2/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      107 2023-05-10 06:00:24.000000 discotoolkit-1.0.2/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:28:52.256664 discotoolkit-1.0.2/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      104 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-11 01:28:52.000000 discotoolkit-1.0.2/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-11 01:28:52.268664 discotoolkit-1.0.2/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-11 01:28:23.000000 discotoolkit-1.0.2/setup.py
```

### Comparing `discotoolkit-1.0.1/PKG-INFO` & `discotoolkit-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.1
+Version: 1.0.2
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
 Description: 
             DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
```

### Comparing `discotoolkit-1.0.1/README.md` & `discotoolkit-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 - Scanpy 1.9.3
 - Scipy 1.8.0
 - joblib 1.1.0
 - pandarallel 1.6.5
 
 Installation using pip:
 ``` 
-pip3 install discotoolkit
+pip install discotoolkit
 ```
 
 ## Basic Usage
 Example in Jupyter notebook
 
 ### [Filter and download DISCO data](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/download_data.ipynb)
```

### Comparing `discotoolkit-1.0.1/discotoolkit/CELLiD.py` & `discotoolkit-1.0.2/discotoolkit/CELLiD.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.1/discotoolkit/DiscoClass.py` & `discotoolkit-1.0.2/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.1/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.0.2/discotoolkit/DownloadDiscoData.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.1/discotoolkit/GetMetadata.py` & `discotoolkit-1.0.2/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.1/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.2/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.1/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.2/discotoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.1
+Version: 1.0.2
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
 Description: 
             DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
```

### Comparing `discotoolkit-1.0.1/setup.py` & `discotoolkit-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='discotoolkit',
-    version='1.0.1',
+    version='1.0.2',
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
     python_requires = '>=3.8.10',
```


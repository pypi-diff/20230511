# Comparing `tmp/ykenan_file-0.1.7.tar.gz` & `tmp/ykenan_file-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.7.tar", last modified: Wed May 10 07:25:39 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.8.tar", last modified: Wed May 10 10:51:58 2023, max compression
```

## Comparing `ykenan_file-0.1.7.tar` & `ykenan_file-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.428038 ykenan_file-0.1.7/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-05-10 07:25:39.427040 ykenan_file-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.7/README.md
--rw-rw-rw-   0        0        0      676 2023-05-10 07:24:54.000000 ykenan_file-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 07:25:39.428038 ykenan_file-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.411038 ykenan_file-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.415037 ykenan_file-0.1.7/src/ykenan_file/
--rw-rw-rw-   0        0        0    23488 2023-05-10 07:24:54.000000 ykenan_file-0.1.7/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.7/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.426037 ykenan_file-0.1.7/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      829 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.414476 ykenan_file-0.1.8/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      827 2023-05-10 10:51:58.414476 ykenan_file-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-10 10:51:14.000000 ykenan_file-0.1.8/README.md
+-rw-rw-rw-   0        0        0      696 2023-05-10 10:46:17.000000 ykenan_file-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       50 2023-05-10 10:43:14.000000 ykenan_file-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:51:58.414476 ykenan_file-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.399476 ykenan_file-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.403476 ykenan_file-0.1.8/src/ykenan_file/
+-rw-rw-rw-   0        0        0    24001 2023-05-10 10:43:14.000000 ykenan_file-0.1.8/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.8/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.412476 ykenan_file-0.1.8/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      827 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.7/LICENSE` & `ykenan_file-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.7/PKG-INFO` & `ykenan_file-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.1.7
+Version: 0.1.8
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,8 +30,7 @@
 
 > import
 
 ```shell
 import ykenan_file as yf
 ```
 
-
```

### Comparing `ykenan_file-0.1.7/pyproject.toml` & `ykenan_file-0.1.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
-requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
+requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3", "requests>=2.30.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.1.7/src/ykenan_file/__init__.py` & `ykenan_file-0.1.8/src/ykenan_file/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 
 import os
 
 import pandas as pd
+import requests
 from ykenan_log import Logger
 from pandas import DataFrame
 
 '''
  * @Author       : YKenan
  * @Description  : file handler
 '''
@@ -597,7 +598,17 @@
     def entry_dirs_dict(self, path: str) -> dict:
         """
         Obtain all files in the specified path
         :param path: path
         :return: dirs
         """
         return self.entry_contents_dict(path, 2)
+
+    def download_file(self, url: str, filename: str, chunk_size: int = 1024):
+        self.log.info(f"下载 {url} 文件")
+        response_data_file = requests.get(url, stream=True)
+        self.log.info(f"创建 {filename} 文件")
+        with open(filename, 'wb') as f:
+            for chunk in response_data_file.iter_content(chunk_size=chunk_size):
+                if chunk:
+                    f.write(chunk)
+        self.log.info(f"下载 {url} ===> {filename} 文件完成")
```

### Comparing `ykenan_file-0.1.7/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.8/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.1.7
+Version: 0.1.8
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,8 +30,7 @@
 
 > import
 
 ```shell
 import ykenan_file as yf
 ```
 
-
```


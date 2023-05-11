# Comparing `tmp/rape_identification-0.1.8.tar.gz` & `tmp/rape_identification-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rape_identification-0.1.8.tar", last modified: Tue May  9 11:35:49 2023, max compression
+gzip compressed data, was "rape_identification-0.1.9.tar", last modified: Tue May  9 11:42:54 2023, max compression
```

## Comparing `rape_identification-0.1.8.tar` & `rape_identification-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:35:49.804752 rape_identification-0.1.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/rape_identification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/rape_identification/config/
--rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:34:55.000000 rape_identification-0.1.8/rape_identification/config/a.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/config/default.py
--rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/config/default_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/rape_identification/dataset/
--rw-rw-r--   0 root         (0) root         (0)     1989 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/dataset/SlidingWindowDataset.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:44.000000 rape_identification-0.1.8/rape_identification/dataset/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/inference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/rape_identification/model/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/rape_identification/model/SwinUNet/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:40.000000 rape_identification-0.1.8/rape_identification/model/SwinUNet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31715 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py
--rw-rw-r--   0 root         (0) root         (0)     4177 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/model/SwinUNet/vision_transformer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:35.000000 rape_identification-0.1.8/rape_identification/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/rape_identification/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 10:54:56.000000 rape_identification-0.1.8/rape_identification/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2764 2023-05-09 09:48:54.000000 rape_identification-0.1.8/rape_identification/utils/convert2uint8.py
--rw-rw-r--   0 root         (0) root         (0)      858 2023-05-09 11:10:50.000000 rape_identification-0.1.8/rape_identification/utils/segment.py
--rw-rw-r--   0 root         (0) root         (0)     4086 2023-05-09 11:11:11.000000 rape_identification-0.1.8/rape_identification/utils/test.py
--rw-rw-r--   0 root         (0) root         (0)    14057 2023-05-09 11:33:02.000000 rape_identification-0.1.8/rape_identification/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:35:49.804752 rape_identification-0.1.8/rape_identification.egg-info/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:35:49.000000 rape_identification-0.1.8/rape_identification.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      954 2023-05-09 11:35:49.000000 rape_identification-0.1.8/rape_identification.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:35:49.000000 rape_identification-0.1.8/rape_identification.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 11:35:49.000000 rape_identification-0.1.8/rape_identification.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 11:35:49.000000 rape_identification-0.1.8/rape_identification.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 11:35:49.804752 rape_identification-0.1.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 11:35:00.000000 rape_identification-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/
+-rw-rw-r--   0 root         (0) root         (0)       43 2023-05-09 11:41:30.000000 rape_identification-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:42:54.137705 rape_identification-0.1.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/rape_identification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/rape_identification/config/
+-rw-rw-r--   0 root         (0) root         (0)     1358 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/config/GID.yaml
+-rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:34:55.000000 rape_identification-0.1.9/rape_identification/config/a.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/config/default.py
+-rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/config/default_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/rape_identification/dataset/
+-rw-rw-r--   0 root         (0) root         (0)     1989 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/dataset/SlidingWindowDataset.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:44.000000 rape_identification-0.1.9/rape_identification/dataset/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/inference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/rape_identification/model/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/rape_identification/model/SwinUNet/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:40.000000 rape_identification-0.1.9/rape_identification/model/SwinUNet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31715 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py
+-rw-rw-r--   0 root         (0) root         (0)     4177 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/model/SwinUNet/vision_transformer.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:35.000000 rape_identification-0.1.9/rape_identification/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/rape_identification/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 10:54:56.000000 rape_identification-0.1.9/rape_identification/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2764 2023-05-09 09:48:54.000000 rape_identification-0.1.9/rape_identification/utils/convert2uint8.py
+-rw-rw-r--   0 root         (0) root         (0)      858 2023-05-09 11:10:50.000000 rape_identification-0.1.9/rape_identification/utils/segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4086 2023-05-09 11:11:11.000000 rape_identification-0.1.9/rape_identification/utils/test.py
+-rw-rw-r--   0 root         (0) root         (0)    14057 2023-05-09 11:33:02.000000 rape_identification-0.1.9/rape_identification/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:42:54.137705 rape_identification-0.1.9/rape_identification.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:42:54.000000 rape_identification-0.1.9/rape_identification.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-09 11:42:54.000000 rape_identification-0.1.9/rape_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:42:54.000000 rape_identification-0.1.9/rape_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 11:42:54.000000 rape_identification-0.1.9/rape_identification.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 11:42:54.000000 rape_identification-0.1.9/rape_identification.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 11:42:54.137705 rape_identification-0.1.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 11:41:36.000000 rape_identification-0.1.9/setup.py
```

### Comparing `rape_identification-0.1.8/PKG-INFO` & `rape_identification-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rape_identification
-Version: 0.1.8
+Version: 0.1.9
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.8/rape_identification/config/default.py` & `rape_identification-0.1.9/rape_identification/config/default.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/config/default_test.py` & `rape_identification-0.1.9/rape_identification/config/default_test.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/dataset/SlidingWindowDataset.py` & `rape_identification-0.1.9/rape_identification/dataset/SlidingWindowDataset.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/inference.py` & `rape_identification-0.1.9/rape_identification/inference.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py` & `rape_identification-0.1.9/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/model/SwinUNet/vision_transformer.py` & `rape_identification-0.1.9/rape_identification/model/SwinUNet/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/utils/convert2uint8.py` & `rape_identification-0.1.9/rape_identification/utils/convert2uint8.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/utils/segment.py` & `rape_identification-0.1.9/rape_identification/utils/segment.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/utils/test.py` & `rape_identification-0.1.9/rape_identification/utils/test.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification/utils/utils.py` & `rape_identification-0.1.9/rape_identification/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.8/rape_identification.egg-info/PKG-INFO` & `rape_identification-0.1.9/rape_identification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rape-identification
-Version: 0.1.8
+Version: 0.1.9
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.8/rape_identification.egg-info/SOURCES.txt` & `rape_identification-0.1.9/rape_identification.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+MANIFEST.in
 README.md
 setup.py
 rape_identification/__init__.py
 rape_identification/inference.py
 rape_identification.egg-info/PKG-INFO
 rape_identification.egg-info/SOURCES.txt
 rape_identification.egg-info/dependency_links.txt
 rape_identification.egg-info/requires.txt
 rape_identification.egg-info/top_level.txt
+rape_identification/config/GID.yaml
 rape_identification/config/__init__.py
 rape_identification/config/a.py
 rape_identification/config/default.py
 rape_identification/config/default_test.py
 rape_identification/dataset/SlidingWindowDataset.py
 rape_identification/dataset/__init__.py
 rape_identification/model/__init__.py
```

### Comparing `rape_identification-0.1.8/setup.py` & `rape_identification-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rape_identification',  # 与项目文件夹结构中的包名相同
-    version='0.1.8',
+    version='0.1.9',
     description='Segmentation any rape',
     author='PingYang',
     author_email='PingYang97@163.com',
     # url='https://github.com/yourusername/your_project',
     packages=find_packages(),
     install_requires=[
         # Add your project's dependencies here, e.g., 'numpy', 'pandas', etc.
```


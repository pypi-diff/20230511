# Comparing `tmp/vision_xformer-0.1.6.tar.gz` & `tmp/vision_xformer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_xformer-0.1.6.tar", last modified: Wed May 10 21:09:07 2023, max compression
+gzip compressed data, was "vision_xformer-0.1.7.tar", last modified: Wed May 10 21:15:50 2023, max compression
```

## Comparing `vision_xformer-0.1.6.tar` & `vision_xformer-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:09:07.726871 vision_xformer-0.1.6/
--rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3823 2023-05-10 21:09:07.724870 vision_xformer-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 21:09:07.727872 vision_xformer-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-05-10 21:08:53.000000 vision_xformer-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:09:07.643330 vision_xformer-0.1.6/vision_xformer/
--rw-rw-rw-   0        0        0      233 2023-05-10 21:08:21.000000 vision_xformer-0.1.6/vision_xformer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-06 19:02:18.000000 vision_xformer-0.1.6/vision_xformer/fnet.py
--rw-rw-rw-   0        0        0     1913 2023-05-07 00:12:55.000000 vision_xformer-0.1.6/vision_xformer/fnet2d.py
--rw-rw-rw-   0        0        0     6497 2023-05-06 18:56:56.000000 vision_xformer-0.1.6/vision_xformer/vision_linformer.py
--rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.6/vision_xformer/vision_nystromformer.py
--rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.6/vision_xformer/vision_performer.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:09:07.722869 vision_xformer-0.1.6/vision_xformer.egg-info/
--rw-rw-rw-   0        0        0     3823 2023-05-10 21:09:07.000000 vision_xformer-0.1.6/vision_xformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-05-10 21:09:07.000000 vision_xformer-0.1.6/vision_xformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:09:07.000000 vision_xformer-0.1.6/vision_xformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-10 21:09:07.000000 vision_xformer-0.1.6/vision_xformer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 21:09:07.000000 vision_xformer-0.1.6/vision_xformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 21:15:50.586242 vision_xformer-0.1.7/
+-rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3823 2023-05-10 21:15:50.585252 vision_xformer-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 21:15:50.587243 vision_xformer-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-05-10 21:15:15.000000 vision_xformer-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:15:50.513377 vision_xformer-0.1.7/vision_xformer/
+-rw-rw-rw-   0        0        0      235 2023-05-10 21:15:07.000000 vision_xformer-0.1.7/vision_xformer/__init__.py
+-rw-rw-rw-   0        0        0     3471 2023-05-10 21:14:04.000000 vision_xformer-0.1.7/vision_xformer/fnet.py
+-rw-rw-rw-   0        0        0     1913 2023-05-07 00:12:55.000000 vision_xformer-0.1.7/vision_xformer/fnet2d.py
+-rw-rw-rw-   0        0        0     6497 2023-05-06 18:56:56.000000 vision_xformer-0.1.7/vision_xformer/vision_linformer.py
+-rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.7/vision_xformer/vision_nystromformer.py
+-rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.7/vision_xformer/vision_performer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:15:50.582251 vision_xformer-0.1.7/vision_xformer.egg-info/
+-rw-rw-rw-   0        0        0     3823 2023-05-10 21:15:50.000000 vision_xformer-0.1.7/vision_xformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-10 21:15:50.000000 vision_xformer-0.1.7/vision_xformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 21:15:50.000000 vision_xformer-0.1.7/vision_xformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-10 21:15:50.000000 vision_xformer-0.1.7/vision_xformer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 21:15:50.000000 vision_xformer-0.1.7/vision_xformer.egg-info/top_level.txt
```

### Comparing `vision_xformer-0.1.6/LICENSE` & `vision_xformer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.6/PKG-INFO` & `vision_xformer-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_xformer
-Version: 0.1.6
+Version: 0.1.7
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vision_xformer-0.1.6/README.md` & `vision_xformer-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.6/setup.py` & `vision_xformer-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'vision_xformer',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'Vision Xformers',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/VisionXformer',
```

### Comparing `vision_xformer-0.1.6/vision_xformer/fnet2d.py` & `vision_xformer-0.1.7/vision_xformer/fnet2d.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.6/vision_xformer/vision_linformer.py` & `vision_xformer-0.1.7/vision_xformer/vision_linformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.6/vision_xformer/vision_nystromformer.py` & `vision_xformer-0.1.7/vision_xformer/vision_nystromformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.6/vision_xformer/vision_performer.py` & `vision_xformer-0.1.7/vision_xformer/vision_performer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.6/vision_xformer.egg-info/PKG-INFO` & `vision_xformer-0.1.7/vision_xformer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-xformer
-Version: 0.1.6
+Version: 0.1.7
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```


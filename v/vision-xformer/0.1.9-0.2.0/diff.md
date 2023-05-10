# Comparing `tmp/vision_xformer-0.1.9.tar.gz` & `tmp/vision_xformer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_xformer-0.1.9.tar", last modified: Wed May 10 22:21:04 2023, max compression
+gzip compressed data, was "vision_xformer-0.2.0.tar", last modified: Wed May 10 22:24:06 2023, max compression
```

## Comparing `vision_xformer-0.1.9.tar` & `vision_xformer-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:04.862636 vision_xformer-0.1.9/
--rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     6147 2023-05-10 22:21:04.861641 vision_xformer-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     5302 2023-05-10 22:01:03.000000 vision_xformer-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 22:21:04.863635 vision_xformer-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-05-10 22:20:23.000000 vision_xformer-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:04.817034 vision_xformer-0.1.9/vision_xformer/
--rw-rw-rw-   0        0        0      231 2023-05-10 22:20:31.000000 vision_xformer-0.1.9/vision_xformer/__init__.py
--rw-rw-rw-   0        0        0     3456 2023-05-10 22:20:27.000000 vision_xformer-0.1.9/vision_xformer/fnet.py
--rw-rw-rw-   0        0        0     1843 2023-05-10 22:20:32.000000 vision_xformer-0.1.9/vision_xformer/fnet2d.py
--rw-rw-rw-   0        0        0     6497 2023-05-10 22:02:57.000000 vision_xformer-0.1.9/vision_xformer/vision_linformer.py
--rw-rw-rw-   0        0        0     7009 2023-05-10 22:02:54.000000 vision_xformer-0.1.9/vision_xformer/vision_nystromformer.py
--rw-rw-rw-   0        0        0    14796 2023-05-10 22:20:29.000000 vision_xformer-0.1.9/vision_xformer/vision_performer.py
-drwxrwxrwx   0        0        0        0 2023-05-10 22:21:04.859638 vision_xformer-0.1.9/vision_xformer.egg-info/
--rw-rw-rw-   0        0        0     6147 2023-05-10 22:21:04.000000 vision_xformer-0.1.9/vision_xformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-05-10 22:21:04.000000 vision_xformer-0.1.9/vision_xformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 22:21:04.000000 vision_xformer-0.1.9/vision_xformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-10 22:21:04.000000 vision_xformer-0.1.9/vision_xformer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 22:21:04.000000 vision_xformer-0.1.9/vision_xformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 22:24:06.091367 vision_xformer-0.2.0/
+-rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6147 2023-05-10 22:24:06.090371 vision_xformer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5302 2023-05-10 22:01:03.000000 vision_xformer-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 22:24:06.092392 vision_xformer-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-05-10 22:23:45.000000 vision_xformer-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:24:06.021835 vision_xformer-0.2.0/vision_xformer/
+-rw-rw-rw-   0        0        0      231 2023-05-10 22:23:54.000000 vision_xformer-0.2.0/vision_xformer/__init__.py
+-rw-rw-rw-   0        0        0     3456 2023-05-10 22:20:27.000000 vision_xformer-0.2.0/vision_xformer/fnet.py
+-rw-rw-rw-   0        0        0     1843 2023-05-10 22:23:50.000000 vision_xformer-0.2.0/vision_xformer/fnet2d.py
+-rw-rw-rw-   0        0        0     6497 2023-05-10 22:02:57.000000 vision_xformer-0.2.0/vision_xformer/vision_linformer.py
+-rw-rw-rw-   0        0        0     7009 2023-05-10 22:02:54.000000 vision_xformer-0.2.0/vision_xformer/vision_nystromformer.py
+-rw-rw-rw-   0        0        0    14796 2023-05-10 22:20:29.000000 vision_xformer-0.2.0/vision_xformer/vision_performer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:24:06.085368 vision_xformer-0.2.0/vision_xformer.egg-info/
+-rw-rw-rw-   0        0        0     6147 2023-05-10 22:24:05.000000 vision_xformer-0.2.0/vision_xformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-10 22:24:05.000000 vision_xformer-0.2.0/vision_xformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 22:24:05.000000 vision_xformer-0.2.0/vision_xformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-10 22:24:05.000000 vision_xformer-0.2.0/vision_xformer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 22:24:05.000000 vision_xformer-0.2.0/vision_xformer.egg-info/top_level.txt
```

### Comparing `vision_xformer-0.1.9/LICENSE` & `vision_xformer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.9/PKG-INFO` & `vision_xformer-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_xformer
-Version: 0.1.9
+Version: 0.2.0
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vision_xformer-0.1.9/README.md` & `vision_xformer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.9/setup.py` & `vision_xformer-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'vision_xformer',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.9',
+  version = '0.2.0',
   license='MIT',
   description = 'Vision Xformers',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/VisionXformer',
```

### Comparing `vision_xformer-0.1.9/vision_xformer/fnet.py` & `vision_xformer-0.2.0/vision_xformer/fnet.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.9/vision_xformer/fnet2d.py` & `vision_xformer-0.2.0/vision_xformer/fnet2d.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         return x
         
 class FNet2D(nn.Module):
     def __init__(
         self,
         *,
         num_classes,
-        depth,
         dim,
+        depth,
         mlp_dim, 
         dropout = 0.,
         
     ):
         super().__init__()
         
         self.layers = nn.ModuleList([])
```

### Comparing `vision_xformer-0.1.9/vision_xformer/vision_linformer.py` & `vision_xformer-0.2.0/vision_xformer/vision_linformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.9/vision_xformer/vision_nystromformer.py` & `vision_xformer-0.2.0/vision_xformer/vision_nystromformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.9/vision_xformer/vision_performer.py` & `vision_xformer-0.2.0/vision_xformer/vision_performer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.9/vision_xformer.egg-info/PKG-INFO` & `vision_xformer-0.2.0/vision_xformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-xformer
-Version: 0.1.9
+Version: 0.2.0
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```


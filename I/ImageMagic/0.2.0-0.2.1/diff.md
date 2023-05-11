# Comparing `tmp/ImageMagic-0.2.0.tar.gz` & `tmp/ImageMagic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageMagic-0.2.0.tar", last modified: Thu May 11 15:42:11 2023, max compression
+gzip compressed data, was "ImageMagic-0.2.1.tar", last modified: Thu May 11 15:47:08 2023, max compression
```

## Comparing `ImageMagic-0.2.0.tar` & `ImageMagic-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:42:11.278939 ImageMagic-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:42:11.271934 ImageMagic-0.2.0/ImageMagic/
--rw-rw-rw-   0        0        0     6237 2023-05-07 00:54:28.000000 ImageMagic-0.2.0/ImageMagic/Aocr.py
--rw-rw-rw-   0        0        0    16609 2023-05-11 15:40:21.000000 ImageMagic-0.2.0/ImageMagic/Image.py
--rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.2.0/ImageMagic/_Atesseract.py
--rw-rw-rw-   0        0        0      259 2023-05-10 13:15:56.000000 ImageMagic-0.2.0/ImageMagic/__init__.py
--rw-rw-rw-   0        0        0       86 2023-05-11 15:40:21.000000 ImageMagic-0.2.0/ImageMagic/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:42:11.275940 ImageMagic-0.2.0/ImageMagic.egg-info/
--rw-rw-rw-   0        0        0     2114 2023-05-11 15:42:11.000000 ImageMagic-0.2.0/ImageMagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-05-11 15:42:11.000000 ImageMagic-0.2.0/ImageMagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:42:11.000000 ImageMagic-0.2.0/ImageMagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-11 15:42:11.000000 ImageMagic-0.2.0/ImageMagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-11 15:42:11.000000 ImageMagic-0.2.0/ImageMagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2114 2023-05-11 15:42:11.277940 ImageMagic-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1677 2023-05-07 05:32:38.000000 ImageMagic-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 15:42:11.278939 ImageMagic-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-05-10 05:29:35.000000 ImageMagic-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:42:11.276940 ImageMagic-0.2.0/test/
--rw-rw-rw-   0        0        0       26 2023-05-06 05:17:57.000000 ImageMagic-0.2.0/test/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-05-07 05:15:55.000000 ImageMagic-0.2.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:47:08.240799 ImageMagic-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:47:08.234843 ImageMagic-0.2.1/ImageMagic/
+-rw-rw-rw-   0        0        0     6237 2023-05-07 00:54:28.000000 ImageMagic-0.2.1/ImageMagic/Aocr.py
+-rw-rw-rw-   0        0        0    16609 2023-05-11 15:40:21.000000 ImageMagic-0.2.1/ImageMagic/Image.py
+-rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.2.1/ImageMagic/_Atesseract.py
+-rw-rw-rw-   0        0        0      259 2023-05-10 13:15:56.000000 ImageMagic-0.2.1/ImageMagic/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-05-11 15:46:53.000000 ImageMagic-0.2.1/ImageMagic/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:47:08.237842 ImageMagic-0.2.1/ImageMagic.egg-info/
+-rw-rw-rw-   0        0        0     2119 2023-05-11 15:47:08.000000 ImageMagic-0.2.1/ImageMagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-05-11 15:47:08.000000 ImageMagic-0.2.1/ImageMagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:47:08.000000 ImageMagic-0.2.1/ImageMagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-11 15:47:08.000000 ImageMagic-0.2.1/ImageMagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-11 15:47:08.000000 ImageMagic-0.2.1/ImageMagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2119 2023-05-11 15:47:08.239793 ImageMagic-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1677 2023-05-07 05:32:38.000000 ImageMagic-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:47:08.240799 ImageMagic-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-05-11 15:46:35.000000 ImageMagic-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:47:08.239793 ImageMagic-0.2.1/test/
+-rw-rw-rw-   0        0        0       26 2023-05-06 05:17:57.000000 ImageMagic-0.2.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-05-07 05:15:55.000000 ImageMagic-0.2.1/test/test.py
```

### Comparing `ImageMagic-0.2.0/ImageMagic/Aocr.py` & `ImageMagic-0.2.1/ImageMagic/Aocr.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.2.0/ImageMagic/Image.py` & `ImageMagic-0.2.1/ImageMagic/Image.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.2.0/ImageMagic/_Atesseract.py` & `ImageMagic-0.2.1/ImageMagic/_Atesseract.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.2.0/ImageMagic.egg-info/PKG-INFO` & `ImageMagic-0.2.1/ImageMagic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ImageMagic
-Version: 0.2.0
+Version: 0.2.1
 Summary: 图像处理库（包括但不限于图像）【Image processing libraries (including but not limited to images)】
 Home-page: https://github.com/asxez/ImageMagic
 Author: asxe
 Author-email: 2973918177@qq.com
 License: GNU GPL 3.0
 Keywords: Python library,image process,imagemagic,ocr function and more!
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="https://i.328888.xyz/2023/05/04/iPlOg8.png" width="500" height="450" alt=""><br>
 </div>
 
 # ImageMagic:A concise image (including but not limited to) processing library
```

### Comparing `ImageMagic-0.2.0/LICENSE` & `ImageMagic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.2.0/PKG-INFO` & `ImageMagic-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ImageMagic
-Version: 0.2.0
+Version: 0.2.1
 Summary: 图像处理库（包括但不限于图像）【Image processing libraries (including but not limited to images)】
 Home-page: https://github.com/asxez/ImageMagic
 Author: asxe
 Author-email: 2973918177@qq.com
 License: GNU GPL 3.0
 Keywords: Python library,image process,imagemagic,ocr function and more!
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="https://i.328888.xyz/2023/05/04/iPlOg8.png" width="500" height="450" alt=""><br>
 </div>
 
 # ImageMagic:A concise image (including but not limited to) processing library
```

### Comparing `ImageMagic-0.2.0/README.md` & `ImageMagic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.2.0/setup.py` & `ImageMagic-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     packages=find_packages(exclude='test'),
     url='https://github.com/asxez/ImageMagic',
     license='GNU GPL 3.0',
     author='asxe',
     author_email='2973918177@qq.com',
     description='图像处理库（包括但不限于图像）【Image processing libraries (including but not limited to images)】',
     long_description=long_description,
-    long_description_content_type='markdown',
+    long_description_content_type='text/markdown',
     keywords='Python library, image process, imagemagic, ocr function and more! ',
     install_requires=[
         'Pillow',
         'requests',
         'loguru',
         'numpy',
         'pandas',
```

### Comparing `ImageMagic-0.2.0/test/test.py` & `ImageMagic-0.2.1/test/test.py`

 * *Files identical despite different names*


# Comparing `tmp/HyperEvalSR-0.31.tar.gz` & `tmp/HyperEvalSR-0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyperEvalSR-0.31.tar", last modified: Wed May 10 13:01:30 2023, max compression
+gzip compressed data, was "HyperEvalSR-0.32.tar", last modified: Thu May 11 11:37:56 2023, max compression
```

## Comparing `HyperEvalSR-0.31.tar` & `HyperEvalSR-0.32.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/HyperEvalSR/
--rw-rw-rw-   0        0        0        0 2023-03-06 08:18:38.000000 HyperEvalSR-0.31/HyperEvalSR/__init__.py
--rw-rw-rw-   0        0        0     8892 2023-05-08 07:44:02.000000 HyperEvalSR-0.31/HyperEvalSR/ev.py
--rw-rw-rw-   0        0        0    38940 2023-05-10 12:54:15.000000 HyperEvalSR-0.31/HyperEvalSR/sr.py
--rw-rw-rw-   0        0        0      482 2023-03-09 11:55:25.000000 HyperEvalSR-0.31/HyperEvalSR/test.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/HyperEvalSR.egg-info/
--rw-rw-rw-   0        0        0     8517 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2023-03-06 08:15:40.000000 HyperEvalSR-0.31/LICENSE
--rw-rw-rw-   0        0        0     8517 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/PKG-INFO
--rw-rw-rw-   0        0        0     7111 2023-05-08 13:24:26.000000 HyperEvalSR-0.31/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-10 13:00:46.000000 HyperEvalSR-0.31/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/test/
--rw-rw-rw-   0        0        0        0 2023-05-10 12:56:45.000000 HyperEvalSR-0.31/test/test_ev.py
--rw-rw-rw-   0        0        0        0 2023-05-10 12:56:56.000000 HyperEvalSR-0.31/test/test_sr.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:37:56.655204 HyperEvalSR-0.32/
+drwxrwxrwx   0        0        0        0 2023-05-11 11:37:56.649206 HyperEvalSR-0.32/HyperEvalSR/
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:18:38.000000 HyperEvalSR-0.32/HyperEvalSR/__init__.py
+-rw-rw-rw-   0        0        0     8892 2023-05-08 07:44:02.000000 HyperEvalSR-0.32/HyperEvalSR/ev.py
+-rw-rw-rw-   0        0        0    38947 2023-05-11 11:27:02.000000 HyperEvalSR-0.32/HyperEvalSR/sr.py
+-rw-rw-rw-   0        0        0      482 2023-03-09 11:55:25.000000 HyperEvalSR-0.32/HyperEvalSR/test.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:37:56.652205 HyperEvalSR-0.32/HyperEvalSR.egg-info/
+-rw-rw-rw-   0        0        0     8517 2023-05-11 11:37:56.000000 HyperEvalSR-0.32/HyperEvalSR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-05-11 11:37:56.000000 HyperEvalSR-0.32/HyperEvalSR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:37:56.000000 HyperEvalSR-0.32/HyperEvalSR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 11:37:56.000000 HyperEvalSR-0.32/HyperEvalSR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 11:37:56.000000 HyperEvalSR-0.32/HyperEvalSR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-03-06 08:15:40.000000 HyperEvalSR-0.32/LICENSE
+-rw-rw-rw-   0        0        0     8517 2023-05-11 11:37:56.654204 HyperEvalSR-0.32/PKG-INFO
+-rw-rw-rw-   0        0        0     7111 2023-05-08 13:24:26.000000 HyperEvalSR-0.32/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 11:37:56.655204 HyperEvalSR-0.32/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-11 11:33:03.000000 HyperEvalSR-0.32/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:37:56.653206 HyperEvalSR-0.32/test/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:56:45.000000 HyperEvalSR-0.32/test/test_ev.py
+-rw-rw-rw-   0        0        0      192 2023-05-11 11:24:22.000000 HyperEvalSR-0.32/test/test_sr.py
```

### Comparing `HyperEvalSR-0.31/HyperEvalSR/ev.py` & `HyperEvalSR-0.32/HyperEvalSR/ev.py`

 * *Files identical despite different names*

### Comparing `HyperEvalSR-0.31/HyperEvalSR/sr.py` & `HyperEvalSR-0.32/HyperEvalSR/sr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from scipy import ndimage
+from scipy.special import erfinv
 
 def fspecial_gauss(size, sigma):
     x, y = np.mgrid[-size//2 + 1:size//2 + 1, -size//2 + 1:size//2 + 1]
     g = np.exp(-((x**2 + y**2)/(2.0*sigma**2)))
     return g/g.sum()
 
 def downsample(image, factor, method='uniform'):
```

### Comparing `HyperEvalSR-0.31/HyperEvalSR.egg-info/PKG-INFO` & `HyperEvalSR-0.32/HyperEvalSR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperEvalSR
-Version: 0.31
+Version: 0.32
 Summary: An open source python package for super-resolution/recovery quality evaluation of hyperspectral images, including RMSE, ERGAS, SSIM, RSNR, PSNR, CC, DD, and SAM.
 Home-page: https://github.com/jingmengzhiyue/HyperEvalSR
 Author: jingmengzhiyue
 Author-email: jingmengzhiyue@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HyperEvalSR-0.31/LICENSE` & `HyperEvalSR-0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `HyperEvalSR-0.31/PKG-INFO` & `HyperEvalSR-0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperEvalSR
-Version: 0.31
+Version: 0.32
 Summary: An open source python package for super-resolution/recovery quality evaluation of hyperspectral images, including RMSE, ERGAS, SSIM, RSNR, PSNR, CC, DD, and SAM.
 Home-page: https://github.com/jingmengzhiyue/HyperEvalSR
 Author: jingmengzhiyue
 Author-email: jingmengzhiyue@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HyperEvalSR-0.31/README.md` & `HyperEvalSR-0.32/README.md`

 * *Files identical despite different names*

### Comparing `HyperEvalSR-0.31/setup.py` & `HyperEvalSR-0.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from re import U
 from struct import pack
 import setuptools
 with open(".\docs\index.md", "r") as f:
     long_description = f.read()
 setuptools.setup(
     name = "HyperEvalSR",
-    version="0.31",
+    version="0.32",
     author = "jingmengzhiyue",
     author_email = "jingmengzhiyue@gmail.com",
     description = "An open source python package for super-resolution/recovery quality evaluation of hyperspectral images, including RMSE, ERGAS, SSIM, RSNR, PSNR, CC, DD, and SAM.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/jingmengzhiyue/HyperEvalSR",
     packages =  setuptools.find_packages(),
```


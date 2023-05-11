# Comparing `tmp/foscat-2.0.1.tar.gz` & `tmp/foscat-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-mi8in77j/foscat-2.0.1.tar", last modified: Wed May 10 14:16:02 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-k7bp7gwi/foscat-2.0.2.tar", last modified: Thu May 11 10:46:11 2023, max compression
```

## Comparing `foscat-2.0.1.tar` & `foscat-2.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-10 14:16:02.000000 foscat-2.0.1/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.1/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-05-10 14:16:02.000000 foscat-2.0.1/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-05-10 14:15:16.000000 foscat-2.0.1/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57131 2023-05-02 14:56:56.000000 foscat-2.0.1/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.1/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1766 2023-03-31 09:38:33.000000 foscat-2.0.1/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    15268 2023-05-10 13:27:24.000000 foscat-2.0.1/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.1/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13465 2023-03-31 07:45:21.000000 foscat-2.0.1/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.1/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.1/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    21467 2023-05-02 15:09:32.000000 foscat-2.0.1/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.1/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    46097 2023-04-26 15:05:16.000000 foscat-2.0.1/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.1/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 10:46:11.000000 foscat-2.0.2/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-11 10:46:11.000000 foscat-2.0.2/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.2/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-05-11 10:46:11.000000 foscat-2.0.2/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-05-11 10:45:17.000000 foscat-2.0.2/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 10:46:11.000000 foscat-2.0.2/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 10:46:11.000000 foscat-2.0.2/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57131 2023-05-02 14:56:56.000000 foscat-2.0.2/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.2/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1766 2023-03-31 09:38:33.000000 foscat-2.0.2/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    15268 2023-05-11 10:09:32.000000 foscat-2.0.2/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.2/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13465 2023-03-31 07:45:21.000000 foscat-2.0.2/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.2/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.2/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    21467 2023-05-02 15:09:32.000000 foscat-2.0.2/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.2/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    46094 2023-05-11 10:27:00.000000 foscat-2.0.2/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.2/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 10:46:11.000000 foscat-2.0.2/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-11 10:46:11.000000 foscat-2.0.2/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-05-11 10:46:11.000000 foscat-2.0.2/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-05-11 10:46:11.000000 foscat-2.0.2/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-05-11 10:46:11.000000 foscat-2.0.2/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-05-11 10:46:11.000000 foscat-2.0.2/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.0.1/PKG-INFO` & `foscat-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.1
+Version: 2.0.2
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.0.1/README.md` & `foscat-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/setup.py` & `foscat-2.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.0.1',
+    version='2.0.2',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulqieur, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.0.1/src/foscat/FoCUS.py` & `foscat-2.0.2/src/foscat/FoCUS.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/GetGPUinfo.py` & `foscat-2.0.2/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/Rformat.py` & `foscat-2.0.2/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/Synthesis.py` & `foscat-2.0.2/src/foscat/Synthesis.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/backend.py` & `foscat-2.0.2/src/foscat/backend.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/build_demo.py` & `foscat-2.0.2/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/scat.py` & `foscat-2.0.2/src/foscat/scat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/scat_cov.old.py` & `foscat-2.0.2/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat/scat_cov.py` & `foscat-2.0.2/src/foscat/scat_cov.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
         if self.S1 is None:
             s1 = None
         else:
             if isinstance(other, scat_cov):
                 s1 = other.S1 / self.S1
             else:
-                s1 = other.S1 / other
+                s1 = other/self.S1
 
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
                 c10 = self.dodiv(other.C10 , self.C10)
             else:
```

### Comparing `foscat-2.0.1/src/foscat/scat_cov_new.py` & `foscat-2.0.2/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.1/src/foscat.egg-info/PKG-INFO` & `foscat-2.0.2/src/foscat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.1
+Version: 2.0.2
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```


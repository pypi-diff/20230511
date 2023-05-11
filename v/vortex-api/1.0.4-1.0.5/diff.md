# Comparing `tmp/vortex_api-1.0.4.tar.gz` & `tmp/vortex_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-sltf9og_/vortex_api-1.0.4.tar", last modified: Wed May 10 20:16:31 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-pdch_rig/vortex_api-1.0.5.tar", last modified: Thu May 11 05:00:36 2023, max compression
```

## Comparing `vortex_api-1.0.4.tar` & `vortex_api-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-10 20:16:31.770668 vortex_api-1.0.4/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.4/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1771 2023-05-10 20:16:31.770849 vortex_api-1.0.4/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      915 2023-05-10 20:08:17.000000 vortex_api-1.0.4/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-10 20:16:31.771187 vortex_api-1.0.4/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1408 2023-05-10 18:30:10.000000 vortex_api-1.0.4/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-10 20:16:31.769029 vortex_api-1.0.4/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1331 2023-05-10 17:24:32.000000 vortex_api-1.0.4/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      336 2023-05-10 12:15:34.000000 vortex_api-1.0.4/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    24579 2023-05-10 20:13:55.000000 vortex_api-1.0.4/vortex_api/api.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-10 20:16:31.770485 vortex_api-1.0.4/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1771 2023-05-10 20:16:31.000000 vortex_api-1.0.4/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      272 2023-05-10 20:16:31.000000 vortex_api-1.0.4/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-10 20:16:31.000000 vortex_api-1.0.4/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       30 2023-05-10 20:16:31.000000 vortex_api-1.0.4/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-10 20:16:31.000000 vortex_api-1.0.4/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-11 05:00:36.275211 vortex_api-1.0.5/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.5/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1771 2023-05-11 05:00:36.275314 vortex_api-1.0.5/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      915 2023-05-10 20:08:17.000000 vortex_api-1.0.5/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-11 05:00:36.275603 vortex_api-1.0.5/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1409 2023-05-11 04:56:57.000000 vortex_api-1.0.5/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-11 05:00:36.272567 vortex_api-1.0.5/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1331 2023-05-10 17:24:32.000000 vortex_api-1.0.5/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      336 2023-05-11 04:59:05.000000 vortex_api-1.0.5/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    24579 2023-05-10 20:13:55.000000 vortex_api-1.0.5/vortex_api/api.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-11 05:00:36.275046 vortex_api-1.0.5/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1771 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      272 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       31 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.4/LICENSE` & `vortex_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.4/PKG-INFO` & `vortex_api-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `vortex_api-1.0.4/README.md` & `vortex_api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.4/setup.py` & `vortex_api-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     author_email=about["__author_email__"],
     url=about["__url__"],
     download_url=about["__download_url__"],
     license=about["__license__"],
     packages=["vortex_api"],
     install_requires=[
         "requests>=2.25.1",
-        "wrapt-1.15.0"
+        "wrapt>=1.15.0"
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `vortex_api-1.0.4/vortex_api/__init__.py` & `vortex_api-1.0.5/vortex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.4/vortex_api/api.py` & `vortex_api-1.0.5/vortex_api/api.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.4/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.5/vortex_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```


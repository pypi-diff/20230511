# Comparing `tmp/based-metric-0.0.1.tar.gz` & `tmp/based-metric-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "based-metric-0.0.1.tar", last modified: Wed May 10 18:34:49 2023, max compression
+gzip compressed data, was "based-metric-0.0.2.tar", last modified: Thu May 11 12:12:45 2023, max compression
```

## Comparing `based-metric-0.0.1.tar` & `based-metric-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-10 18:34:49.252786 based-metric-0.0.1/
--rw-r--r--   0 mvdremin   (501) staff       (20)       21 2023-05-10 17:15:43.000000 based-metric-0.0.1/MANIFEST.in
--rw-r--r--   0 mvdremin   (501) staff       (20)      292 2023-05-10 18:34:49.252520 based-metric-0.0.1/PKG-INFO
--rw-r--r--   0 mvdremin   (501) staff       (20)      720 2023-05-10 15:45:09.000000 based-metric-0.0.1/README.md
-drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-10 18:34:49.240030 based-metric-0.0.1/based/
--rw-r--r--   0 mvdremin   (501) staff       (20)       25 2023-05-10 18:12:22.000000 based-metric-0.0.1/based/__init__.py
--rw-r--r--   0 mvdremin   (501) staff       (20)    20163 2023-05-10 18:11:04.000000 based-metric-0.0.1/based/metric.py
-drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-10 18:34:49.240735 based-metric-0.0.1/based/model/
--rw-r--r--   0 mvdremin   (501) staff       (20)  6998977 2023-05-10 16:54:34.000000 based-metric-0.0.1/based/model/based_random_forest.joblib
-drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-10 18:34:49.252034 based-metric-0.0.1/based_metric.egg-info/
--rw-r--r--   0 mvdremin   (501) staff       (20)      292 2023-05-10 18:34:49.000000 based-metric-0.0.1/based_metric.egg-info/PKG-INFO
--rw-r--r--   0 mvdremin   (501) staff       (20)      282 2023-05-10 18:34:49.000000 based-metric-0.0.1/based_metric.egg-info/SOURCES.txt
--rw-r--r--   0 mvdremin   (501) staff       (20)        1 2023-05-10 18:34:49.000000 based-metric-0.0.1/based_metric.egg-info/dependency_links.txt
--rw-r--r--   0 mvdremin   (501) staff       (20)      131 2023-05-10 18:34:49.000000 based-metric-0.0.1/based_metric.egg-info/requires.txt
--rw-r--r--   0 mvdremin   (501) staff       (20)        6 2023-05-10 18:34:49.000000 based-metric-0.0.1/based_metric.egg-info/top_level.txt
--rw-r--r--   0 mvdremin   (501) staff       (20)       38 2023-05-10 18:34:49.252867 based-metric-0.0.1/setup.cfg
--rw-r--r--   0 mvdremin   (501) staff       (20)      953 2023-05-10 18:34:48.000000 based-metric-0.0.1/setup.py
+drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-11 12:12:45.643370 based-metric-0.0.2/
+-rw-r--r--   0 mvdremin   (501) staff       (20)       21 2023-05-10 17:15:43.000000 based-metric-0.0.2/MANIFEST.in
+-rw-r--r--   0 mvdremin   (501) staff       (20)      292 2023-05-11 12:12:45.643109 based-metric-0.0.2/PKG-INFO
+-rw-r--r--   0 mvdremin   (501) staff       (20)      720 2023-05-10 15:45:09.000000 based-metric-0.0.2/README.md
+drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-11 12:12:45.626598 based-metric-0.0.2/based/
+-rw-r--r--   0 mvdremin   (501) staff       (20)       25 2023-05-10 18:12:22.000000 based-metric-0.0.2/based/__init__.py
+-rw-r--r--   0 mvdremin   (501) staff       (20)    20159 2023-05-11 12:10:16.000000 based-metric-0.0.2/based/metric.py
+drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-11 12:12:45.627414 based-metric-0.0.2/based/model/
+-rw-r--r--   0 mvdremin   (501) staff       (20)  6998977 2023-05-10 16:54:34.000000 based-metric-0.0.2/based/model/based_random_forest.joblib
+drwxr-xr-x   0 mvdremin   (501) staff       (20)        0 2023-05-11 12:12:45.642638 based-metric-0.0.2/based_metric.egg-info/
+-rw-r--r--   0 mvdremin   (501) staff       (20)      292 2023-05-11 12:12:45.000000 based-metric-0.0.2/based_metric.egg-info/PKG-INFO
+-rw-r--r--   0 mvdremin   (501) staff       (20)      282 2023-05-11 12:12:45.000000 based-metric-0.0.2/based_metric.egg-info/SOURCES.txt
+-rw-r--r--   0 mvdremin   (501) staff       (20)        1 2023-05-11 12:12:45.000000 based-metric-0.0.2/based_metric.egg-info/dependency_links.txt
+-rw-r--r--   0 mvdremin   (501) staff       (20)      131 2023-05-11 12:12:45.000000 based-metric-0.0.2/based_metric.egg-info/requires.txt
+-rw-r--r--   0 mvdremin   (501) staff       (20)        6 2023-05-11 12:12:45.000000 based-metric-0.0.2/based_metric.egg-info/top_level.txt
+-rw-r--r--   0 mvdremin   (501) staff       (20)       38 2023-05-11 12:12:45.643432 based-metric-0.0.2/setup.cfg
+-rw-r--r--   0 mvdremin   (501) staff       (20)      953 2023-05-11 12:12:28.000000 based-metric-0.0.2/setup.py
```

### Comparing `based-metric-0.0.1/README.md` & `based-metric-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `based-metric-0.0.1/based/metric.py` & `based-metric-0.0.2/based/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,15 +705,15 @@
                             laple_calc,
                             log_calc,
                             sharr_calc,
                             hist_cmp,
                             saliency_calc,
                             reblur_calc,
                         ]
-        self.model = joblib_load("based/model/based_random_forest.joblib")
+        self.model = joblib_load("./model/based_random_forest.joblib")
 
     def __call__(self, image1: Union[PIL.Image.Image, np.array, str], image2: Union[PIL.Image.Image, np.array, str]) -> Union[float, None]:
         if isinstance(image1, str):
             try:
                 image1 = PIL.Image.open(image1).convert("RGB")
             except Exception as e:
                 print(e)
```

### Comparing `based-metric-0.0.1/based/model/based_random_forest.joblib` & `based-metric-0.0.2/based/model/based_random_forest.joblib`

 * *Files identical despite different names*

### Comparing `based-metric-0.0.1/setup.py` & `based-metric-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="based-metric",
-    version="0.0.1",
+    version="0.0.2",
     url="",
     author="Nick Alutis",
     author_email="",
     description="BASED metric for deblurring assesement",
     packages=setuptools.find_packages(),
     long_description="",
     install_requires=["numpy",
```


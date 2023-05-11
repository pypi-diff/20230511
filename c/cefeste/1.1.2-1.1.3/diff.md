# Comparing `tmp/cefeste-1.1.2.tar.gz` & `tmp/cefeste-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.1.2.tar", last modified: Wed May 10 10:23:59 2023, max compression
+gzip compressed data, was "cefeste-1.1.3.tar", last modified: Thu May 11 12:59:37 2023, max compression
```

## Comparing `cefeste-1.1.2.tar` & `cefeste-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.880164 cefeste-1.1.2/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.2/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-10 10:23:59.880164 cefeste-1.1.2/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1560 2023-05-10 10:23:33.000000 cefeste-1.1.2/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-10 10:23:33.000000 cefeste-1.1.2/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-10 10:23:59.880164 cefeste-1.1.2/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      997 2023-05-10 10:23:33.000000 cefeste-1.1.2/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.772162 cefeste-1.1.2/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.824163 cefeste-1.1.2/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.824163 cefeste-1.1.2/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15368 2023-05-10 10:23:33.000000 cefeste-1.1.2/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.2/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.844163 cefeste-1.1.2/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.852163 cefeste-1.1.2/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.2/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.824163 cefeste-1.1.2/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.603643 cefeste-1.1.3/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.3/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-11 12:59:37.603643 cefeste-1.1.3/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1560 2023-05-10 10:23:33.000000 cefeste-1.1.3/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-11 12:55:44.000000 cefeste-1.1.3/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-11 12:59:37.603643 cefeste-1.1.3/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      999 2023-05-11 12:55:44.000000 cefeste-1.1.3/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.555639 cefeste-1.1.3/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.591642 cefeste-1.1.3/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.595642 cefeste-1.1.3/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15368 2023-05-10 10:23:33.000000 cefeste-1.1.3/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.3/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.603643 cefeste-1.1.3/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.603643 cefeste-1.1.3/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.3/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.3/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-11 12:59:37.595642 cefeste-1.1.3/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-11 12:59:37.000000 cefeste-1.1.3/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.1.2/LICENCE` & `cefeste-1.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/PKG-INFO` & `cefeste-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.2
+Version: 1.1.3
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.1.2/README.md` & `cefeste-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/pyproject.toml` & `cefeste-1.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cefeste-1.1.2/setup.py` & `cefeste-1.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.1.2",
+    version="1.1.3",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
@@ -16,15 +16,15 @@
     ],
     packages=find_packages(where="src", exclude=["test"]),
     package_dir={"": "src"},
     # Usato solo con 3.9 e 3.10
     python_requires=">=3.9, <4",
     install_requires=[
         "typed-ast==1.5.4",
-        "numpy~=1.22",
+        "numpy==1.22.4",
         "pandas==1.4.2",
         "scikit-learn==1.1.1",
         "scipy==1.8.1",
         "statsmodels==0.13.2",
         "PyYAML==6.0",
         "shap==0.38.1",
         "ipython",
```

### Comparing `cefeste-1.1.2/src/cefeste/__init__.py` & `cefeste-1.1.3/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/elimination/__init__.py` & `cefeste-1.1.3/src/cefeste/elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.3/src/cefeste/elimination/shap_rfe.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/selection/__init__.py` & `cefeste-1.1.3/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/selection/explanatory.py` & `cefeste-1.1.3/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/selection/multivariate.py` & `cefeste-1.1.3/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/selection/univariate.py` & `cefeste-1.1.3/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/transform/__init__.py` & `cefeste-1.1.3/src/cefeste/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste/utils.py` & `cefeste-1.1.3/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.2/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.3/src/cefeste.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.2
+Version: 1.1.3
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.1.2/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.3/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*


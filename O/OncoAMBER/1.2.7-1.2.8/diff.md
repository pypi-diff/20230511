# Comparing `tmp/OncoAMBER-1.2.7.tar.gz` & `tmp/OncoAMBER-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.2.7.tar", last modified: Thu May 11 15:39:27 2023, max compression
+gzip compressed data, was "OncoAMBER-1.2.8.tar", last modified: Thu May 11 15:40:22 2023, max compression
```

## Comparing `OncoAMBER-1.2.7.tar` & `OncoAMBER-1.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:39:27.569521 OncoAMBER-1.2.7/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:39:27.479605 OncoAMBER-1.2.7/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:39:27.000000 OncoAMBER-1.2.7/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-11 15:39:27.000000 OncoAMBER-1.2.7/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-11 15:39:27.000000 OncoAMBER-1.2.7/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.7/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-11 15:39:27.000000 OncoAMBER-1.2.7/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-11 15:39:27.000000 OncoAMBER-1.2.7/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:39:27.569222 OncoAMBER-1.2.7/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.7/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:39:27.567741 OncoAMBER-1.2.7/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.7/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.7/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.7/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    22865 2023-05-11 15:06:44.000000 OncoAMBER-1.2.7/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.7/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.7/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.7/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.7/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5702 2023-05-10 21:23:03.000000 OncoAMBER-1.2.7/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    26555 2023-05-10 22:10:54.000000 OncoAMBER-1.2.7/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      332 2023-05-11 15:37:23.000000 OncoAMBER-1.2.7/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.7/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.7/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.7/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-11 15:39:27.569600 OncoAMBER-1.2.7/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3149 2023-05-11 15:39:24.000000 OncoAMBER-1.2.7/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:40:22.106850 OncoAMBER-1.2.8/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:40:22.014578 OncoAMBER-1.2.8/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-11 15:40:22.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-11 15:40:21.000000 OncoAMBER-1.2.8/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:40:22.106468 OncoAMBER-1.2.8/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.8/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:40:22.104848 OncoAMBER-1.2.8/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.8/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.8/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    22865 2023-05-11 15:06:44.000000 OncoAMBER-1.2.8/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.8/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.8/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5702 2023-05-10 21:23:03.000000 OncoAMBER-1.2.8/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    26555 2023-05-10 22:10:54.000000 OncoAMBER-1.2.8/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      332 2023-05-11 15:40:19.000000 OncoAMBER-1.2.8/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.8/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.8/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-11 15:40:22.106951 OncoAMBER-1.2.8/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3118 2023-05-11 15:40:19.000000 OncoAMBER-1.2.8/setup.py
```

### Comparing `OncoAMBER-1.2.7/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.2.8/OncoAMBER.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.7
+Version: 1.2.8
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.7/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.2.8/OncoAMBER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/PKG-INFO` & `OncoAMBER-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.7
+Version: 1.2.8
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.7/README.md` & `OncoAMBER-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/BasicGeometries.py` & `OncoAMBER-1.2.8/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.2.8/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/Cell.py` & `OncoAMBER-1.2.8/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/Process.py` & `OncoAMBER-1.2.8/amber/Process.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/ReadAndWrite.py` & `OncoAMBER-1.2.8/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/ScalarField.py` & `OncoAMBER-1.2.8/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/Terminal.py` & `OncoAMBER-1.2.8/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/Vessel.py` & `OncoAMBER-1.2.8/amber/Vessel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/Voxel.py` & `OncoAMBER-1.2.8/amber/Voxel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/World.py` & `OncoAMBER-1.2.8/amber/World.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.2.8/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.2.8/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.7/setup.py` & `OncoAMBER-1.2.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.2.7'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
 
@@ -74,15 +73,15 @@
         self.status('Building source and wheel distribution...')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine...')
         os.system('twine upload dist/*')
 
         self.status('Pushing git tags...')
-        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git tag v{0}'.format(VERSION))
         os.system('git push --tags')
 
 # Executing setup
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
```


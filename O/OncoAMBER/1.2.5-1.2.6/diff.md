# Comparing `tmp/OncoAMBER-1.2.5.tar.gz` & `tmp/OncoAMBER-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.2.5.tar", last modified: Wed May 10 21:36:06 2023, max compression
+gzip compressed data, was "OncoAMBER-1.2.6.tar", last modified: Thu May 11 15:07:24 2023, max compression
```

## Comparing `OncoAMBER-1.2.5.tar` & `OncoAMBER-1.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 21:36:06.582318 OncoAMBER-1.2.5/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 21:36:06.511757 OncoAMBER-1.2.5/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-10 21:36:06.582013 OncoAMBER-1.2.5/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.5/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 21:36:06.580727 OncoAMBER-1.2.5/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.5/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.5/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    22736 2023-05-10 20:59:40.000000 OncoAMBER-1.2.5/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.5/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.5/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5702 2023-05-10 21:23:03.000000 OncoAMBER-1.2.5/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    26559 2023-05-10 21:35:52.000000 OncoAMBER-1.2.5/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.5/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.5/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-10 21:36:06.582404 OncoAMBER-1.2.5/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-10 21:35:52.000000 OncoAMBER-1.2.5/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:07:24.361328 OncoAMBER-1.2.6/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:07:24.254047 OncoAMBER-1.2.6/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:07:24.000000 OncoAMBER-1.2.6/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-11 15:07:24.000000 OncoAMBER-1.2.6/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-11 15:07:24.000000 OncoAMBER-1.2.6/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.6/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-11 15:07:24.000000 OncoAMBER-1.2.6/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-11 15:07:24.000000 OncoAMBER-1.2.6/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-11 15:07:24.361035 OncoAMBER-1.2.6/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.6/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-11 15:07:24.359882 OncoAMBER-1.2.6/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.6/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.6/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.6/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    22865 2023-05-11 15:06:44.000000 OncoAMBER-1.2.6/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.6/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.6/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.6/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.6/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5702 2023-05-10 21:23:03.000000 OncoAMBER-1.2.6/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    26555 2023-05-10 22:10:54.000000 OncoAMBER-1.2.6/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-10 21:49:33.000000 OncoAMBER-1.2.6/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.6/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.6/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.6/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-11 15:07:24.361407 OncoAMBER-1.2.6/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-11 15:06:44.000000 OncoAMBER-1.2.6/setup.py
```

### Comparing `OncoAMBER-1.2.5/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.2.6/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.5
+Version: 1.2.6
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.5/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.2.6/OncoAMBER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/PKG-INFO` & `OncoAMBER-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.5
+Version: 1.2.6
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.5/README.md` & `OncoAMBER-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/BasicGeometries.py` & `OncoAMBER-1.2.6/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.2.6/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/Cell.py` & `OncoAMBER-1.2.6/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/Process.py` & `OncoAMBER-1.2.6/amber/Process.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,17 +233,22 @@
             raise ValueError('necrosis threshold must be smaller or equal to apoptosis threshold. you can set apoptosis probability to 0 if you want to avoid apoptosis.')
     def necrosis_curve(self, x):
         r = self.necrosis_probability - x / self.necrosis_threshold
         if r < 0: r = 0
         return r
 
     def apoptosis_curve(self, x):
-        r_ = (self.apoptosis_probability / self.apoptosis_threshold) * x
-        if r_ < 0: r_ = 0
-        return r_
+        # r_ = (self.apoptosis_probability / self.apoptosis_threshold) * x
+        # if r_ < 0: r_ = 0
+        # return r_
+        if x < self.apoptosis_threshold:
+            return self.apoptosis_probability
+        else:
+            return 0
+
 
     def __call__(self, voxel):
         for cell in voxel.list_of_cells:
             vitality = cell.vitality()
             if vitality < self.apoptosis_threshold:
                 sample = np.random.uniform(0, 1)
                 p_necro = (1 - ((1-self.necrosis_curve(vitality))**self.dt))
```

### Comparing `OncoAMBER-1.2.5/amber/ReadAndWrite.py` & `OncoAMBER-1.2.6/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/ScalarField.py` & `OncoAMBER-1.2.6/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/Terminal.py` & `OncoAMBER-1.2.6/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/Vessel.py` & `OncoAMBER-1.2.6/amber/Vessel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/Voxel.py` & `OncoAMBER-1.2.6/amber/Voxel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/World.py` & `OncoAMBER-1.2.6/amber/World.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                     position = np.array([
                         i * voxel_length - self.half_length + voxel_length / 2,
                         j * voxel_length - self.half_length + voxel_length / 2,
                         k * voxel_length - self.half_length + voxel_length / 2
                     ])
                     self.voxel_list.append(Voxel(position, self.half_length / self.number_of_voxels, viscosity= self.config.viscosity, voxel_number=i * self.number_of_voxels ** 2 + j * self.number_of_voxels + k))
         self.vasculature = VasculatureNetwork(self.config)
-        self.o_volume_values = []
+        self.o_diameters = []
         self.o_length_values = []
         self.o_bifurcation_values = []
         self.o_VSL_values = []
 
     def initiate_vasculature(self, list_of_mother_vessels):
         self.vasculature = VasculatureNetwork(self.config, list_of_mother_vessels)
         return
```

### Comparing `OncoAMBER-1.2.5/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.2.6/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.2.6/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.5/setup.py` & `OncoAMBER-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.2.5'
+VERSION = '1.2.6'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
```


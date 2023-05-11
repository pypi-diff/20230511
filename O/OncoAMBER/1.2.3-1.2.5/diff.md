# Comparing `tmp/OncoAMBER-1.2.3.tar.gz` & `tmp/OncoAMBER-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.2.3.tar", last modified: Wed May 10 15:46:09 2023, max compression
+gzip compressed data, was "OncoAMBER-1.2.5.tar", last modified: Wed May 10 21:36:06 2023, max compression
```

## Comparing `OncoAMBER-1.2.3.tar` & `OncoAMBER-1.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 15:46:09.634119 OncoAMBER-1.2.3/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 15:46:09.546304 OncoAMBER-1.2.3/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-10 15:46:09.000000 OncoAMBER-1.2.3/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-10 15:46:09.000000 OncoAMBER-1.2.3/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-10 15:46:09.000000 OncoAMBER-1.2.3/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.3/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-10 15:46:09.000000 OncoAMBER-1.2.3/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-10 15:46:09.000000 OncoAMBER-1.2.3/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-10 15:46:09.633837 OncoAMBER-1.2.3/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.3/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 15:46:09.632496 OncoAMBER-1.2.3/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.3/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.3/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.3/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    22736 2023-05-10 14:45:28.000000 OncoAMBER-1.2.3/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.3/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.3/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.3/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.3/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5702 2023-05-10 14:46:28.000000 OncoAMBER-1.2.3/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    28195 2023-05-09 22:46:33.000000 OncoAMBER-1.2.3/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.3/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.3/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.3/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.3/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-10 15:46:09.634199 OncoAMBER-1.2.3/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-10 15:14:42.000000 OncoAMBER-1.2.3/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 21:36:06.582318 OncoAMBER-1.2.5/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 21:36:06.511757 OncoAMBER-1.2.5/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-10 21:36:06.000000 OncoAMBER-1.2.5/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-10 21:36:06.582013 OncoAMBER-1.2.5/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.5/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-10 21:36:06.580727 OncoAMBER-1.2.5/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.5/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.5/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    22736 2023-05-10 20:59:40.000000 OncoAMBER-1.2.5/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.5/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.5/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5702 2023-05-10 21:23:03.000000 OncoAMBER-1.2.5/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    26559 2023-05-10 21:35:52.000000 OncoAMBER-1.2.5/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.5/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.5/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.5/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-10 21:36:06.582404 OncoAMBER-1.2.5/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-10 21:35:52.000000 OncoAMBER-1.2.5/setup.py
```

### Comparing `OncoAMBER-1.2.3/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.2.5/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.3
+Version: 1.2.5
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.3/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.2.5/OncoAMBER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/PKG-INFO` & `OncoAMBER-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.3
+Version: 1.2.5
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.3/README.md` & `OncoAMBER-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/BasicGeometries.py` & `OncoAMBER-1.2.5/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.2.5/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/Cell.py` & `OncoAMBER-1.2.5/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/Process.py` & `OncoAMBER-1.2.5/amber/Process.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/ReadAndWrite.py` & `OncoAMBER-1.2.5/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/ScalarField.py` & `OncoAMBER-1.2.5/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/Terminal.py` & `OncoAMBER-1.2.5/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/Vessel.py` & `OncoAMBER-1.2.5/amber/Vessel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/Voxel.py` & `OncoAMBER-1.2.5/amber/Voxel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/World.py` & `OncoAMBER-1.2.5/amber/World.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from amber.ScalarField import *
 from amber.BasicGeometries import *
 #np.set_printoptions(threshold=sys.maxsize)
 # from scipy.stats import qmc
 import matplotlib.tri as mtri
 import matplotlib.pyplot as plt
 import scipy.sparse as sparse
-import pyvista as pv
 
 
 class World:
     def __init__(self, config):
         print('Initializing world')
         print(config.voxel_per_side, config.half_length_world)
         self.half_length = config.half_length_world
@@ -554,50 +553,11 @@
         print('Length density')
         print(f'Mean: {length_mean:.2f}, Median: {length_median:.2f}, Std: {np.std(length_values):.2f}, Min: {np.min(length_values):.2f}, Max: {np.max(length_values):.2f}')
         print('Bifurcation density')
         print(f'Mean: {bifurcation_mean:.2f}, Median: {bifurcation_median:.2f}, Std: {np.std(bifurcation_values):.2f}, Min: {np.min(bifurcation_values):.2f}, Max: {np.max(bifurcation_values):.2f}')
         print('Vessel segment length')
         print(f'Mean: {VSL_mean:.2f}, Median: {VSL_median:.2f}, Std: {np.std(VSL_values):.2f}, Min: {np.min(VSL_values):.2f}, Max: {np.max(VSL_values):.2f}')
 
-    def generate_tumor_mesh(self, section='none', color_map='jet'):
-        # Calculate the density values for each voxel
-        voxel_densities = []
-        for voxel in self.voxel_list:
-            num_cells = len(voxel.list_of_cells)
-            voxel_volume = voxel.volume
-            density = num_cells / voxel_volume
-            voxel_densities.append(density)
-
-        # Calculate the dimensions and spacing for the grid
-        dimensions = [self.number_of_voxels] * 3
-        spacing = [2 * self.half_length / self.number_of_voxels] * 3
-
-        # Create a PyVista grid object from the voxel data
-        grid = pv.UniformGrid(dimensions)
-        grid.spacing = spacing
-        grid.origin = [-self.half_length] * 3
-        grid.point_arrays['values'] = np.array(voxel_densities)
-
-        # Generate a surface mesh from the grid using density-based modeling
-        surface = grid.threshold([0.1, 1.0], scalars='values').extract_geometry()
-
-        # Remove a section of the surface mesh to visualize the interior of the tumor
-        if section != 'none':
-            section_plane = pv.Plane(origin=(0, 0, 0), normal=section)
-            surface = surface.clip_with_plane(section_plane)
-
-        # Color-code the surface mesh based on the density of cells within each voxel
-        color_values = np.array(voxel_densities)
-        color_mapper = pv.get_cmap(color_map)
-        surface['Density'] = color_values
-        surface.cell_arrays['Density'] = color_values
-        surface = surface.cell_data_to_point_data()
-        surface['Color'] = color_mapper.map(color_values)
-
-        return surface
-
-
-
```

### Comparing `OncoAMBER-1.2.3/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.2.5/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.2.5/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.3/setup.py` & `OncoAMBER-1.2.5/setup.py`

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
-VERSION = '1.2.3'
+VERSION = '1.2.5'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
```


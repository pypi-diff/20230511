# Comparing `tmp/pyroscopegridding-0.3.1.3.tar.gz` & `tmp/pyroscopegridding-0.3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegridding-0.3.1.3.tar", last modified: Wed May 10 20:42:48 2023, max compression
+gzip compressed data, was "pyroscopegridding-0.3.1.4.tar", last modified: Thu May 11 03:18:16 2023, max compression
```

## Comparing `pyroscopegridding-0.3.1.3.tar` & `pyroscopegridding-0.3.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 20:42:48.931392 pyroscopegridding-0.3.1.3/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-10 20:42:48.927390 pyroscopegridding-0.3.1.3/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.1.3/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 20:42:48.767390 pyroscopegridding-0.3.1.3/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     6679 2023-05-10 20:42:30.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9123 2023-05-10 00:43:58.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:02:30.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10710 2023-05-10 18:17:51.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.3.1.3/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 20:42:48.896391 pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-10 20:42:48.000000 pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 20:42:48.000000 pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 20:42:48.000000 pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 20:42:48.000000 pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 20:42:48.000000 pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 20:42:48.000000 pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 20:42:48.933392 pyroscopegridding-0.3.1.3/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1779 2023-05-10 20:42:45.000000 pyroscopegridding-0.3.1.3/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 03:18:16.650489 pyroscopegridding-0.3.1.4/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-11 03:18:16.618710 pyroscopegridding-0.3.1.4/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.1.4/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 03:18:16.187854 pyroscopegridding-0.3.1.4/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-05-11 03:14:34.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9155 2023-05-10 21:45:39.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:02:30.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10684 2023-05-11 03:17:35.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 03:18:16.529155 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-11 03:18:16.652489 pyroscopegridding-0.3.1.4/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1779 2023-05-11 03:17:47.000000 pyroscopegridding-0.3.1.4/setup.py
```

### Comparing `pyroscopegridding-0.3.1.3/PKG-INFO` & `pyroscopegridding-0.3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.1.3/README.md` & `pyroscopegridding-0.3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/gtools.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/naming_conventions.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         denominator = total_count - 1
         denominator[denominator == 0] = None
         
         return np.sqrt(numerator / denominator)
         """
         data = np.array(data)
         data[data<=-9999.] = np.nan
+        data[data==0] = np.nan
         
         stdtau = np.nanstd(data, axis = 0)
         
         return stdtau
         
     
     if statistic == "TotalPixels":
```

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/solar_zenith.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 ##import pytz
 
 
 import datetime
 import numpy as np
 import pandas as pd
 
-#import numba as nb
-#from numba import jit
-#from numba import cu
+import numba as nb
+from numba import jit
+from numba import cuda
 
 from joblib import Parallel, delayed
 
 
 #global variables 
 rad = 180/math.pi
 
@@ -58,15 +58,15 @@
             - 0.387205*math.cos(2.0*theta_0)
             + 0.051967*math.sin(2.0*theta_0) 
             - 0.154527*math.cos(3.0*theta_0) 
             + 0.084798*math.sin(3.0*theta_0))
     declin = declin / rad  #converts to radians
     return theta_0, declin
 
-#@cuda.jit(device=True)
+@cuda.jit(device=True)
 def sda_gpu(D, rad):
     theta_0 = (360.0 * (D - 1) / 365.0) / rad #converts to radians
     declin  = (0.396372 - 22.91327*math.cos(theta_0)
             + 4.02543*math.sin(theta_0) 
             - 0.387205*math.cos(2.0*theta_0)
             + 0.051967*math.sin(2.0*theta_0) 
             - 0.154527*math.cos(3.0*theta_0) 
@@ -106,15 +106,15 @@
     lat_rad = lat / rad
     lon_rad = lon / rad
 
     angle_rad  = angle / rad
     
     return angle, angle_rad, lat_rad, lon_rad
 
-#@cuda.jit(device=True)
+@cuda.jit(device=True)
 def tcsa_gpu(theta_0, time, lat, lon, rad): #assume theta_0 in radians
     correct = (0.004297 + 0.107029*math.cos(theta_0)
                 - 1.837877*math.sin(theta_0)
                 - 0.837378*math.cos(2.0*theta_0)
                 - 2.342824*math.sin(2.0*theta_0))
                     
                 
@@ -167,15 +167,15 @@
             if tmp1 < 0:
                 tmp1 = -1.0
                 
     theta_rad = math.acos(tmp1)
     
     return theta_rad
 
-#@cuda.jit(device=True)
+@cuda.jit(device=True)
 def sz_gpu(lat_rad, lon_rad, angle_rad, declin):
     
     #tmps are in radians
     tmp1 = math.sin(lat_rad)*math.sin(declin) + math.cos(lat_rad)*math.cos(declin)*math.cos(angle_rad)
     #tmp1 = (math.degrees(math.sin(lat_rad))* math.degrees(math.sin(declin)) 
     #        + math.degrees(math.cos(lat_rad)) * math.degrees(math.cos(declin)) * math.degrees(math.cos(angle_rad)))
     tmp2   = abs(tmp1)
@@ -229,33 +229,33 @@
     theta_0, declin = solar_declination_angle(D)
     angle, angle_rad, lat_rad, lon_rad = time_correction_solar_angle(theta_0, time, lat, lon)
     theta_rad = sun_zenith(lat_rad, lon_rad, angle_rad, declin)
     #azimuth_rad = sun_azimuth(lat, lon, angle, angle_rad, theta_rad, declin)
     
     return math.degrees(theta_rad)
 
-#@cuda.jit
+@cuda.jit
 def get_SZA_GPU(lats, lons, N, D, time, sza, rad):
-    pass
+    
     # Establish thread and block indices
-    #t = cuda.threadIdx.x
+    t = cuda.threadIdx.x
     #-------------------------
-    #d = cuda.blockDim.x
+    d = cuda.blockDim.x
     #-------------------------
-    #b = cuda.blockIdx.x
+    b = cuda.blockIdx.x
 
     # Compute global array index
-    #idx = t + b*d
+    idx = t + b*d
 
-    #if idx < N:
-    #    theta_0, declin = sda_gpu(D, rad)
-    #    angle, angle_rad, lat_rad, lon_rad = tcsa_gpu(theta_0, time, lats[idx], lons[idx], rad)
-    #    theta_rad = sz_gpu(lat_rad, lon_rad, angle_rad, declin)
+    if idx < N:
+        theta_0, declin = sda_gpu(D, rad)
+        angle, angle_rad, lat_rad, lon_rad = tcsa_gpu(theta_0, time, lats[idx], lons[idx], rad)
+        theta_rad = sz_gpu(lat_rad, lon_rad, angle_rad, declin)
 
-    #    sza[idx] = theta_rad * rad # to degrees
+        sza[idx] = theta_rad * rad # to degrees
 
 """
 # uses pysolar library
 def get_SZA(lat, lon, time_start, time_diff):
     time_obj = pd.to_datetime(time_start) + pd.to_timedelta(time_diff, unit="minute")
     time_obj = time_obj.replace(tzinfo=datetime.timezone.utc)
     
@@ -265,15 +265,15 @@
 
 #@jit(nopython=True)
 def get_SZA_parallelized(limit, gsize, time_start, time_diff,num_cores=1):
     # limit = [min lat, max lat, min lon, max lon]
     max_lat = int(1+round(((limit[1]-limit[0])/gsize)))
     max_lon = int(1+round(((limit[3]-limit[2])/gsize)))
      
-    """       
+         
     #solar_zenith = Parallel(n_jobs=num_cores)([get_SZA(limit[0] +  i * gsize, limit[2] + j * gsize, time_start, time_diff) for j in range(0, max_lon)] for i in range(0, max_lat))
     #res = Parallel(n_jobs=1)(delayed(math.sqrt)(i**2) for i in range(10))
     if (len(cuda.list_devices()) != 0):
         datetime_obj = pd.to_datetime(time_start)
         datetime_obj = datetime_obj.replace(tzinfo=datetime.timezone.utc)   
         D, time = date_to_num(datetime_obj)
 
@@ -288,15 +288,15 @@
 
         tpb = (256)
         bpg = (int(np.ceil(N / tpb)))
         get_SZA_GPU[bpg, tpb](d_lats, d_lons, N, D, time, d_sza, rad)
 
         sza = d_sza.copy_to_host()
         return sza
-    """
+    
         
     res = Parallel(n_jobs = num_cores)( 
             delayed( get_SZA )(limit[0] +  i * gsize, limit[2] + j * gsize, time_start, time_diff) 
                                     for i in range(0, max_lat)
                                     for j in range(0, max_lon)
         )
```

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.3.1.4/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.1.3/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.3/setup.py` & `pyroscopegridding-0.3.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.3.1.3',      # Initial version
+    version = '0.3.1.4',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```


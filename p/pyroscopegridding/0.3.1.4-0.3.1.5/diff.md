# Comparing `tmp/pyroscopegridding-0.3.1.4.tar.gz` & `tmp/pyroscopegridding-0.3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegridding-0.3.1.4.tar", last modified: Thu May 11 03:18:16 2023, max compression
+gzip compressed data, was "pyroscopegridding-0.3.1.5.tar", last modified: Thu May 11 15:20:48 2023, max compression
```

## Comparing `pyroscopegridding-0.3.1.4.tar` & `pyroscopegridding-0.3.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 03:18:16.650489 pyroscopegridding-0.3.1.4/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-11 03:18:16.618710 pyroscopegridding-0.3.1.4/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.1.4/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 03:18:16.187854 pyroscopegridding-0.3.1.4/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-05-11 03:14:34.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9155 2023-05-10 21:45:39.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:02:30.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10684 2023-05-11 03:17:35.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.3.1.4/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 03:18:16.529155 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-11 03:18:15.000000 pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-11 03:18:16.652489 pyroscopegridding-0.3.1.4/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1779 2023-05-11 03:17:47.000000 pyroscopegridding-0.3.1.4/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 15:20:48.724166 pyroscopegridding-0.3.1.5/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-11 15:20:48.719099 pyroscopegridding-0.3.1.5/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.1.5/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 15:20:48.510441 pyroscopegridding-0.3.1.5/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     6854 2023-05-11 15:18:39.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    30799 2023-05-11 15:18:59.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10589 2023-05-11 15:19:08.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29412 2023-05-11 15:19:37.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9371 2023-05-11 04:06:02.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:02:30.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10684 2023-05-11 15:19:58.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5186 2023-05-11 03:51:02.000000 pyroscopegridding-0.3.1.5/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-11 15:20:48.685010 pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-11 15:20:47.000000 pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-11 15:20:47.000000 pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-11 15:20:47.000000 pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-11 15:20:47.000000 pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-11 15:20:47.000000 pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-11 15:20:47.000000 pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-11 15:20:48.726164 pyroscopegridding-0.3.1.5/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1779 2023-05-11 15:20:41.000000 pyroscopegridding-0.3.1.5/setup.py
```

### Comparing `pyroscopegridding-0.3.1.4/PKG-INFO` & `pyroscopegridding-0.3.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.1.4
+Version: 0.3.1.5
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.1.4/README.md` & `pyroscopegridding-0.3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/filter_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Luckily, the metadata and attributes of the netcdf4 variables gives us an idea of what we should be looking for through:
 # 
 # 1. valid_range
 # 2. units
 # 3. scale_factor
 
 #import sat_data_input
+#from sat_data_input import *
 from pyroscopegridding.sat_data_input import *
 
 import numpy as np
 
 # nc
 # given GeoID,PhyID (this is read in with open_file) and their corresponding var_lists (variables we care about)
 # output lat, lon, and variables we care about (filtered based on metadata)
@@ -82,21 +83,15 @@
                 m[key] = phy[key][p]
 
         metadata.append(m)
 
     # scale factors
     phy_vars = np.array(phy_vars) #* float(phy['scale_factor'][0]) + float(phy['add_offset'][0])
     #phy_vars = (np.array(phy_vars) - float(phy['add_offset'][0]) )/float(phy['scale_factor'][0])
-    for p in phy_vars:
-        pass
-        #print("FINAL MAXES NC:", p.max())
-    
-    #print("latitude:", len(lat))
-    #print("Physical:", len(phy_vars))
-    print("Metadata: ", metadata)
+
 
     # probably should put in a check that lat lon phys has same length
     # sometimes phys var may differ between aerosol optical depth and angle
     # ALL variables must pass the filter test otherwise get rid of them
 
     return lat,lon,phy_vars, metadata
 
@@ -148,17 +143,14 @@
         lat.append(lat1)
         lon1 = np.array(lon1) * float(geo['scale_factor'][1]) + float(geo['add_offset'][1])
         lon.append(lon1)
         #phy_vars1 = np.array(phy_vars1) * float(phy['scale_factor'][p]) + float(phy['add_offset'][p])
         #phy_vars1[phy_vars1 == 0] = 0.5
         phy_vars.append(phy_vars1)
 
-        #print("phyvars1: ", len(phy_vars1))
-        
-        #print(phy_vars1)
 
         # metadata attributes
         m = {}
         for key in phy:
             # conversion to appropriate values
             if key == "scale_factor" or key == "add_offset":
                 m[key] = float(phy[key][p])
@@ -167,91 +159,15 @@
                 m[key] = phy[key][p]
             
 
         metadata.append(m)
 
     # scale factors
     phy_vars = np.array(phy_vars) * float(phy['scale_factor'][0]) + float(phy['add_offset'][0])
-    for p in phy_vars:
-        pass
-        #print("FINAL MAXES HDF:", p.max())
-    #print("latitude:", len(lat))
-    #print("Physical:", len(phy_vars))
-    
+   
 
     # probably should put in a check that lat lon phys has same length
     # sometimes phys var may differ between aerosol optical depth and angle
     # ALL variables must pass the filter test otherwise get rid of them
 
     return lat,lon,phy_vars, metadata
 
-"""
-# given GeoID,PhyID (this is read in with open_file) and their corresponding var_lists (variables we care about)
-# output lat, lon, and variables we care about (filtered based on metadata)
-# lat lon are n size arrays containing lat, long variables for variable n
-# phy_vars is n size array containing netcdf4.variables
-def filter_data(GeoID,PhyID,geo_list,phy_list, phy_nc = None, phy_hdf=None):
-    if geo_list is None:
-       geo_list = ["latitude", "longitude"]
-    if phy_list is None:
-        phy_list = [] 
-    
-    #basic read in
-    geo = read_geo_data(GeoID, var_list=geo_list)
-    phy = read_phy_data(PhyID, GeoID, phy_list, phy_nc, phy_hdf)
-    lat = []
-    lon = []
-    phy_vars = []
-    metadata = []
-
-    for p in range(len(phy_list)):
-        lat1 = geo['data'][0][:,:]
-        lon1 = geo['data'][1][:,:]
-        phy_vars1 = phy['data'][p][:,:]
-        
-        #filter based on valid range
-        try: # check in the code
-            lat1 = lat1[np.logical_and(phy_vars1>=phy['valid_range'][p][0],phy_vars1<=phy['valid_range'][p][1])]
-            lon1 = lon1[np.logical_and(phy_vars1>=phy['valid_range'][p][0],phy_vars1<=phy['valid_range'][p][1])]
-        except:
-            #in this case, the phy_variable in question is not mapped to every lat,lon coordinate
-            #print("excepted")
-            #we try to map it to where data exists for lat and long
-            #lat1 = lat1[np.logical_not(np.isnan(phy_vars1))]
-            #lon1 = lon1[np.logical_not(np.isnan(phy_vars1))]
-            lat1=[]
-            lon1=[]
-            
-        #print("valid range: ", phy['valid_range'][p][0])
-        phy_vars1 = phy_vars1[np.logical_and(phy_vars1>=phy['valid_range'][p][0],phy_vars1<=phy['valid_range'][p][1])]
-        
-        lat1 = np.array(lat1) * float(geo['scale_factor'][0]) + float(geo['add_offset'][0])
-        lat.append(lat1)
-        lon1 = np.array(lon1) * float(geo['scale_factor'][1]) + float(geo['add_offset'][1])
-        lon.append(lon1)
-        #phy_vars1 = np.array(phy_vars1) * float(phy['scale_factor'][p]) + float(phy['add_offset'][p])
-        #phy_vars1[phy_vars1 == 0] = 0.5
-        phy_vars.append(phy_vars1)
-
-        #print("phyvars1: ", len(phy_vars1))
-        
-        #print(phy_vars1)
-
-        # metadata attributes
-        m = {}
-        for key in phy:
-            m[key] = phy[key][p]
-
-        metadata.append(m)
-
-    # scale factors
-    phy_vars = np.array(phy_vars) * float(phy['scale_factor'][0]) + float(phy['add_offset'][0])
-    #print("latitude:", len(lat))
-    #print("Physical:", len(phy_vars))
-    print("Metadata: ", metadata)
-
-    # probably should put in a check that lat lon phys has same length
-    # sometimes phys var may differ between aerosol optical depth and angle
-    # ALL variables must pass the filter test otherwise get rid of them
-
-    return lat,lon,phy_vars, metadata
-"""
```

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/grid_ncf.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 from http.client import MOVED_PERMANENTLY
 import netCDF4
 import numpy as np
 import numpy.ma as ma
 import time
 import os
 
+"""
+from gridding import *
+from sat_data_input import *
+from filter_data import *
+from naming_conventions import *
+from solar_zenith import *
+from fileparser import *
+"""
 from pyroscopegridding.gridding import *
 from pyroscopegridding.sat_data_input import *
 from pyroscopegridding.filter_data import *
 from pyroscopegridding.naming_conventions import *
 from pyroscopegridding.solar_zenith import *
 from pyroscopegridding.fileparser import *
 
@@ -384,29 +392,21 @@
                     if aod_stat== "Mean":
                         rotated = list(zip(*avgtau))[::-1] # check why zipped
                         #print("AFTER GRIDDING: ", rotated)
                         leogeo_stats_arr[p_vars] ["Mean"].append(np.flipud(rotated)) #for leogeo calculation later
                         
                         #sensor idx (Sensor Weighting)
                         temp_a = np.flipud(rotated)
-                        """
-                        print("\nBEFORE SENSOR IDX \n")
-                        print(temp_a)
-                        print("Fill Value: ", meta[j]["_FillValue"])"""
+                        
                         temp_a[temp_a > -9999] = 1
                         temp_a[temp_a <= meta[j]["_FillValue"]] = 0 #get rid of this 2/1
                         temp_a[np.isnan(temp_a)] = 0
                         #sensor_idx[get_sensor(s_name)] = temp_a
                         sensor_idx_arr[p_vars][get_sensor(s_name)] = temp_a
-                        """
-                        print("\nSENSOR IDX\n")
-                        print(sensor_idx[get_sensor(s_name)])
-                        print("\n")
-                        """
-                    
+                                           
                          
                     elif aod_stat == "STD":
                         rotated = list(zip(*stdtau))[::-1]
                         
                         leogeo_stats_arr[p_vars]["STD"].append(np.flipud(rotated))
                         #print("AOD STD", rotated)
                         
@@ -612,64 +612,14 @@
             #number_of_sensors_variable[leogeo_index].scale_factor = float(1/6)
             
             leogeo_index+=1    
         j += 1
         leogeo_meta_index += 1
     
     
-    """
-    # put in gridded statistics
-    # avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau = grid(limit,float(gsize),indata_stat,inlat_stat,inlon_stat)
-    sensor_id = []
-    shape = (len(np.arange(0,lat_dim)*gsize+minlat), len(np.arange(0,lon_dim)*gsize+minlon))
-    avg = []
-    # all sensors combined statistics (LEOGEO)
-    for k, p_vars in enumerate(phy_list):
-        # averages
-        try:
-            avgtau = np.nanmean(np.array(sensors.get(p_vars)), axis=0 )
-            # other statistics nan
-            # Number of Sensors
-            sensor_id_x = np.zeros(shape)
-            for i in range(len(sensors[p_vars])):
-                sensor_id_x = sensor_id_x + (np.array(sensors.get(p_vars)[i])*0+1)
-                #print(np.nan_to_num(np.array(sensors.get(p_vars)[i])*0+1, -1))
-            avg_name = str("merge_avgtau_" + p_vars)
-            avg.append(ds.createVariable(avg_name, 'f4', ('time', 'lat', 'lon', )))
-            avg[k][0, :, :] = avgtau
-            # metadata
-            # naming convention, units should be consistent
-            # read from configuration file
-            # follow netcdf conventions
-            # avg[k].units = meta["units"]
-            # avg[k].valid_range = meta["valid_range"]
-            # avg[k]._FillValue = meta["_FillValue"]
-            # avg[k].long_name = meta["long_name"]
-            # avg[k].scale_factor = meta["scale_factor"]
-            # avg[k].add_offset = meta["add_offset"]
-            # avg[k].Parameter_Type = meta["Parameter_Type"]
-            sensor_id_name = str("sensor_id_x_" + p_vars)
-            sensor_id.append(ds.createVariable(sensor_id_name, 'f4', ('time', 'lat', 'lon', )))
-            sensor_id[k].units = 'unknown'
-            sensor_id[k][0, :, :] = sensor_id_x
-        except:
-            #print("There are: ", len(sensors.get(p_vars)), " sensors for the var")
-            print(p_vars)
-            print(sensors.get(p_vars))
-    """
-
-    # print modis mean again
-    #print(values)
-    #print(values[0])
-    #print(values[0].long_name)
-    #close file
-    #ds.close()
-    #grid_close(ds)s
-    
-    
     return ds
     # output = 1 netcdf with six variables (one for each sensor) 
     # merge = run two loops (lat lon) (xdim, ydim from grid) 
     # merge aod equal to average of six sensors making sure no nan
     # identify which sensors are availabe - sensor ID variable 0 or 1 (unavailable vs available)
     # byte type array, keep n-dimensional for now
     # minimum number of things to merge: in the future
```

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/gridding.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/gridding.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 import numpy as np
 import numpy.ma as ma
 from numba import cuda
 import math
 
 #import sat_data_input
 #import filter_data
+#from sat_data_input import *
+#from filter_data import *
 from pyroscopegridding.sat_data_input import *
 from pyroscopegridding.filter_data import *
 
 # limit - [lat1,lat2,lon1,lon2]
 # gsize - pixel size
 # indata - inputs
 # inlat - list of latitudes we map for
```

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/gtools.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/gtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,37 @@
 __status__ = "Production"
 # Gtools
 #
 # the control for the file. It parses command line arguments and calls to grid_ncf
 #
 
 #import other module files
+
 from concurrent.futures import process
 from pyroscopegridding.filter_data import *
 from pyroscopegridding.fileparser import *
 from pyroscopegridding.sat_data_input import *
 from pyroscopegridding.gridding import *
 from pyroscopegridding.grid_ncf import *
 from pyroscopegridding.time_conv import *
+
 #import sat_data_input
 #import filter_data
 #import gridding
 #import grid_ncf
 #import fileparser # comment for specific file functions
 #import time_conv
-
+"""
+from filter_data import *
+from fileparser import *
+from sat_data_input import *
+from gridding import *
+from grid_ncf import *
+from time_conv import *
+"""
 import os
 import argparse
 import numpy as np
 import datetime
 import time
 """
 # python3 gtools.py -r -fn "C:/Users/swzhao/Desktop/Old Code and Satellite Inputs/Satellite Sensor Data/AERDT_L2_VIIRS_SNPP.A2021008.2018.001.2021009072852.nc" -gl "latitude longitude" -gp "Optical_Depth_Land_And_Ocean"
@@ -423,14 +432,15 @@
         
         ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
+    print("CFGTIME")
 
 def netCDF_yaml_config_array(file_name):
         
     grid_settings = file_name[0]
     variables =file_name[1]
     file_io = file_name[2]
```

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/naming_conventions.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,16 +129,18 @@
         lat_width = len(data[0])
         lon_width = len(data[0][0])
         data = data.flatten()
         
         data[data<=-9999.] = np.nan
         data = data.reshape(num_sensors, lat_width, lon_width)
         """
+        print("ENTERED MEAN CALCULATION")
         
         data = np.array(data)
+        print(data.shape)
         data[data<=-9999.] = np.nan # fill_value
         
         avgtau = np.nanmean(data, axis=0 ) # [ [avgtau for modis a], [avgtau .. ]  ]
         avgtau = np.nan_to_num(avgtau, nan=-9999) # fill_value
         #print(avgtau.flatten())
         #print("ORIGINAL DATA2:", data)
         
@@ -165,18 +167,24 @@
         numerator_sum = (count - 1) * variances + count * (mean - y_bar)**2
         numerator = np.sum(numerator_sum, axis = 0)
         
         denominator = total_count - 1
         denominator[denominator == 0] = None
         
         return np.sqrt(numerator / denominator)
-        """
+        """        
+        
         data = np.array(data)
         data[data<=-9999.] = np.nan
-        data[data==0] = np.nan
+        #data[data==0] = np.nan
+        
+        #test
+        print(data)
+        print("MEANS: ", data.shape)
+        print("ENTERED STD CALCULATIONS")
         
         stdtau = np.nanstd(data, axis = 0)
         
         return stdtau
         
     
     if statistic == "TotalPixels":
```

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.3.1.5/pyroscopegridding/time_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 #
 
 # due to the introduction of the time variable, we need to know the time of the sensor data
 # this information is not given in the file itself, but rather the file name
 # e.g. "AERDT_L2_ABI_G16.A2021008.0850.001.nc" --> 10/08/2021 8:50 AM
 import datetime
 
-from pyroscopegridding.fileparser import *
+from fileparser import *
+#from pyroscopegridding.fileparser import *
 
 full_satellite_list = ['ABI_G16', 'ABI_G17', 'AHI_H08', 'VIIRS_SNPP', 'MOD04', 'MODIS_T', 'MODIS_A', 'MYD04']
 
 # given 'yyyy/mm/dd/hr/mm' string
 # converts to datetime object
 def to_datetime(date_string):
     format = '%Y/%m/%d/%H/%M'
```

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.1.4
+Version: 0.3.1.5
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.1.4/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.3.1.5/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.4/setup.py` & `pyroscopegridding-0.3.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.3.1.4',      # Initial version
+    version = '0.3.1.5',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```


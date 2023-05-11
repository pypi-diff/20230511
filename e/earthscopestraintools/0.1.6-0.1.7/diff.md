# Comparing `tmp/earthscopestraintools-0.1.6.tar.gz` & `tmp/earthscopestraintools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthscopestraintools-0.1.6.tar", last modified: Thu Apr 27 18:35:12 2023, max compression
+gzip compressed data, was "earthscopestraintools-0.1.7.tar", last modified: Thu May 11 14:03:18 2023, max compression
```

## Comparing `earthscopestraintools-0.1.6.tar` & `earthscopestraintools-0.1.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:35:12.516366 earthscopestraintools-0.1.6/
--rw-r--r--   0 gottlieb   (501) staff       (20)     1042 2023-02-21 23:33:21.000000 earthscopestraintools-0.1.6/LICENSE
--rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-04-27 18:35:12.516049 earthscopestraintools-0.1.6/PKG-INFO
--rw-r--r--   0 gottlieb   (501) staff       (20)     1505 2023-03-07 14:24:27.000000 earthscopestraintools-0.1.6/README.md
--rw-r--r--   0 gottlieb   (501) staff       (20)      955 2023-04-27 18:34:52.000000 earthscopestraintools-0.1.6/pyproject.toml
--rw-r--r--   0 gottlieb   (501) staff       (20)       38 2023-04-27 18:35:12.516455 earthscopestraintools-0.1.6/setup.cfg
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:35:12.481398 earthscopestraintools-0.1.6/src/
--rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.6/src/__init__.py
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:35:12.496330 earthscopestraintools-0.1.6/src/earthscopestraintools/
--rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/__init__.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     6920 2023-03-27 21:01:53.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/ascii2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    10688 2023-02-08 22:58:57.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/bottle.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1563 2023-03-07 13:59:16.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/bottle2mseed.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     5141 2023-03-27 21:06:16.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/bottle2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     6350 2023-03-07 14:19:55.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/bottletar.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     7409 2023-03-27 17:52:37.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/edid.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1591 2023-03-27 17:31:01.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/event.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     8507 2023-03-27 17:34:50.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/event_processing.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4929 2021-03-10 22:31:02.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/event_site_terms.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)    18373 2023-03-30 14:01:59.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/gtsm_metadata.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4353 2023-03-27 19:10:40.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/mseed_tools.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     9700 2023-03-30 16:58:05.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/processing.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4346 2023-03-07 12:51:32.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/tdb2ascii.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     2063 2023-03-07 12:53:14.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/tdb2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    29839 2023-04-27 18:33:05.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/tiledbtools.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    25726 2023-04-04 14:51:28.000000 earthscopestraintools-0.1.6/src/earthscopestraintools/timeseries.py
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:35:12.506409 earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/
--rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-04-27 18:35:12.000000 earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/PKG-INFO
--rw-r--r--   0 gottlieb   (501) staff       (20)     1174 2023-04-27 18:35:12.000000 earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/SOURCES.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)        1 2023-04-27 18:35:12.000000 earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/dependency_links.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)      120 2023-04-27 18:35:12.000000 earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/requires.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)       22 2023-04-27 18:35:12.000000 earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/top_level.txt
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-04-27 18:35:12.515569 earthscopestraintools-0.1.6/test/
--rw-r--r--   0 gottlieb   (501) staff       (20)      240 2023-03-29 13:58:10.000000 earthscopestraintools-0.1.6/test/test_ascii2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1295 2023-03-07 13:56:58.000000 earthscopestraintools-0.1.6/test/test_bottle2mseed.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     2533 2023-03-07 19:39:09.000000 earthscopestraintools-0.1.6/test/test_bottle2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1336 2023-03-07 14:11:58.000000 earthscopestraintools-0.1.6/test/test_bottletar.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1044 2023-03-27 18:40:20.000000 earthscopestraintools-0.1.6/test/test_edid.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      373 2023-03-13 12:24:04.000000 earthscopestraintools-0.1.6/test/test_gtsm_metadata.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      470 2023-03-06 23:40:58.000000 earthscopestraintools-0.1.6/test/test_tdb2ascii.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      277 2023-03-07 00:03:02.000000 earthscopestraintools-0.1.6/test/test_tdb2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1818 2023-03-27 22:45:21.000000 earthscopestraintools-0.1.6/test/test_ts2tdb.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.290856 earthscopestraintools-0.1.7/
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1042 2023-02-21 23:33:21.000000 earthscopestraintools-0.1.7/LICENSE
+-rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-05-11 14:03:18.290442 earthscopestraintools-0.1.7/PKG-INFO
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1505 2023-03-07 14:24:27.000000 earthscopestraintools-0.1.7/README.md
+-rw-r--r--   0 gottlieb   (501) staff       (20)      955 2023-05-01 19:26:39.000000 earthscopestraintools-0.1.7/pyproject.toml
+-rw-r--r--   0 gottlieb   (501) staff       (20)       38 2023-05-11 14:03:18.290957 earthscopestraintools-0.1.7/setup.cfg
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.171108 earthscopestraintools-0.1.7/src/
+-rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.7/src/__init__.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.179001 earthscopestraintools-0.1.7/src/earthscopestraintools/
+-rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/__init__.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     7265 2023-05-04 18:11:43.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/ascii2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    10688 2023-02-08 22:58:57.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottle.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1563 2023-03-07 13:59:16.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2mseed.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     6288 2023-05-11 14:00:15.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     6350 2023-03-07 14:19:55.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottletar.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     7409 2023-03-27 17:52:37.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/edid.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1591 2023-03-27 17:31:01.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/event.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     8507 2023-03-27 17:34:50.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/event_processing.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4929 2021-03-10 22:31:02.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/event_site_terms.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)    18330 2023-05-01 20:18:57.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/gtsm_metadata.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4373 2023-05-02 17:31:35.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/mseed_tools.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    10076 2023-05-01 20:13:12.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/processing.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4346 2023-03-07 12:51:32.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2ascii.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     2725 2023-05-04 20:36:52.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    32284 2023-05-04 19:05:01.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/tiledbtools.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    25945 2023-05-02 17:52:53.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/timeseries.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.193256 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/
+-rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/PKG-INFO
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1174 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/SOURCES.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)        1 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/dependency_links.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)      120 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/requires.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)       22 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/top_level.txt
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.289809 earthscopestraintools-0.1.7/test/
+-rw-r--r--   0 gottlieb   (501) staff       (20)      240 2023-03-29 13:58:10.000000 earthscopestraintools-0.1.7/test/test_ascii2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1295 2023-03-07 13:56:58.000000 earthscopestraintools-0.1.7/test/test_bottle2mseed.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     2497 2023-05-04 17:47:25.000000 earthscopestraintools-0.1.7/test/test_bottle2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1336 2023-03-07 14:11:58.000000 earthscopestraintools-0.1.7/test/test_bottletar.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1044 2023-03-27 18:40:20.000000 earthscopestraintools-0.1.7/test/test_edid.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      373 2023-05-01 20:05:48.000000 earthscopestraintools-0.1.7/test/test_gtsm_metadata.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      470 2023-03-06 23:40:58.000000 earthscopestraintools-0.1.7/test/test_tdb2ascii.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      351 2023-05-04 18:34:51.000000 earthscopestraintools-0.1.7/test/test_tdb2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1818 2023-03-27 22:45:21.000000 earthscopestraintools-0.1.7/test/test_ts2tdb.py
```

### Comparing `earthscopestraintools-0.1.6/LICENSE` & `earthscopestraintools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/PKG-INFO` & `earthscopestraintools-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthscopestraintools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of utilities for working with EarthScope strainmeter data
 Author-email: Mike Gottlieb <mike.gottlieb@eartscope.org>
 License: Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `earthscopestraintools-0.1.6/README.md` & `earthscopestraintools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/pyproject.toml` & `earthscopestraintools-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "earthscopestraintools"
-version ="0.1.6"
+version ="0.1.7"
 authors = [
   { name="Mike Gottlieb", email="mike.gottlieb@eartscope.org" },
 ]
 description = "A collection of utilities for working with EarthScope strainmeter data"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/ascii2tdb.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/ascii2tdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,30 +140,32 @@
         tmp_df["quality"] = " "
         tmp_df = tmp_df[cols]
         logger.info(f"{timeseries}: {len(tmp_df)} samples")
         writer.write_df_to_tiledb(tmp_df)
 
 
 def etl_yearly_ascii_file(
-    network, fcid, year, delete_array=False, workdir="", print_it=False
+    network, station, year, delete_array=False, workdir="", print_it=False
 ):
-    edid = get_station_edid(fcid)
     os.makedirs(workdir, exist_ok=True)
-    uri = f"{workdir}/{edid}_level2.tdb"
+    # edid = get_station_edid(station)
+    # uri = f"{workdir}/{edid}_level2.tdb"
+    uri = f"{workdir}/{network}_{station}_l2_etl.tdb"
     logger.info(f"Array uri: {uri}")
     writer = ProcessedStrainWriter(uri)
     if delete_array:
         writer.array.delete()
 
     # create new array if needed.  note: array_exists only works locally not in s3.
     if not tiledb.array_exists(writer.array.uri):
         writer.array.create(schema_type="3d", schema_source="s3")
+        writer.array.set_array_meta(network=network, station=station, period=300)
 
-    filebase = fcid + "." + year + ".bsm.level2"
-    url = "http://bsm.unavco.org/bsm/level2/" + fcid + "/" + filebase + ".tar"
+    filebase = station + "." + year + ".bsm.level2"
+    url = "http://bsm.unavco.org/bsm/level2/" + station + "/" + filebase + ".tar"
     response = requests.get(url, stream=True)
     print(url)
     tar = tarfile.open(fileobj=BytesIO(response.raw.read()), mode="r")
     tar.extractall()
     files = os.listdir(filebase)
     for file in files:
         logger.info(file)
@@ -174,14 +176,17 @@
     writer.array.vacuum_array_meta()
     writer.array.consolidate_fragment_meta()
     writer.array.vacuum_fragment_meta()
     writer.array.consolidate_fragments()
     writer.array.vacuum_fragments()
     if print_it:
         reader = ProcessedStrainReader(uri)
+        logger.info(f"Network: {reader.array.get_network()}")
+        logger.info(f"Station: {reader.array.get_station()}")
+        logger.info(f"Period: {reader.array.get_period()}")
         start_str = f"{year}-01-01T00:00:00"
         end_str = f"{int(year)+1}-01-01T00:00:00"
         df = reader.to_df(
             data_types=["CH0", "CH1", "CH2", "CH3", "Eee+Enn", "Eee-Enn", "2Ene"],
             timeseries="microstrain",
             attrs="data",
             start_str=start_str,
@@ -189,16 +194,16 @@
         )
         logger.info(f"\n{df}")
 
 
 # if __name__ == "__main__":
 #     workdir = "arrays"
 #     network = sys.argv[1]
-#     fcid = sys.argv[2]
+#     station = sys.argv[2]
 #     year = sys.argv[3]
-#     etl_yearly_ascii_file(network, fcid, year, workdir=workdir)
+#     etl_yearly_ascii_file(network, station, year, workdir=workdir)
 # years = ["2005","2006","2007","2008","2009",
 #          "2010","2011","2012","2013","2014","2015","2016","2017","2018","2019",
 #          "2020","2021","2022"]
 # for year in years:
-#     etl_yearly_ascii_file(network, fcid, year)
+#     etl_yearly_ascii_file(network, station, year)
 #
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/bottle.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/bottle.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/bottle2mseed.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2mseed.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/bottle2tdb.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2tdb.py`

 * *Files 15% similar despite different names*

```diff
@@ -72,18 +72,19 @@
             bottle_df = pd.DataFrame(data=d)
             bottle_dfs.append(bottle_df)
     tiledb_buffer = pd.concat(bottle_dfs, axis=0).reset_index(drop=True)
     tiledb_buffer["data"] = tiledb_buffer["data"].astype(np.float64)
     return tiledb_buffer
 
 
-def write_buffer(uri, buffer: pd.DataFrame):
+def write_buffer(uri, buffer: pd.DataFrame, cleanup_meta=True):
     writer = RawStrainWriter(uri)
     writer.write_df_to_tiledb(buffer)
-    writer.array.cleanup_meta()
+    if cleanup_meta:
+        writer.array.cleanup_meta()
 
 
 def check_result(buffer, uri):
     try:
         start = int(buffer.time.iloc[0])
         end = int(buffer.time.iloc[-1])
         channels = list(buffer["channel"].unique())
@@ -114,31 +115,53 @@
         try:
             logger.info(f"{filepath}: Writing to {strain_uri}")
             write_buffer(strain_uri, strain_buffer)
         except tiledb.TileDBError as e:
             logger.error(e)
             array = StrainArray(uri=strain_uri)
             array.create(schema_type="2D_INT", schema_source="s3")
+            if session.casefold() == "Min".casefold():
+                period = 0.05
+            elif session.casefold() == "Hour".casefold():
+                period = 1
+            elif session.casefold() == "Day".casefold():
+                period = 600
+            else:
+                logger.error(
+                    f"Invalid session {session}, cannot determine period for array metadata"
+                )
+            array.set_array_meta(
+                station=gbt.file_metadata["fcid"], period=period
+            )  # todo: set network meta?
             logger.info(f"{filepath}: Writing to {strain_uri}")
             write_buffer(strain_uri, strain_buffer)
 
         if session.casefold() == "Day".casefold():
             try:
                 logger.info(f"{filepath}: Writing to {ancillary_uri}")
                 write_buffer(ancillary_uri, ancillary_buffer)
             except tiledb.TileDBError as e:
                 logger.error(e)
-                array = StrainArray(uri=ancillary_uri)
-                array.create(schema_type="2D_FLOAT", schema_source="s3")
+                ancillary_array = StrainArray(uri=ancillary_uri)
+                ancillary_array.create(schema_type="2D_FLOAT", schema_source="s3")
+                ancillary_array.set_array_meta(
+                    station=gbt.file_metadata["fcid"], period=1800
+                )  # todo: set network meta?
                 logger.info(f"{filepath}: Writing to {ancillary_uri}")
                 write_buffer(ancillary_uri, ancillary_buffer)
 
     if print_it:
         logger.info(f"Strain Buffer:\n{strain_buffer}")
         if session.casefold() == "Day".casefold():
             logger.info(f"Ancillary Buffer:\n{ancillary_buffer}")
 
     if check_it:
         logger.info(f"Reading data back from array")
+        logger.info(f"Network: {array.get_network()}")
+        logger.info(f"Station: {array.get_station()}")
+        logger.info(f"Period: {array.get_period()}")
         check_result(strain_buffer, strain_uri)
         if session.casefold() == "Day".casefold():
+            logger.info(f"Network: {ancillary_array.get_network()}")
+            logger.info(f"Station: {ancillary_array.get_station()}")
+            logger.info(f"Period: {ancillary_array.get_period()}")
             check_result(ancillary_buffer, ancillary_uri)
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/bottletar.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/bottletar.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/edid.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/edid.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/event.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/event.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/event_processing.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/event_processing.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/event_site_terms.txt` & `earthscopestraintools-0.1.7/src/earthscopestraintools/event_site_terms.txt`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/gtsm_metadata.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/gtsm_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
         self.orientation = self.get_orientation()
         self.reference_strains = self.get_reference_strains()
         self.start_date = self.get_start_date()
         matrices = {}
         if not gauge_weights:
             self.gauge_weights = [1, 1, 1, 1]
         # matrices['weighted_strain_matrix'] = self.make_weighted_strain_matrix(gauge_weights=gauge_weights)
-        matrices["lab_strain_matrix"] = self.get_lab_strain_matrix()
-        matrices["er2010_strain_matrix"] = self.get_er2010_strain_matrix()
-        matrices["ch_prelim_strain_matrix"] = self.get_ch_prelim_strain_matrix()
-        self.strain_matrices = {k: v for k, v in matrices.items() if v is not None}
+        matrices["lab"] = self.get_lab_strain_matrix()
+        matrices["ER2010"] = self.get_er2010_strain_matrix()
+        matrices["CH_prelim"] = self.get_ch_prelim_strain_matrix()
+        self.strain_matrices = {k: v for k, v in matrices.items()}
         self.atmp_response = self.get_atmp_response()
         self.tidal_params = self.get_tidal_params()
 
     #        self.xml = self.get_xml()
     #        self.detrend = self.get_detrend_xml()
 
     # def get_xml(self):
@@ -217,14 +217,15 @@
                         [
                             lines[i + 3].decode("utf-8").rstrip().split()[1:],
                             lines[i + 4].decode("utf-8").rstrip().split()[1:],
                             lines[i + 5].decode("utf-8").rstrip().split()[1:],
                         ]
                     )
                     return er2010.astype(float)
+            return None
         except Exception as e:
             logger.error("Could not load ER2010 strain matrix")
             return None
 
     def get_ch_prelim_strain_matrix(self):
         url = f"http://bsm.unavco.org/bsm/level2/{self.fcid}/{self.fcid}.README.txt"
         try:
@@ -237,15 +238,15 @@
                         [
                             lines[i + 3].decode("utf-8").rstrip().split()[1:],
                             lines[i + 4].decode("utf-8").rstrip().split()[1:],
                             lines[i + 5].decode("utf-8").rstrip().split()[1:],
                         ]
                     )
                     return ch_prelim.astype(float)
-            return np.array([])
+            return None
         except Exception as e:
             logger.exception("Could not load ch_prelim strain matrix")
             return None
 
     def get_reference_strains(self):
         reference_strains = {}
         reference_strains["linear_date"] = self.meta_df.loc[self.fcid]["L_DATE"]
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/mseed_tools.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/mseed_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,17 @@
 
     :param loc: FDSN Location code, accepts wildcards
     :param cha: FDSN Channel code, accepts wildcards
     :param start:
     :param end:
     :return:
     """
-    logger.info(f"Loading {loc} {cha} from {start} to {end} from IRIS DMC miniseed")
+    logger.info(
+        f"Loading {loc} {cha} from {start} to {end} from Earthscope DMC miniseed"
+    )
     url = (
         f"https://service.iris.edu/fdsnws/dataselect/1/query?net={net}"
         f"&sta={sta}&loc={loc}&cha={cha}&starttime={start}&endtime={end}"
         f"&format=miniseed&nodata=404"
     )
     if print_url:
         logger.info(f"Reading from {url}")
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/processing.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,33 @@
         * (gap / 0.087)
         * 1000000
     )
     return linearized_data
 
 
 def apply_calibration_matrix(
-    df: pd.DataFrame, calibration_matrix: np.array, use_channels: list
+    df: pd.DataFrame,
+    calibration_matrix: np.array,
+    calibration_matrix_name: str = None,
+    use_channels: list = [1, 1, 1, 1],
 ):
     # todo: implement use channels
-    logger.info(f"Applying matrix: {calibration_matrix}")
+    logger.info(f"Applying {calibration_matrix_name} matrix: {calibration_matrix}")
+    areal = "Eee+Enn"
+    differential = "Eee-Enn"
+    shear = "2Ene"
+    if calibration_matrix_name and calibration_matrix_name != "lab":
+        areal += "." + calibration_matrix_name
+        differential += "." + calibration_matrix_name
+        shear += "." + calibration_matrix_name
     regional_strain_df = np.matmul(
         calibration_matrix, df[df.columns].transpose()
     ).transpose()
     regional_strain_df = regional_strain_df.rename(
-        columns={0: "Eee+Enn", 1: "Eee-Enn", 2: "2Ene"}
+        columns={0: areal, 1: differential, 2: shear}
     )
     return regional_strain_df
 
 
 def butterworth_filter(
     df: pd.DataFrame,
     period: float,
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/tdb2ascii.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2ascii.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/tdb2tdb.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2tdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 # write tarred tiledb arrays from tiledb arrays
 # slice by start and end time
 # use in lambda with web service to deliver data in tiledb
+# only works for processed strain data currently
 
-import tiledb
 import numpy as np
-import pandas as pd
-
-# import datetime
-# import sys, os
-import shutil
-import json
-
-# from straintiledbarray import StrainTiledbArray
-
-from earthscopestraintools.edid import get_station_edid
 from earthscopestraintools.tiledbtools import (
     ProcessedStrainReader,
     ProcessedStrainWriter,
 )
 
 import logging
 
@@ -32,17 +22,15 @@
 #
 # def to_date(datetime64):
 #     ts = pd.to_datetime(str(datetime64))
 #     d = ts.strftime("%Y%m%d")
 #     return d
 
 
-def read_date_range(network, station, start_str, end_str):
-    edid = get_station_edid(network, station)
-    uri = f"{workdir}/{edid}_level2.tdb"
+def read_date_range(uri, start_str, end_str):
     logger.info(f"Array uri: {uri}")
     reader = ProcessedStrainReader(uri)
     data_types = reader.array.get_data_types()
     timeseries = reader.array.get_timeseries()
     attrs = ["data", "quality", "level", "version"]
     df = reader.to_df(
         data_types=data_types,
@@ -53,26 +41,51 @@
         reindex=False,
     )
     return df
 
 
 def convert_time_to_unix_ms(df):
     df = df.reset_index()
-    df["time"] = df["time"].astype(int) / 10 ** 6
+    df["time"] = df["time"].astype(int) / 10**6
     df["time"] = df["time"].astype(np.int64)
     return df
 
 
 def export_date_range(
-    network, station, start_str, end_str, write_it=True, print_it=False
+    uri, start_str, end_str, save_as=None, write_it=True, print_it=False
 ):
-    df = read_date_range(network, station, start_str, end_str)
+    reader = ProcessedStrainReader(uri=uri)
+    network = reader.array.get_network()
+    station = reader.array.get_station()
+    period = reader.array.get_period()
+
+    df = read_date_range(uri, start_str, end_str)
     df = convert_time_to_unix_ms(df)
-    if print_it:
-        logger.info(f"\n{df}")
 
     if write_it:
-        uri = f"{workdir}/{network}_{station}_level2_{start_str}_{end_str}.tdb"
-        writer = ProcessedStrainWriter(uri=uri)
+        if save_as:
+            uri2 = save_as
+        else:
+            uri2 = f"{workdir}/{network}_{station}_level2_{start_str}_{end_str}.tdb"
+        writer = ProcessedStrainWriter(uri=uri2)
         writer.array.delete()
         writer.array.create(schema_type="3D", schema_source="s3")
+        writer.array.set_array_meta(network=network, station=station, period=period)
         writer.write_df_to_tiledb(df)
+
+    if print_it:
+        reader = ProcessedStrainReader(uri=uri2)
+        logger.info(f"Network: {reader.array.get_network()}")
+        logger.info(f"Station: {reader.array.get_station()}")
+        logger.info(f"Period: {reader.array.get_period()}")
+        data_types = reader.array.get_data_types()
+        timeseries = reader.array.get_timeseries()
+        attrs = ["data", "quality", "level", "version"]
+        df = reader.to_df(
+            data_types=data_types,
+            timeseries=timeseries,
+            attrs=attrs,
+            start_str=start_str,
+            end_str=end_str,
+            reindex=False,
+        )
+        logger.info(f"\n{df}")
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/tiledbtools.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/tiledbtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,14 +161,56 @@
 
         try:
             tiledb.Array.create(self.uri, self.schema, ctx=self.ctx)
             logger.info(f"Created array at {self.uri}")
         except tiledb.TileDBError as e:
             logger.warning(e)
 
+    def set_array_meta(
+        self,
+        network: str = None,
+        station: str = None,
+        period: float = None,
+    ):
+        # don't overwrite existing metadata
+        with tiledb.open(self.uri, "r", ctx=self.ctx) as A:
+            keys = A.meta.keys()
+            if "network" not in keys:
+                if network:
+                    logger.info(f"Setting array metadata network={network}")
+                    with tiledb.open(self.uri, "w", ctx=self.ctx) as B:
+                        B.meta["network"] = network
+            if "station" not in keys:
+                if station:
+                    logger.info(f"Setting array metadata station={station}")
+                    with tiledb.open(self.uri, "w", ctx=self.ctx) as B:
+                        B.meta["station"] = station
+            if "period" not in keys:
+                if period:
+                    logger.info(f"Setting array metadata period={period}")
+                    with tiledb.open(self.uri, "w", ctx=self.ctx) as B:
+                        B.meta["period"] = period
+
+    def update_array_meta(
+        self,
+        network: str = None,
+        station: str = None,
+        period: float = None,
+    ):
+        # overwrite existing metadata
+        if network:
+            with tiledb.open(self.uri, "w", ctx=self.ctx) as A:
+                A.meta["network"] = network
+        if station:
+            with tiledb.open(self.uri, "w", ctx=self.ctx) as A:
+                A.meta["station"] = station
+        if period:
+            with tiledb.open(self.uri, "w", ctx=self.ctx) as A:
+                A.meta["period"] = period
+
     def delete(self):
         try:
             tiledb.remove(self.uri, ctx=self.ctx)
             print("Deleted ", self.uri)
         except tiledb.TileDBError as e:
             print(e)
 
@@ -248,14 +290,35 @@
         with tiledb.open(self.uri, "r", ctx=self.ctx) as A:
             return json.loads(A.meta["dimensions"])["timeseries"]
 
     def get_channels(self):
         with tiledb.open(self.uri, "r", ctx=self.ctx) as A:
             return json.loads(A.meta["channels"])["channels"]
 
+    def get_network(self):
+        with tiledb.open(self.uri, "r", ctx=self.ctx) as A:
+            try:
+                return A.meta["network"]
+            except KeyError:
+                return None
+
+    def get_station(self):
+        with tiledb.open(self.uri, "r", ctx=self.ctx) as A:
+            try:
+                return A.meta["station"]
+            except KeyError:
+                return None
+
+    def get_period(self):
+        with tiledb.open(self.uri, "r", ctx=self.ctx) as A:
+            try:
+                return A.meta["period"]
+            except KeyError:
+                return None
+
     def print_schema(self):
         with tiledb.open(self.uri, "r", ctx=self.ctx) as A:
             print(A.schema)
 
 
 class ProcessedStrainReader:
     def __init__(self, uri: str, period=300):
@@ -339,15 +402,17 @@
                 df2 = df_data_type
             else:
                 df2 = pd.concat([df2, df_data_type], axis=1)
         return df2
 
     def check_query_result(self, epochs, start, end):
         if self.array.period is not None:
-            expected_epochs = int((end - start) / 1000 / self.array.period)
+            expected_epochs = (
+                int((end - start) / 1000 / self.array.period) + 1
+            )  # inclusive of last epoch
             if epochs >= expected_epochs:
                 logger.info(
                     f"Query complete, expected {expected_epochs} epochs and returned {epochs}"
                 )
             else:
                 logger.info(
                     f"Query incomplete, expected {expected_epochs} epochs and returned {epochs}"
@@ -429,21 +494,23 @@
         else:
             logger.info(f"Array exists at {self.array.uri}")
 
     def write_df_to_tiledb(self, df: pd.DataFrame):
         mode = "append"
         # make sure there aren't any nans, replace with 999999 if so
         df = df.replace(np.nan, 999999)
+        logger.debug("writing buffer")
         tiledb.from_pandas(
             uri=self.array.uri,
             dataframe=df,
             index_dims=["data_type", "timeseries", "time"],
             mode=mode,
             ctx=self.array.ctx,
         )
+        logger.debug("buffer written")
         # update the string dimension metadata
         data_type = df["data_type"].unique()
         timeseries = df["timeseries"].unique()
         if type(data_type) == str:
             data_type = [data_type]
         if type(timeseries) == str:
             timeseries = [timeseries]
@@ -481,14 +548,15 @@
         uri - string. which tiledb array to write to
         data_types - list of strings. data_types to map columns into.  ie CH0, 2Ene, pressure, time_index
         timeseries - string. name of timeseries.  counts, microstrain, offset_c, tide_c, atmp_c, atmp, pore, mjd, doy
         level - 2char string.  '0a', '1a', '2a', '2b'
         quality_df- dataframe, optional.  if not included, quality flags will be set to 'g'
         print_it - bool, optional.  show the constructed dataframe as it is being written to tiledb.
         """
+        logger.debug("creating buffer")
         df_buffer = pd.DataFrame(
             columns=[
                 "data_type",
                 "timeseries",
                 "time",
                 "data",
                 "level",
@@ -619,15 +687,17 @@
                 df2 = df_channel
             else:
                 df2 = pd.concat([df2, df_channel], axis=1)
         return df2
 
     def check_query_result(self, df, start, end):
         if self.array.period is not None:
-            expected_samples = int((end - start) / 1000 / self.array.period)
+            expected_samples = (
+                int((end - start) / 1000 / self.array.period) + 1
+            )  # inclusive of last epoch
             # expected_samples = int((str_to_unix_ms(end) - str_to_unix_ms(start)) / 1000 / self.array.period)
             # print("expected samples:", expected_samples)
             if len(df) >= expected_samples:
                 logger.info(
                     f"Query complete, expected {expected_samples} and returned {len(df)}"
                 )
             else:
@@ -759,17 +829,14 @@
             print_it=False,
         )
         logger.info(f"Wrote {ts.columns} to {self.array.uri}")
         if cleanup:
             self.array.cleanup()
 
 
-# def ts_from_tiledb_raw(
-
-
 # def ts_from_tiledb_processed(
 #     network: str,
 #     station: str,
 #     channels: list,
 #     series: str,
 #     units: str = "",
 #     period: int = 300,
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools/timeseries.py` & `earthscopestraintools-0.1.7/src/earthscopestraintools/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
     def remove_999999s(
         self,
         interpolate: bool = False,
         method: str = "linear",
         limit_direction: str = "both",
         limit: any = None,
     ):
+        logger.info("  Converting 999999 values to nan")
         if interpolate:
             df = self.data.replace(999999, np.nan).interpolate(
                 method=method, limit_direction=limit_direction, limit=limit
             )
             quality_df = self.quality_df.replace("m", "i")
         else:
             df = self.data.replace(999999, np.nan)
@@ -400,29 +401,33 @@
             name=name,
         )
         return ts
 
     def apply_calibration_matrix(
         self,
         calibration_matrix: np.array,
+        calibration_matrix_name: str = None,
         use_channels: list = [1, 1, 1, 1],
         name: str = None,
     ):
         """
         Processing step to convert gauge strains into areal and shear strains
         :param ts: Timeseries object containing gauge data in microstrain
         :param calibration_matrix: np.array containing strain matrix
+        :param calibration_matrix_name: str describing which calibration matrix is used
         :return: Timeseries object, in units of microstrain
         """
         # calculate areal and shear strains from gauge strains
         # todo: implement UseChannels to arbitrary matrices
-        data = apply_calibration_matrix(self.data, calibration_matrix, use_channels)
+        data = apply_calibration_matrix(
+            self.data, calibration_matrix, calibration_matrix_name, use_channels
+        )
         quality_df = pd.DataFrame(
             index=self.quality_df.index,
-            columns=["Eee+Enn", "Eee-Enn", "2Ene"],
+            columns=data.columns,
             data="g",
         )
         quality_df[self.quality_df[self.quality_df == "m"].any(axis=1)] = "m"
         if not name:
             name = f"{self.name}.calibrated"
         ts2 = Timeseries(
             data=data,
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/PKG-INFO` & `earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthscopestraintools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of utilities for working with EarthScope strainmeter data
 Author-email: Mike Gottlieb <mike.gottlieb@eartscope.org>
 License: Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `earthscopestraintools-0.1.6/src/earthscopestraintools.egg-info/SOURCES.txt` & `earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/test/test_bottle2mseed.py` & `earthscopestraintools-0.1.7/test/test_bottle2mseed.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/test/test_bottle2tdb.py` & `earthscopestraintools-0.1.7/test/test_bottle2tdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 
 if __name__ == '__main__':
 
     t1 = datetime.now()
 
     network = "PB"
     station = "B001"
-    station_edid = get_station_edid(network, station)
+    station_edid = get_station_edid(station)
     ancillary_uri = f"arrays/{station_edid}_ancillary.tdb"
     write_it = True
     print_it = True
     check_it = True
 
 
     filepath = 'bottles/B001.2022001Day.tgz'  #24 hr Day session (archive and logger format)
     session = "Day"
-    session_edid = get_session_edid(network, station, session)
+    session_edid = get_session_edid(station, session)
     strain_uri = f"arrays/{session_edid}.tdb"
     bottle2tdb(filepath, strain_uri, ancillary_uri, session, write_it=write_it, print_it=print_it, check_it=check_it)
 
     filepath = 'bottles/B0012200100.tgz'  # 1 Hour, Hour Session (logger format)
     session = "Hour"
-    session_edid = get_session_edid(network, station, session)
+    session_edid = get_session_edid(station, session)
     strain_uri = f"arrays/{session_edid}.tdb"
     bottle2tdb(filepath, strain_uri, ancillary_uri, session, write_it=write_it, print_it=print_it, check_it=check_it)
 
     filepath = 'bottles/B0012200100_20.tar'  # 1 Hour, Min Session (logger format)
     session = "Min"
-    session_edid = get_session_edid(network, station, session)
+    session_edid = get_session_edid(station, session)
     strain_uri = f"arrays/{session_edid}.tdb"
     bottle2tdb(filepath, strain_uri, ancillary_uri, session, write_it=write_it, print_it=print_it, check_it=check_it)
 
     # filepath = 'bottles/B001.2022001_01.tar' #24 Hour, Hour Session (archive format)
     # session = "Hour"
     # session_edid = get_session_edid(network, station, session)
     # strain_uri = f"arrays/{session_edid}.tdb"
```

### Comparing `earthscopestraintools-0.1.6/test/test_bottletar.py` & `earthscopestraintools-0.1.7/test/test_bottletar.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/test/test_edid.py` & `earthscopestraintools-0.1.7/test/test_edid.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.6/test/test_ts2tdb.py` & `earthscopestraintools-0.1.7/test/test_ts2tdb.py`

 * *Files identical despite different names*


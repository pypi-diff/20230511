# Comparing `tmp/reixs-0.5.7.1.tar.gz` & `tmp/reixs-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.5.7.1.tar", last modified: Mon May  1 22:18:32 2023, max compression
+gzip compressed data, was "reixs-0.5.8.tar", last modified: Thu May 11 18:34:55 2023, max compression
```

## Comparing `reixs-0.5.7.1.tar` & `reixs-0.5.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:18:32.389612 reixs-0.5.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 22:18:15.000000 reixs-0.5.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-01 22:18:32.389612 reixs-0.5.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-01 22:18:15.000000 reixs-0.5.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 22:18:15.000000 reixs-0.5.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-01 22:18:32.389612 reixs-0.5.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:18:32.385612 reixs-0.5.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:18:32.389612 reixs-0.5.7.1/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    59076 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    33022 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/beamline_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-01 22:18:15.000000 reixs-0.5.7.1/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:18:32.389612 reixs-0.5.7.1/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-01 22:18:32.000000 reixs-0.5.7.1/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-01 22:18:32.000000 reixs-0.5.7.1/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:18:32.000000 reixs-0.5.7.1/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 22:18:32.000000 reixs-0.5.7.1/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 22:18:32.000000 reixs-0.5.7.1/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:34:55.929800 reixs-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-11 18:34:40.000000 reixs-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-11 18:34:55.929800 reixs-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-11 18:34:40.000000 reixs-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 18:34:40.000000 reixs-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-11 18:34:55.929800 reixs-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:34:55.925800 reixs-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:34:55.929800 reixs-0.5.8/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    59604 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33022 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-11 18:34:40.000000 reixs-0.5.8/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:34:55.929800 reixs-0.5.8/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-11 18:34:55.000000 reixs-0.5.8/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-11 18:34:55.000000 reixs-0.5.8/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:34:55.000000 reixs-0.5.8/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 18:34:55.000000 reixs-0.5.8/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 18:34:55.000000 reixs-0.5.8/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.5.7.1/LICENSE` & `reixs-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/PKG-INFO` & `reixs-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.7.1
+Version: 0.5.8
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLS REIXS Analysis
 
 This is a library to analyse, plot, and export REIXS beamline data. The package is meant to provide a framework to load data into jupyter and enable data interaction.
 
-Further [beamline information](https://reixs.leightsource.ca/) is available on the Website of the Canadian Light Source.
+Further [beamline information](https://reixs.lightsource.ca/) is available on the Website of the Canadian Light Source.
 
 ## Installation
 
 Install the package from PyPi with the pip package manager. This is the recommended way to obtain a copy for your local machine and will install all required dependencies.
 
 ```
     $ pip install reixs
```

### Comparing `reixs-0.5.7.1/README.md` & `reixs-0.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # CLS REIXS Analysis
 
 This is a library to analyse, plot, and export REIXS beamline data. The package is meant to provide a framework to load data into jupyter and enable data interaction.
 
-Further [beamline information](https://reixs.leightsource.ca/) is available on the Website of the Canadian Light Source.
+Further [beamline information](https://reixs.lightsource.ca/) is available on the Website of the Canadian Light Source.
 
 ## Installation
 
 Install the package from PyPi with the pip package manager. This is the recommended way to obtain a copy for your local machine and will install all required dependencies.
 
 ```
     $ pip install reixs
@@ -277,8 +277,8 @@
 - _xcoffset_ (Defines a constant shift in the x-stream)
 - _xoffset_ (Takes a list of tuples and defines a polynomial fit of the x-stream)
 - _ycoffset_ (Defines a constant shift in the y-stream)
 - _yoffset_ (Takes a list of tuples and defines a polynomial fit of the y-stream)
   e.g. offset = [(100,102),(110,112),(120,121)]
 - _background_ (Subtracts a XEOL background from XEOL scans)
   Set to True, uses the getXEOLback function with the background data stored (only supported with HDF5)
-  Specify scan number, subtracts the XEOL scan taken at this particular scan
+  Specify scan number, subtracts the XEOL scan taken at this particular scan
```

### Comparing `reixs-0.5.7.1/setup.cfg` & `reixs-0.5.8/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.5.7.1
+version = 0.5.8
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls =
```

### Comparing `reixs-0.5.7.1/src/reixs/LoadData.py` & `reixs-0.5.8/src/reixs/LoadData.py`

 * *Files 3% similar despite different names*

```diff
@@ -330,34 +330,38 @@
         Returns
         -------
         dfT : pandas DataFrame 
             All loaded data.
         files : list
             List of all loaded files.
         """
-        df = pd.DataFrame()
+        
         files = list()
+        series_data = list()
+        series_header = list()
 
         # Iterate over all "load" calls
         for i, val in enumerate(self.data):
             # Iterate over all scans per load call.
             for k, v in val.items():
                 name = f"~{self.filename[i]}"
                 if name not in files:
                     files.append(name)
                 fileindex = files.index(name)
 
-                s1 = pd.Series(
-                    v.x_stream, name=f"F{fileindex+1}_S{v.scan}_I{i+1}-{self.x_stream[i]}")
-                df = df.append(s1)
-                s2 = pd.Series(
-                    v.y_stream, name=f"F{fileindex+1}_S{v.scan}_I{i+1}-{self.type[i]}")
-                df = df.append(s2)
+                # Append the x_stream data and header name
+                series_data.append(pd.Series(v.x_stream))
+                series_header.append(f"F{fileindex+1}_S{v.scan}_I{i+1}-{self.x_stream[i]}")
+
+                # Append the y_stream data and header name
+                series_data.append(pd.Series(v.y_stream))
+                series_header.append(f"F{fileindex+1}_S{v.scan}_I{i+1}-{self.type[i]}")
 
-        dfT = df.transpose(copy=True)
+        dfT = pd.DataFrame(series_data).transpose(copy=True)
+        dfT.columns = series_header
 
         return dfT, files
 
     def export(self, filename):
         """
         Export and write data to specified file.
 
@@ -819,24 +823,26 @@
         """Make data available in memory as exported to file.
 
         Returns
         -------
         f : string.IO object
             Motor and Detector Scales. Pandas Data Series.
             1) Rewind memory with f.seek(0)
-            2) Load with pandas.from_csv(object)
+            2) Load with pandas.read_csv(f,skiprows=3)
         g : string.IO object
             Actual gridded detector image.
             1) Rewind memory with g.seek(0)
-            2) Load with numpy.genfromtxt(object)
+            2) Load with numpy.genfromtxt(g,skip_header=4)
         """
         # Set up the data frame and the two string objects for export
-        df = pd.DataFrame()
         f = io.StringIO()
         g = io.StringIO()
+        series_data = list()
+        series_header = list()
+
         for i, val in enumerate(self.data):
             for k, v in val.items():
                 # Gridded scales now calculated directly during the MCA load and only need to be referenced here
 
                 # Start writing string f
                 f.write("========================\n")
                 f.write(
@@ -846,21 +852,24 @@
                 # Start writing string g
                 g.write("========================\n")
                 g.write(
                     f"F~{self.filename[i]}_S{v.scan}_{self.detector[i]}_{self.x_stream[i]}_{self.y_stream[i]}\n")
                 g.write("========================\n")
 
                 # Append data to string now.
-                s1 = pd.Series(
-                    v.new_x, name="Motor Scale Gridded")
-                df = df.append(s1)
-                s2 = pd.Series(
-                    v.new_y, name="Detector Scale Gridded")
-                df = df.append(s2)
-                dfT = df.transpose(copy=True)
+                # Append x-stream
+                series_data.append( pd.Series(v.new_x))
+                series_header.append("Motor Scale Gridded")
+
+                # Append y-stream
+                series_data.append(pd.Series(v.new_y))
+                series_header.append("Detector Scale Gridded")
+
+                dfT = pd.DataFrame(series_data).transpose(copy=True)
+                dfT.columns = series_header
                 dfT.to_csv(f, index=False, line_terminator='\n')
 
                 g.write("=== Image ===\n")
                 np.savetxt(g, v.new_z, fmt="%.9g")
 
             return f, g
 
@@ -1259,33 +1268,37 @@
         if xlabel != None:
             p.xaxis.axis_label = str(xlabel)
         if ylabel != None:
             p.yaxis.axis_label = str(ylabel)
         show(p)
 
     def get_data(self):
-        df = pd.DataFrame()
+        
         files = list()
+        series_data = list()
+        series_header = list()
 
         for i, val in enumerate(self.data):
             for k, v in val.items():
                 name = f"~{self.filename[i]}"
                 if name not in files:
                     files.append(name)
                 fileindex = files.index(name)
 
                 for image, imagevalue in v.caxis.items():
-                    s1 = pd.Series(
-                        imagevalue, name=f"F{fileindex+1}_S{v.scan}_I{i+1}_Img{image}-{v.caxis_label}")
-                    df = df.append(s1)
-                    s2 = pd.Series(
-                        v.imagesca[image], name=f"F{fileindex+1}_S{v.scan}_I{i+1}_Img{image}_Counts")
-                    df = df.append(s2)
+                    # Append the x stream
+                    series_data.append(pd.Series(imagevalue))
+                    series_header.append(f"F{fileindex+1}_S{v.scan}_I{i+1}_Img{image}-{v.caxis_label}")
+
+                    # Append the y stream
+                    series_data.append(pd.Series(v.imagesca[image]))
+                    series_header.append(f"F{fileindex+1}_S{v.scan}_I{i+1}_Img{image}_Counts")
 
-        dfT = df.transpose(copy=True)
+        dfT = pd.DataFrame(series_data).transpose(copy=True)
+        dfT.columns = series_header
 
         return dfT, files
 
     def export(self, filename):
 
         dfT, files = self.get_data()
```

### Comparing `reixs-0.5.7.1/src/reixs/ReadData.py` & `reixs-0.5.8/src/reixs/ReadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/add_subtract.py` & `reixs-0.5.8/src/reixs/add_subtract.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/beamline_info.py` & `reixs-0.5.8/src/reixs/beamline_info.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/mca.py` & `reixs-0.5.8/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/mesh.py` & `reixs-0.5.8/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/parser.py` & `reixs-0.5.8/src/reixs/parser.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/rixs_readutil.py` & `reixs-0.5.8/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/rsxs_mcp.py` & `reixs-0.5.8/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/rsxs_readutil.py` & `reixs-0.5.8/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/sca.py` & `reixs-0.5.8/src/reixs/sca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/simplemath.py` & `reixs-0.5.8/src/reixs/simplemath.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/spec_config.py` & `reixs-0.5.8/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/util.py` & `reixs-0.5.8/src/reixs/util.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs/xeol.py` & `reixs-0.5.8/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.7.1/src/reixs.egg-info/PKG-INFO` & `reixs-0.5.8/src/reixs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.7.1
+Version: 0.5.8
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLS REIXS Analysis
 
 This is a library to analyse, plot, and export REIXS beamline data. The package is meant to provide a framework to load data into jupyter and enable data interaction.
 
-Further [beamline information](https://reixs.leightsource.ca/) is available on the Website of the Canadian Light Source.
+Further [beamline information](https://reixs.lightsource.ca/) is available on the Website of the Canadian Light Source.
 
 ## Installation
 
 Install the package from PyPi with the pip package manager. This is the recommended way to obtain a copy for your local machine and will install all required dependencies.
 
 ```
     $ pip install reixs
```

### Comparing `reixs-0.5.7.1/src/reixs.egg-info/SOURCES.txt` & `reixs-0.5.8/src/reixs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


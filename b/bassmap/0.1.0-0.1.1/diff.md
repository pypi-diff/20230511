# Comparing `tmp/bassmap-0.1.0.tar.gz` & `tmp/bassmap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bassmap-0.1.0.tar", last modified: Thu May 11 05:13:03 2023, max compression
+gzip compressed data, was "bassmap-0.1.1.tar", last modified: Thu May 11 21:23:31 2023, max compression
```

## Comparing `bassmap-0.1.0.tar` & `bassmap-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:03.267306 bassmap-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 05:12:52.000000 bassmap-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 05:12:52.000000 bassmap-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-11 05:13:03.267306 bassmap-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-11 05:12:52.000000 bassmap-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:03.267306 bassmap-0.1.0/bassmap/
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-11 05:12:52.000000 bassmap-0.1.0/bassmap/Foliumatic.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 05:12:52.000000 bassmap-0.1.0/bassmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-05-11 05:12:52.000000 bassmap-0.1.0/bassmap/bassmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:03.267306 bassmap-0.1.0/bassmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 05:12:53.000000 bassmap-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 05:13:03.267306 bassmap-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-11 05:12:53.000000 bassmap-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:23:31.789992 bassmap-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 21:23:18.000000 bassmap-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 21:23:18.000000 bassmap-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-11 21:23:31.789992 bassmap-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-11 21:23:18.000000 bassmap-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:23:31.789992 bassmap-0.1.1/bassmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-11 21:23:18.000000 bassmap-0.1.1/bassmap/Foliumatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 21:23:18.000000 bassmap-0.1.1/bassmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29486 2023-05-11 21:23:18.000000 bassmap-0.1.1/bassmap/bassmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:23:31.789992 bassmap-0.1.1/bassmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-11 21:23:31.000000 bassmap-0.1.1/bassmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 21:23:31.000000 bassmap-0.1.1/bassmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 21:23:31.000000 bassmap-0.1.1/bassmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:23:31.000000 bassmap-0.1.1/bassmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 21:23:31.000000 bassmap-0.1.1/bassmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 21:23:31.000000 bassmap-0.1.1/bassmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 21:23:18.000000 bassmap-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 21:23:31.789992 bassmap-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-11 21:23:18.000000 bassmap-0.1.1/setup.py
```

### Comparing `bassmap-0.1.0/LICENSE` & `bassmap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bassmap-0.1.0/PKG-INFO` & `bassmap-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bassmap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/bassneel/bassmap
 Author: Bass Neel
 Author-email: maps.bassneel@gmail.com
 License: MIT license
 Keywords: bassmap
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,18 +20,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BassMap
 
 [![image](https://img.shields.io/pypi/v/bassmap.svg)](https://pypi.python.org/pypi/bassmap)
 [![LinkedIn Badge](https://img.shields.io/badge/My-LinkedIn-blue)](https://www.linkedin.com/in/bassneel)
+[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/channel/UCT8zQZMTdzOm3u0Ojq0piRg)
 ![BassMap](https://github.com/bassneel/basspublicfiles/blob/main/bassmap_logo.png)
 
 **BassMap is an intuitive Python Package that allows the user to display a variety of features on an iPyLeaflet and Folium map display. In addition the Landsat 8 Tools allows the user to create a variety of multispectral composites using local GeoTIFFs from Landsat 8 spectral bands**
 
+[BassMap on Streamlit](https://bassmap.streamlit.app/)
+
 
 -   Free software: MIT license
 -   Documentation: https://bassneel.github.io/bassmap
     
 
 ## Features
 
@@ -55,12 +58,12 @@
     -   Change basemap
     -   Display shapefiles
     -   Display GeoJSON files
     -   Display vector files
 
 ## Demo
 
-
+[![IMAGE ALT TEXT](http://img.youtube.com/vi/5dLXxnTaNv4/0.jpg)](https://www.youtube.com/watch?v=5dLXxnTaNv4 "BassMap - Satellite Image Processing with Python")
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `bassmap-0.1.0/README.md` & `bassmap-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # BassMap
 
 [![image](https://img.shields.io/pypi/v/bassmap.svg)](https://pypi.python.org/pypi/bassmap)
 [![LinkedIn Badge](https://img.shields.io/badge/My-LinkedIn-blue)](https://www.linkedin.com/in/bassneel)
+[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/channel/UCT8zQZMTdzOm3u0Ojq0piRg)
 ![BassMap](https://github.com/bassneel/basspublicfiles/blob/main/bassmap_logo.png)
 
 **BassMap is an intuitive Python Package that allows the user to display a variety of features on an iPyLeaflet and Folium map display. In addition the Landsat 8 Tools allows the user to create a variety of multispectral composites using local GeoTIFFs from Landsat 8 spectral bands**
 
+[BassMap on Streamlit](https://bassmap.streamlit.app/)
+
 
 -   Free software: MIT license
 -   Documentation: https://bassneel.github.io/bassmap
     
 
 ## Features
 
@@ -33,12 +36,12 @@
     -   Change basemap
     -   Display shapefiles
     -   Display GeoJSON files
     -   Display vector files
 
 ## Demo
 
-
+[![IMAGE ALT TEXT](http://img.youtube.com/vi/5dLXxnTaNv4/0.jpg)](https://www.youtube.com/watch?v=5dLXxnTaNv4 "BassMap - Satellite Image Processing with Python")
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `bassmap-0.1.0/bassmap/Foliumatic.py` & `bassmap-0.1.1/bassmap/Foliumatic.py`

 * *Files identical despite different names*

### Comparing `bassmap-0.1.0/bassmap/bassmap.py` & `bassmap-0.1.1/bassmap/bassmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -685,14 +685,42 @@
         ndvi_ds.GetRasterBand(1).WriteArray(ndvi)
         ndvi_ds.FlushCache()
     else:
         raise Exception("Failed to create TIFF file")
         
     return ndvi_path
 
+
+def csv_to_points(in_csv):
+
+    df = pd.read_csv(in_csv)
+
+    geometry = [Point(xy) for xy in zip(df['longitude'], df['latitude'])]
+    gdf = gpd.GeoDataFrame(df, geometry=geometry)
+    gdf.to_file('csv_points.shp', driver='ESRI Shapefile')
+
+def add_marker_cluster(in_csv):
+
+    df = pd.read_csv(in_csv)
+
+    geometry = [Point(xy) for xy in zip(df['longitude'], df['latitude'])]
+    gdf = gpd.GeoDataFrame(df, geometry=geometry)
+    gdf.to_file('marker_cluster.shp', driver='ESRI Shapefile')
+
+    colors = {}
+    for i, name in enumerate(gdf['name']):
+        colors[name] = f"#{i+1:02x}0000"
+
+    style = {'fillOpacity': 0.7, 'weight': 1, 'color': 'black'}
+    m = Mapomatic(center=[0, 0], zoom=2)
+    m.add_shp('marker_cluster.shp')
+
+    from IPython.display import display
+    display(m)
+
 locations = {}
 
 def generate_input_points():
     """Input name and either generate random point or input coordinates to shapefile and display on map.
 
     Args:
         name (): Name of the location.
```

### Comparing `bassmap-0.1.0/bassmap.egg-info/PKG-INFO` & `bassmap-0.1.1/bassmap.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bassmap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/bassneel/bassmap
 Author: Bass Neel
 Author-email: maps.bassneel@gmail.com
 License: MIT license
 Keywords: bassmap
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,18 +20,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BassMap
 
 [![image](https://img.shields.io/pypi/v/bassmap.svg)](https://pypi.python.org/pypi/bassmap)
 [![LinkedIn Badge](https://img.shields.io/badge/My-LinkedIn-blue)](https://www.linkedin.com/in/bassneel)
+[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/channel/UCT8zQZMTdzOm3u0Ojq0piRg)
 ![BassMap](https://github.com/bassneel/basspublicfiles/blob/main/bassmap_logo.png)
 
 **BassMap is an intuitive Python Package that allows the user to display a variety of features on an iPyLeaflet and Folium map display. In addition the Landsat 8 Tools allows the user to create a variety of multispectral composites using local GeoTIFFs from Landsat 8 spectral bands**
 
+[BassMap on Streamlit](https://bassmap.streamlit.app/)
+
 
 -   Free software: MIT license
 -   Documentation: https://bassneel.github.io/bassmap
     
 
 ## Features
 
@@ -55,12 +58,12 @@
     -   Change basemap
     -   Display shapefiles
     -   Display GeoJSON files
     -   Display vector files
 
 ## Demo
 
-
+[![IMAGE ALT TEXT](http://img.youtube.com/vi/5dLXxnTaNv4/0.jpg)](https://www.youtube.com/watch?v=5dLXxnTaNv4 "BassMap - Satellite Image Processing with Python")
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `bassmap-0.1.0/setup.py` & `bassmap-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='bassmap',
     name='bassmap',
     packages=find_packages(include=['bassmap', 'bassmap.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bassneel/bassmap',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```


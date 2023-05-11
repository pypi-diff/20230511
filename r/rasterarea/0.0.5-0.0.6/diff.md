# Comparing `tmp/rasterarea-0.0.5.tar.gz` & `tmp/rasterarea-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterarea-0.0.5.tar", last modified: Tue May  9 18:56:47 2023, max compression
+gzip compressed data, was "rasterarea-0.0.6.tar", last modified: Thu May 11 20:59:18 2023, max compression
```

## Comparing `rasterarea-0.0.5.tar` & `rasterarea-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:56:47.834867 rasterarea-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 18:56:37.000000 rasterarea-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 18:56:37.000000 rasterarea-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-09 18:56:47.834867 rasterarea-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-09 18:56:37.000000 rasterarea-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:56:47.834867 rasterarea-0.0.5/rasterarea/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/ipyleafletmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/rasterarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:56:47.834867 rasterarea-0.0.5/rasterarea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 18:56:37.000000 rasterarea-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-09 18:56:47.838867 rasterarea-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-09 18:56:37.000000 rasterarea-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:59:18.594867 rasterarea-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 20:59:06.000000 rasterarea-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 20:59:06.000000 rasterarea-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-11 20:59:18.594867 rasterarea-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 20:59:06.000000 rasterarea-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:59:18.594867 rasterarea-0.0.6/rasterarea/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-11 20:59:06.000000 rasterarea-0.0.6/rasterarea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-11 20:59:06.000000 rasterarea-0.0.6/rasterarea/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-05-11 20:59:06.000000 rasterarea-0.0.6/rasterarea/ipyleafletmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-05-11 20:59:06.000000 rasterarea-0.0.6/rasterarea/rasterarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:59:18.594867 rasterarea-0.0.6/rasterarea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-11 20:59:18.000000 rasterarea-0.0.6/rasterarea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 20:59:18.000000 rasterarea-0.0.6/rasterarea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 20:59:18.000000 rasterarea-0.0.6/rasterarea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:59:18.000000 rasterarea-0.0.6/rasterarea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 20:59:18.000000 rasterarea-0.0.6/rasterarea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 20:59:18.000000 rasterarea-0.0.6/rasterarea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-11 20:59:06.000000 rasterarea-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-11 20:59:18.594867 rasterarea-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-11 20:59:06.000000 rasterarea-0.0.6/setup.py
```

### Comparing `rasterarea-0.0.5/LICENSE` & `rasterarea-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.5/rasterarea/foliummap.py` & `rasterarea-0.0.6/rasterarea/foliummap.py`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.5/rasterarea/ipyleafletmap.py` & `rasterarea-0.0.6/rasterarea/ipyleafletmap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import ipyleaflet
 from ipyleaflet import WidgetControl
 import ipywidgets as widgets
+import pandas as pd
+import geopandas as gpd
+from shapely.geometry import Point
+
 class Map(ipyleaflet.Map):
     
     def __init__(self, center=[20, 0], zoom=2, **kwargs) -> None:
 
         if "scroll_wheel_zoom" not in kwargs:
             kwargs["scroll_wheel_zoom"] = True
 
@@ -212,14 +216,79 @@
             height (int): The height of the image.
             position (str, optional): The position of the image. Defaults to 'bottomright'.
         """
         widget = widgets.HTML(value = f'<img src="{url}" width="{width}" height="{height}">')
         control = WidgetControl(widget=widget, position=position)
         self.add(control)
 
+
+    def csv_to_shp(in_csv,out_shp, x="longitude", y="latitude"):
+        """
+        This function takes a csv file and converts it to a shapefile.
+        """
+    
+        # Read in the csv file
+        df = pd.read_csv(in_csv)
+    
+        # Create a geometry column
+        geometry = [Point(xy) for xy in zip(df[x], df[y])]
+    
+        # Create a geodataframe
+        gdf = gpd.GeoDataFrame(df, geometry=geometry)
+    
+        # Save the geodataframe as a shapefile
+        gdf.to_file(out_shp,driver='ESRI Shapefile')
+    
+        return gdf
+
+    
+    def csv_to_geojson(in_csv, out_geojson, x="longitude", y="latitude"):
+        """
+        This function takes a csv file and converts it to a geojson file.
+        """
+    
+        # Read in the csv file
+        df = pd.read_csv(in_csv)
+    
+        # Create a geometry column
+        geometry = [Point(xy) for xy in zip(df[x], df[y])]
+    
+        # Create a geodataframe
+        gdf = gpd.GeoDataFrame(df, geometry=geometry)
+    
+        # Save the geodataframe as a geojson file
+        gdf.to_file(out_geojson, driver="GeoJSON")
+    
+        return gdf
+
+
+    def add_marker_from_csv(self, in_csv, x="longitude", y="latitude", label=None, layer_name="Marker cluster"):
+        """
+        This function takes a csv file and adds a marker cluster to the map.
+        """
+        
+        # Read in the csv file
+        df = pd.read_csv(in_csv)
+        
+        # Create a geometry column
+        geometry = [Point(xy) for xy in zip(df[x], df[y])]
+        
+        # Create a geodataframe
+        gdf = gpd.GeoDataFrame(df, geometry=geometry)
+        
+        # Create a marker cluster
+        marker_cluster = ipyleaflet.MarkerCluster(
+            markers=[ipyleaflet.Marker(location=[point.y, point.x]) for point in gdf.geometry]
+        )
+        
+        # Add the marker cluster to the map
+        self.add_layer(marker_cluster)
+        
+        return marker_cluster
+
     
     def add_toolbar(self, position='topright', **kwargs):
         """Adds a toolbar to the map.
 
         Args:
             toolbar (str, optional): The toolbar to add. Defaults to 'draw'.
             position (str, optional): The position of the toolbar. Defaults to 'topright'.
@@ -299,27 +368,46 @@
             value=None,
             description="Basemap:",
             style={"description_width": "initial"},
             layout=widgets.Layout(width="200px"),
         )
         basemap_ctrl = WidgetControl(widget=basemap, position="topright")
 
+        csv_input = widgets.Text(
+            value='',
+            placeholder='Type the path to the CSV file',
+            description='CSV File:',
+            disabled=False
+        )
+
+        csv_input_ctrl = WidgetControl(widget=csv_input, position="topright")
+
         def tool_click(b):    
             with output:
                 output.clear_output()
                 print(f"You clicked the {b.icon} button")
 
                 if b.icon == "map":
                     self.add_control(basemap_ctrl)
-
+                elif b.icon == "folder-open":
+                    self.add_control(csv_input_ctrl)
+    
         for i in range(rows):
             for j in range(cols):
                 tool = grid[i, j]
                 tool.on_click(tool_click)
 
         def change_basemap(change):
             if change["new"]:
                 self.add_basemap(basemap.value)
 
+
+        def change_csv_input(change):
+            if change["new"]:
+                csv_file = csv_input.value
+                self.add_marker_from_csv(in_csv=csv_file, x="longitude", y="latitude")
+        
+        csv_input.observe(change_csv_input, names="value")
+
         basemap.observe(change_basemap, names='value')
-        self.add_control(toolbar_ctrl)
 
+        self.add_control(toolbar_ctrl)
```

### Comparing `rasterarea-0.0.5/rasterarea/rasterarea.py` & `rasterarea-0.0.6/rasterarea/rasterarea.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,14 +337,18 @@
 
         b.description = "Files Selected"
         b.icon = "check-square-o"
         b.style.button_color = "lightgreen"
 
 
 class Toolbar(widgets.VBox):
+    """
+    create a widget for interactive plot
+        
+    """    
     def __init__(self,parent,**kwargs):
         super().__init__()
         self.create_widgets()
         self.output = widgets.Output()
         self.setup_interactive_plot()   
         self.parent = parent
```

### Comparing `rasterarea-0.0.5/setup.py` & `rasterarea-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='rasterarea',
     name='rasterarea',
     packages=find_packages(include=['rasterarea', 'rasterarea.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Feng96/rasterarea',
-    version='0.0.5',
+    version='0.0.6',
     zip_safe=False,
 )
```


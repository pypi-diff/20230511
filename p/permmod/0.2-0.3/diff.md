# Comparing `tmp/permmod-0.2.tar.gz` & `tmp/permmod-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permmod-0.2.tar", last modified: Wed May  3 07:06:58 2023, max compression
+gzip compressed data, was "permmod-0.3.tar", last modified: Thu May 11 06:37:26 2023, max compression
```

## Comparing `permmod-0.2.tar` & `permmod-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 07:06:58.917872 permmod-0.2/
--rw-rw-rw-   0        0        0     1876 2023-05-03 07:06:58.917872 permmod-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1367 2023-03-06 12:08:24.000000 permmod-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 07:06:58.886620 permmod-0.2/permmod/
--rw-rw-rw-   0        0        0      216 2023-03-08 09:11:06.000000 permmod-0.2/permmod/__init__.py
--rw-rw-rw-   0        0        0    12009 2023-03-08 10:01:54.000000 permmod-0.2/permmod/import_data.py
--rw-rw-rw-   0        0        0     5769 2023-03-08 11:13:05.000000 permmod-0.2/permmod/linear_system.py
--rw-rw-rw-   0        0        0     7194 2023-03-06 12:08:24.000000 permmod-0.2/permmod/measurement.py
--rw-rw-rw-   0        0        0     2737 2023-03-06 12:08:24.000000 permmod-0.2/permmod/optimize.py
--rw-rw-rw-   0        0        0    10423 2023-03-06 12:08:24.000000 permmod-0.2/permmod/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:06:58.902246 permmod-0.2/permmod.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      677 2023-05-03 07:03:52.000000 permmod-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 07:06:58.917872 permmod-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 06:37:26.109269 permmod-0.3/
+-rw-rw-rw-   0        0        0     1928 2023-05-11 06:37:26.109269 permmod-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1419 2023-05-04 05:13:12.000000 permmod-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 06:37:26.091268 permmod-0.3/permmod/
+-rw-rw-rw-   0        0        0      216 2023-03-08 09:11:06.000000 permmod-0.3/permmod/__init__.py
+-rw-rw-rw-   0        0        0    12009 2023-03-08 10:01:54.000000 permmod-0.3/permmod/import_data.py
+-rw-rw-rw-   0        0        0     5769 2023-03-08 11:13:05.000000 permmod-0.3/permmod/linear_system.py
+-rw-rw-rw-   0        0        0     7858 2023-05-10 09:18:48.000000 permmod-0.3/permmod/measurement.py
+-rw-rw-rw-   0        0        0     2737 2023-03-06 12:08:24.000000 permmod-0.3/permmod/optimize.py
+-rw-rw-rw-   0        0        0    11751 2023-05-10 09:22:34.000000 permmod-0.3/permmod/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:37:26.107267 permmod-0.3/permmod.egg-info/
+-rw-rw-rw-   0        0        0     1928 2023-05-11 06:37:26.000000 permmod-0.3/permmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-11 06:37:26.000000 permmod-0.3/permmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 06:37:26.000000 permmod-0.3/permmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-11 06:37:26.000000 permmod-0.3/permmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 06:37:26.000000 permmod-0.3/permmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      677 2023-05-11 06:35:27.000000 permmod-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 06:37:26.110269 permmod-0.3/setup.cfg
```

### Comparing `permmod-0.2/PKG-INFO` & `permmod-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permmod
-Version: 0.2
+Version: 0.3
 Summary: A package to calculate the permeability of rock samples
 Author-email: Martin Kirch <mkirch@web.de>
 Project-URL: Homepage, https://github.com/kirchma/permmod
 Project-URL: Bug Tracker, https://github.com/kirchma/permmod/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,36 +17,39 @@
 
 permmod is a Python package that is used to calculate the permeability of two-chamber-method measurements.
 This type of measurement is based on Brace's pulse decay method and extends it to include pressure- and 
 temperature-dependent material parameters. More details are available in the following paper.
 
 ## How to use it.
 
-In order to use the package there must be a measurement, a database and a measurement_units file in the following 
+In order to use the package there must be a measurement-, a database- and a measurement_units-file in the following 
 folder structure:
 ```
 Measurements
 │   database.csv
 │   measurement_units.csv   
 │
 └───raw_data
 │   │   measurement_file1.txt
 │   │   ...
 │   
 └───sim_data
-    │
+│   │   ...
+│   
+└───pics
+│   │   ...
 ```
 
 An example of the structure of the folders and the 3 files is given in the **example folder**. 
 
 To evaluate a measurement, you can proceed as follows:
 ```sh
 from permmod import Measurement
 
-path = '/raw_data/measurement_file1.txt'
+path = 'raw_data/measurement_file1.txt'
 measurement = Measurement(path=path)
 measurement.calculate_permeability([1e-19, 0.001], parameter='both')
 ```
 For more information see the documentation
 
 ## Installation
 The source code is hosted on GitHub at:
```

### Comparing `permmod-0.2/README.md` & `permmod-0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,36 +4,39 @@
 
 permmod is a Python package that is used to calculate the permeability of two-chamber-method measurements.
 This type of measurement is based on Brace's pulse decay method and extends it to include pressure- and 
 temperature-dependent material parameters. More details are available in the following paper.
 
 ## How to use it.
 
-In order to use the package there must be a measurement, a database and a measurement_units file in the following 
+In order to use the package there must be a measurement-, a database- and a measurement_units-file in the following 
 folder structure:
 ```
 Measurements
 │   database.csv
 │   measurement_units.csv   
 │
 └───raw_data
 │   │   measurement_file1.txt
 │   │   ...
 │   
 └───sim_data
-    │
+│   │   ...
+│   
+└───pics
+│   │   ...
 ```
 
 An example of the structure of the folders and the 3 files is given in the **example folder**. 
 
 To evaluate a measurement, you can proceed as follows:
 ```sh
 from permmod import Measurement
 
-path = '/raw_data/measurement_file1.txt'
+path = 'raw_data/measurement_file1.txt'
 measurement = Measurement(path=path)
 measurement.calculate_permeability([1e-19, 0.001], parameter='both')
 ```
 For more information see the documentation
 
 ## Installation
 The source code is hosted on GitHub at:
```

### Comparing `permmod-0.2/permmod/import_data.py` & `permmod-0.3/permmod/import_data.py`

 * *Files identical despite different names*

### Comparing `permmod-0.2/permmod/linear_system.py` & `permmod-0.3/permmod/linear_system.py`

 * *Files identical despite different names*

### Comparing `permmod-0.2/permmod/measurement.py` & `permmod-0.3/permmod/measurement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pandas as pd
+import CoolProp.CoolProp as cp
 from .import_data import Data, DataReaktor
 from .optimize import Optimizer
 from .plots import Plotter, PlotterReaktor
 
 
 class Measurement:
 
@@ -12,14 +13,27 @@
         self.file_name, _ = os.path.splitext(os.path.split(path)[1])
         self.path_raw, _ = os.path.splitext(os.path.split(path)[0])
         self.path_sim = os.path.join(os.path.dirname(os.path.dirname(path)), 'sim_data')
         self.df_100 = None
         self.df_final = None
         self.sample_data = None
 
+    def guess_permeability(self):
+        self.set_data()
+        df = self.df_100
+        df['V'] = cp.PropsSI('VISCOSITY', 'T', df['Temperature'].to_list(), 'P', df['Outlet_Pressure'].to_list(),
+                             self.sample_data['gas'])
+        V = self.sample_data['inlet_chamber_volume']
+        L = self.sample_data['length']
+        A = self.sample_data['area']
+        df['k'] = - ((V * df['V'] * 2 * L * df['Inlet_Pressure'].diff()) /
+                     (A * (df['Inlet_Pressure'] ** 2 - df['Outlet_Pressure'] ** 2) * df['Duration'].diff()))
+        plot = Plotter(df)
+        plot.guess_chart()
+
     def calculate_permeability(self, guess, parameter='k'):
         if self.find_file():
             user_input = input('''
             This measurement has already been evaluated. 
             Do you want to use the time adjusted measurement file? (y/n)''')
             if user_input == 'y':
                 self.set_adjusted_data()
```

### Comparing `permmod-0.2/permmod/optimize.py` & `permmod-0.3/permmod/optimize.py`

 * *Files identical despite different names*

### Comparing `permmod-0.2/permmod/plots.py` & `permmod-0.3/permmod/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,40 @@
 class Plotter:
 
     def __init__(self, df, **kwargs):
         self.df = df
         for key, value in kwargs.items():
             setattr(self, key, value)
 
+    def guess_chart(self):
+        fig = make_subplots(specs=[[{'secondary_y': True}]])
+        # Add traces
+        fig.add_trace(
+            go.Scatter(x=self.df['Duration'], y=self.df['Inlet_Pressure'] * 1e-6, name='Eingangsdruck',
+                       line_color='blue'),
+            secondary_y=False)
+        fig.add_trace(
+            go.Scatter(x=self.df['Duration'], y=self.df['Outlet_Pressure'] * 1e-6, name='Ausgangsdruck',
+                       line_color='blue'),
+            secondary_y=False)
+        fig.add_trace(
+            go.Scatter(x=self.df['Duration'],
+                       y=self.df['Inlet_Pressure'] * 1e-6 - self.df['Outlet_Pressure'] * 1e-6,
+                       name='Differenzdruck', line_color='black', line_dash='dot'),
+            secondary_y=False)
+        fig.add_trace(
+            go.Scatter(x=self.df['Duration'], y=self.df['k'], name='Permeabilität', line_color='red', mode='markers'),
+            secondary_y=True)
+
+        fig.update_layout(xaxis=dict(showexponent='all', exponentformat='power'))
+        fig.update_xaxes(title_text='Messdauer in s', type='log', range=[1, 6])
+        fig.update_yaxes(title_text='Druck in MPa', secondary_y=False)
+        fig.update_yaxes(title_text='Permeabilität', secondary_y=True, type='log')
+        fig.show()
+
     def raw_data_chart(self):
         fig = make_subplots(specs=[[{'secondary_y': True}]])
         # Add traces
         fig.add_trace(
             go.Scatter(x=self.df['Duration'], y=self.df['Inlet_Pressure'] * 1e-6, name='Eingangsdruck',
                        line_color='blue'),
             secondary_y=False)
```

### Comparing `permmod-0.2/permmod.egg-info/PKG-INFO` & `permmod-0.3/permmod.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permmod
-Version: 0.2
+Version: 0.3
 Summary: A package to calculate the permeability of rock samples
 Author-email: Martin Kirch <mkirch@web.de>
 Project-URL: Homepage, https://github.com/kirchma/permmod
 Project-URL: Bug Tracker, https://github.com/kirchma/permmod/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,36 +17,39 @@
 
 permmod is a Python package that is used to calculate the permeability of two-chamber-method measurements.
 This type of measurement is based on Brace's pulse decay method and extends it to include pressure- and 
 temperature-dependent material parameters. More details are available in the following paper.
 
 ## How to use it.
 
-In order to use the package there must be a measurement, a database and a measurement_units file in the following 
+In order to use the package there must be a measurement-, a database- and a measurement_units-file in the following 
 folder structure:
 ```
 Measurements
 │   database.csv
 │   measurement_units.csv   
 │
 └───raw_data
 │   │   measurement_file1.txt
 │   │   ...
 │   
 └───sim_data
-    │
+│   │   ...
+│   
+└───pics
+│   │   ...
 ```
 
 An example of the structure of the folders and the 3 files is given in the **example folder**. 
 
 To evaluate a measurement, you can proceed as follows:
 ```sh
 from permmod import Measurement
 
-path = '/raw_data/measurement_file1.txt'
+path = 'raw_data/measurement_file1.txt'
 measurement = Measurement(path=path)
 measurement.calculate_permeability([1e-19, 0.001], parameter='both')
 ```
 For more information see the documentation
 
 ## Installation
 The source code is hosted on GitHub at:
```

### Comparing `permmod-0.2/pyproject.toml` & `permmod-0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "permmod"
-version = "0.2"
+version = "0.3"
 authors = [
   { name='Martin Kirch', email='mkirch@web.de' },
 ]
 description = "A package to calculate the permeability of rock samples"
 dependencies = ['pandas', 'numpy', 'CoolProp', 'scipy', 'plotly']
 readme = "README.md"
 requires-python = ">=3.11"
```


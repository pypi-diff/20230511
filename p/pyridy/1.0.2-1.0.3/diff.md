# Comparing `tmp/pyridy-1.0.2.tar.gz` & `tmp/pyridy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyridy-1.0.2.tar", max compression
+gzip compressed data, was "pyridy-1.0.3.tar", max compression
```

## Comparing `pyridy-1.0.2.tar` & `pyridy-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.2/LICENSE
--rw-r--r--   0        0        0      971 2023-05-02 13:38:35.459789 pyridy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.2/pyridy/__init__.py
--rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.2/pyridy/campaign.py
--rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.2/pyridy/config.py
--rw-r--r--   0        0        0    62789 2023-03-09 12:44:02.626960 pyridy-1.0.2/pyridy/file.py
--rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.2/pyridy/osm/__init__.py
--rw-r--r--   0        0        0    30598 2023-04-27 12:36:22.469380 pyridy-1.0.2/pyridy/osm/osm.py
--rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.2/pyridy/osm/utils/__init__.py
--rw-r--r--   0        0        0    12461 2023-04-27 12:36:22.472382 pyridy-1.0.2/pyridy/osm/utils/elements.py
--rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.2/pyridy/osm/utils/overpass.py
--rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.2/pyridy/osm/utils/query.py
--rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.2/pyridy/osm/utils/relation.py
--rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.2/pyridy/osm/utils/tools.py
--rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.2/pyridy/processing/__init__.py
--rw-r--r--   0        0        0    16957 2023-03-09 16:42:58.467625 pyridy-1.0.2/pyridy/processing/comfort.py
--rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.2/pyridy/processing/condition.py
--rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.2/pyridy/processing/excitation.py
--rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.2/pyridy/processing/processor.py
--rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.2/pyridy/utils/__init__.py
--rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.2/pyridy/utils/device.py
--rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.2/pyridy/utils/sensor.py
--rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.2/pyridy/utils/timeseries.py
--rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.2/pyridy/utils/tools.py
--rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.2/pyridy/widgets/__init__.py
--rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.2/pyridy/widgets/map.py
--rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.2/README.md
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 pyridy-1.0.2/setup.py
--rw-r--r--   0        0        0     3626 1970-01-01 00:00:00.000000 pyridy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.3/LICENSE
+-rw-r--r--   0        0        0      971 2023-05-11 13:19:47.076041 pyridy-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.3/pyridy/__init__.py
+-rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.3/pyridy/campaign.py
+-rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.3/pyridy/config.py
+-rw-r--r--   0        0        0    62789 2023-03-09 12:44:02.626960 pyridy-1.0.3/pyridy/file.py
+-rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.3/pyridy/osm/__init__.py
+-rw-r--r--   0        0        0    30598 2023-04-27 12:36:22.469380 pyridy-1.0.3/pyridy/osm/osm.py
+-rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.3/pyridy/osm/utils/__init__.py
+-rw-r--r--   0        0        0    12461 2023-04-27 12:36:22.472382 pyridy-1.0.3/pyridy/osm/utils/elements.py
+-rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.3/pyridy/osm/utils/overpass.py
+-rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.3/pyridy/osm/utils/query.py
+-rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.3/pyridy/osm/utils/relation.py
+-rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.3/pyridy/osm/utils/tools.py
+-rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.3/pyridy/processing/__init__.py
+-rw-r--r--   0        0        0    16957 2023-03-09 16:42:58.467625 pyridy-1.0.3/pyridy/processing/comfort.py
+-rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.3/pyridy/processing/condition.py
+-rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.3/pyridy/processing/excitation.py
+-rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.3/pyridy/processing/processor.py
+-rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.3/pyridy/utils/__init__.py
+-rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.3/pyridy/utils/device.py
+-rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.3/pyridy/utils/sensor.py
+-rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.3/pyridy/utils/timeseries.py
+-rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.3/pyridy/utils/tools.py
+-rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.3/pyridy/widgets/__init__.py
+-rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.3/pyridy/widgets/map.py
+-rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.3/README.md
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 pyridy-1.0.3/setup.py
+-rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 pyridy-1.0.3/PKG-INFO
```

### Comparing `pyridy-1.0.2/LICENSE` & `pyridy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyproject.toml` & `pyridy-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyridy"
-version = "1.0.2"
+version = "1.0.3"
 description = "Support library for measurements made with the Ridy Android App"
 authors = ["Philipp Simon Leibner <philipp.leibner@ifs.rwth-aachen.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 classifiers = [
     "Topic :: Scientific/Engineering :: Information Analysis",
@@ -14,15 +14,15 @@
 keywords = ["signal processing", "ridy", "android"]
 
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8, <3.11"
+python = "^3.8, <3.12"
 pytest = "^7.1.1"
 numpy = "^1.21.5"
 requests = "^2.28.1"
 pandas = "^1.2.0"
 matplotlib = "^3.4.1"
 tqdm = "^4.60.0"
 overpy = "^0.6"
```

### Comparing `pyridy-1.0.2/pyridy/campaign.py` & `pyridy-1.0.3/pyridy/campaign.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/config.py` & `pyridy-1.0.3/pyridy/config.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/file.py` & `pyridy-1.0.3/pyridy/file.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/osm/osm.py` & `pyridy-1.0.3/pyridy/osm/osm.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/osm/utils/elements.py` & `pyridy-1.0.3/pyridy/osm/utils/elements.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/osm/utils/overpass.py` & `pyridy-1.0.3/pyridy/osm/utils/overpass.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/osm/utils/query.py` & `pyridy-1.0.3/pyridy/osm/utils/query.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/osm/utils/tools.py` & `pyridy-1.0.3/pyridy/osm/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/processing/comfort.py` & `pyridy-1.0.3/pyridy/processing/comfort.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/processing/condition.py` & `pyridy-1.0.3/pyridy/processing/condition.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/processing/excitation.py` & `pyridy-1.0.3/pyridy/processing/excitation.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/utils/device.py` & `pyridy-1.0.3/pyridy/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/utils/sensor.py` & `pyridy-1.0.3/pyridy/utils/sensor.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/utils/timeseries.py` & `pyridy-1.0.3/pyridy/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/utils/tools.py` & `pyridy-1.0.3/pyridy/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/pyridy/widgets/map.py` & `pyridy-1.0.3/pyridy/widgets/map.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/README.md` & `pyridy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.2/setup.py` & `pyridy-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,23 +28,23 @@
  'requests>=2.28.1,<3.0.0',
  'rwthcolors>=0.2.3,<0.3.0',
  'scipy>=1.6.3,<2.0.0',
  'tqdm>=4.60.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pyridy',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'Support library for measurements made with the Ridy Android App',
     'long_description': '# PyRidy\n\n![alt text](assets/ic_launcher.png "PyRidy Logo")\n\nPython Support Library to import and process Ridy files\n\n### About Ridy\nRidy is an Android App to record sensor data for uses in science and engineering. The app is currently actively being \ndeveloped at the [Chair and Institute for Rail Vehicles and Transport Systems (IFS)](http://www.ifs.rwth-aachen.de/en/start/)\n\n<img src="assets/screenshot.png" alt="Ridy Screenshot" width="200"/>\n\nAt the institute Ridy is e.g. used for condition monitoring of railway tracks and several more use-cases are currently\nresearched upon.\nAmong other, Ridy can record:\n* Acceleration\n* Linear Acceleration (i.e., without g-Force)\n* Magnetic Field\n* Gyroscope\n* Orientation\n* GNSS Location (+ Android Raw GNSS Measurements)\n* Pressure, Humidity, Temperature, Ambient Light\n\nCompared to other existing apps Ridy can perform long measurements even in the background when the phone is locked.\nThe app supports two formats for data export, JSON and SQLITE. If you would like to use or try out the app please contact the\ndeveloper (see below) to get access.\n\n### About PyRidy\nPyRidy is the companion python library for the Ridy Android App. It provides easy access to the data no matter which\nrecording format was used. If pyridy is used, one does no longer need to manually write code to import the files.\n\nIn addition, pyridy provides several more features:\n* Automatic conversion of sensor data into objects and numpy arrays\n* Conversion of arrays to Pandas DataFrame objects\n* Time synchronization of individual files (e.g. from different phones)\n* Download of OSM Railway Data via the Overpass API\n* Plotting of GPS tracks onto a map using ipyleaflet\n\n### Documentation\n[PyRidy Documentation](https://pyridy.readthedocs.io/)\n#### Installation\n\nInstall using pip\n```python\n    pip install pyridy\n```\n\n#### Usage\n\nInformation and examples on how to use the library can be found in the [PyRidy documentation](https://pyridy.readthedocs.io/)\n\n### Creator\nPhilipp Leibner - philipp.leibner@ifs.rwth-aachen.de\n\n### Contributor\nDaniel Pujiula Buhl - daniel.pujiula@rwth-aachen.de\nSarra Bouchkati - sarra.bouchkati@rwth-aachen.de\n\n<div>  \n<a href="">\n    <img src="assets/ifs_logo_rgb.svg" alt="IFS Logo" width="400">\n  </a>\n</div>\n',
     'author': 'Philipp Simon Leibner',
     'author_email': 'philipp.leibner@ifs.rwth-aachen.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'pyridy.osm', 'pyridy.osm.utils', 'pyridy.processing', 'pyridy.utils',
 'pyridy.widgets'] package_data = \ {'': ['*']} install_requires = \
 ['HeapDict>=1.0.1,<2.0.0', 'Shapely>=1.8.1,<2.0.0', 'geopy>=2.1.0,<3.0.0',
 'ipyleaflet>=0.17.0,<0.18.0', 'matplotlib>=3.4.1,<4.0.0', 'networkx>=3.1,<4.0',
 'numpy>=1.21.5,<2.0.0', 'overpy>=0.6,<0.7', 'pandas>=1.2.0,<2.0.0',
 'pyproj>=3.3.0,<4.0.0', 'pytest>=7.1.1,<8.0.0', 'requests-cache>=1.0.1,<2.0.0',
 'requests>=2.28.1,<3.0.0', 'rwthcolors>=0.2.3,<0.3.0', 'scipy>=1.6.3,<2.0.0',
-'tqdm>=4.60.0,<5.0.0'] setup_kwargs = { 'name': 'pyridy', 'version': '1.0.2',
+'tqdm>=4.60.0,<5.0.0'] setup_kwargs = { 'name': 'pyridy', 'version': '1.0.3',
 'description': 'Support library for measurements made with the Ridy Android
 App', 'long_description': '# PyRidy\n\n![alt text](assets/ic_launcher.png
 "PyRidy Logo")\n\nPython Support Library to import and process Ridy
 files\n\n### About Ridy\nRidy is an Android App to record sensor data for uses
 in science and engineering. The app is currently actively being \ndeveloped at
 the [Chair and Institute for Rail Vehicles and Transport Systems (IFS)](http://
 www.ifs.rwth-aachen.de/en/start/)\n\n[Ridy Screenshot]\n\nAt the institute Ridy
@@ -38,9 +38,9 @@
 philipp.leibner@ifs.rwth-aachen.de\n\n### Contributor\nDaniel Pujiula Buhl -
 daniel.pujiula@rwth-aachen.de\nSarra Bouchkati - sarra.bouchkati@rwth-
 aachen.de\n\n
 \n\n [IFS Logo]\n\n
 \n', 'author': 'Philipp Simon Leibner', 'author_email':
 'philipp.leibner@ifs.rwth-aachen.de', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<3.11', } setup
+'install_requires': install_requires, 'python_requires': '>=3.8,<3.12', } setup
 (**setup_kwargs)
```

### Comparing `pyridy-1.0.2/PKG-INFO` & `pyridy-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyridy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Support library for measurements made with the Ridy Android App
 License: Apache-2.0
 Keywords: signal processing,ridy,android
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: HeapDict (>=1.0.1,<2.0.0)
 Requires-Dist: Shapely (>=1.8.1,<2.0.0)
 Requires-Dist: geopy (>=2.1.0,<3.0.0)
 Requires-Dist: ipyleaflet (>=0.17.0,<0.18.0)
 Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1 Name: pyridy Version: 1.0.2 Summary: Support library for
+Metadata-Version: 2.1 Name: pyridy Version: 1.0.3 Summary: Support library for
 measurements made with the Ridy Android App License: Apache-2.0 Keywords:
 signal processing,ridy,android Author: Philipp Simon Leibner Author-email:
-philipp.leibner@ifs.rwth-aachen.de Requires-Python: >=3.8,<3.11 Classifier:
+philipp.leibner@ifs.rwth-aachen.de Requires-Python: >=3.8,<3.12 Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Information Analysis Requires-
-Dist: HeapDict (>=1.0.1,<2.0.0) Requires-Dist: Shapely (>=1.8.1,<2.0.0)
-Requires-Dist: geopy (>=2.1.0,<3.0.0) Requires-Dist: ipyleaflet
-(>=0.17.0,<0.18.0) Requires-Dist: matplotlib (>=3.4.1,<4.0.0) Requires-Dist:
-networkx (>=3.1,<4.0) Requires-Dist: numpy (>=1.21.5,<2.0.0) Requires-Dist:
-overpy (>=0.6,<0.7) Requires-Dist: pandas (>=1.2.0,<2.0.0) Requires-Dist:
-pyproj (>=3.3.0,<4.0.0) Requires-Dist: pytest (>=7.1.1,<8.0.0) Requires-Dist:
-requests (>=2.28.1,<3.0.0) Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: rwthcolors (>=0.2.3,<0.3.0) Requires-Dist: scipy
-(>=1.6.3,<2.0.0) Requires-Dist: tqdm (>=4.60.0,<5.0.0) Description-Content-
-Type: text/markdown # PyRidy ![alt text](assets/ic_launcher.png "PyRidy Logo")
-Python Support Library to import and process Ridy files ### About Ridy Ridy is
-an Android App to record sensor data for uses in science and engineering. The
-app is currently actively being developed at the [Chair and Institute for Rail
-Vehicles and Transport Systems (IFS)](http://www.ifs.rwth-aachen.de/en/start/)
-[Ridy Screenshot] At the institute Ridy is e.g. used for condition monitoring
-of railway tracks and several more use-cases are currently researched upon.
-Among other, Ridy can record: * Acceleration * Linear Acceleration (i.e.,
-without g-Force) * Magnetic Field * Gyroscope * Orientation * GNSS Location (+
-Android Raw GNSS Measurements) * Pressure, Humidity, Temperature, Ambient Light
-Compared to other existing apps Ridy can perform long measurements even in the
-background when the phone is locked. The app supports two formats for data
-export, JSON and SQLITE. If you would like to use or try out the app please
-contact the developer (see below) to get access. ### About PyRidy PyRidy is the
-companion python library for the Ridy Android App. It provides easy access to
-the data no matter which recording format was used. If pyridy is used, one does
-no longer need to manually write code to import the files. In addition, pyridy
-provides several more features: * Automatic conversion of sensor data into
-objects and numpy arrays * Conversion of arrays to Pandas DataFrame objects *
-Time synchronization of individual files (e.g. from different phones) *
-Download of OSM Railway Data via the Overpass API * Plotting of GPS tracks onto
-a map using ipyleaflet ### Documentation [PyRidy Documentation](https://
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering :: Information Analysis Requires-Dist: HeapDict
+(>=1.0.1,<2.0.0) Requires-Dist: Shapely (>=1.8.1,<2.0.0) Requires-Dist: geopy
+(>=2.1.0,<3.0.0) Requires-Dist: ipyleaflet (>=0.17.0,<0.18.0) Requires-Dist:
+matplotlib (>=3.4.1,<4.0.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist:
+numpy (>=1.21.5,<2.0.0) Requires-Dist: overpy (>=0.6,<0.7) Requires-Dist:
+pandas (>=1.2.0,<2.0.0) Requires-Dist: pyproj (>=3.3.0,<4.0.0) Requires-Dist:
+pytest (>=7.1.1,<8.0.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-
+Dist: requests-cache (>=1.0.1,<2.0.0) Requires-Dist: rwthcolors
+(>=0.2.3,<0.3.0) Requires-Dist: scipy (>=1.6.3,<2.0.0) Requires-Dist: tqdm
+(>=4.60.0,<5.0.0) Description-Content-Type: text/markdown # PyRidy ![alt text]
+(assets/ic_launcher.png "PyRidy Logo") Python Support Library to import and
+process Ridy files ### About Ridy Ridy is an Android App to record sensor data
+for uses in science and engineering. The app is currently actively being
+developed at the [Chair and Institute for Rail Vehicles and Transport Systems
+(IFS)](http://www.ifs.rwth-aachen.de/en/start/) [Ridy Screenshot] At the
+institute Ridy is e.g. used for condition monitoring of railway tracks and
+several more use-cases are currently researched upon. Among other, Ridy can
+record: * Acceleration * Linear Acceleration (i.e., without g-Force) * Magnetic
+Field * Gyroscope * Orientation * GNSS Location (+ Android Raw GNSS
+Measurements) * Pressure, Humidity, Temperature, Ambient Light Compared to
+other existing apps Ridy can perform long measurements even in the background
+when the phone is locked. The app supports two formats for data export, JSON
+and SQLITE. If you would like to use or try out the app please contact the
+developer (see below) to get access. ### About PyRidy PyRidy is the companion
+python library for the Ridy Android App. It provides easy access to the data no
+matter which recording format was used. If pyridy is used, one does no longer
+need to manually write code to import the files. In addition, pyridy provides
+several more features: * Automatic conversion of sensor data into objects and
+numpy arrays * Conversion of arrays to Pandas DataFrame objects * Time
+synchronization of individual files (e.g. from different phones) * Download of
+OSM Railway Data via the Overpass API * Plotting of GPS tracks onto a map using
+ipyleaflet ### Documentation [PyRidy Documentation](https://
 pyridy.readthedocs.io/) #### Installation Install using pip ```python pip
 install pyridy ``` #### Usage Information and examples on how to use the
 library can be found in the [PyRidy documentation](https://
 pyridy.readthedocs.io/) ### Creator Philipp Leibner - philipp.leibner@ifs.rwth-
 aachen.de ### Contributor Daniel Pujiula Buhl - daniel.pujiula@rwth-aachen.de
 Sarra Bouchkati - sarra.bouchkati@rwth-aachen.de
 [IFS Logo]
```


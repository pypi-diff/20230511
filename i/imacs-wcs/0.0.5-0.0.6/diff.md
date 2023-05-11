# Comparing `tmp/imacs_wcs-0.0.5.tar.gz` & `tmp/imacs_wcs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imacs_wcs-0.0.5.tar", last modified: Thu May 11 16:37:46 2023, max compression
+gzip compressed data, was "imacs_wcs-0.0.6.tar", last modified: Thu May 11 16:42:48 2023, max compression
```

## Comparing `imacs_wcs-0.0.5.tar` & `imacs_wcs-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-11 16:37:46.837704 imacs_wcs-0.0.5/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      779 2023-05-11 16:37:46.837704 imacs_wcs-0.0.5/PKG-INFO
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-11 16:37:46.837704 imacs_wcs-0.0.5/imacs_wcs/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:12:38.761607 imacs_wcs-0.0.5/imacs_wcs/__init__.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      843 2023-05-10 14:26:51.861324 imacs_wcs-0.0.5/imacs_wcs/chip.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2144 2023-05-10 15:11:54.666085 imacs_wcs-0.0.5/imacs_wcs/draggable_scatter.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     5753 2023-05-10 15:44:02.256229 imacs_wcs-0.0.5/imacs_wcs/header_reader.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      766 2023-05-10 15:25:20.188957 imacs_wcs-0.0.5/imacs_wcs/imacs_wcs.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      270 2023-05-10 15:12:40.853585 imacs_wcs-0.0.5/imacs_wcs/instrument_constants.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)    10877 2023-05-11 16:36:00.810692 imacs_wcs-0.0.5/imacs_wcs/manual_astrometry.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2150 2023-05-10 15:44:28.207938 imacs_wcs-0.0.5/imacs_wcs/semi_auto_astrometry.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-10 15:12:50.089484 imacs_wcs-0.0.5/setup.cfg
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1198 2023-05-11 16:35:54.362753 imacs_wcs-0.0.5/setup.py
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-11 16:42:48.918975 imacs_wcs-0.0.6/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      779 2023-05-11 16:42:48.918975 imacs_wcs-0.0.6/PKG-INFO
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-11 16:42:48.918975 imacs_wcs-0.0.6/imacs_wcs/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:12:38.761607 imacs_wcs-0.0.6/imacs_wcs/__init__.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      843 2023-05-10 14:26:51.861324 imacs_wcs-0.0.6/imacs_wcs/chip.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2144 2023-05-10 15:11:54.666085 imacs_wcs-0.0.6/imacs_wcs/draggable_scatter.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     5753 2023-05-10 15:44:02.256229 imacs_wcs-0.0.6/imacs_wcs/header_reader.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      766 2023-05-10 15:25:20.188957 imacs_wcs-0.0.6/imacs_wcs/imacs_wcs.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      270 2023-05-10 15:12:40.853585 imacs_wcs-0.0.6/imacs_wcs/instrument_constants.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)    10979 2023-05-11 16:41:17.239793 imacs_wcs-0.0.6/imacs_wcs/manual_astrometry.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2150 2023-05-10 15:44:28.207938 imacs_wcs-0.0.6/imacs_wcs/semi_auto_astrometry.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-10 15:12:50.089484 imacs_wcs-0.0.6/setup.cfg
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1198 2023-05-11 16:41:55.015455 imacs_wcs-0.0.6/setup.py
```

### Comparing `imacs_wcs-0.0.5/PKG-INFO` & `imacs_wcs-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: imacs_wcs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library for determining and writing wcs information for IMACS images.
 Home-page: https://github.com/TrystanScottLambert
 Author: Trystan Scott Lambert
 Author-email: trystanscottlambert@gmail.com
 License: MIT
-Download-URL: https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.5.tar.gz
+Download-URL: https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.6.tar.gz
 Description: UNKNOWN
 Keywords: astronomy,wcs,imacs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imacs_wcs-0.0.5/imacs_wcs/chip.py` & `imacs_wcs-0.0.6/imacs_wcs/chip.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.5/imacs_wcs/draggable_scatter.py` & `imacs_wcs-0.0.6/imacs_wcs/draggable_scatter.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.5/imacs_wcs/header_reader.py` & `imacs_wcs-0.0.6/imacs_wcs/header_reader.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.5/imacs_wcs/imacs_wcs.py` & `imacs_wcs-0.0.6/imacs_wcs/imacs_wcs.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.5/imacs_wcs/manual_astrometry.py` & `imacs_wcs-0.0.6/imacs_wcs/manual_astrometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,20 +141,19 @@
     def query_gaia(self):
         """Gets the gaia positions in the chip frame."""
         center_y_pix = self.data.shape[0]/2
         center_x_pix = self.data.shape[1]/2
 
         # Assuming square pixels.
         if np.abs(self.header['PC1_1']) >= np.abs(self.header['PC1_2']):
-            keyword = 'PC1_1'
+            search_width = self.data.shape[1] * np.abs(self.header['PC1_1'])
+            search_height = self.data.shape[0] * np.abs(self.header['PC1_1'])
         else:
-            keyword = 'PC1_2'
-
-        search_width = self.data.shape[1] * np.abs(self.header[keyword])
-        search_height = self.data.shape[0] * np.abs(self.header[keyword])
+            search_height = self.data.shape[1] * np.abs(self.header['PC1_2'])
+            search_width = self.data.shape[0] * np.abs(self.header['PC1_2'])
 
         center_ra, center_dec = self.current_wcs.pixel_to_world_values(center_x_pix, center_y_pix)
         gaia_ra, gaia_dec = search_gaia_archives(
             center_ra, center_dec, width = search_width, height=search_height)
         gaia_x, gaia_y = self.current_wcs.world_to_pixel_values(gaia_ra, gaia_dec)
 
         return gaia_ra, gaia_dec, gaia_x, gaia_y
```

### Comparing `imacs_wcs-0.0.5/imacs_wcs/semi_auto_astrometry.py` & `imacs_wcs-0.0.6/imacs_wcs/semi_auto_astrometry.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.5/setup.py` & `imacs_wcs-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'imacs_wcs',
   packages = ['imacs_wcs'],
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Library for determining and writing wcs information for IMACS images.',
   author = 'Trystan Scott Lambert',
   author_email = 'trystanscottlambert@gmail.com',
   url = 'https://github.com/TrystanScottLambert',
-  download_url = 'https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.5.tar.gz',
+  download_url = 'https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.6.tar.gz',
   keywords = ['astronomy', 'wcs', 'imacs'],
   install_requires=[
     'numpy',
     'photutils',
     'astropy',
     'scipy',
     'matplotlib',
```


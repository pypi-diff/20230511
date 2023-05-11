# Comparing `tmp/lisflood-utilities-0.8.tar.gz` & `tmp/lisflood-utilities-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lisflood-utilities-0.8.tar", last modified: Fri Dec  6 13:07:55 2019, max compression
+gzip compressed data, was "dist/lisflood-utilities-0.9.tar", last modified: Wed Dec 11 09:07:45 2019, max compression
```

## Comparing `lisflood-utilities-0.8.tar` & `lisflood-utilities-0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/bin/
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)      313 2019-10-11 09:43:34.000000 lisflood-utilities-0.8/bin/compare
--rwxrwxr-x   0 nappodo   (1006) nappodo  (23911)      327 2019-08-30 13:55:10.000000 lisflood-utilities-0.8/bin/cutmaps
--rwxrwxr-x   0 nappodo   (1006) nappodo  (23911)      312 2019-08-30 13:55:10.000000 lisflood-utilities-0.8/bin/pcr2nc
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/src/
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/src/lisflood_utilities.egg-info/
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    14996 2019-12-06 13:07:54.000000 lisflood-utilities-0.8/src/lisflood_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)      814 2019-12-06 13:07:54.000000 lisflood-utilities-0.8/src/lisflood_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        1 2019-12-06 13:07:54.000000 lisflood-utilities-0.8/src/lisflood_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       53 2019-12-06 13:07:54.000000 lisflood-utilities-0.8/src/lisflood_utilities.egg-info/requires.txt
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       18 2019-12-06 13:07:54.000000 lisflood-utilities-0.8/src/lisflood_utilities.egg-info/top_level.txt
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        1 2019-11-29 08:21:50.000000 lisflood-utilities-0.8/src/lisflood_utilities.egg-info/zip-safe
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/src/lisfloodutilities/
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/src/lisfloodutilities/compare/
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     5620 2019-12-06 12:59:40.000000 lisflood-utilities-0.8/src/lisfloodutilities/compare/__init__.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)      529 2019-11-13 15:24:42.000000 lisflood-utilities-0.8/src/lisfloodutilities/compare/helpers.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     1622 2019-11-13 15:24:42.000000 lisflood-utilities-0.8/src/lisfloodutilities/compare/main.py
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/src/lisfloodutilities/cutmaps/
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        0 2019-08-12 13:11:48.000000 lisflood-utilities-0.8/src/lisfloodutilities/cutmaps/__init__.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     4818 2019-09-12 08:27:48.000000 lisflood-utilities-0.8/src/lisfloodutilities/cutmaps/cutlib.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     4140 2019-09-12 08:27:48.000000 lisflood-utilities-0.8/src/lisfloodutilities/cutmaps/main.py
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/src/lisfloodutilities/pcr2nc/
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        0 2019-08-12 13:11:48.000000 lisflood-utilities-0.8/src/lisfloodutilities/pcr2nc/__init__.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     2893 2019-12-03 10:57:25.000000 lisflood-utilities-0.8/src/lisfloodutilities/pcr2nc/main.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    12298 2019-12-06 12:58:01.000000 lisflood-utilities-0.8/src/lisfloodutilities/pcr2nc/writer.py
-drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/src/lisfloodutilities/readers/
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       45 2019-12-06 10:55:16.000000 lisflood-utilities-0.8/src/lisfloodutilities/readers/__init__.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     6349 2019-12-06 12:35:55.000000 lisflood-utilities-0.8/src/lisfloodutilities/readers/pcr.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        0 2019-08-12 13:11:48.000000 lisflood-utilities-0.8/src/lisfloodutilities/__init__.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       16 2019-08-30 13:45:34.000000 lisflood-utilities-0.8/MANIFEST.in
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    11528 2019-08-30 14:13:27.000000 lisflood-utilities-0.8/README.md
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        4 2019-12-06 13:07:05.000000 lisflood-utilities-0.8/VERSION
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     4566 2019-11-13 15:29:29.000000 lisflood-utilities-0.8/setup.py
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    14996 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/PKG-INFO
--rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       38 2019-12-06 13:07:55.000000 lisflood-utilities-0.8/setup.cfg
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/bin/
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)      313 2019-10-11 09:43:34.000000 lisflood-utilities-0.9/bin/compare
+-rwxrwxr-x   0 nappodo   (1006) nappodo  (23911)      327 2019-08-30 13:55:10.000000 lisflood-utilities-0.9/bin/cutmaps
+-rwxrwxr-x   0 nappodo   (1006) nappodo  (23911)      312 2019-08-30 13:55:10.000000 lisflood-utilities-0.9/bin/pcr2nc
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/src/
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/src/lisflood_utilities.egg-info/
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    14996 2019-12-11 09:07:43.000000 lisflood-utilities-0.9/src/lisflood_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)      814 2019-12-11 09:07:43.000000 lisflood-utilities-0.9/src/lisflood_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        1 2019-12-11 09:07:43.000000 lisflood-utilities-0.9/src/lisflood_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       53 2019-12-11 09:07:43.000000 lisflood-utilities-0.9/src/lisflood_utilities.egg-info/requires.txt
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       18 2019-12-11 09:07:43.000000 lisflood-utilities-0.9/src/lisflood_utilities.egg-info/top_level.txt
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        1 2019-11-29 08:21:50.000000 lisflood-utilities-0.9/src/lisflood_utilities.egg-info/zip-safe
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/src/lisfloodutilities/
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/src/lisfloodutilities/compare/
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     5757 2019-12-10 16:27:48.000000 lisflood-utilities-0.9/src/lisfloodutilities/compare/__init__.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)      529 2019-11-13 15:24:42.000000 lisflood-utilities-0.9/src/lisfloodutilities/compare/helpers.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     1622 2019-11-13 15:24:42.000000 lisflood-utilities-0.9/src/lisfloodutilities/compare/main.py
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/src/lisfloodutilities/cutmaps/
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        0 2019-08-12 13:11:48.000000 lisflood-utilities-0.9/src/lisfloodutilities/cutmaps/__init__.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     4818 2019-09-12 08:27:48.000000 lisflood-utilities-0.9/src/lisfloodutilities/cutmaps/cutlib.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     4140 2019-09-12 08:27:48.000000 lisflood-utilities-0.9/src/lisfloodutilities/cutmaps/main.py
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/src/lisfloodutilities/pcr2nc/
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        0 2019-08-12 13:11:48.000000 lisflood-utilities-0.9/src/lisfloodutilities/pcr2nc/__init__.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     2893 2019-12-03 10:57:25.000000 lisflood-utilities-0.9/src/lisfloodutilities/pcr2nc/main.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    12415 2019-12-09 15:19:23.000000 lisflood-utilities-0.9/src/lisfloodutilities/pcr2nc/writer.py
+drwxrwxr-x   0 nappodo   (1006) nappodo  (23911)        0 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/src/lisfloodutilities/readers/
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       45 2019-12-06 10:55:16.000000 lisflood-utilities-0.9/src/lisfloodutilities/readers/__init__.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     6349 2019-12-06 12:35:55.000000 lisflood-utilities-0.9/src/lisfloodutilities/readers/pcr.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        0 2019-08-12 13:11:48.000000 lisflood-utilities-0.9/src/lisfloodutilities/__init__.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       16 2019-08-30 13:45:34.000000 lisflood-utilities-0.9/MANIFEST.in
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    11528 2019-08-30 14:13:27.000000 lisflood-utilities-0.9/README.md
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)        4 2019-12-11 09:06:47.000000 lisflood-utilities-0.9/VERSION
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)     4566 2019-11-13 15:29:29.000000 lisflood-utilities-0.9/setup.py
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)    14996 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/PKG-INFO
+-rw-rw-r--   0 nappodo   (1006) nappodo  (23911)       38 2019-12-11 09:07:45.000000 lisflood-utilities-0.9/setup.cfg
```

### Comparing `lisflood-utilities-0.8/src/lisflood_utilities.egg-info/PKG-INFO` & `lisflood-utilities-0.9/src/lisflood_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisflood-utilities
-Version: 0.8
+Version: 0.9
 Summary: A set of utilities for lisfloodutilities users. pcr2nc: Convert PCRaster files to netCDF; cutmaps: cut netCDF files;compare: to compare two set of netcdf files
 Home-page: https://github.com/ec-jrc/lisflood-utilities
 Author: Valerio Lorini, Domenico Nappo, Lorenzo Alfieri
 Author-email: valerio.lorini@ec.europa.eu,domenico.nappo@gmail.com,lorenzo.alfieri@ec.europa.eu
 License: EUPL 1.2
 Description: # Lisflood Utilities
```

### Comparing `lisflood-utilities-0.8/src/lisflood_utilities.egg-info/SOURCES.txt` & `lisflood-utilities-0.9/src/lisflood_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/compare/__init__.py` & `lisflood-utilities-0.9/src/lisfloodutilities/compare/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         path_a = Path(path_a)
         path_b = Path(path_b)
         for fa in itertools.chain(*(path_a.glob(e) for e in self.glob_expr)):
             fb = path_b.joinpath(fa.name)
             if not fb.exists():
                 logger.info('skipping %s as it is not in %s', fb.name, path_b.as_posix())
                 continue
-            errors = self.compare_files(fa, fb)
+            errors = self.compare_files(fa.as_posix(), fb.as_posix())
             if errors:
                 self.errors += errors
         return self.errors
 
     def compare_files(self, fa, fb):
         raise NotImplementedError()
 
@@ -67,23 +67,23 @@
                     return None
 
 
 class NetCDFComparator(Comparator):
     glob_expr = ['**/*.nc']
 
     def __init__(self, mask, atol=0.05, rtol=0.1, max_perc_diff=0.2, max_perc_large_diff=0.1):
+        super().__init__()
         self.mask = Dataset(mask)
         maskvar = [k for k in self.mask.variables if len(self.mask.variables[k].dimensions) == 2][0]
         self.maskarea = np.logical_not(self.mask.variables[maskvar][:, :])
         self.atol = atol
         self.rtol = rtol
         self.max_perc_large_diff = max_perc_large_diff
         self.max_perc_diff = max_perc_diff
         self.large_diff_th = self.atol * 10
-        super().__init__()
 
     def check_vars(self, maskarea, step, vara_step, varb_step, varname, filepath):
         step = step if step is not None else '(no time)'
         filepath = os.path.basename(filepath)
         vara_step = np.ma.masked_array(vara_step, maskarea)
         varb_step = np.ma.masked_array(varb_step, maskarea)
         vara_step = np.ma.compressed(vara_step).astype('float64')
@@ -102,36 +102,34 @@
                 rel_diff = np.array_str(rel_diff)
                 logger.error(f'Var: {varname} - STEP {step}: {perc_wrong:3.2f}% of values are different. max diff: {max_diff:3.2f} (rel diff: {rel_diff}%)')
                 logger.error('\nA: %s\nB: %s', np.array_str(vara_step[result]), np.array_str(varb_step[result]))
                 return f'{filepath}/{varname}/{step} - {perc_wrong:3.2f}% of different values - max diff: {max_diff:3.2f} (rel diff: {rel_diff}%)'
 
     def compare_files(self, file_a, file_b):
         errors = []
-        nca = Dataset(file_a)
-        ncb = Dataset(file_b)
-        num_dims = 3 if 'time' in nca.variables else 2
-        var_name = [k for k in nca.variables if len(nca.variables[k].dimensions) == num_dims][0]
-        vara = nca.variables[var_name]
-        varb = ncb.variables[var_name]
-        if 'time' in nca.variables:
-            stepsa = nca.variables['time'][:]
-            stepsb = ncb.variables['time'][:]
-            if len(stepsa) != len(stepsb):
-                logger.error('Different number of timesteps')
-                len_stepsa = len(stepsa)
-                len_stepsb = len(stepsb)
-                return f'Files: {file_a} vs {file_b}: different size in time axis A:{len_stepsa} B:{len_stepsb}'
-            for i, step in enumerate(stepsa):
-                vara_step = vara[i][:, :]
-                varb_step = varb[i][:, :]
-                err = self.check_vars(self.maskarea, i, vara_step, varb_step, var_name, file_a)
+        logger.info('Comparing %s and %s', file_a, file_b)
+        with Dataset(file_a)as nca, Dataset(file_b) as ncb:
+            num_dims = 3 if 'time' in nca.variables else 2
+            var_name = [k for k in nca.variables if len(nca.variables[k].dimensions) == num_dims][0]
+            vara = nca.variables[var_name]
+            varb = ncb.variables[var_name]
+            if 'time' in nca.variables:
+                stepsa = nca.variables['time'][:]
+                stepsb = ncb.variables['time'][:]
+                if len(stepsa) != len(stepsb):
+                    logger.error('Different number of timesteps')
+                    len_stepsa = len(stepsa)
+                    len_stepsb = len(stepsb)
+                    return f'Files: {file_a} vs {file_b}: different size in time axis A:{len_stepsa} B:{len_stepsb}'
+                for i, step in enumerate(stepsa):
+                    vara_step = vara[i][:, :]
+                    varb_step = varb[i][:, :]
+                    err = self.check_vars(self.maskarea, i, vara_step, varb_step, var_name, file_a)
+                    if err:
+                        errors.append(err)
+            else:
+                vara_step = vara[:, :]
+                varb_step = varb[:, :]
+                err = self.check_vars(self.maskarea, None, vara_step, varb_step, var_name, file_a)
                 if err:
                     errors.append(err)
-        else:
-            vara_step = vara[:, :]
-            varb_step = varb[:, :]
-            err = self.check_vars(self.maskarea, None, vara_step, varb_step, var_name, file_a)
-            if err:
-                errors.append(err)
-        nca.close()
-        ncb.close()
         return errors
```

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/compare/helpers.py` & `lisflood-utilities-0.9/src/lisfloodutilities/compare/helpers.py`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/compare/main.py` & `lisflood-utilities-0.9/src/lisfloodutilities/compare/main.py`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/cutmaps/cutlib.py` & `lisflood-utilities-0.9/src/lisfloodutilities/cutmaps/cutlib.py`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/cutmaps/main.py` & `lisflood-utilities-0.9/src/lisfloodutilities/cutmaps/main.py`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/pcr2nc/main.py` & `lisflood-utilities-0.9/src/lisfloodutilities/pcr2nc/main.py`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/pcr2nc/writer.py` & `lisflood-utilities-0.9/src/lisfloodutilities/pcr2nc/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 See the Licence for the specific language governing permissions and limitations under the Licence.
 
 Module containing the code for the NetCDFWriter class
 """
 
 import datetime
 import time
+import logging
 
 import numpy as np
 from netCDF4 import Dataset
 
 from lisfloodutilities.readers import PCRasterReader
 
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger()
+
 
 class NetCDFWriter:
     """
     This class manages all aspects concerning definition and writing of a NetCDF4 file.
     """
 
     FORMATS = {'classic': 'NETCDF4_CLASSIC', 'normal': 'NETCDF4'}
@@ -96,15 +100,15 @@
             time_nc.calendar = self.nc_metadata['time'].get('calendar', 'proleptic_gregorian')
             vardimensions = ('time', 'lat', 'lon')
 
         # data variable
         complevel = self.nc_metadata['variable'].get('compression')
         additional_args = {'zlib': bool(complevel)}
         if complevel:
-            print('Applying compression level', str(complevel))
+            logger.info('Applying compression level %s', str(complevel))
             additional_args['complevel'] = complevel
             if np.issubdtype(self.pcr_metadata['dtype'], np.floating):
                 additional_args['least_significant_digit'] = self.nc_metadata.get('least_significant_digit')
 
         values_nc = self.nf.createVariable(self.nc_metadata['variable'].get('shortname', ''),
                                            self.pcr_metadata['dtype'], vardimensions,
                                            fill_value=self.mv, **additional_args)
@@ -118,25 +122,25 @@
     def add_to_stack(self, pcr_map, time_step=None):
         """
         Add a PCRaster map to the NetCDF4 file.
         :param time_step: int, it's basically the extension of pcraster map file
             For single files (ie not time series) time_step is None
         :param pcr_map: PCRasterMap object
         """
-        print('Adding', pcr_map.filename, 'timestep', str(time_step), 'hour', self.hour_timestep)
+        logger.info('Adding %s - timestep %s - hour %s', pcr_map.filename, str(time_step), self.hour_timestep)
         values = pcr_map.data
         values[values == pcr_map.mv] = self.mv
         self.values.append(values)
         if time_step:
             self.timesteps.append(float(time_step))
         self.current_count += 1
 
         if self.current_count == 20:
             self.current_idx2 += self.current_count
-            print('Writing a chunk...')
+            logger.info('Writing a chunk into output file...')
             dtype = self.values[0].dtype
             if self.is_mapstack:
                 self.variable[self.current_idx1:self.current_idx2, :, :] = np.array(self.values, dtype=dtype)
             else:
                 self.variable[:, :] = np.array(self.values, dtype=dtype)
             # update slicing indexes
             self.current_idx1 = self.current_idx2
@@ -144,17 +148,17 @@
             self.values = []
             self.current_count = 0
 
     def finalize(self):
         """
         Write last maps to the stack and close the NetCDF4 dataset.
         """
-        print('Writing...', self.name)
+        logger.info('Writing %s', self.name)
         if self.is_mapstack:
-            print('Writing time dimension...', self.timesteps[:4], '...', self.timesteps[-4:])
+            logger.info('Writing time dimension... %s ... %s', self.timesteps[:4], self.timesteps[-4:])
             self.time[:] = np.array(self.timesteps, dtype=np.float64)
 
         if self.values:
             dtype = self.values[0].dtype
             if self.is_mapstack:
                 self.current_idx2 += self.current_count
                 self.variable[self.current_idx1:self.current_idx2, :, :] = np.array(self.values, dtype=dtype)
@@ -163,15 +167,15 @@
         self.nf.close()
 
     def define_wgs84(self):
         """
         Define WGS84 reference system
         """
         # coordinates variables
-        print('Defining WGS84 coordinates variables')
+        logger.info('Defining WGS84 coordinates variables')
         longitude = self.nf.createVariable('lon', 'f8', ('lon',))
         longitude.standard_name = 'longitude'
         longitude.long_name = 'longitude coordinate'
         longitude.units = 'degrees_east'
 
         latitude = self.nf.createVariable('lat', 'f8', ('lat',))
         latitude.standard_name = 'latitude'
@@ -184,15 +188,15 @@
         values_var.coordinates = 'lon lat'
         values_var.esri_pe_string = self.DATUM.get(self.nc_metadata['geographical'].get('datum', 'WGS84').upper(), '')
 
     def define_etrs89(self):
         """
         Define a ETRS89 reference system
         """
-        print('Defining ETRS89 coordinates variables')
+        logger.info('Defining ETRS89 coordinates variables')
         # Variables
         x = self.nf.createVariable('x', 'f8', ('lon',))
         y = self.nf.createVariable('y', 'f8', ('lat',))
         x.standard_name = 'projection_x_coordinate'
         x.long_name = 'x coordinate of projection'
         x.units = 'Meter'
 
@@ -253,15 +257,17 @@
         values_var.esri_pe_string = self.DATUM.get(self.nc_metadata['geographical'].get('datum', 'WGS84').upper(), '')
 
 
 def convert(config):
     input_set = config['input_set']
     reader = PCRasterReader(input_set)
     pcr_metadata = reader.get_metadata_from_set()
-    writer = NetCDFWriter(config.get('output_filename') or config.get('variable'),
-                          config['metadata'],
-                          pcr_metadata,
-                          mapstack=not reader.input_is_single_file())
+    writer = NetCDFWriter(
+        config.get('output_filename') or config.get('variable'),
+        config['metadata'],
+        pcr_metadata,
+        mapstack=not reader.input_is_single_file()
+    )
     for pcr_map, time_step in reader.fileset:
         writer.add_to_stack(pcr_map, time_step)
         pcr_map.close()
     writer.finalize()
```

### Comparing `lisflood-utilities-0.8/src/lisfloodutilities/readers/pcr.py` & `lisflood-utilities-0.9/src/lisfloodutilities/readers/pcr.py`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/README.md` & `lisflood-utilities-0.9/README.md`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/setup.py` & `lisflood-utilities-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `lisflood-utilities-0.8/PKG-INFO` & `lisflood-utilities-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisflood-utilities
-Version: 0.8
+Version: 0.9
 Summary: A set of utilities for lisfloodutilities users. pcr2nc: Convert PCRaster files to netCDF; cutmaps: cut netCDF files;compare: to compare two set of netcdf files
 Home-page: https://github.com/ec-jrc/lisflood-utilities
 Author: Valerio Lorini, Domenico Nappo, Lorenzo Alfieri
 Author-email: valerio.lorini@ec.europa.eu,domenico.nappo@gmail.com,lorenzo.alfieri@ec.europa.eu
 License: EUPL 1.2
 Description: # Lisflood Utilities
```


# Comparing `tmp/jwst_mast_query-0.0.4.tar.gz` & `tmp/jwst_mast_query-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwst_mast_query-0.0.4.tar", last modified: Fri Apr 28 16:04:01 2023, max compression
+gzip compressed data, was "jwst_mast_query-0.0.5.tar", last modified: Thu May 11 15:46:39 2023, max compression
```

## Comparing `jwst_mast_query-0.0.4.tar` & `jwst_mast_query-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.410217 jwst_mast_query-0.0.4/
--rw-r--r--   0 hilbert   (3978) staff       (20)     2366 2022-03-04 20:55:11.000000 jwst_mast_query-0.0.4/.gitignore
--rw-r--r--   0 hilbert   (3978) staff       (20)     2194 2023-04-28 15:55:05.000000 jwst_mast_query-0.0.4/CHANGES.rst
--rw-r--r--   0 hilbert   (3978) staff       (20)     4528 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 hilbert   (3978) staff       (20)     1553 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.4/LICENSE.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)      812 2023-04-28 16:04:01.409863 jwst_mast_query-0.0.4/PKG-INFO
--rw-r--r--   0 hilbert   (3978) staff       (20)    39611 2023-04-14 18:08:15.000000 jwst_mast_query-0.0.4/README.md
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.406109 jwst_mast_query-0.0.4/jwst_mast_query/
--rw-r--r--   0 hilbert   (3978) staff       (20)       89 2022-02-16 16:07:13.000000 jwst_mast_query-0.0.4/jwst_mast_query/__init__.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     8344 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/jwst_download.py
--rw-r--r--   0 hilbert   (3978) staff       (20)     8471 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.cfg
--rwxr-xr-x   0 hilbert   (3978) staff       (20)    91265 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)    59698 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.4/jwst_mast_query/pdastro.py
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.408810 jwst_mast_query-0.0.4/jwst_mast_query/scripts/
--rw-r--r--   0 hilbert   (3978) staff       (20)     1793 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/scripts/jwst_download.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     8605 2023-03-10 17:35:18.000000 jwst_mast_query-0.0.4/jwst_mast_query/sortable.js
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.409289 jwst_mast_query-0.0.4/jwst_mast_query/utils/
--rw-r--r--   0 hilbert   (3978) staff       (20)     3917 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/utils/constants.py
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.408375 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/
--rw-r--r--   0 hilbert   (3978) staff       (20)      812 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/PKG-INFO
--rw-r--r--   0 hilbert   (3978) staff       (20)      534 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/SOURCES.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)        1 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/dependency_links.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)      191 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/requires.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)       16 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/top_level.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)       98 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.4/pyproject.toml
--rw-r--r--   0 hilbert   (3978) staff       (20)       38 2023-04-28 16:04:01.410340 jwst_mast_query-0.0.4/setup.cfg
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     2846 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/setup.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-05-11 15:46:39.676102 jwst_mast_query-0.0.5/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     2366 2022-03-04 20:55:11.000000 jwst_mast_query-0.0.5/.gitignore
+-rw-r--r--   0 hilbert   (3978) staff       (20)     2628 2023-05-11 15:40:39.000000 jwst_mast_query-0.0.5/CHANGES.rst
+-rw-r--r--   0 hilbert   (3978) staff       (20)     4528 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 hilbert   (3978) staff       (20)     1553 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.5/LICENSE.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)      812 2023-05-11 15:46:39.675459 jwst_mast_query-0.0.5/PKG-INFO
+-rw-r--r--   0 hilbert   (3978) staff       (20)    39798 2023-05-11 15:13:10.000000 jwst_mast_query-0.0.5/README.md
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-05-11 15:46:39.665103 jwst_mast_query-0.0.5/jwst_mast_query/
+-rw-r--r--   0 hilbert   (3978) staff       (20)       89 2022-02-16 16:07:13.000000 jwst_mast_query-0.0.5/jwst_mast_query/__init__.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     8344 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.5/jwst_mast_query/jwst_download.py
+-rw-r--r--   0 hilbert   (3978) staff       (20)     8654 2023-05-11 14:18:35.000000 jwst_mast_query-0.0.5/jwst_mast_query/jwst_query.cfg
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)    91655 2023-05-11 14:18:35.000000 jwst_mast_query-0.0.5/jwst_mast_query/jwst_query.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)    59698 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.5/jwst_mast_query/pdastro.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-05-11 15:46:39.669505 jwst_mast_query-0.0.5/jwst_mast_query/scripts/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     1793 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.5/jwst_mast_query/scripts/jwst_download.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     8605 2023-03-10 17:35:18.000000 jwst_mast_query-0.0.5/jwst_mast_query/sortable.js
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-05-11 15:46:39.670487 jwst_mast_query-0.0.5/jwst_mast_query/tests/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     4534 2023-05-11 15:13:10.000000 jwst_mast_query-0.0.5/jwst_mast_query/tests/test_jwst_download.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-05-11 15:46:39.673491 jwst_mast_query-0.0.5/jwst_mast_query/tests/testing_config_files/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     8691 2023-05-11 15:13:10.000000 jwst_mast_query-0.0.5/jwst_mast_query/tests/testing_config_files/1063_obs108_query.cfg
+-rw-r--r--   0 hilbert   (3978) staff       (20)     8691 2023-05-11 15:13:10.000000 jwst_mast_query-0.0.5/jwst_mast_query/tests/testing_config_files/1068_obs34_query.cfg
+-rw-r--r--   0 hilbert   (3978) staff       (20)     8699 2023-05-11 15:13:10.000000 jwst_mast_query-0.0.5/jwst_mast_query/tests/testing_config_files/1068_obs3_query_guidestars_only.cfg
+-rw-r--r--   0 hilbert   (3978) staff       (20)     8702 2023-05-11 15:13:10.000000 jwst_mast_query-0.0.5/jwst_mast_query/tests/testing_config_files/1068_obs3_query_with_guidestars.cfg
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-05-11 15:46:39.674374 jwst_mast_query-0.0.5/jwst_mast_query/utils/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     3965 2023-05-11 14:18:35.000000 jwst_mast_query-0.0.5/jwst_mast_query/utils/constants.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-05-11 15:46:39.668897 jwst_mast_query-0.0.5/jwst_mast_query.egg-info/
+-rw-r--r--   0 hilbert   (3978) staff       (20)      812 2023-05-11 15:46:39.000000 jwst_mast_query-0.0.5/jwst_mast_query.egg-info/PKG-INFO
+-rw-r--r--   0 hilbert   (3978) staff       (20)      865 2023-05-11 15:46:39.000000 jwst_mast_query-0.0.5/jwst_mast_query.egg-info/SOURCES.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)        1 2023-05-11 15:46:39.000000 jwst_mast_query-0.0.5/jwst_mast_query.egg-info/dependency_links.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)      198 2023-05-11 15:46:39.000000 jwst_mast_query-0.0.5/jwst_mast_query.egg-info/requires.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)       16 2023-05-11 15:46:39.000000 jwst_mast_query-0.0.5/jwst_mast_query.egg-info/top_level.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)       98 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.5/pyproject.toml
+-rw-r--r--   0 hilbert   (3978) staff       (20)       38 2023-05-11 15:46:39.676320 jwst_mast_query-0.0.5/setup.cfg
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     2864 2023-05-11 15:13:10.000000 jwst_mast_query-0.0.5/setup.py
```

### Comparing `jwst_mast_query-0.0.4/.gitignore` & `jwst_mast_query-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.4/CHANGES.rst` & `jwst_mast_query-0.0.5/CHANGES.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+0.0.5
+=====
+
+MAST Query
+----------
+
+Fixed a bug that was preventing guidestar data from being downloaded. Use the "guidestar" keyword to download guidestar data along with science data. Also added the "guidestar_only_data" keyword, which will remove science data and download only guidestar data. (#55)
+
+
+Tests
+-----
+
+Added some initial regression tests to be sure the behavior with and without the config file is consistent. (#53)
+
+
 0.0.4
 =====
 
 Config File
 -----------
 
 Fix a bug that was causing parameters with default values other than None or [] to be set back to the default value after adjusting parameter values based on the contents of the config file. (#51)
```

### Comparing `jwst_mast_query-0.0.4/CODE_OF_CONDUCT.md` & `jwst_mast_query-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.4/LICENSE.txt` & `jwst_mast_query-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.4/PKG-INFO` & `jwst_mast_query-0.0.5/jwst_mast_query.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jwst_mast_query
-Version: 0.0.4
+Name: jwst-mast-query
+Version: 0.0.5
 Summary: Query MAST for JWST products, and download them
 Home-page: https://github.com/spacetelescope/jwst_mast_query
 Author: STScI (Rest)
 Author-email: arest@stsci.edu
 Keywords: astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `jwst_mast_query-0.0.4/README.md` & `jwst_mast_query-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 | propIDs_obsnum2outsubdir: [1409]                                                                    | Specify list of propID for which obsnum2outsubdir is True. Only for the listed proposal numbers will observation numbers be used to create a subdirectory into which the appropriate files will be placed. e.g. $JWSTDOWNLOAD_OUTDIR/01410/obsnum23/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | skip_check_if_outfile_exists: False                                                                 | By default, the script queries MAST for products, and then checks if each file already exists in the output directory or not ("dl_code" and "dl_str" columns). For large numbers of products, this can take time. By setting this option to True, this check can be skipped.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | Nobs_per_batch: 2                                                                                   | For large programs, the query for the products can time out, and in these cases it is better to split up the query into Nobs_per_batch observations per batch. For example, if there are 22 observations, and Nobs_per_batch=4, then there will be 6 batches, 5 batches with 4 observations, and the last batch with 2.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | obsmode: ['image', 'wfss']                                                                          | Optionally specify the observation modes to query for. If provided, MAST will be queried only for these types of observations. e.g. assuming instrument is 'nircam', obsmode: ['image', 'wfss'] will query MAST for NIRCAM/IMAGE and NIRCAM/WFSS data. If left empty, the query will include all modes. For a list of valid modes, see the example config file in the repository. Note that as of 24 March 2023, MAST is in the process of reprocessing all data to add the mode values to the instrument names. Until this process is complete, some older data may not include the mode name, and therefore will not be found via a query that includes the mode name.                                                                                                                                                                                                                                                                                                                                                                      |
 | filetypes: ['uncal']                                                                                | List of file types to select in the product table, e.g., \_uncal.fits or \_uncal.jpg. If no suffix is given, .fits is appended. If only letters, then \_ and .fits are added. For example, 'uncal' gets expanded to \_uncal.fits. Typical image filetypes are uncal, rate, rateints, cal. For downloading a single file type, the brackets must still surround the file suffix, as the script expects a list. A relatively complete list of options includes: ['\_segm.fits', '\_asn.json', '\_pool.csv', '\_i2d.jpg', '\_thumb.jpg', '\_cat.ecsv', '\_i2d.fits', '\_uncal.fits', '\_uncal.jpg', '\_cal.fits', '\_trapsfilled.fits', '\_cal.jpg', '\_rate.jpg', '\_rateints.jpg', '\_trapsfilled.jpg', '\_rate.fits', '\_rateints.fits'] See the [JWST calibration pipeline documentation](https://jwst-pipeline.readthedocs.io/en/latest/jwst/introduction.html#pipeline-step-suffix-definitions) for a complete list. |
 | jpg_separate_subdir: False                                                                          | If True, downloaded jpgs are saved in separate "jpg" subdirectories, along side the fits files.																					|
 | guidestars: False                                                                                   | If guidestars is set to True, guidestar products are also included. Note: there are a **lot** of guide star products. We recommend you set to True only if really needed!                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| guidestar_data_only : False																		  | If guidestar_data_only is set to True, only guidestar products will be included. Science products will be filtered out.														 |
 | lookbacktime: 1.0                                                                                   | Lookback time in days. The script will query MAST over a time from the lookback time to the present moment. Note that all other time parameters (date_select, etc) override the lookback time.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | date_select: []                                                                                     | Specify date range (MJD or isot format) applied to "dateobs_center" column. If single value, then only exact matches will be returned. If a single value has "+" or "-" at the end, then it is a lower and upper limit, respectively. date_select will override the lookbacktime. Examples: 58400+, 58400-, 2020-11-23+,2020-11-23 2020-11-25                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 | savetables:                                                                                         | Save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the specified string as basename. Tables are saved in the same output directory as the data.  If no string is provided, the tables are not saved.                                                                                                                                                                                                                                                                                                        |    
 | mastcolumns_obsTable: ['proposal_id', 'dataURL', 'obs_id', 't_min','t_exptime']                     | Core columns returned from MAST to the obsTable                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | outcolumns_productTable                                                                             | List of columns to be shown in product table, e.g., ['proposal_id', 'obsnum', 'obsID', 'parent_obsid', 'obs_id', 'dataproduct_type', 'productFilename', 'filetype', 'calib_level', 'size', 'outfilename', 'dl_code', 'dl_str']                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | outcolumns_obsTable: ['proposal_id', 'obsnum', 'obsid', 'obs_id', 't_min', 't_exptime', 'date_min'] | Output columns for the obsTable.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | sortcols_productTable: ['calib_level','filetype','obsID']                                           | The productTable is sorted based on these columns. The default sorts the table based on calibration level.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
```

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query/jwst_download.py` & `jwst_mast_query-0.0.5/jwst_mast_query/jwst_download.py`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.cfg` & `jwst_mast_query-0.0.5/jwst_mast_query/tests/testing_config_files/1068_obs3_query_guidestars_only.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # specify the instrument. The default set in the code is nircam
 instrument: nircam
 
 # define the output directory
 # outrootdir[/outsubdir][/propID][/obsnumXYZ]
 # propID is the proposal ID number (APT number). Only added if not skip_propID2outsubdir. Note option --skip_propID2outsubdir
 # XYZ is the obsnum. Only added if obsnum2outsubdir==True. Note option --obsnum2outsubdir
-outrootdir: $JWSTDOWNLOAD_OUTDIR
+#outrootdir: $JWSTDOWNLOAD_OUTDIR
+outrootdir: ./
 outsubdir:
 skip_propID2outsubdir: False
 obsnum2outsubdir: True
 # specify list of propID for which obsnum2outsubdir: True
 # This might be useful for propIDs with lots of images: split the products up into subdirs 'obsnumXY'
 propIDs_obsnum2outsubdir: [1409]
 
@@ -20,27 +21,27 @@
 skip_check_if_outfile_exists: False
 
 # The script first gets all observations for the given query. Then it queries all products for these
 # observations. For large programs, the query for the products can time out, and in these cases it
 # is better to split up the query into Nobs_per_batch observations per batch. For example, if there are
 # 22 observations, and Nobs_per_batch=4, then there will be 6 batches, 5 batches with 4 observations, and
 # the last batch with 2.
-Nobs_per_batch: 2
+Nobs_per_batch: 3
 
 # Specify the proposal ID to query for. Can be an integer, or a 5-digit string, e.g.
 # propID: 1068
 # propID: '01068'
-propID:
+propID: 1068
 
 # Optionally specify the observation numbers to query for. Can be a single integer or string, or a list
 # of integers or strings.
 # e.g. obsnums: 001
 # obsnums: 1
 # obsnums: [001, 002]
-obsnums:
+obsnums: 3
 
 # Optionally specify the observation modes to query for. If provided, MAST will be queried only for these
 # types of observations. e.g. assuming instrument is 'nircam', obsmode: ['image', 'wfss'] will query MAST
 # for NIRCAM/IMAGE and NIRCAM/WFSS data. If left empty, the query will include all modes. Valid modes include:
 # miri: ['coron', 'ifu', 'image', 'slit', 'slitless', 'targacq']
 # nircam: ['coron', 'grism', 'image', 'targacq', 'wfss']
 # niriss: ['ami', 'image', 'soss', 'wfss']
@@ -64,39 +65,42 @@
 # choices=['a1','a2','a3','a4','along','b1','b2','b3','b4','blong']
 # If not specified, all SCAs are selected
 # sca: a1
 # sca: [a1, a3]
 sca:
 
 # if guidestars is set to True, guidestar products are also included
-guidestars: False
+guidestars: True
+
+# If guidestar_data_only is set to True, only guidestar products will be included. Science products will be filtered out.
+guidestar_data_only: True
 
 # lookback time in days
 # Note that all other time parameters (date_select) override the lookback time.
 lookbacktime: 1.0
 
 # Specify date range (MJD or isot format) applied to "dateobs_center" column. If single value, then exact match.
 # If single value has "+" or "-" at the end, then it is a lower and upper limit, respectively. date_select will
 # override the lookback parameter value.
 # Examples: 58400+, 58400-,2020-11-23+, 2020-11-23 2020-11-25, 59934 59934.125
 # date_select: 2021-05-23+
 # date_select: 2022-06-06 2022-06-08
-date_select:
+date_select: 2022-05-15 2022-05-16
 
 # save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the
 # specified string as basename. Tables will be saved in outrootdir.
 # If left empty, the tables will not be saved.
-savetables:
+savetables: 1068_obs3_query_guidestars_only_cfg
 
 # If clobber is True, all files will be downloaded. If false, only files that do not already exist in the
 # local directory will be downloaded.
 clobber: False
 
 # If True, the data will not be downloaded. Only the summary tables will be produced
-skipdownload: False
+skipdownload: True
 
 # columns returned from MAST to the obsTable
 # The default set in the code is mastcolumns_obsTable=['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime']
 mastcolumns_obsTable: ['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime','instrument_name']
 
 # output columns for the tables. Note that the columns for the individual filetypes
 # are automatically added to the obsTable.
```

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.py` & `jwst_mast_query-0.0.5/jwst_mast_query/jwst_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,17 @@
         parser.add_argument('--obsnums', type=int, nargs='+', default=PARAM_DEFAULTS['obsnums'], help=('Specify the observation numbers within the propID. This '
                                                                                                        'can be a single number, or a bracketed list of numbers. '
                                                                                                        'e.g. 3 or [3, 103] (default=%(default)s)'))
         parser.add_argument('--guidestars', action='store_true', default=PARAM_DEFAULTS['guidestars'], help=('If this is set to True, guidestar products are '
                                                                                                              'also included. Note: there are a **lot** of guide '
                                                                                                              'star products. We recommend you set to True only if '
                                                                                                              'really needed! (default=%(default)s)'))
+        parser.add_argument('--guidestar_data_only', action='store_true', default=PARAM_DEFAULTS['guidestar_data_only'], help=('If this is set to True, only guidestar '
+                                                                                                                               'products are included. No science data '
+                                                                                                                               'will be included. (default=%(default)s)'))
         parser.add_argument('-f','--filetypes',  type=str, nargs="+", default=PARAM_DEFAULTS['filetypes'], help=('List of file types to select in the product table, '
                                                                                                                  'e.g., _uncal.fits or _uncal.jpg. If no suffix is '
                                                                                                                  'given, .fits is appended. If only letters, then _ '
                                                                                                                  'and .fits are added. For example, "uncal" gets '
                                                                                                                  'expanded to _uncal.fits. Typical image filetypes '
                                                                                                                  'are uncal, rate, rateints, cal. For downloading a '
                                                                                                                  'single file type, the brackets must still surround '
@@ -896,28 +899,23 @@
         if self.verbose: print('productTable columns:',self.productTable.t.columns)
         if self.verbose:
             allfiletypes = unique(self.productTable.t['filetype'])
             print('List of all filetypes of obtained products:',allfiletypes)
 
         return self.productTable
 
-    def product_query(self, obsTable=None, guidestars=None, Nobs_per_batch=2):
+    def product_query(self, obsTable=None):
         '''
         Perform query for data products based on obs_id's in observation table
         '''
+        Nobs_per_batch = self.params['Nobs_per_batch']
 
         if obsTable is None:
             obsTable=self.obsTable
 
-        if guidestars is None:
-            guidestars = self.params['guidestars']
-            if guidestars is None:
-                guidestars = False
-
-
         # query MAST for all products for the obsid's
         obsids = ','.join(obsTable.t['obsid'].astype('str'))
         service = self.SERVICES['Product_search']
         #params = {"obsid":obsids,
         #          "columns":['type','productType'],
         #          "format":"json"
         #          }
@@ -959,24 +957,14 @@
             if self.verbose:
                 print('\n#### Querying ProductTable....')
             self.productTable.t = self.JwstObs.service_request(service, params).to_pandas()
         #self.productTable.write()
         if self.verbose:
             print(f'productTable obtained with {len(self.productTable.t)} entries')
 
-        # remove guide stars if wanted...
-        if not guidestars:
-            ixs_products = self.productTable.getindices()
-            gs_text = '_gs-'
-            ixs_gs = self.productTable.ix_matchregex('productFilename',gs_text)
-            ixs_keep_products = AnotB(ixs_products,ixs_gs)
-            self.productTable.t=self.productTable.t.loc[ixs_keep_products].reset_index()
-            if self.verbose:
-                print('Removing %d guide star products from a total of %d products, %d left' % (len(ixs_gs),len(ixs_products),len(ixs_keep_products)))
-
         # Fill the suffix column with the suffix of the form _bla1.bla2, e.g. _uncal.fits
         # This will later be used to figure out
         self.productTable.t['filetype'] = self.productTable.t['productFilename'].str.extract(r'(\_[a-zA-Z0-9]+\.[a-zA-Z0-9]+)$')
 
         scas = list(np.repeat(np.nan, len(self.productTable.t['obs_id'])))
         for i, oid in enumerate(self.productTable.t['obs_id']):
             match = [word for word in ALL_SCAS if word in oid]
@@ -1022,15 +1010,15 @@
         if self.verbose:
             allfiletypes = unique(self.productTable.t['filetype'])
             print('List of all filetypes of obtained products:',allfiletypes)
 
         return self.productTable
 
 
-    def product_filter(self, productTable=None, filetypes=None, calib_levels=None, gs_omit=True):
+    def product_filter(self, productTable=None, filetypes=None, calib_levels=None):
         '''
         Filter the list of products based on the filetype (or better suffix)
         '''
         if productTable is None:
            productTable=self.productTable
 
         if filetypes is None:
@@ -1052,35 +1040,41 @@
                     filetypes[i] = '_'+filetypes[i]
                 if re.search('\.',filetypes[i]) is None:
                     filetypes[i] += '.fits'
 
             print('allowed filetype list:',filetypes)
 
         ix_products = self.productTable.getindices()
-        # remove guide stars if wanted...
-        if gs_omit:
+        if not self.params['guidestars'] and not self.params['guidestar_data_only']:
+            # If both guidestars and guidestar_data_only are False, filter out guide star products
             gs_text = '_gs-'
             ix_gs = self.productTable.ix_matchregex('productFilename',gs_text)
             if self.verbose>1:
-                print('Removing %d guide star products from a total of %d products, %d left' % (len(ix_gs),len(ix_products),len(ix_products)-len(ix_gs)))
-            ix_products = AnotB(ix_products,ix_gs)
-
+                print(f'Removing {len(ix_gs)} guide star products from a total of {len(ix_products)} products, {len(ix_products)-len(ix_gs)} left')
+            ix_products = AnotB(ix_products, ix_gs)
+        elif self.params['guidestar_data_only']:
+            # If guidestar_data_only is True, then (regardless of guidestars value) filter out the science products.
+            gs_text = '_gs-'
+            ix_gs = self.productTable.ix_matchregex('productFilename',gs_text)
+            if self.verbose>1:
+                print(f'Keeping only guide star products, {len(ix_gs)} from a total of {len(ix_products)} products. Removing {len(ix_products)-len(ix_gs)} science products.')
+            ix_products = AandB(ix_products, ix_gs)
 
         if calib_levels is not None:
             ix_calib_level = []
             for calib_level in calib_levels:
                 ixs = self.productTable.ix_equal('calib_level',calib_level,indices=ix_products)
                 if self.verbose>1:
-                    print('Keeping %d products with calib_level %d' % (len(ixs),calib_level))
+                    print(f'Keeping {len(ixs)} products with calib_level {calib_level}')
                 ix_calib_level.extend(ixs)
             if self.verbose>1:
-                print('Keeping %d out of %d products with the correct calib_levels' % (len(ix_calib_level),len(ix_products)))
+                print(f'Keeping {len(ix_calib_level)} out of {len(ix_products)} products with the correct calib_levels')
             ix_products = ix_calib_level
 
-        # Loop trough the filetypes and get all entries from ix_products list
+        # Loop through the filetypes and get all entries from ix_products list
         self.ix_selected_products = []
         if filetypes is not None:
             for filetype in filetypes:
 
                 # make sure the '.' in the regular expression is literal, and also add '$' to the end
                 regex=re.sub('\.','\.',filetype)+'$'
 
@@ -1097,15 +1091,14 @@
             self.ix_selected_products = ix_products
 
         # get the list of valid filetypes that exist
         self.params['filetypes'] = unique(self.productTable.t.loc[self.ix_selected_products,'filetype'])
 
         self.ix_selected_products = self.productTable.ix_sort_by_cols(self.params['sortcols_productTable'],indices=self.ix_selected_products)
 
-
         return(self.ix_selected_products)
 
     def update_obstable_indices(self, ixs_prod, ix_obs_sorted=None, obsTable=None, productTable=None):
         if obsTable is None:
             obsTable=self.obsTable
 
         if productTable is None:
@@ -1620,15 +1613,15 @@
 
         if self.verbose>1:
             print(self.obsTable.t)
 
         # get the products:  stored in self.productTable
         # this list contains in general several entries for each observations.
         # If not otherwise specified, uses self.obsTable as starting point
-        self.product_query(Nobs_per_batch=self.params['Nobs_per_batch'])
+        self.product_query()
         if self.verbose>1:
             print(self.productTable.t)
 
         # select the products to download
         # If not otherwise specified, uses self.productTable as starting point
         # uses self.filetypes for filtering, which is set by optional parameters.
         # the selected products indices are put into self.ix_selected_products
```

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query/pdastro.py` & `jwst_mast_query-0.0.5/jwst_mast_query/pdastro.py`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query/scripts/jwst_download.py` & `jwst_mast_query-0.0.5/jwst_mast_query/scripts/jwst_download.py`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query/sortable.js` & `jwst_mast_query-0.0.5/jwst_mast_query/sortable.js`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query/utils/constants.py` & `jwst_mast_query-0.0.5/jwst_mast_query/utils/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                   'obsnums': None,
                   'obsid_select': [],
                   'obsid_list': [],
                   'sca': None,
                   'verbose': 0,
                   'filetypes': ['fits'],
                   'guidestars': False,
+                  'guidestar_data_only': False,
                   'lookbacktime': 1.,
                   'calib_levels': None,
                   'Nobs_per_batch': 2,
                   'obsnum2outsubdir': None,
                   'propIDs_obsnum2outsubdir': [],
                   'date_select': [],
                   'savetables': None,
```

### Comparing `jwst_mast_query-0.0.4/jwst_mast_query.egg-info/PKG-INFO` & `jwst_mast_query-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jwst-mast-query
-Version: 0.0.4
+Name: jwst_mast_query
+Version: 0.0.5
 Summary: Query MAST for JWST products, and download them
 Home-page: https://github.com/spacetelescope/jwst_mast_query
 Author: STScI (Rest)
 Author-email: arest@stsci.edu
 Keywords: astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `jwst_mast_query-0.0.4/setup.py` & `jwst_mast_query-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,16 @@
         'ipython',
         'jinja2',
         'numpy',
         'pandas',
         'pyyaml',
         'scipy',
         'argparse',
-        'pillow'
+        'pillow',
+        'pytest'
     ],
     scripts=['jwst_mast_query/scripts/jwst_download.py'],
     include_package_data=True,
     extras_require={
         'docs': DOCS_REQUIRE,
         'test': TESTS_REQUIRE,
     },
```


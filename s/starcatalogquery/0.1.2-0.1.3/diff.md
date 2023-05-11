# Comparing `tmp/starcatalogquery-0.1.2-py3-none-any.whl.zip` & `tmp/starcatalogquery-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26714 bytes, number of entries: 17
+Zip file size: 26764 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/__init__.py
--rw-r--r--  2.0 unx     3066 b- defN 23-May-08 07:21 starcatalogquery/astroalign.py
 -rw-r--r--  2.0 unx     6048 b- defN 23-May-09 01:27 starcatalogquery/catalog_check.py
 -rw-r--r--  2.0 unx     6716 b- defN 23-May-09 01:26 starcatalogquery/catalog_download.py
 -rw-r--r--  2.0 unx    15124 b- defN 23-May-08 13:32 starcatalogquery/catalog_query.py
--rw-r--r--  2.0 unx    50891 b- defN 23-May-11 04:45 starcatalogquery/classes.py
+-rw-r--r--  2.0 unx    50907 b- defN 23-May-11 15:16 starcatalogquery/classes.py
+-rw-r--r--  2.0 unx     3091 b- defN 23-May-11 15:15 starcatalogquery/invariantfeatures.py
 -rw-r--r--  2.0 unx     5624 b- defN 23-May-10 03:48 starcatalogquery/tiles_draw.py
 -rw-r--r--  2.0 unx     1937 b- defN 23-May-09 08:46 starcatalogquery/wcs.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-11 04:20 starcatalogquery/utils/__init__.py
 -rw-r--r--  2.0 unx      612 b- defN 23-May-09 08:08 starcatalogquery/utils/df2info.py
 -rw-r--r--  2.0 unx     4272 b- defN 23-May-09 08:33 starcatalogquery/utils/starcatalog_statistic.py
 -rw-r--r--  2.0 unx      477 b- defN 23-May-09 08:06 starcatalogquery/utils/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    11895 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1503 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/RECORD
-17 files, 109376 bytes uncompressed, 24208 bytes compressed:  77.9%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11946 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1510 b- defN 23-May-11 15:26 starcatalogquery-0.1.3.dist-info/RECORD
+17 files, 109475 bytes uncompressed, 24244 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: starcatalogquery/__init__.py
 Comment: 
 
-Filename: starcatalogquery/astroalign.py
-Comment: 
-
 Filename: starcatalogquery/catalog_check.py
 Comment: 
 
 Filename: starcatalogquery/catalog_download.py
 Comment: 
 
 Filename: starcatalogquery/catalog_query.py
 Comment: 
 
 Filename: starcatalogquery/classes.py
 Comment: 
 
+Filename: starcatalogquery/invariantfeatures.py
+Comment: 
+
 Filename: starcatalogquery/tiles_draw.py
 Comment: 
 
 Filename: starcatalogquery/wcs.py
 Comment: 
 
 Filename: starcatalogquery/utils/__init__.py
@@ -30,23 +30,23 @@
 
 Filename: starcatalogquery/utils/starcatalog_statistic.py
 Comment: 
 
 Filename: starcatalogquery/utils/try_download.py
 Comment: 
 
-Filename: starcatalogquery-0.1.2.dist-info/LICENSE
+Filename: starcatalogquery-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: starcatalogquery-0.1.2.dist-info/METADATA
+Filename: starcatalogquery-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: starcatalogquery-0.1.2.dist-info/WHEEL
+Filename: starcatalogquery-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: starcatalogquery-0.1.2.dist-info/top_level.txt
+Filename: starcatalogquery-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: starcatalogquery-0.1.2.dist-info/RECORD
+Filename: starcatalogquery-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starcatalogquery/classes.py

```diff
@@ -11,15 +11,15 @@
 from .catalog_download import catalog_download,hygv3_download
 from .catalog_check import catalog_check
 from .utils.starcatalog_statistic import tiles_statistic,starcatalog_info
 from .utils.df2info import df2info
 from .catalog_query import search_box,search_cone,search_box_magpm,search_cone_magpm,box2seqs,cone2seqs,_load_files
 from .tiles_draw import search_draw
 from .wcs import xy_catalog
-from .astroalign import _generate_invariants
+from .invariantfeatures import _generate_invariants
 
 class StarCatalog(object):
 
     def get(sc_name,tile_size=None,dir_to=None):
         """
         Grab star catalog data files from a remote server.
 
@@ -954,15 +954,15 @@
             nside = 4
             search_radius = 15
 
         npix = hp.nside2npix(nside)
         fp_radecs = []
         for seq in range(npix):
 
-            desc = 'Generating starcatalog tiles {:s}{:d}{:s} of {:d}'.format(Fore.BLUE,seq+1,Fore.RESET,npix)
+            desc = 'Generating starcatalog sky area index {:s}{:d}{:s} of {:d}'.format(Fore.BLUE,seq+1,Fore.RESET,npix)
             print(desc,end='\r')
 
             fp_radec = hp.pix2ang(nside,seq,lonlat=True)
             fp_radecs.append(fp_radec)
 
             stars = self.search_cone(fp_radec,search_radius,max_control_points)
             pixels = stars.pixel_xy(pixel_width)
```

## Comparing `starcatalogquery/astroalign.py` & `starcatalogquery/invariantfeatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
-Some subfunctions of ASTROALIGN from Martin Beroiz.
+Some slightly modified subroutines of package ASTROALIGN from Martin Beroiz.
 """
 
 import numpy as _np
 
 # The number of nearest neighbors of a given star(including itself) to construct the triangle invariants.
-NUM_NEAREST_NEIGHBORS = 5
+NUM_NEAREST_NEIGHBORS = 6
 
 def _invariantfeatures(x1, x2, x3):
     """
     Given 3 points x1, x2, x3, return the invariant features for the set.
     """
     sides = _np.sort(
         [
```

## Comparing `starcatalogquery-0.1.2.dist-info/LICENSE` & `starcatalogquery-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starcatalogquery-0.1.2.dist-info/METADATA` & `starcatalogquery-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: starcatalogquery
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to establish an offline star catalog query database
 Home-page: https://github.com/lcx366/STARQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: Star Catalog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyshtools
 Requires-Dist: astropy (>=4.3.1)
 Requires-Dist: pandas
```

## Comparing `starcatalogquery-0.1.2.dist-info/RECORD` & `starcatalogquery-0.1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 starcatalogquery/__init__.py,sha256=F5XhiD_gjaRsVVK_KfSD9ZkmgQnoNiJQqIMoMsceHRY,33
-starcatalogquery/astroalign.py,sha256=cmssoOl0zkhr6VulR18CLWFfOyEg4tV2hf9lA7CPDG0,3066
 starcatalogquery/catalog_check.py,sha256=r6B-MtO3bq3NVRHkyq0xnZxBvTRf8Epmn-thBD53gHo,6048
 starcatalogquery/catalog_download.py,sha256=gDFjQEtwKX56Sdwv7L53YIZKLrLy_3CtbvE3tfyxrvQ,6716
 starcatalogquery/catalog_query.py,sha256=kBY8F25jt_WiLLY_SNJWseHCx0XWVti-b7ToL17csV4,15124
-starcatalogquery/classes.py,sha256=Bj2VkvwMGVIZhR-G7ul8Ikal2WQNDIU80og6Hzz_Nl4,50891
+starcatalogquery/classes.py,sha256=0VQQcu4XWqDY6M_n_eg67fQLOGNt-NurlcofahUhL-o,50907
+starcatalogquery/invariantfeatures.py,sha256=jEqRc1GFN691eWOcSPPH4-mumyemFzytyitBioPk8A8,3091
 starcatalogquery/tiles_draw.py,sha256=zsL2lOnfOrb-fWXDSSmdGwdfYWNIL08D84Kvk8Lvc0E,5624
 starcatalogquery/wcs.py,sha256=SMhSDUNat1755eyzwY9A56DZzDBqhz2XVVMBx8SYFQw,1937
 starcatalogquery/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 starcatalogquery/utils/df2info.py,sha256=_eQENb_DxX5Q5EGxbanJuo9nQKBm-A6Tz8pEsLFinxI,612
 starcatalogquery/utils/starcatalog_statistic.py,sha256=xnyKAJFuduuXo3dKkO0B1YoeTlvu-j-BtNtgrRMvZIY,4272
 starcatalogquery/utils/try_download.py,sha256=cTfNaevU_ELwKP3R9SpYQsiGtEvoBETnsi__EdkLSVE,477
-starcatalogquery-0.1.2.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starcatalogquery-0.1.2.dist-info/METADATA,sha256=_j9DSNN6KoBRJ0ngozCwumS6D5Qz9OmS5tcW22OpTBk,11895
-starcatalogquery-0.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starcatalogquery-0.1.2.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
-starcatalogquery-0.1.2.dist-info/RECORD,,
+starcatalogquery-0.1.3.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starcatalogquery-0.1.3.dist-info/METADATA,sha256=xEyLbwscGxcSyyaRiSsRPdnmqOzFKCggF5I4Ni1ksfc,11946
+starcatalogquery-0.1.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starcatalogquery-0.1.3.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
+starcatalogquery-0.1.3.dist-info/RECORD,,
```


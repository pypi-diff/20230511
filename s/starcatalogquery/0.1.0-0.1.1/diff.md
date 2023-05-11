# Comparing `tmp/starcatalogquery-0.1.0-py3-none-any.whl.zip` & `tmp/starcatalogquery-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26723 bytes, number of entries: 17
+Zip file size: 26722 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/__init__.py
 -rw-r--r--  2.0 unx     3066 b- defN 23-May-08 07:21 starcatalogquery/astroalign.py
 -rw-r--r--  2.0 unx     6048 b- defN 23-May-09 01:27 starcatalogquery/catalog_check.py
 -rw-r--r--  2.0 unx     6716 b- defN 23-May-09 01:26 starcatalogquery/catalog_download.py
 -rw-r--r--  2.0 unx    15124 b- defN 23-May-08 13:32 starcatalogquery/catalog_query.py
 -rw-r--r--  2.0 unx    50849 b- defN 23-May-10 07:10 starcatalogquery/classes.py
 -rw-r--r--  2.0 unx     5624 b- defN 23-May-10 03:48 starcatalogquery/tiles_draw.py
 -rw-r--r--  2.0 unx     1937 b- defN 23-May-09 08:46 starcatalogquery/wcs.py
--rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/utils/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 23-May-11 04:20 starcatalogquery/utils/__init__.py
 -rw-r--r--  2.0 unx      612 b- defN 23-May-09 08:08 starcatalogquery/utils/df2info.py
 -rw-r--r--  2.0 unx     4272 b- defN 23-May-09 08:33 starcatalogquery/utils/starcatalog_statistic.py
 -rw-r--r--  2.0 unx      477 b- defN 23-May-09 08:06 starcatalogquery/utils/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-10 07:56 starcatalogquery-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    11883 b- defN 23-May-10 07:56 starcatalogquery-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 07:56 starcatalogquery-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-10 07:56 starcatalogquery-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1504 b- defN 23-May-10 07:56 starcatalogquery-0.1.0.dist-info/RECORD
-17 files, 109355 bytes uncompressed, 24217 bytes compressed:  77.9%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11895 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1503 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/RECORD
+17 files, 109334 bytes uncompressed, 24216 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: starcatalogquery/utils/starcatalog_statistic.py
 Comment: 
 
 Filename: starcatalogquery/utils/try_download.py
 Comment: 
 
-Filename: starcatalogquery-0.1.0.dist-info/LICENSE
+Filename: starcatalogquery-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: starcatalogquery-0.1.0.dist-info/METADATA
+Filename: starcatalogquery-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: starcatalogquery-0.1.0.dist-info/WHEEL
+Filename: starcatalogquery-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: starcatalogquery-0.1.0.dist-info/top_level.txt
+Filename: starcatalogquery-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: starcatalogquery-0.1.0.dist-info/RECORD
+Filename: starcatalogquery-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starcatalogquery/utils/__init__.py

```diff
@@ -1,3 +1 @@
-00000000: 6672 6f6d 202e 636c 6173 7365 7320 696d  from .classes im
-00000010: 706f 7274 2053 7461 7243 6174 616c 6f67  port StarCatalog
-00000020: 0a                                       .
+00000000: 0a                                       .
```

## Comparing `starcatalogquery-0.1.0.dist-info/LICENSE` & `starcatalogquery-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starcatalogquery-0.1.0.dist-info/METADATA` & `starcatalogquery-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starcatalogquery
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to establish an offline star catalog query database
 Home-page: https://github.com/lcx366/STARQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: Star Catalog
 Classifier: Development Status :: 4 - Beta
@@ -182,19 +182,19 @@
 </p>
 
 ### Divide the sky
 
 The celestial sphere can be divided into multiple equal-area sky regions using the HEALPix algorithm. Then a feature library is established in each sky area for blind matching of star maps. 
 
 <p align="middle">
-  <img src="readme_figs/healpix_list.png" width="350" />
+  <img src="readme_figs/healpix_list.png" width="400" />
 </p>
 
 <p align="middle">
-  <img src="readme_figs/healpix_table.png" width="350" />
+  <img src="readme_figs/healpix_table.png" width="400" />
 </p>
 
 By default, we adopt the following strategy to divide the sky area:
 
 - For FOV > 30, k = 0; 
 
 - For FOV > 10, k = 1;
@@ -211,15 +211,15 @@
 A h5-formatted star catalog file `outh5`is generated, which records the center pointing of each sky area, the pixel coordinates, the triangle invariants and the asterism indices of the stars.
 
 ### Read in h5-formatted star catalog file
 
 ```python
 >>> from starcatalogquery import StarCatalog
 >>> infile_h5 = 'starcatalogs/indices/hygv3/fov20_mag8_mcp40_2023.0.h5'
->>> fp_radecs,stars_xy,stars_invariants,stars_asterisms = read_h5_indices(infile_h5)
+>>> fp_radecs,stars_xy,stars_invariants,stars_asterisms = StarCatalog.read_h5_indices(infile_h5)
 ```
 
 ### Load the local offline star catalog database
 
 Load the raw star catalog
 
 ```python
```

## Comparing `starcatalogquery-0.1.0.dist-info/RECORD` & `starcatalogquery-0.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 starcatalogquery/astroalign.py,sha256=cmssoOl0zkhr6VulR18CLWFfOyEg4tV2hf9lA7CPDG0,3066
 starcatalogquery/catalog_check.py,sha256=r6B-MtO3bq3NVRHkyq0xnZxBvTRf8Epmn-thBD53gHo,6048
 starcatalogquery/catalog_download.py,sha256=gDFjQEtwKX56Sdwv7L53YIZKLrLy_3CtbvE3tfyxrvQ,6716
 starcatalogquery/catalog_query.py,sha256=kBY8F25jt_WiLLY_SNJWseHCx0XWVti-b7ToL17csV4,15124
 starcatalogquery/classes.py,sha256=AgLkoFra8w5bFXRgw1sFJdZCHX12Qty1JNk6YJvm6cM,50849
 starcatalogquery/tiles_draw.py,sha256=zsL2lOnfOrb-fWXDSSmdGwdfYWNIL08D84Kvk8Lvc0E,5624
 starcatalogquery/wcs.py,sha256=SMhSDUNat1755eyzwY9A56DZzDBqhz2XVVMBx8SYFQw,1937
-starcatalogquery/utils/__init__.py,sha256=F5XhiD_gjaRsVVK_KfSD9ZkmgQnoNiJQqIMoMsceHRY,33
+starcatalogquery/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 starcatalogquery/utils/df2info.py,sha256=_eQENb_DxX5Q5EGxbanJuo9nQKBm-A6Tz8pEsLFinxI,612
 starcatalogquery/utils/starcatalog_statistic.py,sha256=xnyKAJFuduuXo3dKkO0B1YoeTlvu-j-BtNtgrRMvZIY,4272
 starcatalogquery/utils/try_download.py,sha256=cTfNaevU_ELwKP3R9SpYQsiGtEvoBETnsi__EdkLSVE,477
-starcatalogquery-0.1.0.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starcatalogquery-0.1.0.dist-info/METADATA,sha256=S5e-CUZjbbne-HHe8saE9eA1tgd_dVqknWl6RCFjyWc,11883
-starcatalogquery-0.1.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starcatalogquery-0.1.0.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
-starcatalogquery-0.1.0.dist-info/RECORD,,
+starcatalogquery-0.1.1.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starcatalogquery-0.1.1.dist-info/METADATA,sha256=FKCPMhUfDSeIM4EPzSc9vMxVT2U3oCxWeOZnDHd-yWs,11895
+starcatalogquery-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starcatalogquery-0.1.1.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
+starcatalogquery-0.1.1.dist-info/RECORD,,
```


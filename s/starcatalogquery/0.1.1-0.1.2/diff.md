# Comparing `tmp/starcatalogquery-0.1.1-py3-none-any.whl.zip` & `tmp/starcatalogquery-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26722 bytes, number of entries: 17
+Zip file size: 26714 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/__init__.py
 -rw-r--r--  2.0 unx     3066 b- defN 23-May-08 07:21 starcatalogquery/astroalign.py
 -rw-r--r--  2.0 unx     6048 b- defN 23-May-09 01:27 starcatalogquery/catalog_check.py
 -rw-r--r--  2.0 unx     6716 b- defN 23-May-09 01:26 starcatalogquery/catalog_download.py
 -rw-r--r--  2.0 unx    15124 b- defN 23-May-08 13:32 starcatalogquery/catalog_query.py
--rw-r--r--  2.0 unx    50849 b- defN 23-May-10 07:10 starcatalogquery/classes.py
+-rw-r--r--  2.0 unx    50891 b- defN 23-May-11 04:45 starcatalogquery/classes.py
 -rw-r--r--  2.0 unx     5624 b- defN 23-May-10 03:48 starcatalogquery/tiles_draw.py
 -rw-r--r--  2.0 unx     1937 b- defN 23-May-09 08:46 starcatalogquery/wcs.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-11 04:20 starcatalogquery/utils/__init__.py
 -rw-r--r--  2.0 unx      612 b- defN 23-May-09 08:08 starcatalogquery/utils/df2info.py
 -rw-r--r--  2.0 unx     4272 b- defN 23-May-09 08:33 starcatalogquery/utils/starcatalog_statistic.py
 -rw-r--r--  2.0 unx      477 b- defN 23-May-09 08:06 starcatalogquery/utils/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    11895 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1503 b- defN 23-May-11 04:26 starcatalogquery-0.1.1.dist-info/RECORD
-17 files, 109334 bytes uncompressed, 24216 bytes compressed:  77.9%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11895 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1503 b- defN 23-May-11 04:49 starcatalogquery-0.1.2.dist-info/RECORD
+17 files, 109376 bytes uncompressed, 24208 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: starcatalogquery/utils/starcatalog_statistic.py
 Comment: 
 
 Filename: starcatalogquery/utils/try_download.py
 Comment: 
 
-Filename: starcatalogquery-0.1.1.dist-info/LICENSE
+Filename: starcatalogquery-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: starcatalogquery-0.1.1.dist-info/METADATA
+Filename: starcatalogquery-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: starcatalogquery-0.1.1.dist-info/WHEEL
+Filename: starcatalogquery-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: starcatalogquery-0.1.1.dist-info/top_level.txt
+Filename: starcatalogquery-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: starcatalogquery-0.1.1.dist-info/RECORD
+Filename: starcatalogquery-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starcatalogquery/classes.py

```diff
@@ -240,15 +240,15 @@
                 desc = 'Reducing {:s}{:d}{:s} of {:d}'.format(Fore.BLUE,j,Fore.RESET,self.tiles_num)
                 print(desc,end='\r')
 
                 df = pd.read_csv(tile_file,skiprows=1,dtype=str)
                 # units: ra->hourangle, dec->deg, pmra->mas/a, pmdec->mas/a, epoch->2000.0 
                 df_reduced = df.loc[:,['ra','dec','pmra','pmdec','mag']]
                 df_reduced['epoch'] = '2000.0'
-                df_reduced['ra'] = (df_reduced['ra']*15).round(6) # Convert hourangle to deg
+                df_reduced['ra'] = (df_reduced['ra'].astype(float)*15).round(6) # Convert hourangle to deg
                 df_reduced.to_csv(tile_file.replace('raw','reduced'),index=False)
 
                 j += 1
         elif sc_name == 'gsc12':
             j = 1
             for tile_file in file_list:
                 desc = 'Reducing {:s}{:d}{:s} of {:d}'.format(Fore.BLUE,j,Fore.RESET,self.tiles_num)
@@ -256,16 +256,16 @@
 
                 df = pd.read_csv(tile_file,skiprows=1,dtype=str)
                 # units: ra->deg, dec->deg, RApm->arcs/0.1a, Decpm->arcs/0.1a, Epoch->1980.552
                 df_reduced = df.loc[:,['ra','dec','RApm','Decpm','mag','Epoch']]
                 columns_dict = {'RApm':'pmra', 'Decpm':'pmdec', 'Epoch':'epoch'}
                 df_reduced.rename(columns=columns_dict, inplace=True)
                 # Convert to standard proper motion in mas/a
-                df_reduced['pmra'] = (df_reduced['pmra']*1e4).round(2) 
-                df_reduced['pmdec'] = (df_reduced['pmdec']*1e4).round(2)
+                df_reduced['pmra'] = (df_reduced['pmra'].astype(float)*1e4).round(2) 
+                df_reduced['pmdec'] = (df_reduced['pmdec'].astype(float)*1e4).round(2)
                 df_reduced.to_csv(tile_file.replace('raw','reduced'),index=False)
 
                 j += 1
         elif sc_name == 'gsc242':
             j = 1
             for tile_file in file_list:
                 desc = 'Reducing {:s}{:d}{:s} of {:d}'.format(Fore.BLUE,j,Fore.RESET,self.tiles_num)
@@ -789,15 +789,15 @@
         self.info = info
 
         for key in info.keys():
             setattr(self, key, info[key])
 
     def __repr__(self):
     
-        return 'instance of class StarCatalogSimplified'        
+        return 'Instance of class StarCatalogSimplified'        
 
     def load(sc_name,tile_size,mag_cutoff,epoch,dir_from=None):
         """
         Load the simplified star catalog files from the local database.
 
         Usage:
             >>> from starcatalogquery import StarCatalogSimplified
```

## Comparing `starcatalogquery-0.1.1.dist-info/LICENSE` & `starcatalogquery-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starcatalogquery-0.1.1.dist-info/METADATA` & `starcatalogquery-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starcatalogquery
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to establish an offline star catalog query database
 Home-page: https://github.com/lcx366/STARQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: Star Catalog
 Classifier: Development Status :: 4 - Beta
```

## Comparing `starcatalogquery-0.1.1.dist-info/RECORD` & `starcatalogquery-0.1.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 starcatalogquery/__init__.py,sha256=F5XhiD_gjaRsVVK_KfSD9ZkmgQnoNiJQqIMoMsceHRY,33
 starcatalogquery/astroalign.py,sha256=cmssoOl0zkhr6VulR18CLWFfOyEg4tV2hf9lA7CPDG0,3066
 starcatalogquery/catalog_check.py,sha256=r6B-MtO3bq3NVRHkyq0xnZxBvTRf8Epmn-thBD53gHo,6048
 starcatalogquery/catalog_download.py,sha256=gDFjQEtwKX56Sdwv7L53YIZKLrLy_3CtbvE3tfyxrvQ,6716
 starcatalogquery/catalog_query.py,sha256=kBY8F25jt_WiLLY_SNJWseHCx0XWVti-b7ToL17csV4,15124
-starcatalogquery/classes.py,sha256=AgLkoFra8w5bFXRgw1sFJdZCHX12Qty1JNk6YJvm6cM,50849
+starcatalogquery/classes.py,sha256=Bj2VkvwMGVIZhR-G7ul8Ikal2WQNDIU80og6Hzz_Nl4,50891
 starcatalogquery/tiles_draw.py,sha256=zsL2lOnfOrb-fWXDSSmdGwdfYWNIL08D84Kvk8Lvc0E,5624
 starcatalogquery/wcs.py,sha256=SMhSDUNat1755eyzwY9A56DZzDBqhz2XVVMBx8SYFQw,1937
 starcatalogquery/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 starcatalogquery/utils/df2info.py,sha256=_eQENb_DxX5Q5EGxbanJuo9nQKBm-A6Tz8pEsLFinxI,612
 starcatalogquery/utils/starcatalog_statistic.py,sha256=xnyKAJFuduuXo3dKkO0B1YoeTlvu-j-BtNtgrRMvZIY,4272
 starcatalogquery/utils/try_download.py,sha256=cTfNaevU_ELwKP3R9SpYQsiGtEvoBETnsi__EdkLSVE,477
-starcatalogquery-0.1.1.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starcatalogquery-0.1.1.dist-info/METADATA,sha256=FKCPMhUfDSeIM4EPzSc9vMxVT2U3oCxWeOZnDHd-yWs,11895
-starcatalogquery-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starcatalogquery-0.1.1.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
-starcatalogquery-0.1.1.dist-info/RECORD,,
+starcatalogquery-0.1.2.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starcatalogquery-0.1.2.dist-info/METADATA,sha256=_j9DSNN6KoBRJ0ngozCwumS6D5Qz9OmS5tcW22OpTBk,11895
+starcatalogquery-0.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starcatalogquery-0.1.2.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
+starcatalogquery-0.1.2.dist-info/RECORD,,
```


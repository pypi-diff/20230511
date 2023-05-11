# Comparing `tmp/Slpapy-0.3.8.tar.gz` & `tmp/Slpapy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.8.tar", last modified: Wed May 10 02:31:52 2023, max compression
+gzip compressed data, was "Slpapy-0.3.9.tar", last modified: Wed May 10 04:04:15 2023, max compression
```

## Comparing `Slpapy-0.3.8.tar` & `Slpapy-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 02:31:52.825191 Slpapy-0.3.8/
--rw-rw-rw-   0        0        0      159 2023-05-10 02:31:52.824222 Slpapy-0.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 02:31:52.788289 Slpapy-0.3.8/Slpapy/
--rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.8/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.8/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-10 02:31:52.822226 Slpapy-0.3.8/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.8/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.8/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5816 2023-05-10 02:31:34.000000 Slpapy-0.3.8/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-10 02:31:52.797265 Slpapy-0.3.8/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-10 02:31:52.000000 Slpapy-0.3.8/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-05-10 02:31:52.000000 Slpapy-0.3.8/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 02:31:52.000000 Slpapy-0.3.8/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-10 02:31:52.000000 Slpapy-0.3.8/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 02:31:52.000000 Slpapy-0.3.8/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 02:31:52.825191 Slpapy-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-05-10 02:31:34.000000 Slpapy-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 04:04:15.697428 Slpapy-0.3.9/
+-rw-rw-rw-   0        0        0      159 2023-05-10 04:04:15.697428 Slpapy-0.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 04:04:15.659530 Slpapy-0.3.9/Slpapy/
+-rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.9/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.9/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-10 04:04:15.695433 Slpapy-0.3.9/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.9/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.9/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5803 2023-05-10 04:03:41.000000 Slpapy-0.3.9/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-10 04:04:15.669503 Slpapy-0.3.9/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-10 04:04:15.000000 Slpapy-0.3.9/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-05-10 04:04:15.000000 Slpapy-0.3.9/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 04:04:15.000000 Slpapy-0.3.9/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-10 04:04:15.000000 Slpapy-0.3.9/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 04:04:15.000000 Slpapy-0.3.9/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 04:04:15.698425 Slpapy-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-05-10 04:04:01.000000 Slpapy-0.3.9/setup.py
```

### Comparing `Slpapy-0.3.8/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.9/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.9/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.3.9/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.8/Slpapy/processing_analyze.py` & `Slpapy-0.3.9/Slpapy/processing_analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
     result = adata.uns['rank_genes_groups']
     groups = result['names'].dtype.names
     res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
                         ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
     res.to_csv("dif.csv")
     sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_Wilcoxon.png')
-    sc.pl.rank_genes_groups_violin(adata, n_genes=25, sharey=False, dendrogram=True, save='_violin_Wilcoxon.png')
+    sc.pl.rank_genes_groups_violin(adata, n_genes=25,  dendrogram=True, save='_violin_Wilcoxon.png')
     return adata
 
 
 def Basic_processing_flow(
         adata: ad.AnnData,
         *,
         use_spacial: bool = False,
```

### Comparing `Slpapy-0.3.8/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.9/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


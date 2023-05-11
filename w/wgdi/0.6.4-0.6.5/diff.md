# Comparing `tmp/wgdi-0.6.4.tar.gz` & `tmp/wgdi-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wgdi-0.6.4.tar", last modified: Sat Apr 22 12:00:48 2023, max compression
+gzip compressed data, was "dist\wgdi-0.6.5.tar", last modified: Thu May 11 13:38:16 2023, max compression
```

## Comparing `wgdi-0.6.4.tar` & `wgdi-0.6.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.321730 wgdi-0.6.4/
--rw-rw-rw-   0        0        0     5499 2023-04-22 12:00:48.321203 wgdi-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     4119 2023-04-22 11:59:58.000000 wgdi-0.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 12:00:48.321730 wgdi-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-04-22 11:59:58.000000 wgdi-0.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.255522 wgdi-0.6.4/wgdi/
--rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/__init__.py
--rw-rw-rw-   0        0        0     8121 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/align_dotplot.py
--rw-rw-rw-   0        0        0     2646 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/ancestral_karyotype.py
--rw-rw-rw-   0        0        0     3385 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/ancestral_karyotype_repertoire.py
--rw-rw-rw-   0        0        0     8288 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/base.py
--rw-rw-rw-   0        0        0     3889 2022-11-21 05:06:20.000000 wgdi-0.6.4/wgdi/block_correspondence.py
--rw-rw-rw-   0        0        0     7791 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/block_info.py
--rw-rw-rw-   0        0        0     5023 2022-12-07 13:57:34.000000 wgdi-0.6.4/wgdi/block_ks.py
--rw-rw-rw-   0        0        0    11229 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/circos.py
--rw-rw-rw-   0        0        0     6798 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/collinearity.py
--rw-rw-rw-   0        0        0     6225 2022-12-07 14:12:47.000000 wgdi-0.6.4/wgdi/dotplot.py
-drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.319103 wgdi-0.6.4/wgdi/example/
--rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/__init__.py
--rw-rw-rw-   0        0        0      398 2023-04-04 06:33:01.000000 wgdi-0.6.4/wgdi/example/align.conf
--rw-rw-rw-   0        0        0      540 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/alignmenttrees.conf
--rw-rw-rw-   0        0        0      341 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ancestral_karyotype.conf
--rw-rw-rw-   0        0        0      473 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ancestral_karyotype_repertoire.conf
--rw-rw-rw-   0        0        0      281 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/blockinfo.conf
--rw-rw-rw-   0        0        0      315 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/blockks.conf
--rw-rw-rw-   0        0        0      443 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/circos.conf
--rw-rw-rw-   0        0        0      302 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/collinearity.conf
--rw-rw-rw-   0        0        0      368 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/conf.ini
--rw-rw-rw-   0        0        0      237 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/corr.conf
--rw-rw-rw-   0        0        0      423 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/dotplot.conf
--rw-rw-rw-   0        0        0      120 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/karyotype.conf
--rw-rw-rw-   0        0        0      434 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/karyotype_mapping.conf
--rw-rw-rw-   0        0        0      183 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ks.conf
--rw-rw-rw-   0        0        0      383 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ks_fit_result.csv
--rw-rw-rw-   0        0        0      250 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ksfigure.conf
--rw-rw-rw-   0        0        0      260 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/kspeaks.conf
--rw-rw-rw-   0        0        0      200 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/peaksfit.conf
--rw-rw-rw-   0        0        0      178 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/pindex.conf
--rw-rw-rw-   0        0        0      182 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/polyploidy_classification.conf
--rw-rw-rw-   0        0        0      235 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/retain.conf
--rw-rw-rw-   0        0        0      332 2023-03-31 14:17:47.000000 wgdi-0.6.4/wgdi/example/shared_fusion.conf
--rw-rw-rw-   0        0        0     1637 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/karyotype.py
--rw-rw-rw-   0        0        0     8505 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/karyotype_mapping.py
--rw-rw-rw-   0        0        0     6258 2023-03-31 14:23:24.000000 wgdi-0.6.4/wgdi/ks.py
--rw-rw-rw-   0        0        0     3992 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/ks_peaks.py
--rw-rw-rw-   0        0        0     3459 2022-12-07 13:59:23.000000 wgdi-0.6.4/wgdi/ksfigure.py
--rw-rw-rw-   0        0        0     3535 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/peaksfit.py
--rw-rw-rw-   0        0        0     5326 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/pindex.py
--rw-rw-rw-   0        0        0     2765 2022-12-07 14:03:46.000000 wgdi-0.6.4/wgdi/polyploidy_classification.py
--rw-rw-rw-   0        0        0     3548 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/retain.py
--rw-rw-rw-   0        0        0     7700 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/run.py
--rw-rw-rw-   0        0        0     5929 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/run_colliearity.py
--rw-rw-rw-   0        0        0     3799 2023-03-14 08:55:40.000000 wgdi-0.6.4/wgdi/shared_fusion.py
--rw-rw-rw-   0        0        0     7886 2022-10-20 11:27:44.000000 wgdi-0.6.4/wgdi/trees.py
-drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.270232 wgdi-0.6.4/wgdi.egg-info/
--rw-rw-rw-   0        0        0     5499 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-11 13:38:16.380595 wgdi-0.6.5/
+-rw-rw-rw-   0        0        0     5611 2023-05-11 13:38:16.380595 wgdi-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4199 2023-05-11 13:25:34.000000 wgdi-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 13:38:16.381596 wgdi-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-05-11 13:10:09.000000 wgdi-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:38:16.321059 wgdi-0.6.5/wgdi/
+-rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/__init__.py
+-rw-rw-rw-   0        0        0     8121 2023-04-22 11:59:58.000000 wgdi-0.6.5/wgdi/align_dotplot.py
+-rw-rw-rw-   0        0        0     2644 2023-05-11 12:33:44.000000 wgdi-0.6.5/wgdi/ancestral_karyotype.py
+-rw-rw-rw-   0        0        0     3385 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/ancestral_karyotype_repertoire.py
+-rw-rw-rw-   0        0        0     8288 2023-04-27 12:13:13.000000 wgdi-0.6.5/wgdi/base.py
+-rw-rw-rw-   0        0        0     3889 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/block_correspondence.py
+-rw-rw-rw-   0        0        0     7791 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/block_info.py
+-rw-rw-rw-   0        0        0     5023 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/block_ks.py
+-rw-rw-rw-   0        0        0    11229 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/circos.py
+-rw-rw-rw-   0        0        0     6798 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/collinearity.py
+-rw-rw-rw-   0        0        0     6225 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/dotplot.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:38:16.378597 wgdi-0.6.5/wgdi/example/
+-rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/__init__.py
+-rw-rw-rw-   0        0        0      398 2023-04-04 06:33:01.000000 wgdi-0.6.5/wgdi/example/align.conf
+-rw-rw-rw-   0        0        0      540 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/alignmenttrees.conf
+-rw-rw-rw-   0        0        0      341 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/ancestral_karyotype.conf
+-rw-rw-rw-   0        0        0      473 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/ancestral_karyotype_repertoire.conf
+-rw-rw-rw-   0        0        0      281 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/blockinfo.conf
+-rw-rw-rw-   0        0        0      315 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/blockks.conf
+-rw-rw-rw-   0        0        0      443 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/circos.conf
+-rw-rw-rw-   0        0        0      302 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/collinearity.conf
+-rw-rw-rw-   0        0        0      368 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/conf.ini
+-rw-rw-rw-   0        0        0      237 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/corr.conf
+-rw-rw-rw-   0        0        0      423 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/dotplot.conf
+-rw-rw-rw-   0        0        0      120 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/karyotype.conf
+-rw-rw-rw-   0        0        0      434 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/karyotype_mapping.conf
+-rw-rw-rw-   0        0        0      183 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/ks.conf
+-rw-rw-rw-   0        0        0      383 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/ks_fit_result.csv
+-rw-rw-rw-   0        0        0      250 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/ksfigure.conf
+-rw-rw-rw-   0        0        0      260 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/kspeaks.conf
+-rw-rw-rw-   0        0        0      200 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/peaksfit.conf
+-rw-rw-rw-   0        0        0      178 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/pindex.conf
+-rw-rw-rw-   0        0        0      182 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/polyploidy_classification.conf
+-rw-rw-rw-   0        0        0      235 2022-09-16 11:35:58.000000 wgdi-0.6.5/wgdi/example/retain.conf
+-rw-rw-rw-   0        0        0      332 2023-03-31 14:17:47.000000 wgdi-0.6.5/wgdi/example/shared_fusion.conf
+-rw-rw-rw-   0        0        0     1637 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/karyotype.py
+-rw-rw-rw-   0        0        0     8505 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/karyotype_mapping.py
+-rw-rw-rw-   0        0        0     6258 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/ks.py
+-rw-rw-rw-   0        0        0     3992 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/ks_peaks.py
+-rw-rw-rw-   0        0        0     3459 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/ksfigure.py
+-rw-rw-rw-   0        0        0     3535 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/peaksfit.py
+-rw-rw-rw-   0        0        0     5326 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/pindex.py
+-rw-rw-rw-   0        0        0     2765 2023-05-09 20:29:45.000000 wgdi-0.6.5/wgdi/polyploidy_classification.py
+-rw-rw-rw-   0        0        0     3548 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/retain.py
+-rw-rw-rw-   0        0        0     7700 2023-05-11 13:11:15.000000 wgdi-0.6.5/wgdi/run.py
+-rw-rw-rw-   0        0        0     6088 2023-05-11 13:34:29.000000 wgdi-0.6.5/wgdi/run_colliearity.py
+-rw-rw-rw-   0        0        0     4081 2023-05-11 13:11:18.000000 wgdi-0.6.5/wgdi/shared_fusion.py
+-rw-rw-rw-   0        0        0     7886 2023-04-23 11:33:17.000000 wgdi-0.6.5/wgdi/trees.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:38:16.334058 wgdi-0.6.5/wgdi.egg-info/
+-rw-rw-rw-   0        0        0     5611 2023-05-11 13:38:16.000000 wgdi-0.6.5/wgdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-05-11 13:38:16.000000 wgdi-0.6.5/wgdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 13:38:16.000000 wgdi-0.6.5/wgdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-11 13:38:16.000000 wgdi-0.6.5/wgdi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-05-11 13:38:16.000000 wgdi-0.6.5/wgdi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-11 13:38:16.000000 wgdi-0.6.5/wgdi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-11 13:38:16.000000 wgdi-0.6.5/wgdi.egg-info/zip-safe
```

### Comparing `wgdi-0.6.4/PKG-INFO` & `wgdi-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgdi
-Version: 0.6.4
+Version: 0.6.5
 Summary: Whole Genome Duplication Identification
 Home-page: https://github.com/SunPengChuan/wgdi
 Author: Pengchuan Sun
 Author-email: sunpengchuan@gmail.com
 License: BSD License
 Description: # WGDI
         
@@ -54,14 +54,18 @@
         
         If you use wgdi in your work, please cite:
         
         > Sun P., Jiao B., Yang Y., Shan L., Li T., Li X., Xi Z., Wang X., and Liu J. (2022). WGDI: A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes. Mol. Plant. doi: https://doi.org/10.1016/j.molp.2022.10.018.
         
         ## News
         
+        ## 0.6.5
+        * Fixed some issues (-sf).
+        * Added new tips to avoid some errors.
+        
         ## 0.6.4
         * Fixed the problem caused by the Python version, now it is compatible with version 3.11.3.
         
         ## 0.6.3
         * Fixed some issues (-ks, -sf).
         
         ## 0.6.2
```

### Comparing `wgdi-0.6.4/README.md` & `wgdi-0.6.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 
 If you use wgdi in your work, please cite:
 
 > Sun P., Jiao B., Yang Y., Shan L., Li T., Li X., Xi Z., Wang X., and Liu J. (2022). WGDI: A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes. Mol. Plant. doi: https://doi.org/10.1016/j.molp.2022.10.018.
 
 ## News
 
+## 0.6.5
+* Fixed some issues (-sf).
+* Added new tips to avoid some errors.
+
 ## 0.6.4
 * Fixed the problem caused by the Python version, now it is compatible with version 3.11.3.
 
 ## 0.6.3
 * Fixed some issues (-ks, -sf).
 
 ## 0.6.2
```

### Comparing `wgdi-0.6.4/setup.py` & `wgdi-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 required = ['pandas>=1.1.0', 'numpy', 'biopython', 'matplotlib', 'scipy']
 
 setup(
     name="wgdi",
-    version="0.6.4",
+    version="0.6.5",
     author="Pengchuan Sun",
     author_email="sunpengchuan@gmail.com",
     description="Whole Genome Duplication Identification",
     license="BSD License",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunPengChuan/wgdi",
```

### Comparing `wgdi-0.6.4/wgdi/align_dotplot.py` & `wgdi-0.6.5/wgdi/align_dotplot.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/ancestral_karyotype.py` & `wgdi-0.6.5/wgdi/ancestral_karyotype.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                     data.append(newgff.loc[k, :].values.tolist()+[k])
             dict1[str(num)] = cla
             dict2[str(num)] = group[3].values[0]
             num+=1
         df = pd.DataFrame(data)
         pep = SeqIO.to_dict(SeqIO.parse(self.pep_file, "fasta"))
         df = df[df[6].isin(pep.keys())]
-        for name, group in df.groupby([0]):
+        for name, group in df.groupby(0):
             df.loc[group.index, 'order'] = list(range(1, len(group)+1))
             df.loc[group.index, 'newname'] = list(
                 [str(self.mark)+str(name)+'g'+str(i).zfill(5) for i in range(1, len(group)+1)])
         df['order'] = df['order'].astype('int')
         df = df[[0, 'newname', 1, 2, 3, 'order', 6]]
         df = df.sort_values(by=[0, 'order'])
         df.to_csv(self.ancestor_gff, sep="\t", index=False, header=None)
```

### Comparing `wgdi-0.6.4/wgdi/ancestral_karyotype_repertoire.py` & `wgdi-0.6.5/wgdi/ancestral_karyotype_repertoire.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/base.py` & `wgdi-0.6.5/wgdi/base.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/block_correspondence.py` & `wgdi-0.6.5/wgdi/block_correspondence.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/block_info.py` & `wgdi-0.6.5/wgdi/block_info.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/block_ks.py` & `wgdi-0.6.5/wgdi/block_ks.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/circos.py` & `wgdi-0.6.5/wgdi/circos.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/collinearity.py` & `wgdi-0.6.5/wgdi/collinearity.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/dotplot.py` & `wgdi-0.6.5/wgdi/dotplot.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/example/alignmenttrees.conf` & `wgdi-0.6.5/wgdi/example/alignmenttrees.conf`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/karyotype.py` & `wgdi-0.6.5/wgdi/karyotype.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/karyotype_mapping.py` & `wgdi-0.6.5/wgdi/karyotype_mapping.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/ks.py` & `wgdi-0.6.5/wgdi/ks.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/ks_peaks.py` & `wgdi-0.6.5/wgdi/ks_peaks.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/ksfigure.py` & `wgdi-0.6.5/wgdi/ksfigure.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/peaksfit.py` & `wgdi-0.6.5/wgdi/peaksfit.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/pindex.py` & `wgdi-0.6.5/wgdi/pindex.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/polyploidy_classification.py` & `wgdi-0.6.5/wgdi/polyploidy_classification.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/retain.py` & `wgdi-0.6.5/wgdi/retain.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi/run.py` & `wgdi-0.6.5/wgdi/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 parser = argparse.ArgumentParser(
     prog='wgdi', usage='%(prog)s [options]', epilog="", formatter_class=argparse.RawDescriptionHelpFormatter,)
 parser.description = '''\
 WGDI(Whole-Genome Duplication Integrated analysis):  A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes.
 
     https://wgdi.readthedocs.io/en/latest/
     -------------------------------------- '''
-parser.add_argument("-v", "--version", action='version', version='0.6.4')
+parser.add_argument("-v", "--version", action='version', version='0.6.5')
 parser.add_argument("-d", dest="dotplot",
                     help="Show homologous gene dotplot")
 parser.add_argument("-icl", dest="improvedcollinearity",
                     help="Improved version of ColinearScan ")
 parser.add_argument("-ks", dest="calks",
                     help="Calculate Ka/Ks for homologous gene pairs by YN00")
 parser.add_argument("-bk", dest="blockks",
```

### Comparing `wgdi-0.6.4/wgdi/run_colliearity.py` & `wgdi-0.6.5/wgdi/run_colliearity.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         blast = self.deal_blast(blast, int(
             self.multiple), int(self.repeat_number))
         blast['loc1'] = blast[0].map(gff1[self.position])
         blast['loc2'] = blast[1].map(gff2[self.position])
         blast['chr1'] = blast[0].map(gff1['chr'])
         blast['chr2'] = blast[1].map(gff2['chr'])
         print('The filtered homologous gene pairs are '+str(len(blast))+'.\n')
+        if len(blast)<1:
+            print('Stoped! \n\nIt may be that the id1 and id2 in the BLAST file do not match with (gff1,lens1) and (gff2, lens2).')
         total = []
         for (chr1, chr2), group in blast.groupby(['chr1', 'chr2']):
             total.append([chr1, chr2, group])
         del blast, group
         gc.collect()
         n = int(np.ceil(len(total) / float(self.process)))
         result, data = '', []
```

### Comparing `wgdi-0.6.4/wgdi/shared_fusion.py` & `wgdi-0.6.5/wgdi/shared_fusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,26 +54,28 @@
         for index, row in bkinfo.iterrows():
             # for specie1
             a, b = sorted([row['start1'], row['end1']])
             d1 = ancestor_left[(ancestor_left[0] == row['chr1']) & (
                 ancestor_left[2] >= a) & (ancestor_left[1] <= b)]
             if len(d1) > 1:
                 bkinfo.loc[index, 'breakpoints1'] = 1
+                breaklength_max = 0
                 for index2, row2 in d1.iterrows():
                     length_in = len(
                         [k for k in range(a, b) if k in range(row2[1], row2[2])])
                     length_out = (b-a)-length_in
-                bkinfo.loc[index, 'break_length1'] = min(
-                    length_in, length_out)+1
+                    breaklength_max =breaklength_max  if breaklength_max > min(length_in, length_out)+1 else min(length_in, length_out)+1
+                bkinfo.loc[index, 'break_length1'] = breaklength_max
             #for species2
             c, d = sorted([row['start2'], row['end2']])
             d2 = ancestor_top[(ancestor_top[0] == row['chr2']) & (
                 ancestor_top[2] >= c) & (ancestor_top[1] <= d)]
             if len(d2) > 1:
                 bkinfo.loc[index, 'breakpoints2'] = 1
+                breaklength_max = 0
                 for index2, row2 in d2.iterrows():
                     length_in = len(
                         [k for k in range(c, d) if k in range(row2[1], row2[2])])
                     length_out = (d-c)-length_in
-                bkinfo.loc[index, 'break_length2'] = min(
-                    length_in, length_out)+1
+                    breaklength_max =breaklength_max  if breaklength_max > min(length_in, length_out)+1 else min(length_in, length_out)+1
+                bkinfo.loc[index, 'break_length2'] = breaklength_max
         return bkinfo
```

### Comparing `wgdi-0.6.4/wgdi/trees.py` & `wgdi-0.6.5/wgdi/trees.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.4/wgdi.egg-info/PKG-INFO` & `wgdi-0.6.5/wgdi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgdi
-Version: 0.6.4
+Version: 0.6.5
 Summary: Whole Genome Duplication Identification
 Home-page: https://github.com/SunPengChuan/wgdi
 Author: Pengchuan Sun
 Author-email: sunpengchuan@gmail.com
 License: BSD License
 Description: # WGDI
         
@@ -54,14 +54,18 @@
         
         If you use wgdi in your work, please cite:
         
         > Sun P., Jiao B., Yang Y., Shan L., Li T., Li X., Xi Z., Wang X., and Liu J. (2022). WGDI: A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes. Mol. Plant. doi: https://doi.org/10.1016/j.molp.2022.10.018.
         
         ## News
         
+        ## 0.6.5
+        * Fixed some issues (-sf).
+        * Added new tips to avoid some errors.
+        
         ## 0.6.4
         * Fixed the problem caused by the Python version, now it is compatible with version 3.11.3.
         
         ## 0.6.3
         * Fixed some issues (-ks, -sf).
         
         ## 0.6.2
```

### Comparing `wgdi-0.6.4/wgdi.egg-info/SOURCES.txt` & `wgdi-0.6.5/wgdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


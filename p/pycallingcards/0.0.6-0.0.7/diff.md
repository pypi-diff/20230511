# Comparing `tmp/pycallingcards-0.0.6.tar.gz` & `tmp/pycallingcards-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycallingcards-0.0.6.tar", last modified: Thu May 11 04:59:48 2023, max compression
+gzip compressed data, was "pycallingcards-0.0.7.tar", last modified: Thu May 11 05:25:58 2023, max compression
```

## Comparing `pycallingcards-0.0.6.tar` & `pycallingcards-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.610863 pycallingcards-0.0.6/
--rw-r--r--   0 guojuanru   (501) staff       (20)     1500 2023-01-01 06:38:05.000000 pycallingcards-0.0.6/LICENSE
--rw-r--r--   0 guojuanru   (501) staff       (20)     2820 2023-05-11 04:59:48.610951 pycallingcards-0.0.6/PKG-INFO
--rw-r--r--   0 guojuanru   (501) staff       (20)     2466 2023-05-10 04:36:57.000000 pycallingcards-0.0.6/README.md
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.598290 pycallingcards-0.0.6/pycallingcards/
--rw-r--r--   0 guojuanru   (501) staff       (20)      273 2023-05-10 04:36:16.000000 pycallingcards-0.0.6/pycallingcards/__init__.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.599811 pycallingcards-0.0.6/pycallingcards/datasets/
--rw-r--r--   0 guojuanru   (501) staff       (20)      181 2023-01-24 21:27:26.000000 pycallingcards-0.0.6/pycallingcards/datasets/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    10887 2023-03-27 19:11:11.000000 pycallingcards-0.0.6/pycallingcards/datasets/_datasets.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.603704 pycallingcards-0.0.6/pycallingcards/plotting/
--rw-r--r--   0 guojuanru   (501) staff       (20)     9483 2023-05-10 04:35:29.000000 pycallingcards-0.0.6/pycallingcards/plotting/_Chipseq.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    10462 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/plotting/_GWAS.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6988 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/plotting/_WashU_browser.py
--rw-r--r--   0 guojuanru   (501) staff       (20)      473 2023-01-24 21:27:26.000000 pycallingcards-0.0.6/pycallingcards/plotting/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    33597 2023-03-30 18:36:40.000000 pycallingcards-0.0.6/pycallingcards/plotting/_dotplots.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     7669 2023-05-10 17:47:15.000000 pycallingcards-0.0.6/pycallingcards/plotting/_heatmap_ccrna.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     3399 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/plotting/_pair.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    63328 2023-05-11 04:38:48.000000 pycallingcards-0.0.6/pycallingcards/plotting/_peaks.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     4833 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/plotting/_plotting.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     3984 2023-03-30 18:20:24.000000 pycallingcards-0.0.6/pycallingcards/plotting/_volcano.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.607441 pycallingcards-0.0.6/pycallingcards/preprocessing/
--rw-r--r--   0 guojuanru   (501) staff       (20)      322 2023-03-27 19:58:22.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     7135 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_annotation.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    15203 2023-03-27 19:11:11.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_blo_algorithms.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6719 2023-03-27 19:11:11.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_blo_segmentation.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     2213 2023-03-27 19:11:10.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_blo_utilities.py
--rw-r--r--   0 guojuanru   (501) staff       (20)   212068 2023-05-09 19:01:43.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_callpeaks.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     2400 2023-03-27 19:11:11.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_clean.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     2296 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_filterpeaks.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     7299 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/preprocessing/_makeadata.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.607924 pycallingcards-0.0.6/pycallingcards/reading/
--rw-r--r--   0 guojuanru   (501) staff       (20)      186 2023-01-24 21:27:26.000000 pycallingcards-0.0.6/pycallingcards/reading/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     3330 2023-02-14 19:44:36.000000 pycallingcards-0.0.6/pycallingcards/reading/_read.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.610028 pycallingcards-0.0.6/pycallingcards/tools/
--rw-r--r--   0 guojuanru   (501) staff       (20)     7489 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/tools/_GWAS.py
--rw-r--r--   0 guojuanru   (501) staff       (20)      567 2023-01-24 21:27:26.000000 pycallingcards-0.0.6/pycallingcards/tools/__init__.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6583 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/tools/_call_motif.py
--rw-r--r--   0 guojuanru   (501) staff       (20)      847 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/tools/_find_fastq.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    16173 2023-03-30 18:20:24.000000 pycallingcards-0.0.6/pycallingcards/tools/_find_related_genes.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     4212 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/tools/_footprint.py
--rw-r--r--   0 guojuanru   (501) staff       (20)     6984 2023-03-27 19:11:14.000000 pycallingcards-0.0.6/pycallingcards/tools/_liftover.py
--rw-r--r--   0 guojuanru   (501) staff       (20)    50609 2023-03-30 18:20:24.000000 pycallingcards-0.0.6/pycallingcards/tools/_rank_peaks_group.py
-drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 04:59:48.599327 pycallingcards-0.0.6/pycallingcards.egg-info/
--rw-r--r--   0 guojuanru   (501) staff       (20)     2820 2023-05-11 04:59:48.000000 pycallingcards-0.0.6/pycallingcards.egg-info/PKG-INFO
--rw-r--r--   0 guojuanru   (501) staff       (20)     1454 2023-05-11 04:59:48.000000 pycallingcards-0.0.6/pycallingcards.egg-info/SOURCES.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)        1 2023-05-11 04:59:48.000000 pycallingcards-0.0.6/pycallingcards.egg-info/dependency_links.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)      232 2023-05-11 04:59:48.000000 pycallingcards-0.0.6/pycallingcards.egg-info/requires.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)       15 2023-05-11 04:59:48.000000 pycallingcards-0.0.6/pycallingcards.egg-info/top_level.txt
--rw-r--r--   0 guojuanru   (501) staff       (20)       85 2022-10-02 17:02:35.000000 pycallingcards-0.0.6/pyproject.toml
--rw-r--r--   0 guojuanru   (501) staff       (20)      775 2023-05-11 04:59:48.611313 pycallingcards-0.0.6/setup.cfg
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.383479 pycallingcards-0.0.7/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     1500 2023-01-01 06:38:05.000000 pycallingcards-0.0.7/LICENSE
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2411 2023-05-11 05:25:58.383571 pycallingcards-0.0.7/PKG-INFO
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2490 2023-05-11 05:25:40.000000 pycallingcards-0.0.7/README.md
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2057 2023-05-11 05:20:56.000000 pycallingcards-0.0.7/markdown.md
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.371240 pycallingcards-0.0.7/pycallingcards/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      273 2023-05-11 05:24:45.000000 pycallingcards-0.0.7/pycallingcards/__init__.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.372273 pycallingcards-0.0.7/pycallingcards/datasets/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      181 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/datasets/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    10887 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/datasets/_datasets.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.377335 pycallingcards-0.0.7/pycallingcards/plotting/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     9483 2023-05-10 04:35:29.000000 pycallingcards-0.0.7/pycallingcards/plotting/_Chipseq.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    10462 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_GWAS.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6988 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_WashU_browser.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)      473 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/plotting/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    33597 2023-03-30 18:36:40.000000 pycallingcards-0.0.7/pycallingcards/plotting/_dotplots.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7669 2023-05-10 17:47:15.000000 pycallingcards-0.0.7/pycallingcards/plotting/_heatmap_ccrna.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     3399 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_pair.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    63328 2023-05-11 04:38:48.000000 pycallingcards-0.0.7/pycallingcards/plotting/_peaks.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     4833 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/plotting/_plotting.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     3984 2023-03-30 18:20:24.000000 pycallingcards-0.0.7/pycallingcards/plotting/_volcano.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.380391 pycallingcards-0.0.7/pycallingcards/preprocessing/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      322 2023-03-27 19:58:22.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7135 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_annotation.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    15203 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_algorithms.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6719 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_segmentation.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2213 2023-03-27 19:11:10.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_utilities.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)   212068 2023-05-09 19:01:43.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_callpeaks.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2400 2023-03-27 19:11:11.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_clean.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2296 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_filterpeaks.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7299 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/preprocessing/_makeadata.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.380863 pycallingcards-0.0.7/pycallingcards/reading/
+-rw-r--r--   0 guojuanru   (501) staff       (20)      186 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/reading/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     3330 2023-02-14 19:44:36.000000 pycallingcards-0.0.7/pycallingcards/reading/_read.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.382765 pycallingcards-0.0.7/pycallingcards/tools/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     7489 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_GWAS.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)      567 2023-01-24 21:27:26.000000 pycallingcards-0.0.7/pycallingcards/tools/__init__.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6583 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_call_motif.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)      847 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_find_fastq.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    16173 2023-03-30 18:20:24.000000 pycallingcards-0.0.7/pycallingcards/tools/_find_related_genes.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     4212 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_footprint.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)     6984 2023-03-27 19:11:14.000000 pycallingcards-0.0.7/pycallingcards/tools/_liftover.py
+-rw-r--r--   0 guojuanru   (501) staff       (20)    50609 2023-03-30 18:20:24.000000 pycallingcards-0.0.7/pycallingcards/tools/_rank_peaks_group.py
+drwxr-xr-x   0 guojuanru   (501) staff       (20)        0 2023-05-11 05:25:58.371809 pycallingcards-0.0.7/pycallingcards.egg-info/
+-rw-r--r--   0 guojuanru   (501) staff       (20)     2411 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/PKG-INFO
+-rw-r--r--   0 guojuanru   (501) staff       (20)     1466 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/SOURCES.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)        1 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/dependency_links.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)      232 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/requires.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)       15 2023-05-11 05:25:58.000000 pycallingcards-0.0.7/pycallingcards.egg-info/top_level.txt
+-rw-r--r--   0 guojuanru   (501) staff       (20)       85 2022-10-02 17:02:35.000000 pycallingcards-0.0.7/pyproject.toml
+-rw-r--r--   0 guojuanru   (501) staff       (20)      777 2023-05-11 05:25:58.383939 pycallingcards-0.0.7/setup.cfg
```

### Comparing `pycallingcards-0.0.6/LICENSE` & `pycallingcards-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/PKG-INFO` & `pycallingcards-0.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,13 @@
-Metadata-Version: 2.1
-Name: pycallingcards
-Version: 0.0.6
-Summary: "Calling cards data analysis in Python."
-Home-page: https://github.com/The-Mitra-Lab/pycallingcards
-Author: "The-Mitra-Lab"
-Author-email: "rmitra@wustl.edu"
-License: BSD 3-Clause License
-Platform: any
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Pycallingcards
 
 [![](https://readthedocs.org/projects/pycallingcards/badge/?version=latest)](https://pycallingcards.readthedocs.io/en/latest/)
 
 <p align="center">
-    <img src="./docs/_static/logo.png", width="350">
+    <img src="https://github.com/The-Mitra-Lab/pycallingcards/assets/64772552/4eb2fa43-1f69-4a35-8b7e-72568e0f95e7", width="350">
 </p>
 
 **Pycallingcards** is a package for calling cards data analysis developed and maintained by [Mitra Lab](http://genetics.wustl.edu/rmlab/) at Washington University in St. Louis.
 
 Calling cards is a sequencing technology to assay TF binding which could be done in vitro and in vivo at both bulk and single-cell level. To know more about calling cards technology, please check [Moudgil et al](https://www.sciencedirect.com/science/article/pii/S009286742030814X?via%3Dihub) and [Wang et al](http://genetics.wustl.edu/rmlab/files/2012/09/Calling-Cards-for-DNA-binding.pdf).
 
 
@@ -37,15 +24,15 @@
 ## Documentation.
 
 Please check [**here**](https://pycallingcards.readthedocs.io/en/latest/) for detailed documentation.
 
 ## Installation
 
 ```shell
-pip install "git+https://github.com/The-Mitra-Lab/pycallingcards.git" --upgrade
+pip install pycallingcards
 ```
 
 ## Development
 
 Use pre-commit to format code at `git commit`.
 
 ```shell
@@ -58,10 +45,10 @@
 ```bibtex
 @software{pycallingcards_python,
   author = {Guo, Juanru and Mitra, Robi},
   month = {2},
   year = {2023},
   title = {Pycallingcards: Calling Cards Data Analysis in Python},
   url = {https://github.com/The-Mitra-Lab/pycallingcards},
-  version = {0.0.6},
+  version = {0.0.7},
 }
 ```
```

### Comparing `pycallingcards-0.0.6/README.md` & `pycallingcards-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,25 @@
+Metadata-Version: 2.1
+Name: pycallingcards
+Version: 0.0.7
+Summary: "Calling cards data analysis in Python."
+Home-page: https://github.com/The-Mitra-Lab/pycallingcards
+Author: "The-Mitra-Lab"
+Author-email: "rmitra@wustl.edu"
+License: BSD 3-Clause License
+Platform: any
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Pycallingcards
 
 [![](https://readthedocs.org/projects/pycallingcards/badge/?version=latest)](https://pycallingcards.readthedocs.io/en/latest/)
 
-<p align="center">
-    <img src="./docs/_static/logo.png", width="350">
-</p>
+
 
 **Pycallingcards** is a package for calling cards data analysis developed and maintained by [Mitra Lab](http://genetics.wustl.edu/rmlab/) at Washington University in St. Louis.
 
 Calling cards is a sequencing technology to assay TF binding which could be done in vitro and in vivo at both bulk and single-cell level. To know more about calling cards technology, please check [Moudgil et al](https://www.sciencedirect.com/science/article/pii/S009286742030814X?via%3Dihub) and [Wang et al](http://genetics.wustl.edu/rmlab/files/2012/09/Calling-Cards-for-DNA-binding.pdf).
 
 
 Pycallingcards is composed of five different part: datasets, reading (rd), preprocessing (pp), tools (tl) and plotting (pl).
@@ -24,31 +35,18 @@
 ## Documentation.
 
 Please check [**here**](https://pycallingcards.readthedocs.io/en/latest/) for detailed documentation.
 
 ## Installation
 
 ```shell
-pip install "git+https://github.com/The-Mitra-Lab/pycallingcards.git" --upgrade
+pip install pycallingcards
 ```
 
 ## Development
 
 Use pre-commit to format code at `git commit`.
 
 ```shell
 pip install pre-commit
 pre-commit install
 ```
-
-## Cite
-
-```bibtex
-@software{pycallingcards_python,
-  author = {Guo, Juanru and Mitra, Robi},
-  month = {2},
-  year = {2023},
-  title = {Pycallingcards: Calling Cards Data Analysis in Python},
-  url = {https://github.com/The-Mitra-Lab/pycallingcards},
-  version = {0.0.6},
-}
-```
```

### Comparing `pycallingcards-0.0.6/pycallingcards/datasets/_datasets.py` & `pycallingcards-0.0.7/pycallingcards/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_Chipseq.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_Chipseq.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_GWAS.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_GWAS.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_WashU_browser.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_WashU_browser.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_dotplots.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_dotplots.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_heatmap_ccrna.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_heatmap_ccrna.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_pair.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_pair.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_peaks.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_peaks.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_plotting.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/plotting/_volcano.py` & `pycallingcards-0.0.7/pycallingcards/plotting/_volcano.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_annotation.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_annotation.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_blo_algorithms.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_algorithms.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_blo_segmentation.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_segmentation.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_blo_utilities.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_blo_utilities.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_callpeaks.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_callpeaks.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_clean.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_clean.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_filterpeaks.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_filterpeaks.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/preprocessing/_makeadata.py` & `pycallingcards-0.0.7/pycallingcards/preprocessing/_makeadata.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/reading/_read.py` & `pycallingcards-0.0.7/pycallingcards/reading/_read.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/_GWAS.py` & `pycallingcards-0.0.7/pycallingcards/tools/_GWAS.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/__init__.py` & `pycallingcards-0.0.7/pycallingcards/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/_call_motif.py` & `pycallingcards-0.0.7/pycallingcards/tools/_call_motif.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/_find_fastq.py` & `pycallingcards-0.0.7/pycallingcards/tools/_find_fastq.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/_find_related_genes.py` & `pycallingcards-0.0.7/pycallingcards/tools/_find_related_genes.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/_footprint.py` & `pycallingcards-0.0.7/pycallingcards/tools/_footprint.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/_liftover.py` & `pycallingcards-0.0.7/pycallingcards/tools/_liftover.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards/tools/_rank_peaks_group.py` & `pycallingcards-0.0.7/pycallingcards/tools/_rank_peaks_group.py`

 * *Files identical despite different names*

### Comparing `pycallingcards-0.0.6/pycallingcards.egg-info/PKG-INFO` & `pycallingcards-0.0.7/pycallingcards.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: pycallingcards
-Version: 0.0.6
+Version: 0.0.7
 Summary: "Calling cards data analysis in Python."
 Home-page: https://github.com/The-Mitra-Lab/pycallingcards
 Author: "The-Mitra-Lab"
 Author-email: "rmitra@wustl.edu"
 License: BSD 3-Clause License
 Platform: any
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Pycallingcards
 
 [![](https://readthedocs.org/projects/pycallingcards/badge/?version=latest)](https://pycallingcards.readthedocs.io/en/latest/)
 
-<p align="center">
-    <img src="./docs/_static/logo.png", width="350">
-</p>
+
 
 **Pycallingcards** is a package for calling cards data analysis developed and maintained by [Mitra Lab](http://genetics.wustl.edu/rmlab/) at Washington University in St. Louis.
 
 Calling cards is a sequencing technology to assay TF binding which could be done in vitro and in vivo at both bulk and single-cell level. To know more about calling cards technology, please check [Moudgil et al](https://www.sciencedirect.com/science/article/pii/S009286742030814X?via%3Dihub) and [Wang et al](http://genetics.wustl.edu/rmlab/files/2012/09/Calling-Cards-for-DNA-binding.pdf).
 
 
 Pycallingcards is composed of five different part: datasets, reading (rd), preprocessing (pp), tools (tl) and plotting (pl).
@@ -37,31 +35,18 @@
 ## Documentation.
 
 Please check [**here**](https://pycallingcards.readthedocs.io/en/latest/) for detailed documentation.
 
 ## Installation
 
 ```shell
-pip install "git+https://github.com/The-Mitra-Lab/pycallingcards.git" --upgrade
+pip install pycallingcards
 ```
 
 ## Development
 
 Use pre-commit to format code at `git commit`.
 
 ```shell
 pip install pre-commit
 pre-commit install
 ```
-
-## Cite
-
-```bibtex
-@software{pycallingcards_python,
-  author = {Guo, Juanru and Mitra, Robi},
-  month = {2},
-  year = {2023},
-  title = {Pycallingcards: Calling Cards Data Analysis in Python},
-  url = {https://github.com/The-Mitra-Lab/pycallingcards},
-  version = {0.0.6},
-}
-```
```

### Comparing `pycallingcards-0.0.6/pycallingcards.egg-info/SOURCES.txt` & `pycallingcards-0.0.7/pycallingcards.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+markdown.md
 pyproject.toml
 setup.cfg
 pycallingcards/__init__.py
 pycallingcards.egg-info/PKG-INFO
 pycallingcards.egg-info/SOURCES.txt
 pycallingcards.egg-info/dependency_links.txt
 pycallingcards.egg-info/requires.txt
```

### Comparing `pycallingcards-0.0.6/setup.cfg` & `pycallingcards-0.0.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = pycallingcards
 description = "Calling cards data analysis in Python."
 author = "The-Mitra-Lab"
-version = 0.0.6
+version = 0.0.7
 author_email = "rmitra@wustl.edu"
-long_description = file: README.md
+long_description = file: markdown.md
 long_description_content_type = text/markdown
 url = https://github.com/The-Mitra-Lab/pycallingcards
 license = BSD 3-Clause License
 license_file = LICENSE
 platform = any
 
 [options]
```


# Comparing `tmp/astro_ghost-0.2.5.tar.gz` & `tmp/astro_ghost-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-0.2.5.tar", last modified: Wed May 10 06:02:28 2023, max compression
+gzip compressed data, was "astro_ghost-0.2.6.tar", last modified: Thu May 11 04:21:21 2023, max compression
```

## Comparing `astro_ghost-0.2.5.tar` & `astro_ghost-0.2.6.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.651828 astro_ghost-0.2.5/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.572502 astro_ghost-0.2.5/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.580490 astro_ghost-0.2.5/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-0.2.5/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4545 2023-05-10 06:02:28.652168 astro_ghost-0.2.5/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3944 2023-05-09 18:24:32.000000 astro_ghost-0.2.5/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.629822 astro_ghost-0.2.5/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    15169 2023-05-09 21:30:32.000000 astro_ghost-0.2.5/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     5977 2023-05-09 20:44:59.000000 astro_ghost-0.2.5/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    39061 2023-05-10 05:59:47.000000 astro_ghost-0.2.5/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1291 2023-05-09 21:52:41.000000 astro_ghost-0.2.5/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-0.2.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1527 2023-05-09 19:21:33.000000 astro_ghost-0.2.5/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-0.2.5/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-09 18:21:58.000000 astro_ghost-0.2.5/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-0.2.5/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37898 2023-05-09 22:25:05.000000 astro_ghost-0.2.5/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32694 2023-05-09 21:21:00.000000 astro_ghost-0.2.5/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-0.2.5/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    16026 2023-05-09 22:49:43.000000 astro_ghost-0.2.5/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    10333 2023-05-09 19:38:06.000000 astro_ghost-0.2.5/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     6613 2023-05-09 19:30:32.000000 astro_ghost-0.2.5/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     5769 2023-05-09 21:06:58.000000 astro_ghost-0.2.5/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-0.2.5/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.633933 astro_ghost-0.2.5/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4545 2023-05-10 06:02:28.000000 astro_ghost-0.2.5/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1124 2023-05-10 06:02:28.000000 astro_ghost-0.2.5/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-10 06:02:28.000000 astro_ghost-0.2.5/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-10 06:02:28.000000 astro_ghost-0.2.5/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2023-05-10 06:02:28.000000 astro_ghost-0.2.5/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-10 06:02:28.000000 astro_ghost-0.2.5/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.634581 astro_ghost-0.2.5/database/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3288 2023-02-16 19:42:21.000000 astro_ghost-0.2.5/database/GHOST.csv
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.638861 astro_ghost-0.2.5/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-0.2.5/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.642403 astro_ghost-0.2.5/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2377 2023-05-10 05:52:52.000000 astro_ghost-0.2.5/docs/source/astro_ghost.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3853 2023-05-10 05:28:17.000000 astro_ghost-0.2.5/docs/source/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)       70 2023-05-10 00:04:14.000000 astro_ghost-0.2.5/docs/source/modules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.646031 astro_ghost-0.2.5/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-0.2.5/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1603 2023-05-10 06:02:28.655654 astro_ghost-0.2.5/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1805 2023-05-09 22:18:50.000000 astro_ghost-0.2.5/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-10 06:02:28.650459 astro_ghost-0.2.5/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-0.2.5/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       58 2023-02-16 19:42:21.000000 astro_ghost-0.2.5/tests/test_basic.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4050 2023-05-09 18:37:23.000000 astro_ghost-0.2.5/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-09 18:27:03.000000 astro_ghost-0.2.5/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.113041 astro_ghost-0.2.6/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:20.990882 astro_ghost-0.2.6/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:20.997858 astro_ghost-0.2.6/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-0.2.6/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 04:21:21.113361 astro_ghost-0.2.6/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-0.2.6/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.087980 astro_ghost-0.2.6/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    15169 2023-05-09 21:30:32.000000 astro_ghost-0.2.6/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-0.2.6/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    39061 2023-05-10 05:59:47.000000 astro_ghost-0.2.6/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-0.2.6/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-0.2.6/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1527 2023-05-09 19:21:33.000000 astro_ghost-0.2.6/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-0.2.6/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-11 04:20:13.000000 astro_ghost-0.2.6/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-0.2.6/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37898 2023-05-09 22:25:05.000000 astro_ghost-0.2.6/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32745 2023-05-10 22:07:36.000000 astro_ghost-0.2.6/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-0.2.6/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    15960 2023-05-10 22:18:36.000000 astro_ghost-0.2.6/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    10333 2023-05-09 19:38:06.000000 astro_ghost-0.2.6/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     6616 2023-05-10 22:27:43.000000 astro_ghost-0.2.6/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4604 2023-05-11 04:18:51.000000 astro_ghost-0.2.6/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-0.2.6/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.092649 astro_ghost-0.2.6/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1301 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.096909 astro_ghost-0.2.6/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-0.2.6/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-0.2.6/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.105385 astro_ghost-0.2.6/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-0.2.6/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-0.2.6/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-0.2.6/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-0.2.6/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-0.2.6/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-0.2.6/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-0.2.6/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-0.2.6/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.109190 astro_ghost-0.2.6/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1603 2023-05-11 04:21:21.115497 astro_ghost-0.2.6/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-11 04:19:54.000000 astro_ghost-0.2.6/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.112222 astro_ghost-0.2.6/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-0.2.6/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1655 2023-05-11 04:18:55.000000 astro_ghost-0.2.6/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2421 2023-05-10 23:12:38.000000 astro_ghost-0.2.6/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-10 20:57:05.000000 astro_ghost-0.2.6/tox.ini
```

### Comparing `astro_ghost-0.2.5/.github/workflows/tests.yml` & `astro_ghost-0.2.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/.gitignore` & `astro_ghost-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/PKG-INFO` & `astro_ghost-0.2.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +23,18 @@
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
 .. image:: https://img.shields.io/pypi/dm/astro-ghost
    :target: https://pypi.org/project/astro-ghost/
-   :alt: PyPI - Downloads
+   :alt: PyPI
 
-.. image:: https://img.shields.io/readthedocs/astro-ghost
-   :target: https://astro-ghost.readthedocs.io/en/latest/
+.. image:: https://img.shields.io/readthedocs/uiucsnastro-ghost
+   :target: https://uiucsnastro-ghost.readthedocs.io/en/latest/
    :alt: Read the Docs
 
 "At the last dim horizon, we search among ghostly errors of observations for
 landmarks that are scarcely more substantial. The search will continue. The
 urge is older than history. It is not satisfied and it will not be oppressed."
 --Edwin Hubble
 
@@ -43,15 +43,15 @@
 classes in Gagliano et al. (2020). Installation instructions for the analysis
 tools are below.
 
 Installation
 ------------
 
 For details on installing and using GHOST, see the
-`documentation <https://astro-ghost.readthedocs.io/en/latest/>`_.
+`documentation <https://uiucsnastro-ghost.readthedocs.io/en/latest/>`_.
 
 
 Citation
 ------------
 If you use this code, please cite the associated paper with the bibtex entry below::
 
    @ARTICLE{2021ApJ...908..170G,
@@ -97,19 +97,12 @@
 We assure you - the little voice in your head is wrong. If you can write code at
 all, you can contribute code to open source. Contributing to open source
 projects is a fantastic way to advance one's coding skills. Writing perfect code
 isn't the measure of a good developer (that would disqualify all of us!); it's
 trying to create something, making mistakes, and learning from those
 mistakes. That's how we all improve, and we are happy to help others learn.
 
-Being an open source contributor doesn't just mean writing code, either. You can
-help out by writing documentation, tests, or even giving feedback about the
-project (and yes - that includes giving feedback about the contribution
-process). Some of these contributions may be the most valuable to the project as
-a whole, because you're coming to the project with fresh eyes, so you can see
-the errors and assumptions that seasoned contributors have glossed over.
-
 Note: This disclaimer was originally written by
 `Adrienne Lowe <https://github.com/adriennefriend>`_ for a
 `PyCon talk <https://www.youtube.com/watch?v=6Uj746j9Heo>`_, and was adapted by
 astro_ghost based on its use in the README file for the
 `MetPy project <https://github.com/Unidata/MetPy>`_.
```

### Comparing `astro_ghost-0.2.5/README.rst` & `astro_ghost-0.2.6/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
 .. image:: https://img.shields.io/pypi/dm/astro-ghost
    :target: https://pypi.org/project/astro-ghost/
-   :alt: PyPI - Downloads
+   :alt: PyPI
 
-.. image:: https://img.shields.io/readthedocs/astro-ghost
-   :target: https://astro-ghost.readthedocs.io/en/latest/
+.. image:: https://img.shields.io/readthedocs/uiucsnastro-ghost
+   :target: https://uiucsnastro-ghost.readthedocs.io/en/latest/
    :alt: Read the Docs
 
 "At the last dim horizon, we search among ghostly errors of observations for
 landmarks that are scarcely more substantial. The search will continue. The
 urge is older than history. It is not satisfied and it will not be oppressed."
 --Edwin Hubble
 
@@ -25,15 +25,15 @@
 classes in Gagliano et al. (2020). Installation instructions for the analysis
 tools are below.
 
 Installation
 ------------
 
 For details on installing and using GHOST, see the
-`documentation <https://astro-ghost.readthedocs.io/en/latest/>`_.
+`documentation <https://uiucsnastro-ghost.readthedocs.io/en/latest/>`_.
 
 
 Citation
 ------------
 If you use this code, please cite the associated paper with the bibtex entry below::
 
    @ARTICLE{2021ApJ...908..170G,
@@ -79,19 +79,12 @@
 We assure you - the little voice in your head is wrong. If you can write code at
 all, you can contribute code to open source. Contributing to open source
 projects is a fantastic way to advance one's coding skills. Writing perfect code
 isn't the measure of a good developer (that would disqualify all of us!); it's
 trying to create something, making mistakes, and learning from those
 mistakes. That's how we all improve, and we are happy to help others learn.
 
-Being an open source contributor doesn't just mean writing code, either. You can
-help out by writing documentation, tests, or even giving feedback about the
-project (and yes - that includes giving feedback about the contribution
-process). Some of these contributions may be the most valuable to the project as
-a whole, because you're coming to the project with fresh eyes, so you can see
-the errors and assumptions that seasoned contributors have glossed over.
-
 Note: This disclaimer was originally written by
 `Adrienne Lowe <https://github.com/adriennefriend>`_ for a
 `PyCon talk <https://www.youtube.com/watch?v=6Uj746j9Heo>`_, and was adapted by
 astro_ghost based on its use in the README file for the
 `MetPy project <https://github.com/Unidata/MetPy>`_.
```

### Comparing `astro_ghost-0.2.5/astro_ghost/DLR.py` & `astro_ghost-0.2.6/astro_ghost/DLR.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-0.2.6/astro_ghost/NEDQueryFunctions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from astropy import units as u
 from astropy.coordinates import SkyCoord
-from astroquery.ned import Ned
+from astroquery.ipac.ned import Ned
 import re
 import numpy as np
 from astro_ghost.PS1QueryFunctions import find_all
 
 import warnings
 warnings.filterwarnings("ignore", category=UserWarning)
 
@@ -59,21 +59,14 @@
     df["NED_redshift"] = np.nan
     df["NED_mag"] = np.nan
     df["NED_redshift_flag"] = ""
 
     ra = df["raMean"]
     dec = df["decMean"]
 
-    # setup lists for ra and dec in hr format, names of NED-identified object, and
-    # separation between host in PS1 and host in NED
-    ra_hms = []
-    dec_dms = []
-    names = []
-    sep = []
-
     missingCounter = 0
 
     for index, row in df.iterrows():
         tempRA = ra[index]
         tempDEC = dec[index]
 
         # create a sky coordinate to query NED
@@ -85,60 +78,44 @@
         tempType = ""
         tempRed = np.nan
         tempVel = np.nan
         tempMag = np.nan
 
         try:
             #query NED with a 2'' radius.
-            result_table = Ned.query_region(c, radius=(0.00055555)*u.deg, equinox='J2000.0')
-
+            result_table = Ned.query_region(c, radius=(2/3600)*u.deg, equinox='J2000.0')
             if len(result_table) > 0:
                 missingCounter = 0
         except:
             missingCounter += 1
         if len(result_table) > 0:
-            result_table = result_table[result_table['Separation'] == np.min(result_table['Separation'])]
-            result_table = result_table[result_table['Type'] != b'SN']
-            result_table = result_table[result_table['Type'] != b'MCld']
-            result_gal = result_table[result_table['Type'] == b'G']
+            #if Messier or NGC object, take that, otherwise take the closest object
+            result_df = result_table.to_pandas()
+            if len(result_df) > 1:
+                result_NGC = result_df[[x.startswith("NGC") for x in result_df['Object Name']]]
+                if len(result_NGC) > 0:
+                    result_df = result_NGC.copy()
+                else:
+                    result_M = result_df[[x.startswith("NGC") for x in result_df['Object Name']]]
+                    if len(result_M) > 0:
+                        result_df = result_M.copy()
+            result_gal = result_df[result_df['Type'] == b'G']
             if len(result_gal) > 0:
-                result_table = result_gal
-            if len(result_table) > 0:
-
-                # Subset for the objects with listed references and photometry, if more than one option.
-                result_table = result_table[result_table['Photometry Points'] == np.nanmax(result_table['Photometry Points'])]
-                result_table = result_table[result_table['References'] == np.nanmax(result_table['References'])]
-
-                # NED Info is presented as:
-                # No. ObjectName	RA	DEC	Type	Velocity	Redshift	Redshift Flag	Magnitude and Filter	Separation	References	Notes	Photometry Points	Positions	Redshift Points	Diameter Points	Associations
-                #Split NED info up - specifically, we want to pull the type, velocity, redshift, mag
-                tempNED = str(np.array(result_table)[0]).split(",")
-                if len(tempNED) > 2:
-                    tempName = tempNED[1].strip().strip("b").strip("'")
-                    if len(tempNED) > 20:
-                        seps = [float(tempNED[9].strip()), float(tempNED[25].strip())]
-                        if np.argmin(seps):
-                            tempNED = tempNED[16:]
-                    tempType =  tempNED[4].strip().strip("b").strip("''")
-                    tempVel = tempNED[5].strip()
-                    tempRed = tempNED[6].strip()
-                    tempRedFlag = tempNED[7].strip().replace("'", "")
-                    tempMag = tempNED[8].strip().strip("b").strip("''").strip(">").strip("<")
-                    if tempName:
-                        df.loc[index, 'NED_name'] = tempName
-                    if tempType:
-                        df.loc[index, 'NED_type'] = tempType
-                    if tempVel:
-                        df.loc[index, 'NED_vel'] = float(tempVel)
-                    if tempRed:
-                        df.loc[index, 'NED_redshift'] = float(tempRed)
-                    if tempMag:
-                        tempMag = re.findall(r"[-+]?\d*\.\d+|\d+", tempMag)[0]
-                        df.loc[index, 'NED_mag'] = float(tempMag)
-                    if tempRedFlag:
-                        df.loc[index, 'NED_redshift_flag'] = str(tempRedFlag)
+                result_df = result_gal.copy()
+            #get closest object
+            result_df = result_df[result_df['Separation'] == np.min(result_df['Separation'])]
+
+            #remove supernovae, etc
+            result_df = result_df[result_df['Type'] != b'SN']
+
+            # Note - sometimes the colon appears in names when a sub-structure of a galaxy. Get rid of it below!
+            df.loc[index, 'NED_name'] = result_df['Object Name'].values[0].split(":")[0]
+            df.loc[index, 'NED_type'] = result_df['Type'].values[0]
+            df.loc[index, 'NED_vel'] = result_df['Velocity'].values[0]
+            df.loc[index, 'NED_redshift'] = result_df['Redshift'].values[0]
+            df.loc[index, 'NED_mag'] = result_df['Redshift Flag'].values[0]
 
         # if the method fails for many in a row, it's likely that too many queries have been made.
         if missingCounter > 5000:
             print("Locked out of NED, will have to try again later...")
             return df
     return df
```

### Comparing `astro_ghost-0.2.5/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-0.2.6/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-0.2.6/astro_ghost/SimbadQueryFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib
 from astropy import units as u
 from astropy.coordinates import SkyCoord
-from astroquery.ned import Ned
+from astroquery.ipac.ned import Ned
 from astroquery.simbad import Simbad
 import warnings
 warnings.filterwarnings("ignore", category=UserWarning)
 import re
 import os
 import pandas as pd
 import numpy as np
```

### Comparing `astro_ghost-0.2.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-0.2.6/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-0.2.6/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/conftest.py` & `astro_ghost-0.2.6/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-0.2.6/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/gradientAscent.py` & `astro_ghost-0.2.6/astro_ghost/gradientAscent.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from astropy import units as u
 from astropy.io import fits, ascii
 from astropy.utils.exceptions import AstropyUserWarning,AstropyWarning
 from astropy.wcs import WCS
 from astropy.utils.data import get_pkg_data_filename
 from matplotlib import pyplot as plt
 from matplotlib import colors
-from photutils import Background2D
 from astropy.stats import sigma_clipped_stats, SigmaClip
-from photutils import CircularAperture, DAOStarFinder, MedianBackground, MeanBackground
+from photutils.detection import DAOStarFinder
+from photutils.background import MeanBackground, MedianBackground, Background2D
+from photutils.aperture import CircularAperture
 from joblib import dump, load
 import gc
 import warnings
 
 def updateStep(px, gradx, grady, step, point, size):
     """ Determine direction of movement by image gradients.
     :param px: The maximum size of the image, in pixels.
```

### Comparing `astro_ghost-0.2.5/astro_ghost/hostMatching.py` & `astro_ghost-0.2.6/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/photoz_helper.py` & `astro_ghost-0.2.6/astro_ghost/photoz_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from astropy.table import Table
-import pkg_resources
-
+#import pkg_resources
 import sys
 import re
 import numpy as np
 import pylab
 import json
 import requests
 from astropy.io import fits
@@ -354,15 +353,14 @@
 
         OUTPUT = tf.keras.layers.Dense(360,activation=tf.keras.activations.softmax)(DENSE4)
 
         model = tf.keras.Model(INPUT,OUTPUT)
 
         return model
     mymodel = model()
-    #stream = pkg_resources.resource_stream(__name__, model_path)
     mymodel.load_weights(model_path)
 
     NB_BINS = 360
     ZMIN = 0.0
     ZMAX = 1.0
     BIN_SIZE = (ZMAX - ZMIN) / NB_BINS
     range_z = np.linspace(ZMIN, ZMAX, NB_BINS + 1)[:NB_BINS]
```

### Comparing `astro_ghost-0.2.5/astro_ghost/sourceCleaning.py` & `astro_ghost-0.2.6/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/astro_ghost/starSeparation.py` & `astro_ghost-0.2.6/astro_ghost/starSeparation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sklearn import svm
 import seaborn as sns
 import matplotlib.pyplot as plt
 from astro_ghost.stellarLocus import *
 import pickle
-import pkg_resources
+import importlib_resources
 
 def separateStars_STRM(df, model_path='.', plot=False, verbose=False, starcut='gentle'):
     """Star-galaxy separation, using a random forest trained on the PS1-STRM-classified star
        and galaxy labels given in Beck et al., 2021.
 
     :param df: Dataframe of PS1 sources.
     :type df: Pandas DataFrame
@@ -30,15 +30,17 @@
     # remove all sources with bad values for any required PS1 properties
     df_dropped = df.dropna(subset=['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag'])
     only_na = df[~df.index.isin(df_dropped.index)]
     unsure = df_dropped.reset_index(drop=True)
 
     # load random forest model
     modelName = "Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav"
-    stream = pkg_resources.resource_stream(__name__, modelName)
+    #stream = pkg_resources.resource_stream(__name__, modelName)
+    #use of pkg_resources is discouraged
+    stream = importlib_resources.files(__name__).joinpath(modelName)
     if verbose:
         print("Loading model %s."%modelName)
     model = pickle.load(stream)
 
     # plot the distribution of objects before classifying
     if plot:
         sns.set_style("dark")
@@ -54,22 +56,21 @@
     if len(unsure) <1:
         if verbose:
             print("No sources in field with feature values, skipping star/galaxy separation...")
         return df, unsure
     test_X = np.asarray(unsure[['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag']])
 
     # define probability threshold for classification
-    if starcut is 'normal':
-        test_y = model.predict(test_X)
-    elif starcut is 'aggressive':
-        test_y = model.predict_proba(test_X)[:,1] > 0.3
-    elif starcut is 'gentle':
-        test_y = model.predict_proba(test_X)[:,1] > 0.8
-    else:
+    cutdict = {'normal':0.5, 'aggressive':0.3, 'gentle':0.8}
+
+    try: 
+        test_y = model.predict_proba(test_X)[:,1] > cutdict[starcut]
+    except:
         print("Error! I didn't understand your starcut option.")
+
     unsure['class'] = test_y
     test_stars = unsure[unsure['class'] == 1]
     test_gals = unsure[unsure['class'] == 0]
 
     # plot the distribution of classified stars and galaxies.
     if plot:
         c_gals = '#087e8b'
@@ -127,18 +128,20 @@
     :rtype: Pandas DataFrame
     :return: A dataframe of sources classified as stars.
     :rtype: Pandas DataFrame
     """
 
     df_dropped = df[df['SkyMapper_StarClass']>0]
     only_na = df[~df.index.isin(df_dropped.index)]
-    if starcut is 'normal':
-        df_stars = df_dropped[df_dropped['SkyMapper_StarClass']>=0.5]
-    elif starcut is 'aggressive':
-        df_stars = df_dropped[df_dropped['SkyMapper_StarClass']>=0.3]
-    elif starcut is 'gentle':
-        df_stars = df_dropped[df_dropped['SkyMapper_StarClass']>=0.8]
+
+    # define probability threshold for classification
+    cutdict = {'normal':0.5, 'aggressive':0.3, 'gentle':0.8}
+    try:
+        df_stars = df_dropped[df_dropped['SkyMapper_StarClass']> cutdict[starcut]] 
+    except:
+        print("Error! I didn't understand your starcut option.")
+
     df_class_gals = df_dropped[~df_dropped.index.isin(df_stars.index)]
     df_stars.reset_index(inplace=True, drop=True)
     df_class_gals.reset_index(inplace=True, drop=True)
     df_gals = pd.concat([df_class_gals, only_na], ignore_index=True).drop_duplicates()
     return df_gals, df_stars
```

### Comparing `astro_ghost-0.2.5/astro_ghost/stellarLocus.py` & `astro_ghost-0.2.6/astro_ghost/stellarLocus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,31 @@
 import seaborn as sns
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import LogNorm
 from astropy.table import Table
 import scipy.interpolate as scinterp
-import pkg_resources
-
-def convert_to_SDSS(conversions, g_iPS1, band, mPS1):
-    """Convert PS1 to SDSS photometry. Recalibration done via the coefficients in
-       Hypercalibration: A Pan-starrs1-Based recalibration of the sloan digital sky survey
-       photometry (Finkbeiner et al., 2016). Publication can be found at
-       https://iopscience.iop.org/article/10.3847/0004-637X/822/2/66.
-
-    :param conversions: Coefficients from Finkbeiner et al., 2016.
-    :type conversions: Pandas DataFrame
-    :param g_iPS1: Apparent g - i color of the source in PS1.
-    :type g_iPS1: float
-    :param band: Band in which to calculate the conversion.
-    :type band: str
-    :param mPS1: AB apparent magnitude of the source in PS1.
-    :type mPS1: float
-
-    Returns
-    -------
-    :return: Estimated AB apparent magnitude of the source in SDSS.
-    :rtype: float
-
-    """
-    a0 = conversions.loc[conversions['Band'] == band, 'a_0'].values[0]
-    a1 = conversions.loc[conversions['Band'] == band, 'a_1'].values[0]
-    a2 = conversions.loc[conversions['Band'] == band, 'a_2'].values[0]
-    a3 = conversions.loc[conversions['Band'] == band, 'a_3'].values[0]
-    mPS1_mSDSS = a0 + a1*g_iPS1 + a2*g_iPS1**2 + a3*g_iPS1**3
-    mSDSS = mPS1 - (mPS1_mSDSS)
-    return mSDSS
+import importlib_resources
 
 def calc_7DCD(df):
     """Calculates the color distance (7DCD) of objects in df from the
        stellar locus from Tonry et al., 2012.
 
     :param df: Dataframe of PS1 objects.
     :type df: Pandas DataFrame
 
     :return: The same dataframe as input, with new column 7DCD.
     :rtype: Pandas DataFrame
     """
     df.replace(999.00, np.nan)
     df.replace(-999.00, np.nan)
 
-    #read the stellar locus table from SDSS
-    stream = pkg_resources.resource_stream(__name__, 'tonry_ps1_locus.txt')
+    #read the stellar locus table from PS1
+    stream = importlib_resources.files(__name__).joinpath('tonry_ps1_locus.txt')
     skt = Table.read(stream, format='ascii')
 
     gr = scinterp.interp1d(skt['ri'], skt['gr'], kind='cubic', fill_value='extrapolate')
     iz = scinterp.interp1d(skt['ri'], skt['iz'], kind='cubic', fill_value='extrapolate')
     zy = scinterp.interp1d(skt['ri'], skt['zy'], kind='cubic', fill_value='extrapolate')
     ri = np.arange(-0.4, 2.01, 0.001)
 
@@ -113,15 +84,16 @@
         cbar.set_label("4D Color Distance")
         if save:
             plt.savefig("PS1_%s_StellarLocus_%s_Colored.pdf"%(type, timestamp))
         else:
             plt.show()
     else:
         #read the stellar locus table from PS1
-        skt = Table.read('./tonry_ps1_locus.txt', format='ascii')
+        stream = importlib_resources.files(__name__).joinpath('tonry_ps1_locus.txt')
+        skt = Table.read(stream, format='ascii')
 
         gr = scinterp.interp1d(skt['ri'], skt['gr'], kind='cubic', fill_value='extrapolate')
         iz = scinterp.interp1d(skt['ri'], skt['iz'], kind='cubic', fill_value='extrapolate')
         zy = scinterp.interp1d(skt['ri'], skt['zy'], kind='cubic', fill_value='extrapolate')
         ri = np.arange(-0.4, 2.01, 0.001)
 
         gr_new = gr(ri)
```

### Comparing `astro_ghost-0.2.5/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-0.2.6/astro_ghost.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +23,18 @@
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
 .. image:: https://img.shields.io/pypi/dm/astro-ghost
    :target: https://pypi.org/project/astro-ghost/
-   :alt: PyPI - Downloads
+   :alt: PyPI
 
-.. image:: https://img.shields.io/readthedocs/astro-ghost
-   :target: https://astro-ghost.readthedocs.io/en/latest/
+.. image:: https://img.shields.io/readthedocs/uiucsnastro-ghost
+   :target: https://uiucsnastro-ghost.readthedocs.io/en/latest/
    :alt: Read the Docs
 
 "At the last dim horizon, we search among ghostly errors of observations for
 landmarks that are scarcely more substantial. The search will continue. The
 urge is older than history. It is not satisfied and it will not be oppressed."
 --Edwin Hubble
 
@@ -43,15 +43,15 @@
 classes in Gagliano et al. (2020). Installation instructions for the analysis
 tools are below.
 
 Installation
 ------------
 
 For details on installing and using GHOST, see the
-`documentation <https://astro-ghost.readthedocs.io/en/latest/>`_.
+`documentation <https://uiucsnastro-ghost.readthedocs.io/en/latest/>`_.
 
 
 Citation
 ------------
 If you use this code, please cite the associated paper with the bibtex entry below::
 
    @ARTICLE{2021ApJ...908..170G,
@@ -97,19 +97,12 @@
 We assure you - the little voice in your head is wrong. If you can write code at
 all, you can contribute code to open source. Contributing to open source
 projects is a fantastic way to advance one's coding skills. Writing perfect code
 isn't the measure of a good developer (that would disqualify all of us!); it's
 trying to create something, making mistakes, and learning from those
 mistakes. That's how we all improve, and we are happy to help others learn.
 
-Being an open source contributor doesn't just mean writing code, either. You can
-help out by writing documentation, tests, or even giving feedback about the
-project (and yes - that includes giving feedback about the contribution
-process). Some of these contributions may be the most valuable to the project as
-a whole, because you're coming to the project with fresh eyes, so you can see
-the errors and assumptions that seasoned contributors have glossed over.
-
 Note: This disclaimer was originally written by
 `Adrienne Lowe <https://github.com/adriennefriend>`_ for a
 `PyCon talk <https://www.youtube.com/watch?v=6Uj746j9Heo>`_, and was adapted by
 astro_ghost based on its use in the README file for the
 `MetPy project <https://github.com/Unidata/MetPy>`_.
```

### Comparing `astro_ghost-0.2.5/docs/Makefile` & `astro_ghost-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/docs/conf.py` & `astro_ghost-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/docs/make.bat` & `astro_ghost-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/docs/source/index.rst` & `astro_ghost-0.2.6/docs/source/basicusage.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,12 @@
-***********
-Astro GHOST
-***********
-
-Galaxies HOsting Supernovae and other Transients (GHOST): A database of
-supernovae and the photometric and spectroscopic properties of their host
-galaxies.
-
-Installation
-============
-
-1. Create a clean conda environment.
-
-2. Run the following code:
-
-.. code-block:: bash
-
-   pip install astro_ghost
-
-Or, download this repo and run
-
-.. code-block:: bash
-
-   python setup.py install
-
-from the main directory.
-
 Example Usage
 =============
 
+The database of supernova-host galaxy matches can be found at http://ghost.ncsa.illinois.edu/static/GHOST.csv, and retrieved using the getGHOST() function. This database will need to be created before running the association pipeline.
+
 .. code-block:: python
 
     import os
     import sys
     from astro_ghost.PS1QueryFunctions import getAllPostageStamps
     from astro_ghost.TNSQueryFunctions import getTNSSpectra
     from astro_ghost.NEDQueryFunctions import getNEDSpectra
@@ -79,14 +54,7 @@
     fn_SN = 'transients_%s.csv' % dateStr
     transients = pd.read_csv("./transients_%s/tables/%s"%(dateStr,fn_SN))
 
     #get postage stamps and spectra
     getAllPostageStamps(hosts, 120, psPath, verbose) #get postage stamps of hosts
     getNEDSpectra(hosts, hSpecPath, verbose) #get spectra of hosts
     getTNSSpectra(transients, tSpecPath, verbose) #get spectra of transients (if on TNS)
-
-The database of supernova-host galaxy matches can be found at http://ghost.ncsa.illinois.edu/static/GHOST.csv, and retrieved using the getGHOST() function. This database will need to be created before running the association pipeline. Helper functions can be found in ghostHelperFunctions.py for querying and getting quick stats about SNe within the database. The software to associate these supernovae with host galaxies is also provided, and tutorial.py provides examples for using this code.
-
-
-GHOST Viewer
-============
-In addition to these software tools, a website has been constructed for rapid viewing of many objects in this database. It is located at ghost.ncsa.illinois.edu.  Json files containing supernova and host information can be found at http://ghost.ncsa.illinois.edu/static/json.tar.gz. host spectra, SN spectra, and SN photometry are found at http://ghost.ncsa.illinois.edu/static/hostSpectra.zip, http://ghost.ncsa.illinois.edu/static/SNspectra.zip, and http://ghost.ncsa.illinois.edu/static/SNphotometry.zip.
```

### Comparing `astro_ghost-0.2.5/licenses/LICENSE.rst` & `astro_ghost-0.2.6/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/setup.cfg` & `astro_ghost-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.5/setup.py` & `astro_ghost-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "0.2.5"
+version = "0.2.6"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
@@ -35,15 +35,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
     package_data={
     'astro_ghost': ['Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav','tonry_ps1_locus.txt'],
     },
-    install_requires=['pandas', 'scikit-learn', 'numpy', 'seaborn', 'matplotlib', 'joypy','astropy', 'photutils', 'scipy', 'datetime', 'requests','imblearn','rfpimp','Pillow', 'pyvo', 'astroquery', 'mastcasjobs', 'opencv-python','tensorflow','sfdmap'],
+    install_requires=['pandas', 'scikit-learn', 'numpy', 'seaborn', 'matplotlib', 'joypy','astropy', 'photutils', 'scipy', 'datetime', 'requests<2.29.0','imblearn','rfpimp','Pillow', 'pyvo', 'astroquery', 'mastcasjobs', 'opencv-python','tensorflow','sfdmap','importlib_resources'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 #    use_scm_version={'write_to': os.path.join('astro_ghost', 'version.py'),
```

### Comparing `astro_ghost-0.2.5/tox.ini` & `astro_ghost-0.2.6/tox.ini`

 * *Files identical despite different names*


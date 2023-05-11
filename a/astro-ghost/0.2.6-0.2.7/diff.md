# Comparing `tmp/astro_ghost-0.2.6.tar.gz` & `tmp/astro_ghost-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-0.2.6.tar", last modified: Thu May 11 04:21:21 2023, max compression
+gzip compressed data, was "astro_ghost-0.2.7.tar", last modified: Thu May 11 05:43:33 2023, max compression
```

## Comparing `astro_ghost-0.2.6.tar` & `astro_ghost-0.2.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.113041 astro_ghost-0.2.6/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:20.990882 astro_ghost-0.2.6/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:20.997858 astro_ghost-0.2.6/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-0.2.6/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 04:21:21.113361 astro_ghost-0.2.6/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-0.2.6/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.087980 astro_ghost-0.2.6/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    15169 2023-05-09 21:30:32.000000 astro_ghost-0.2.6/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-0.2.6/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    39061 2023-05-10 05:59:47.000000 astro_ghost-0.2.6/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-0.2.6/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-0.2.6/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1527 2023-05-09 19:21:33.000000 astro_ghost-0.2.6/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-0.2.6/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-11 04:20:13.000000 astro_ghost-0.2.6/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-0.2.6/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37898 2023-05-09 22:25:05.000000 astro_ghost-0.2.6/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32745 2023-05-10 22:07:36.000000 astro_ghost-0.2.6/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-0.2.6/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    15960 2023-05-10 22:18:36.000000 astro_ghost-0.2.6/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    10333 2023-05-09 19:38:06.000000 astro_ghost-0.2.6/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     6616 2023-05-10 22:27:43.000000 astro_ghost-0.2.6/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4604 2023-05-11 04:18:51.000000 astro_ghost-0.2.6/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-0.2.6/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.092649 astro_ghost-0.2.6/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1301 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-11 04:21:20.000000 astro_ghost-0.2.6/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.096909 astro_ghost-0.2.6/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-0.2.6/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-0.2.6/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.105385 astro_ghost-0.2.6/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-0.2.6/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-0.2.6/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-0.2.6/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-0.2.6/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-0.2.6/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-0.2.6/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-0.2.6/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-0.2.6/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.109190 astro_ghost-0.2.6/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-0.2.6/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1603 2023-05-11 04:21:21.115497 astro_ghost-0.2.6/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-11 04:19:54.000000 astro_ghost-0.2.6/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 04:21:21.112222 astro_ghost-0.2.6/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-0.2.6/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1655 2023-05-11 04:18:55.000000 astro_ghost-0.2.6/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2421 2023-05-10 23:12:38.000000 astro_ghost-0.2.6/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-10 20:57:05.000000 astro_ghost-0.2.6/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.928088 astro_ghost-0.2.7/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.862445 astro_ghost-0.2.7/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.869078 astro_ghost-0.2.7/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-0.2.7/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 05:43:33.928364 astro_ghost-0.2.7/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-0.2.7/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.903931 astro_ghost-0.2.7/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    15169 2023-05-11 04:59:00.000000 astro_ghost-0.2.7/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-0.2.7/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38356 2023-05-11 04:54:25.000000 astro_ghost-0.2.7/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-0.2.7/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-0.2.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-0.2.7/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-0.2.7/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-11 05:43:06.000000 astro_ghost-0.2.7/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-0.2.7/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37898 2023-05-11 05:12:32.000000 astro_ghost-0.2.7/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32745 2023-05-10 22:07:36.000000 astro_ghost-0.2.7/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-0.2.7/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    15960 2023-05-10 22:18:36.000000 astro_ghost-0.2.7/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    10333 2023-05-09 19:38:06.000000 astro_ghost-0.2.7/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     6519 2023-05-11 05:26:18.000000 astro_ghost-0.2.7/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-0.2.7/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-0.2.7/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.906971 astro_ghost-0.2.7/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1301 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.911363 astro_ghost-0.2.7/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-0.2.7/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-0.2.7/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.921653 astro_ghost-0.2.7/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-0.2.7/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-0.2.7/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-0.2.7/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-0.2.7/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-0.2.7/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-0.2.7/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-0.2.7/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-0.2.7/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.924429 astro_ghost-0.2.7/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1603 2023-05-11 05:43:33.929535 astro_ghost-0.2.7/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-11 05:42:57.000000 astro_ghost-0.2.7/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.927621 astro_ghost-0.2.7/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-0.2.7/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      560 2023-05-11 05:42:33.000000 astro_ghost-0.2.7/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4207 2023-05-11 05:35:01.000000 astro_ghost-0.2.7/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-10 20:57:05.000000 astro_ghost-0.2.7/tox.ini
```

### Comparing `astro_ghost-0.2.6/.github/workflows/tests.yml` & `astro_ghost-0.2.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/.gitignore` & `astro_ghost-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/PKG-INFO` & `astro_ghost-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-0.2.6/README.rst` & `astro_ghost-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/DLR.py` & `astro_ghost-0.2.7/astro_ghost/DLR.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-0.2.7/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-0.2.7/astro_ghost/PS1QueryFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -482,36 +482,14 @@
     data = kw.copy()
     data['ra'] = ra
     data['dec'] = dec
     data['radius'] = radius
     return ps1search(table=table,release=release,format=format,columns=columns,
                     baseurl=baseurl, verbose=verbose, **data)
 
-def create_df(tns_loc):
-    """Combine all supernova data into a single dataframe.
-
-    :param tns_loc: Filepath where files containing TNS data is stored.
-    :type tns_loc: str
-    :param df: Dataframe of all TNS metadata.
-    :type df: Pandas DataFrame
-    """
-
-    files = [f for f in listdir(tns_loc) if isfile(join(tns_loc, f))]
-    arr = []
-    for file in files:
-        tempPD = pd.read_csv(tns_loc+file)
-        arr.append(tempPD)
-    df = pd.concat(arr)
-    df = df.loc[df['RA'] != '00:00:00.000']
-    df = df.drop_duplicates()
-    df = df.replace({'Anon.': ''})
-    df = df.replace({'2019-02-13.49': ''})
-    df = df.apply(lambda x: x.str.strip() if x.dtype == "object" else x)
-    return df
-
 def ps1metadata(table="mean", release="dr1", baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs"):
     """Return metadata for the specified catalog and table. Snagged from the
        wonderful API at https://ps1images.stsci.edu/ps1_dr2_api.html.
 
     :param table: Table type. Can be \\'mean\\', \\'stack\\', or \\'detection\\'
     :type table: str
     :param release: The Pan-STARRS data release. Can be \\'dr1\\' or \\'dr2\\'.
```

### Comparing `astro_ghost-0.2.6/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-0.2.7/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-0.2.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-0.2.7/astro_ghost/TNSQueryFunctions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bs4 import BeautifulSoup
 import requests
-from astro_ghost.PS1QueryFunctions import create_df
 import urllib.request
 from astro_ghost.PS1QueryFunctions import find_all
 from astro_ghost.ghostHelperFunctions import remove_prefix
 
 def getTNSSpectra(transients, path, verbose=False):
     """Scrapes the Transient Name Server for all public spectra of a transient.
```

### Comparing `astro_ghost-0.2.6/astro_ghost/conftest.py` & `astro_ghost-0.2.7/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-0.2.7/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/gradientAscent.py` & `astro_ghost-0.2.7/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/hostMatching.py` & `astro_ghost-0.2.7/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/photoz_helper.py` & `astro_ghost-0.2.7/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/sourceCleaning.py` & `astro_ghost-0.2.7/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/astro_ghost/starSeparation.py` & `astro_ghost-0.2.7/astro_ghost/starSeparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
     # remove all sources with bad values for any required PS1 properties
     df_dropped = df.dropna(subset=['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag'])
     only_na = df[~df.index.isin(df_dropped.index)]
     unsure = df_dropped.reset_index(drop=True)
 
     # load random forest model
     modelName = "Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav"
-    #stream = pkg_resources.resource_stream(__name__, modelName)
-    #use of pkg_resources is discouraged
-    stream = importlib_resources.files(__name__).joinpath(modelName)
+    stream = importlib_resources.files(__name__).joinpath(modelName).open("rb")
     if verbose:
         print("Loading model %s."%modelName)
     model = pickle.load(stream)
 
     # plot the distribution of objects before classifying
     if plot:
         sns.set_style("dark")
@@ -58,15 +56,15 @@
             print("No sources in field with feature values, skipping star/galaxy separation...")
         return df, unsure
     test_X = np.asarray(unsure[['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag']])
 
     # define probability threshold for classification
     cutdict = {'normal':0.5, 'aggressive':0.3, 'gentle':0.8}
 
-    try: 
+    try:
         test_y = model.predict_proba(test_X)[:,1] > cutdict[starcut]
     except:
         print("Error! I didn't understand your starcut option.")
 
     unsure['class'] = test_y
     test_stars = unsure[unsure['class'] == 1]
     test_gals = unsure[unsure['class'] == 0]
@@ -132,15 +130,15 @@
 
     df_dropped = df[df['SkyMapper_StarClass']>0]
     only_na = df[~df.index.isin(df_dropped.index)]
 
     # define probability threshold for classification
     cutdict = {'normal':0.5, 'aggressive':0.3, 'gentle':0.8}
     try:
-        df_stars = df_dropped[df_dropped['SkyMapper_StarClass']> cutdict[starcut]] 
+        df_stars = df_dropped[df_dropped['SkyMapper_StarClass']> cutdict[starcut]]
     except:
         print("Error! I didn't understand your starcut option.")
 
     df_class_gals = df_dropped[~df_dropped.index.isin(df_stars.index)]
     df_stars.reset_index(inplace=True, drop=True)
     df_class_gals.reset_index(inplace=True, drop=True)
     df_gals = pd.concat([df_class_gals, only_na], ignore_index=True).drop_duplicates()
```

### Comparing `astro_ghost-0.2.6/astro_ghost/stellarLocus.py` & `astro_ghost-0.2.7/astro_ghost/stellarLocus.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,13 +102,13 @@
             c = '#087e8b'
         elif type == "Stars":
             c = '#ffbf00'
         else:
             c = 'violet'
         g = sns.JointGrid(x="i-z", y="g-r", data=df, height=9, ratio=5, xlim=(-0.4, 0.8), ylim=(-0.2, 2.0), space=0)
         g = g.plot_joint(sns.kdeplot, color=c,gridsize=200)
-        plt.plot(iz_new, gr_new, '--', c='#8c837c', lw=2)
+        g.ax_joint.plot(iz_new, gr_new, '--', c='#8c837c', lw=2)
         plt.xlabel(r"$i-z$",fontsize=18)
         plt.ylabel(r"$g-r$",fontsize=18)
         g = g.plot_marginals(sns.kdeplot, color=c, shade=True)
         if save:
             g.savefig("PS1_%s_StellarLocus_%s.pdf"%(type, timestamp))
```

### Comparing `astro_ghost-0.2.6/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-0.2.7/astro_ghost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-0.2.6/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-0.2.7/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/Makefile` & `astro_ghost-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/conf.py` & `astro_ghost-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/index.rst` & `astro_ghost-0.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/make.bat` & `astro_ghost-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/source/associationmodules.rst` & `astro_ghost-0.2.7/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/source/basicusage.rst` & `astro_ghost-0.2.7/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/source/catalogmodules.rst` & `astro_ghost-0.2.7/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/source/installation.rst` & `astro_ghost-0.2.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/docs/source/preprocessingmodules.rst` & `astro_ghost-0.2.7/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/licenses/LICENSE.rst` & `astro_ghost-0.2.7/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/setup.cfg` & `astro_ghost-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.6/setup.py` & `astro_ghost-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "0.2.6"
+version = "0.2.7"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-0.2.6/tox.ini` & `astro_ghost-0.2.7/tox.ini`

 * *Files identical despite different names*


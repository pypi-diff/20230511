# Comparing `tmp/Orange3-ImageAnalytics-0.8.0.tar.gz` & `tmp/Orange3-ImageAnalytics-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-ImageAnalytics-0.8.0.tar", last modified: Mon Feb 28 08:18:21 2022, max compression
+gzip compressed data, was "Orange3-ImageAnalytics-0.9.0.tar", last modified: Fri Oct 14 11:54:51 2022, max compression
```

## Comparing `Orange3-ImageAnalytics-0.8.0.tar` & `Orange3-ImageAnalytics-0.9.0.tar`

### file list

```diff
@@ -1,228 +1,218 @@
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.763548 Orange3-ImageAnalytics-0.8.0/
--rw-r--r--   0 primoz     (501) staff       (20)      324 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/.coveragerc
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.490481 Orange3-ImageAnalytics-0.8.0/.github/
--rw-r--r--   0 primoz     (501) staff       (20)      646 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/.github/FUNDING.yml
--rw-r--r--   0 primoz     (501) staff       (20)      442 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 primoz     (501) staff       (20)      216 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.491228 Orange3-ImageAnalytics-0.8.0/.github/workflows/
--rw-r--r--   0 primoz     (501) staff       (20)     2550 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/.github/workflows/test.yml
--rw-r--r--   0 primoz     (501) staff       (20)      202 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/.gitignore
--rw-r--r--   0 primoz     (501) staff       (20)    35147 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/LICENSE.txt
--rw-r--r--   0 primoz     (501) staff       (20)      244 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/MANIFEST.in
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.496179 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/
--rw-r--r--   0 primoz     (501) staff       (20)     1340 2022-02-28 08:18:21.000000 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)     8715 2022-02-28 08:18:21.000000 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/SOURCES.txt
--rw-r--r--   0 primoz     (501) staff       (20)        1 2022-02-28 08:18:21.000000 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/dependency_links.txt
--rw-r--r--   0 primoz     (501) staff       (20)      233 2022-02-28 08:18:21.000000 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/entry_points.txt
--rw-r--r--   0 primoz     (501) staff       (20)       14 2022-02-28 08:18:21.000000 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/namespace_packages.txt
--rw-r--r--   0 primoz     (501) staff       (20)      172 2022-02-28 08:18:21.000000 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/requires.txt
--rw-r--r--   0 primoz     (501) staff       (20)       14 2022-02-28 08:18:21.000000 Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/top_level.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1340 2022-02-28 08:18:21.763096 Orange3-ImageAnalytics-0.8.0/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)     1282 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/README.md
--rw-r--r--   0 primoz     (501) staff       (20)      628 2021-09-22 12:10:30.000000 Orange3-ImageAnalytics-0.8.0/README.pypi
--rw-r--r--   0 primoz     (501) staff       (20)      178 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/codecov.yml
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.503319 Orange3-ImageAnalytics-0.8.0/doc/
--rw-r--r--   0 primoz     (501) staff       (20)     6806 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/Makefile
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.477796 Orange3-ImageAnalytics-0.8.0/doc/_build/
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.508897 Orange3-ImageAnalytics-0.8.0/doc/_build/html/
--rw-r--r--   0 primoz     (501) staff       (20)      230 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/.buildinfo
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.608609 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/
--rw-r--r--   0 primoz     (501) staff       (20)   227359 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageEmbedding-Example1.png
--rw-r--r--   0 primoz     (501) staff       (20)    79682 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageEmbedding-Example2.png
--rw-r--r--   0 primoz     (501) staff       (20)     8441 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageEmbedding-stamped.png
--rw-r--r--   0 primoz     (501) staff       (20)    74310 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageGrid-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    51873 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageGrid-stamped.png
--rw-r--r--   0 primoz     (501) staff       (20)    89158 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageViewer-stamped.png
--rw-r--r--   0 primoz     (501) staff       (20)   160938 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImportImages-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    10513 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImportImages-class.png
--rw-r--r--   0 primoz     (501) staff       (20)    10025 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImportImages-stamped.png
--rw-r--r--   0 primoz     (501) staff       (20)    73586 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/SaveImages-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    10268 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/SaveImages.png
--rw-r--r--   0 primoz     (501) staff       (20)    51280 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/header-example.png
--rw-r--r--   0 primoz     (501) staff       (20)   103417 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/image-viewer-example1.png
--rw-r--r--   0 primoz     (501) staff       (20)   108042 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/image-viewer-example2.png
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.612759 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_modules/
--rw-r--r--   0 primoz     (501) staff       (20)     4094 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_modules/index.html
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.478365 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_modules/orangecontrib/
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.615296 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_modules/orangecontrib/imageanalytics/
--rw-r--r--   0 primoz     (501) staff       (20)    46476 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_modules/orangecontrib/imageanalytics/image_embedder.html
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.617135 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/
--rw-r--r--   0 primoz     (501) staff       (20)      439 2022-02-03 15:17:49.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.617949 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/scripting/
--rw-r--r--   0 primoz     (501) staff       (20)      133 2022-02-03 15:17:49.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/scripting/image_embedder.rst.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.622402 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     4900 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/imageembedding.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1738 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/imagegrid.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1301 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/imageviewer.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1705 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/importimages.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1787 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/saveimages.md.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.638742 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/
--rw-r--r--   0 primoz     (501) staff       (20)    14667 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/basic.css
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.640988 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/
--rw-r--r--   0 primoz     (501) staff       (20)     3275 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.681836 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/
--rw-r--r--   0 primoz     (501) staff       (20)    87624 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 primoz     (501) staff       (20)    67312 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 primoz     (501) staff       (20)    86288 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 primoz     (501) staff       (20)    66444 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   165742 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 primoz     (501) staff       (20)   444379 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 primoz     (501) staff       (20)   165548 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 primoz     (501) staff       (20)    98024 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 primoz     (501) staff       (20)    77160 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   323344 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 primoz     (501) staff       (20)   193308 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   309728 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 primoz     (501) staff       (20)   184912 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   328412 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 primoz     (501) staff       (20)   195704 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   309192 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 primoz     (501) staff       (20)   182708 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   129674 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/theme.css
--rw-r--r--   0 primoz     (501) staff       (20)      537 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/custom.css
--rw-r--r--   0 primoz     (501) staff       (20)     9630 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/doctools.js
--rw-r--r--   0 primoz     (501) staff       (20)      350 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/documentation_options.js
--rw-r--r--   0 primoz     (501) staff       (20)      286 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/file.png
--rw-r--r--   0 primoz     (501) staff       (20)   287630 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 primoz     (501) staff       (20)    89476 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/jquery.js
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.687208 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/
--rw-r--r--   0 primoz     (501) staff       (20)      934 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/badge_only.js
--rw-r--r--   0 primoz     (501) staff       (20)     4370 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 primoz     (501) staff       (20)     2734 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 primoz     (501) staff       (20)     5023 2022-01-10 14:47:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/theme.js
--rw-r--r--   0 primoz     (501) staff       (20)    10854 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/language_data.js
--rw-r--r--   0 primoz     (501) staff       (20)       90 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/minus.png
--rw-r--r--   0 primoz     (501) staff       (20)       90 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/plus.png
--rw-r--r--   0 primoz     (501) staff       (20)     4846 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/pygments.css
--rw-r--r--   0 primoz     (501) staff       (20)    16793 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/searchtools.js
--rw-r--r--   0 primoz     (501) staff       (20)    68420 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 primoz     (501) staff       (20)    19530 2022-01-10 14:47:29.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/underscore.js
--rw-r--r--   0 primoz     (501) staff       (20)     7220 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/genindex.html
--rw-r--r--   0 primoz     (501) staff       (20)     6243 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/index.html
--rw-r--r--   0 primoz     (501) staff       (20)      517 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/objects.inv
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.687714 Orange3-ImageAnalytics-0.8.0/doc/_build/html/scripting/
--rw-r--r--   0 primoz     (501) staff       (20)    19877 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/scripting/image_embedder.html
--rw-r--r--   0 primoz     (501) staff       (20)     4277 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/search.html
--rw-r--r--   0 primoz     (501) staff       (20)     6034 2022-02-28 08:16:32.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/searchindex.js
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.690936 Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)    11705 2022-02-14 14:20:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/imageembedding.html
--rw-r--r--   0 primoz     (501) staff       (20)     7319 2022-02-14 14:20:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/imagegrid.html
--rw-r--r--   0 primoz     (501) staff       (20)     6858 2022-02-14 14:20:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/imageviewer.html
--rw-r--r--   0 primoz     (501) staff       (20)     7310 2022-02-14 14:20:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/importimages.html
--rw-r--r--   0 primoz     (501) staff       (20)     7778 2022-02-14 14:20:30.000000 Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/saveimages.html
--rw-r--r--   0 primoz     (501) staff       (20)     8975 2022-02-03 15:17:49.000000 Orange3-ImageAnalytics-0.8.0/doc/conf.py
--rw-r--r--   0 primoz     (501) staff       (20)      439 2022-02-03 15:17:49.000000 Orange3-ImageAnalytics-0.8.0/doc/index.rst
--rw-r--r--   0 primoz     (501) staff       (20)     6723 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/make.bat
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.691480 Orange3-ImageAnalytics-0.8.0/doc/scripting/
--rw-r--r--   0 primoz     (501) staff       (20)      133 2022-02-03 15:17:49.000000 Orange3-ImageAnalytics-0.8.0/doc/scripting/image_embedder.rst
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.692113 Orange3-ImageAnalytics-0.8.0/doc/static/
--rw-r--r--   0 primoz     (501) staff       (20)      537 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/doc/static/custom.css
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.696628 Orange3-ImageAnalytics-0.8.0/doc/widgets/
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.700171 Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/
--rwxr-xr-x   0 primoz     (501) staff       (20)     5119 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/image-embedding.png
--rwxr-xr-x   0 primoz     (501) staff       (20)     5099 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/image-grid.png
--rwxr-xr-x   0 primoz     (501) staff       (20)     4903 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/image-viewer.png
--rwxr-xr-x   0 primoz     (501) staff       (20)     5614 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/import-images.png
--rwxr-xr-x   0 primoz     (501) staff       (20)     4900 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/imageembedding.md
--rwxr-xr-x   0 primoz     (501) staff       (20)     1738 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/imagegrid.md
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.714661 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/
--rw-r--r--   0 primoz     (501) staff       (20)   227359 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageEmbedding-Example1.png
--rwxr-xr-x   0 primoz     (501) staff       (20)    79682 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageEmbedding-Example2.png
--rwxr-xr-x   0 primoz     (501) staff       (20)     8441 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageEmbedding-stamped.png
--rwxr-xr-x   0 primoz     (501) staff       (20)    74310 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageGrid-Example.png
--rwxr-xr-x   0 primoz     (501) staff       (20)    51873 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageGrid-stamped.png
--rwxr-xr-x   0 primoz     (501) staff       (20)    89158 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageViewer-stamped.png
--rwxr-xr-x   0 primoz     (501) staff       (20)   332303 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageViewer.png
--rwxr-xr-x   0 primoz     (501) staff       (20)   160938 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImportImages-Example.png
--rwxr-xr-x   0 primoz     (501) staff       (20)    10513 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImportImages-class.png
--rwxr-xr-x   0 primoz     (501) staff       (20)    10025 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImportImages-stamped.png
--rw-r--r--   0 primoz     (501) staff       (20)    73586 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/SaveImages-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    10268 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/SaveImages.png
--rwxr-xr-x   0 primoz     (501) staff       (20)    51280 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/header-example.png
--rwxr-xr-x   0 primoz     (501) staff       (20)   103417 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/image-viewer-example1.png
--rwxr-xr-x   0 primoz     (501) staff       (20)   108042 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/images/image-viewer-example2.png
--rwxr-xr-x   0 primoz     (501) staff       (20)     1301 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/imageviewer.md
--rwxr-xr-x   0 primoz     (501) staff       (20)     1705 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/importimages.md
--rwxr-xr-x   0 primoz     (501) staff       (20)     1787 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets/saveimages.md
--rw-r--r--   0 primoz     (501) staff       (20)     1360 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/doc/widgets.json
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.715963 Orange3-ImageAnalytics-0.8.0/orangecontrib/
--rw-r--r--   0 primoz     (501) staff       (20)       80 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.719522 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    11528 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/image_embedder.py
--rw-r--r--   0 primoz     (501) staff       (20)     7313 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/image_grid.py
--rw-r--r--   0 primoz     (501) staff       (20)     7801 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/import_images.py
--rw-r--r--   0 primoz     (501) staff       (20)     2232 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/local_embedder.py
--rw-r--r--   0 primoz     (501) staff       (20)      817 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/server_embedder.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.721431 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2021-09-22 12:10:30.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    10974 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_image_embedder.py
--rw-r--r--   0 primoz     (501) staff       (20)     1102 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_image_grid.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.739916 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/
--rw-r--r--   0 primoz     (501) staff       (20)     6148 2022-02-15 12:52:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/.DS_Store
--rw-r--r--   0 primoz     (501) staff       (20)     5953 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_0.jpg
--rw-r--r--   0 primoz     (501) staff       (20)   786572 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_1.tiff
--rw-r--r--   0 primoz     (501) staff       (20)   124610 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.bmp
--rw-r--r--   0 primoz     (501) staff       (20)    24724 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.gif
--rw-r--r--   0 primoz     (501) staff       (20)     9745 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpeg
--rw-r--r--   0 primoz     (501) staff       (20)     9745 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpg
--rw-r--r--   0 primoz     (501) staff       (20)     4015 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pbm
--rw-r--r--   0 primoz     (501) staff       (20)    31137 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pgm
--rw-r--r--   0 primoz     (501) staff       (20)    16839 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.png
--rw-r--r--   0 primoz     (501) staff       (20)    31137 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pnm
--rw-r--r--   0 primoz     (501) staff       (20)    93381 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.ppm
--rw-r--r--   0 primoz     (501) staff       (20)    31292 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tif
--rw-r--r--   0 primoz     (501) staff       (20)    31292 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tiff
--rw-r--r--   0 primoz     (501) staff       (20)    25136 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xbm
--rw-r--r--   0 primoz     (501) staff       (20)    67078 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xpm
--rw-r--r--   0 primoz     (501) staff       (20)     1539 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_3.svg
--rw-r--r--   0 primoz     (501) staff       (20)     1644 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_import_images.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.741486 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)     3000 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/embedder_utils.py
--rw-r--r--   0 primoz     (501) staff       (20)     2688 2022-02-11 09:25:26.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/image_utils.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.742705 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)     4180 2022-02-28 08:12:00.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/tests/test_embedder_utils.py
--rw-r--r--   0 primoz     (501) staff       (20)     4521 2022-02-11 09:25:26.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/tests/test_image_utils.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.747501 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     1041 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.750280 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/
--rwxr-xr-x   0 primoz     (501) staff       (20)     4830 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/Category-ImageAnalytics.svg
--rwxr-xr-x   0 primoz     (501) staff       (20)     4097 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImageEmbedding.svg
--rw-r--r--   0 primoz     (501) staff       (20)     1553 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImageGrid.svg
--rw-r--r--   0 primoz     (501) staff       (20)     4831 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImageViewer.svg
--rwxr-xr-x   0 primoz     (501) staff       (20)     5083 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImportImages.svg
--rw-r--r--   0 primoz     (501) staff       (20)     1637 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/SaveImages.svg
--rw-r--r--   0 primoz     (501) staff       (20)    10979 2022-02-11 09:25:26.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimageembedding.py
--rw-r--r--   0 primoz     (501) staff       (20)    45697 2022-02-11 09:25:26.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimagegrid.py
--rw-r--r--   0 primoz     (501) staff       (20)    20884 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimageimport.py
--rw-r--r--   0 primoz     (501) staff       (20)    26577 2022-02-11 09:25:26.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimageviewer.py
--rw-r--r--   0 primoz     (501) staff       (20)    12416 2022-02-11 09:25:26.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owsaveimages.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.754986 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2021-09-22 12:10:30.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.758761 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/
--rw-r--r--   0 primoz     (501) staff       (20)    91156 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/afternoon-4175917_640.jpg
--rw-r--r--   0 primoz     (501) staff       (20)    71036 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/atomium-4179270_640.jpg
--rw-r--r--   0 primoz     (501) staff       (20)    75496 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/kittens-4020199_640.jpg
--rw-r--r--   0 primoz     (501) staff       (20)    76767 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/landscape-2130524_640.jpg
--rw-r--r--   0 primoz     (501) staff       (20)     6888 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimageembedding.py
--rw-r--r--   0 primoz     (501) staff       (20)     7007 2022-02-04 10:30:23.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimagegrid.py
--rw-r--r--   0 primoz     (501) staff       (20)     2887 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimageimport.py
--rw-r--r--   0 primoz     (501) staff       (20)     1704 2022-02-04 10:30:23.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimageviewer.py
--rw-r--r--   0 primoz     (501) staff       (20)    12851 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owsaveimages.py
--rw-r--r--   0 primoz     (501) staff       (20)      534 2022-02-11 09:25:26.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/utils.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.760961 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)     4027 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/imagepreview.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-02-28 08:18:21.762489 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)      515 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/tests/test_imagepreview.py
--rw-r--r--   0 primoz     (501) staff       (20)     1361 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/tests/test_thumnbnailview.py
--rw-r--r--   0 primoz     (501) staff       (20)     7998 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/thumbnailview.py
--rw-r--r--   0 primoz     (501) staff       (20)       90 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/pyproject.toml
--rw-r--r--   0 primoz     (501) staff       (20)       10 2021-09-14 08:19:33.000000 Orange3-ImageAnalytics-0.8.0/requirements-opt.txt
--rw-r--r--   0 primoz     (501) staff       (20)      111 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/requirements.txt
--rw-r--r--   0 primoz     (501) staff       (20)       38 2022-02-28 08:18:21.763675 Orange3-ImageAnalytics-0.8.0/setup.cfg
--rwxr-xr-x   0 primoz     (501) staff       (20)     3078 2022-02-28 08:15:20.000000 Orange3-ImageAnalytics-0.8.0/setup.py
--rw-r--r--   0 primoz     (501) staff       (20)     1564 2022-02-03 13:43:13.000000 Orange3-ImageAnalytics-0.8.0/tox.ini
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.735417 Orange3-ImageAnalytics-0.9.0/
+-rw-r--r--   0 primoz     (501) staff       (20)      324 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/.coveragerc
+-rw-r--r--   0 primoz     (501) staff       (20)    35147 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/LICENSE.txt
+-rw-r--r--   0 primoz     (501) staff       (20)      244 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/MANIFEST.in
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.672929 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/
+-rw-r--r--   0 primoz     (501) staff       (20)     1340 2022-10-14 11:54:51.000000 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/PKG-INFO
+-rw-r--r--   0 primoz     (501) staff       (20)     8566 2022-10-14 11:54:51.000000 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 primoz     (501) staff       (20)        1 2022-10-14 11:54:51.000000 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 primoz     (501) staff       (20)      232 2022-10-14 11:54:51.000000 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/entry_points.txt
+-rw-r--r--   0 primoz     (501) staff       (20)       14 2022-10-14 11:54:51.000000 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/namespace_packages.txt
+-rw-r--r--   0 primoz     (501) staff       (20)      168 2022-10-14 11:54:51.000000 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/requires.txt
+-rw-r--r--   0 primoz     (501) staff       (20)       14 2022-10-14 11:54:51.000000 Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/top_level.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     1340 2022-10-14 11:54:51.735274 Orange3-ImageAnalytics-0.9.0/PKG-INFO
+-rw-r--r--   0 primoz     (501) staff       (20)     1282 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/README.md
+-rw-r--r--   0 primoz     (501) staff       (20)      628 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/README.pypi
+-rw-r--r--   0 primoz     (501) staff       (20)      178 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/codecov.yml
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.673664 Orange3-ImageAnalytics-0.9.0/doc/
+-rw-r--r--   0 primoz     (501) staff       (20)     6806 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/Makefile
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.668595 Orange3-ImageAnalytics-0.9.0/doc/_build/
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.674703 Orange3-ImageAnalytics-0.9.0/doc/_build/html/
+-rw-r--r--   0 primoz     (501) staff       (20)      230 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/.buildinfo
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.680423 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/
+-rw-r--r--   0 primoz     (501) staff       (20)   227359 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageEmbedding-Example1.png
+-rw-r--r--   0 primoz     (501) staff       (20)    79682 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageEmbedding-Example2.png
+-rw-r--r--   0 primoz     (501) staff       (20)     8441 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageEmbedding-stamped.png
+-rw-r--r--   0 primoz     (501) staff       (20)    74310 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageGrid-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    51873 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageGrid-stamped.png
+-rw-r--r--   0 primoz     (501) staff       (20)    89158 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageViewer-stamped.png
+-rw-r--r--   0 primoz     (501) staff       (20)   160938 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImportImages-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    10513 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImportImages-class.png
+-rw-r--r--   0 primoz     (501) staff       (20)    10025 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImportImages-stamped.png
+-rw-r--r--   0 primoz     (501) staff       (20)    73586 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/SaveImages-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    10268 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/SaveImages.png
+-rw-r--r--   0 primoz     (501) staff       (20)    51280 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/header-example.png
+-rw-r--r--   0 primoz     (501) staff       (20)   103417 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/image-viewer-example1.png
+-rw-r--r--   0 primoz     (501) staff       (20)   108042 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/image-viewer-example2.png
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.680724 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_modules/
+-rw-r--r--   0 primoz     (501) staff       (20)     4177 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_modules/index.html
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.668797 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_modules/orangecontrib/
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.680884 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_modules/orangecontrib/imageanalytics/
+-rw-r--r--   0 primoz     (501) staff       (20)    45597 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_modules/orangecontrib/imageanalytics/image_embedder.html
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.681088 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/
+-rw-r--r--   0 primoz     (501) staff       (20)      439 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.681287 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/scripting/
+-rw-r--r--   0 primoz     (501) staff       (20)      133 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/scripting/image_embedder.rst.txt
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.682092 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/
+-rw-r--r--   0 primoz     (501) staff       (20)     4900 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/imageembedding.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     1738 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/imagegrid.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     1301 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/imageviewer.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     1705 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/importimages.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     1787 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/saveimages.md.txt
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.685953 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/
+-rw-r--r--   0 primoz     (501) staff       (20)     4418 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 primoz     (501) staff       (20)    14621 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/basic.css
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.686243 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/
+-rw-r--r--   0 primoz     (501) staff       (20)     3275 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.701905 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/
+-rw-r--r--   0 primoz     (501) staff       (20)    87624 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 primoz     (501) staff       (20)    67312 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)    86288 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 primoz     (501) staff       (20)    66444 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   165742 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 primoz     (501) staff       (20)   444379 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 primoz     (501) staff       (20)   165548 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 primoz     (501) staff       (20)    98024 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 primoz     (501) staff       (20)    77160 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   323344 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   193308 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   309728 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   184912 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   328412 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   195704 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   309192 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   182708 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   129674 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/theme.css
+-rw-r--r--   0 primoz     (501) staff       (20)      537 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/custom.css
+-rw-r--r--   0 primoz     (501) staff       (20)     8171 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/doctools.js
+-rw-r--r--   0 primoz     (501) staff       (20)      415 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/documentation_options.js
+-rw-r--r--   0 primoz     (501) staff       (20)      286 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/file.png
+-rw-r--r--   0 primoz     (501) staff       (20)   288580 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 primoz     (501) staff       (20)    89501 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/jquery.js
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.703765 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/
+-rw-r--r--   0 primoz     (501) staff       (20)      934 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 primoz     (501) staff       (20)     4370 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 primoz     (501) staff       (20)     2734 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 primoz     (501) staff       (20)     5023 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/theme.js
+-rw-r--r--   0 primoz     (501) staff       (20)     4758 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/language_data.js
+-rw-r--r--   0 primoz     (501) staff       (20)       90 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/minus.png
+-rw-r--r--   0 primoz     (501) staff       (20)       90 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/plus.png
+-rw-r--r--   0 primoz     (501) staff       (20)     4846 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/pygments.css
+-rw-r--r--   0 primoz     (501) staff       (20)    17120 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/searchtools.js
+-rw-r--r--   0 primoz     (501) staff       (20)    68420 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 primoz     (501) staff       (20)    19530 2022-08-24 08:40:46.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/underscore.js
+-rw-r--r--   0 primoz     (501) staff       (20)     7022 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/genindex.html
+-rw-r--r--   0 primoz     (501) staff       (20)     6267 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/index.html
+-rw-r--r--   0 primoz     (501) staff       (20)      505 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/objects.inv
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.703965 Orange3-ImageAnalytics-0.9.0/doc/_build/html/scripting/
+-rw-r--r--   0 primoz     (501) staff       (20)    18830 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/scripting/image_embedder.html
+-rw-r--r--   0 primoz     (501) staff       (20)     4357 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/search.html
+-rw-r--r--   0 primoz     (501) staff       (20)     8088 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/searchindex.js
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.704762 Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/
+-rw-r--r--   0 primoz     (501) staff       (20)    11725 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/imageembedding.html
+-rw-r--r--   0 primoz     (501) staff       (20)     7332 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/imagegrid.html
+-rw-r--r--   0 primoz     (501) staff       (20)     6871 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/imageviewer.html
+-rw-r--r--   0 primoz     (501) staff       (20)     7323 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/importimages.html
+-rw-r--r--   0 primoz     (501) staff       (20)     7798 2022-10-14 11:53:36.000000 Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/saveimages.html
+-rw-r--r--   0 primoz     (501) staff       (20)     8975 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/doc/conf.py
+-rw-r--r--   0 primoz     (501) staff       (20)      439 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/doc/index.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     6723 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/make.bat
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.704878 Orange3-ImageAnalytics-0.9.0/doc/scripting/
+-rw-r--r--   0 primoz     (501) staff       (20)      133 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/doc/scripting/image_embedder.rst
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.706205 Orange3-ImageAnalytics-0.9.0/doc/widgets/
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.706726 Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/
+-rwxr-xr-x   0 primoz     (501) staff       (20)     5119 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/image-embedding.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)     5099 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/image-grid.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)     4903 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/image-viewer.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)     5614 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/import-images.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)     4900 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/imageembedding.md
+-rwxr-xr-x   0 primoz     (501) staff       (20)     1738 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/imagegrid.md
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.713134 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/
+-rw-r--r--   0 primoz     (501) staff       (20)   227359 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageEmbedding-Example1.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)    79682 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageEmbedding-Example2.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)     8441 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageEmbedding-stamped.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)    74310 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageGrid-Example.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)    51873 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageGrid-stamped.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)    89158 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageViewer-stamped.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)   332303 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageViewer.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)   160938 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImportImages-Example.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)    10513 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImportImages-class.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)    10025 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImportImages-stamped.png
+-rw-r--r--   0 primoz     (501) staff       (20)    73586 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/SaveImages-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    10268 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/SaveImages.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)    51280 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/header-example.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)   103417 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/image-viewer-example1.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)   108042 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/images/image-viewer-example2.png
+-rwxr-xr-x   0 primoz     (501) staff       (20)     1301 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/imageviewer.md
+-rwxr-xr-x   0 primoz     (501) staff       (20)     1705 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/importimages.md
+-rwxr-xr-x   0 primoz     (501) staff       (20)     1787 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets/saveimages.md
+-rw-r--r--   0 primoz     (501) staff       (20)     1360 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/doc/widgets.json
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.713465 Orange3-ImageAnalytics-0.9.0/orangecontrib/
+-rw-r--r--   0 primoz     (501) staff       (20)       80 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.714450 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    11327 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/image_embedder.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7313 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/image_grid.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7801 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/import_images.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2003 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/local_embedder.py
+-rw-r--r--   0 primoz     (501) staff       (20)      817 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/server_embedder.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.715256 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    10993 2022-10-14 11:52:54.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_image_embedder.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1102 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_image_grid.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.722711 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/
+-rw-r--r--   0 primoz     (501) staff       (20)     5953 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_0.jpg
+-rw-r--r--   0 primoz     (501) staff       (20)   786572 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_1.tiff
+-rw-r--r--   0 primoz     (501) staff       (20)   124610 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.bmp
+-rw-r--r--   0 primoz     (501) staff       (20)    24724 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.gif
+-rw-r--r--   0 primoz     (501) staff       (20)     9745 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpeg
+-rw-r--r--   0 primoz     (501) staff       (20)     9745 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpg
+-rw-r--r--   0 primoz     (501) staff       (20)     4015 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pbm
+-rw-r--r--   0 primoz     (501) staff       (20)    31137 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pgm
+-rw-r--r--   0 primoz     (501) staff       (20)    16839 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.png
+-rw-r--r--   0 primoz     (501) staff       (20)    31137 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pnm
+-rw-r--r--   0 primoz     (501) staff       (20)    93381 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.ppm
+-rw-r--r--   0 primoz     (501) staff       (20)    31292 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tif
+-rw-r--r--   0 primoz     (501) staff       (20)    31292 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tiff
+-rw-r--r--   0 primoz     (501) staff       (20)    25136 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xbm
+-rw-r--r--   0 primoz     (501) staff       (20)    67078 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xpm
+-rw-r--r--   0 primoz     (501) staff       (20)     1539 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_3.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     1644 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_import_images.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.723481 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)     3000 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/embedder_utils.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2688 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/image_utils.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.724725 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)     4180 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/tests/test_embedder_utils.py
+-rw-r--r--   0 primoz     (501) staff       (20)     4521 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/tests/test_image_utils.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.727252 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/
+-rw-r--r--   0 primoz     (501) staff       (20)     1041 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.729811 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/
+-rwxr-xr-x   0 primoz     (501) staff       (20)     4830 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/Category-ImageAnalytics.svg
+-rwxr-xr-x   0 primoz     (501) staff       (20)     4097 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImageEmbedding.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     1553 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImageGrid.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     4831 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImageViewer.svg
+-rwxr-xr-x   0 primoz     (501) staff       (20)     5083 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImportImages.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     1637 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/SaveImages.svg
+-rw-r--r--   0 primoz     (501) staff       (20)    10675 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimageembedding.py
+-rw-r--r--   0 primoz     (501) staff       (20)    45677 2022-09-13 07:27:19.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimagegrid.py
+-rw-r--r--   0 primoz     (501) staff       (20)    20884 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimageimport.py
+-rw-r--r--   0 primoz     (501) staff       (20)    26576 2022-09-13 06:56:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimageviewer.py
+-rw-r--r--   0 primoz     (501) staff       (20)    12416 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owsaveimages.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.732129 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.734012 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/
+-rw-r--r--   0 primoz     (501) staff       (20)    91156 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/afternoon-4175917_640.jpg
+-rw-r--r--   0 primoz     (501) staff       (20)    71036 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/atomium-4179270_640.jpg
+-rw-r--r--   0 primoz     (501) staff       (20)    75496 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/kittens-4020199_640.jpg
+-rw-r--r--   0 primoz     (501) staff       (20)    76767 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/landscape-2130524_640.jpg
+-rw-r--r--   0 primoz     (501) staff       (20)     6721 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimageembedding.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7007 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimagegrid.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2887 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimageimport.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1704 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimageviewer.py
+-rw-r--r--   0 primoz     (501) staff       (20)    12851 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owsaveimages.py
+-rw-r--r--   0 primoz     (501) staff       (20)      534 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/utils.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.734708 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)     4027 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/imagepreview.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2022-10-14 11:54:51.735065 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)      515 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/tests/test_imagepreview.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1361 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/tests/test_thumnbnailview.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7998 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/thumbnailview.py
+-rw-r--r--   0 primoz     (501) staff       (20)       90 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/pyproject.toml
+-rw-r--r--   0 primoz     (501) staff       (20)       10 2022-09-13 06:42:06.000000 Orange3-ImageAnalytics-0.9.0/requirements-opt.txt
+-rw-r--r--   0 primoz     (501) staff       (20)       38 2022-10-14 11:54:51.735470 Orange3-ImageAnalytics-0.9.0/setup.cfg
+-rwxr-xr-x   0 primoz     (501) staff       (20)     3160 2022-10-14 11:54:47.000000 Orange3-ImageAnalytics-0.9.0/setup.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1636 2022-09-13 06:42:46.000000 Orange3-ImageAnalytics-0.9.0/tox.ini
```

### Comparing `Orange3-ImageAnalytics-0.8.0/LICENSE.txt` & `Orange3-ImageAnalytics-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/PKG-INFO` & `Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-ImageAnalytics
-Version: 0.8.0
+Version: 0.9.0
 Summary: Orange3 add-on for image data mining.
 Home-page: http://orange.biolab.si/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
 Keywords: orange3 add-on,orange3-imageanalytics
 Platform: UNKNOWN
```

### Comparing `Orange3-ImageAnalytics-0.8.0/Orange3_ImageAnalytics.egg-info/SOURCES.txt` & `Orange3-ImageAnalytics-0.9.0/Orange3_ImageAnalytics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 .coveragerc
-.gitignore
 LICENSE.txt
 MANIFEST.in
 README.md
 README.pypi
 codecov.yml
 pyproject.toml
 requirements-opt.txt
-requirements.txt
 setup.py
 tox.ini
-.github/FUNDING.yml
-.github/ISSUE_TEMPLATE.md
-.github/PULL_REQUEST_TEMPLATE.md
-.github/workflows/test.yml
 Orange3_ImageAnalytics.egg-info/PKG-INFO
 Orange3_ImageAnalytics.egg-info/SOURCES.txt
 Orange3_ImageAnalytics.egg-info/dependency_links.txt
 Orange3_ImageAnalytics.egg-info/entry_points.txt
 Orange3_ImageAnalytics.egg-info/namespace_packages.txt
 Orange3_ImageAnalytics.egg-info/requires.txt
 Orange3_ImageAnalytics.egg-info/top_level.txt
@@ -51,20 +45,21 @@
 doc/_build/html/_sources/index.rst.txt
 doc/_build/html/_sources/scripting/image_embedder.rst.txt
 doc/_build/html/_sources/widgets/imageembedding.md.txt
 doc/_build/html/_sources/widgets/imagegrid.md.txt
 doc/_build/html/_sources/widgets/imageviewer.md.txt
 doc/_build/html/_sources/widgets/importimages.md.txt
 doc/_build/html/_sources/widgets/saveimages.md.txt
+doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
 doc/_build/html/_static/basic.css
 doc/_build/html/_static/custom.css
 doc/_build/html/_static/doctools.js
 doc/_build/html/_static/documentation_options.js
 doc/_build/html/_static/file.png
-doc/_build/html/_static/jquery-3.5.1.js
+doc/_build/html/_static/jquery-3.6.0.js
 doc/_build/html/_static/jquery.js
 doc/_build/html/_static/language_data.js
 doc/_build/html/_static/minus.png
 doc/_build/html/_static/plus.png
 doc/_build/html/_static/pygments.css
 doc/_build/html/_static/searchtools.js
 doc/_build/html/_static/underscore-1.13.1.js
@@ -95,15 +90,14 @@
 doc/_build/html/scripting/image_embedder.html
 doc/_build/html/widgets/imageembedding.html
 doc/_build/html/widgets/imagegrid.html
 doc/_build/html/widgets/imageviewer.html
 doc/_build/html/widgets/importimages.html
 doc/_build/html/widgets/saveimages.html
 doc/scripting/image_embedder.rst
-doc/static/custom.css
 doc/widgets/imageembedding.md
 doc/widgets/imagegrid.md
 doc/widgets/imageviewer.md
 doc/widgets/importimages.md
 doc/widgets/saveimages.md
 doc/widgets/icons/image-embedding.png
 doc/widgets/icons/image-grid.png
@@ -131,15 +125,14 @@
 orangecontrib/imageanalytics/import_images.py
 orangecontrib/imageanalytics/local_embedder.py
 orangecontrib/imageanalytics/server_embedder.py
 orangecontrib/imageanalytics/tests/__init__.py
 orangecontrib/imageanalytics/tests/test_image_embedder.py
 orangecontrib/imageanalytics/tests/test_image_grid.py
 orangecontrib/imageanalytics/tests/test_import_images.py
-orangecontrib/imageanalytics/tests/test_images/.DS_Store
 orangecontrib/imageanalytics/tests/test_images/example_image_0.jpg
 orangecontrib/imageanalytics/tests/test_images/example_image_1.tiff
 orangecontrib/imageanalytics/tests/test_images/example_image_2.bmp
 orangecontrib/imageanalytics/tests/test_images/example_image_2.gif
 orangecontrib/imageanalytics/tests/test_images/example_image_2.jpeg
 orangecontrib/imageanalytics/tests/test_images/example_image_2.jpg
 orangecontrib/imageanalytics/tests/test_images/example_image_2.pbm
```

### Comparing `Orange3-ImageAnalytics-0.8.0/PKG-INFO` & `Orange3-ImageAnalytics-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-ImageAnalytics
-Version: 0.8.0
+Version: 0.9.0
 Summary: Orange3 add-on for image data mining.
 Home-page: http://orange.biolab.si/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
 Keywords: orange3 add-on,orange3-imageanalytics
 Platform: UNKNOWN
```

### Comparing `Orange3-ImageAnalytics-0.8.0/README.md` & `Orange3-ImageAnalytics-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/README.pypi` & `Orange3-ImageAnalytics-0.9.0/README.pypi`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/Makefile` & `Orange3-ImageAnalytics-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageEmbedding-Example1.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageEmbedding-Example1.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageEmbedding-Example2.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageEmbedding-Example2.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageEmbedding-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageEmbedding-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageGrid-Example.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageGrid-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageGrid-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageGrid-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImageViewer-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImageViewer-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImportImages-Example.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImportImages-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImportImages-class.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImportImages-class.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/ImportImages-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/ImportImages-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/SaveImages-Example.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/SaveImages-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/SaveImages.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/SaveImages.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/header-example.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/header-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/image-viewer-example1.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/image-viewer-example1.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_images/image-viewer-example2.png` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_images/image-viewer-example2.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_modules/index.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_modules/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
+        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" /> 
 </head>
 
 <body class="wy-body-for-nav">
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_modules/orangecontrib/imageanalytics/image_embedder.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_modules/orangecontrib/imageanalytics/image_embedder.html`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   <!--[if lt IE 9]>
     <script src="../../../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../../../" id="documentation_options" src="../../../_static/documentation_options.js"></script>
         <script src="../../../_static/jquery.js"></script>
         <script src="../../../_static/underscore.js"></script>
+        <script src="../../../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../../../_static/doctools.js"></script>
     <script src="../../../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../../../genindex.html" />
     <link rel="search" title="Search" href="../../../search.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
@@ -72,14 +73,15 @@
              
   <h1>Source code for orangecontrib.imageanalytics.image_embedder</h1><div class="highlight"><pre>
 <span></span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">Callable</span><span class="p">,</span> <span class="n">Dict</span><span class="p">,</span> <span class="n">List</span><span class="p">,</span> <span class="n">Optional</span><span class="p">,</span> <span class="n">Tuple</span><span class="p">,</span> <span class="n">Union</span>
 
 <span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
 <span class="kn">from</span> <span class="nn">Orange.data</span> <span class="kn">import</span> <span class="n">ContinuousVariable</span><span class="p">,</span> <span class="n">Domain</span><span class="p">,</span> <span class="n">Table</span><span class="p">,</span> <span class="n">Variable</span>
 <span class="kn">from</span> <span class="nn">Orange.misc.utils.embedder_utils</span> <span class="kn">import</span> <span class="n">EmbedderCache</span>
+<span class="kn">from</span> <span class="nn">Orange.util</span> <span class="kn">import</span> <span class="n">dummy_callback</span>
 
 <span class="kn">from</span> <span class="nn">orangecontrib.imageanalytics.local_embedder</span> <span class="kn">import</span> <span class="n">LocalEmbedder</span>
 <span class="kn">from</span> <span class="nn">orangecontrib.imageanalytics.server_embedder</span> <span class="kn">import</span> <span class="n">ServerEmbedder</span>
 <span class="kn">from</span> <span class="nn">orangecontrib.imageanalytics.utils.image_utils</span> <span class="kn">import</span> <span class="n">extract_paths</span>
 
 <span class="n">MODELS</span> <span class="o">=</span> <span class="p">{</span>
     <span class="s2">&quot;inception-v3&quot;</span><span class="p">:</span> <span class="p">{</span>
@@ -222,15 +224,15 @@
                 <span class="bp">self</span><span class="o">.</span><span class="n">_model_settings</span><span class="p">[</span><span class="s2">&quot;target_image_size&quot;</span><span class="p">]</span>
             <span class="p">)</span>
 
     <span class="k">def</span> <span class="fm">__call__</span><span class="p">(</span>
         <span class="bp">self</span><span class="p">,</span>
         <span class="n">data</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">Table</span><span class="p">,</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">],</span>
         <span class="n">col</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="n">Variable</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-        <span class="n">callback</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Callable</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+        <span class="n">callback</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Callable</span><span class="p">]</span> <span class="o">=</span> <span class="n">dummy_callback</span><span class="p">,</span>
     <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Union</span><span class="p">[</span><span class="n">Tuple</span><span class="p">[</span><span class="n">Table</span><span class="p">,</span> <span class="n">Table</span><span class="p">,</span> <span class="nb">int</span><span class="p">],</span> <span class="n">List</span><span class="p">[</span><span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]]]:</span>
         <span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Embedd images.</span>
 
 <span class="sd">        Parameters</span>
 <span class="sd">        ----------</span>
 <span class="sd">        data</span>
@@ -257,17 +259,15 @@
         <span class="bp">self</span><span class="o">.</span><span class="n">_init_embedder</span><span class="p">()</span>
         <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">Table</span><span class="p">):</span>
             <span class="k">assert</span> <span class="n">col</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">,</span> <span class="s2">&quot;Please provide a column for image path&quot;</span>
             <span class="c1"># if table on input tables on output</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">from_table</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">col</span><span class="o">=</span><span class="n">col</span><span class="p">,</span> <span class="n">callback</span><span class="o">=</span><span class="n">callback</span><span class="p">)</span>
         <span class="k">elif</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">,</span> <span class="nb">list</span><span class="p">)):</span>
             <span class="c1"># if array-like on input array-like on output</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span><span class="o">.</span><span class="n">embedd_data</span><span class="p">(</span>
-                <span class="n">data</span><span class="p">,</span> <span class="n">processed_callback</span><span class="o">=</span><span class="n">callback</span>
-            <span class="p">)</span>
+            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span><span class="o">.</span><span class="n">embedd_data</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">callback</span><span class="o">=</span><span class="n">callback</span><span class="p">)</span>
 
 <div class="viewcode-block" id="ImageEmbedder.from_table"><a class="viewcode-back" href="../../../scripting/image_embedder.html#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.from_table">[docs]</a>    <span class="k">def</span> <span class="nf">from_table</span><span class="p">(</span>
         <span class="bp">self</span><span class="p">,</span>
         <span class="n">data</span><span class="p">:</span> <span class="n">Table</span><span class="p">,</span>
         <span class="n">col</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="n">Variable</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;image&quot;</span><span class="p">,</span>
         <span class="n">callback</span><span class="p">:</span> <span class="n">Callable</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
     <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Tuple</span><span class="p">[</span><span class="n">Table</span><span class="p">,</span> <span class="n">Table</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
@@ -281,22 +281,22 @@
 <span class="sd">        col</span>
 <span class="sd">            The column with image paths</span>
 <span class="sd">        callback</span>
 <span class="sd">            Optional callback - function that is called for every embedded</span>
 <span class="sd">            image and is used to report the progress.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">file_paths</span> <span class="o">=</span> <span class="n">extract_paths</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">data</span><span class="o">.</span><span class="n">domain</span><span class="p">[</span><span class="n">col</span><span class="p">])</span>
-        <span class="n">embeddings_</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span><span class="o">.</span><span class="n">embedd_data</span><span class="p">(</span><span class="n">file_paths</span><span class="p">,</span> <span class="n">callback</span><span class="p">)</span>
+        <span class="n">embeddings_</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span><span class="o">.</span><span class="n">embedd_data</span><span class="p">(</span><span class="n">file_paths</span><span class="p">,</span> <span class="n">callback</span><span class="o">=</span><span class="n">callback</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">ImageEmbedder</span><span class="o">.</span><span class="n">prepare_output_data</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">embeddings_</span><span class="p">)</span></div>
 
     <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;ImageEmbedder&quot;</span><span class="p">:</span>
         <span class="k">return</span> <span class="bp">self</span>
 
-    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">traceback</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-        <span class="bp">self</span><span class="o">.</span><span class="n">set_canceled</span><span class="p">()</span>
+    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">,</span> <span class="n">__</span><span class="p">,</span> <span class="n">___</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="k">pass</span>
 
     <span class="k">def</span> <span class="fm">__del__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="bp">self</span><span class="o">.</span><span class="fm">__exit__</span><span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="kc">None</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
 
 <div class="viewcode-block" id="ImageEmbedder.construct_output_data_table"><a class="viewcode-back" href="../../../scripting/image_embedder.html#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.construct_output_data_table">[docs]</a>    <span class="nd">@staticmethod</span>
     <span class="k">def</span> <span class="nf">construct_output_data_table</span><span class="p">(</span>
             <span class="n">embedded_images</span><span class="p">:</span> <span class="n">Table</span><span class="p">,</span> <span class="n">embeddings_</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span>
@@ -390,22 +390,15 @@
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span><span class="p">:</span>
             <span class="c1"># embedder is loaded so we clean its cache</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span><span class="o">.</span><span class="n">clear_cache</span><span class="p">()</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="c1"># embedder is not initialized yet - clear it cache from file</span>
             <span class="n">cache</span> <span class="o">=</span> <span class="n">EmbedderCache</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">model</span><span class="p">)</span>
-            <span class="n">cache</span><span class="o">.</span><span class="n">clear_cache</span><span class="p">()</span></div>
-
-<div class="viewcode-block" id="ImageEmbedder.set_canceled"><a class="viewcode-back" href="../../../scripting/image_embedder.html#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.set_canceled">[docs]</a>    <span class="k">def</span> <span class="nf">set_canceled</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-        <span class="sd">&quot;&quot;&quot;</span>
-<span class="sd">        Cancel the embedding</span>
-<span class="sd">        &quot;&quot;&quot;</span>
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_embedder</span><span class="o">.</span><span class="n">set_cancelled</span><span class="p">()</span></div></div>
+            <span class="n">cache</span><span class="o">.</span><span class="n">clear_cache</span><span class="p">()</span></div></div>
 
 
 <span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
     <span class="n">image_file_paths</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;tests/test_images/example_image_0.jpg&quot;</span><span class="p">]</span>
     <span class="c1"># with ImageEmbedder(model=&#39;inception-v3&#39;) as embedder:</span>
     <span class="k">with</span> <span class="n">ImageEmbedder</span><span class="p">(</span><span class="n">model</span><span class="o">=</span><span class="s2">&quot;squeezenet&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">embedder</span><span class="p">:</span>
         <span class="n">embedder</span><span class="o">.</span><span class="n">clear_cache</span><span class="p">()</span>
```

#### html2text {}

```diff
@@ -19,14 +19,15 @@
 ===============================================================================
 ****** Source code for orangecontrib.imageanalytics.image_embedder ******
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from Orange.data import ContinuousVariable, Domain, Table, Variable
 from Orange.misc.utils.embedder_utils import EmbedderCache
+from Orange.util import dummy_callback
 
 from orangecontrib.imageanalytics.local_embedder import LocalEmbedder
 from orangecontrib.imageanalytics.server_embedder import ServerEmbedder
 from orangecontrib.imageanalytics.utils.image_utils import extract_paths
 
 MODELS = {
     "inception-v3": {
@@ -173,15 +174,15 @@
                 self._model_settings["target_image_size"]
             )
 
     def __call__(
         self,
         data: Union[Table, List[str], np.array],
         col: Optional[Union[str, Variable]] = None,
-        callback: Optional[Callable] = None,
+        callback: Optional[Callable] = dummy_callback,
     ) -> Union[Tuple[Table, Table, int], List[List[float]]]:
         """
         Embedd images.
 
         Parameters
         ----------
         data
@@ -208,17 +209,15 @@
         self._init_embedder()
         if isinstance(data, Table):
             assert col is not None, "Please provide a column for image path"
             # if table on input tables on output
             return self.from_table(data, col=col, callback=callback)
         elif isinstance(data, (np.ndarray, list)):
             # if array-like on input array-like on output
-            return self._embedder.embedd_data(
-                data, processed_callback=callback
-            )
+            return self._embedder.embedd_data(data, callback=callback)
 
 [docs]    def from_table(
         self,
         data: Table,
         col: Union[str, Variable] = "image",
         callback: Callable = None,
     ) -> Tuple[Table, Table, int]:
@@ -232,23 +231,23 @@
         col
             The column with image paths
         callback
             Optional callback - function that is called for every embedded
             image and is used to report the progress.
         """
         file_paths = extract_paths(data, data.domain[col])
-        embeddings_ = self._embedder.embedd_data(file_paths, callback)
+        embeddings_ = self._embedder.embedd_data(file_paths, callback=callback)
         return ImageEmbedder.prepare_output_data(data, embeddings_)
 
 
     def __enter__(self) -> "ImageEmbedder":
         return self
 
-    def __exit__(self, exception_type, exception_value, traceback) -> None:
-        self.set_canceled()
+    def __exit__(self, _, __, ___) -> None:
+        pass
 
     def __del__(self) -> None:
         self.__exit__(None, None, None)
 
 [docs]    @staticmethod
     def construct_output_data_table(
             embedded_images: Table, embeddings_: np.ndarray
@@ -348,22 +347,14 @@
             self._embedder.clear_cache()
         else:
             # embedder is not initialized yet - clear it cache from file
             cache = EmbedderCache(self.model)
             cache.clear_cache()
 
 
-[docs]    def set_canceled(self) -> None:
-        """
-        Cancel the embedding
-        """
-        if self._embedder is not None:
-            self._embedder.set_cancelled()
-
-
 
 if __name__ == "__main__":
     image_file_paths = ["tests/test_images/example_image_0.jpg"]
     # with ImageEmbedder(model='inception-v3') as embedder:
     with ImageEmbedder(model="squeezenet") as embedder:
         embedder.clear_cache()
         print(embedder(image_file_paths))
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/imageembedding.md.txt` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/imageembedding.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/imagegrid.md.txt` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/imagegrid.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/imageviewer.md.txt` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/imageviewer.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/importimages.md.txt` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/importimages.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_sources/widgets/saveimages.md.txt` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_sources/widgets/saveimages.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/basic.css` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/basic.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -218,39 +218,39 @@
     padding: 2px;
     border-collapse: collapse;
 }
 
 /* -- general body styles --------------------------------------------------- */
 
 div.body {
-    min-width: 450px;
+    min-width: 360px;
     max-width: 800px;
 }
 
 div.body p, div.body dd, div.body li, div.body blockquote {
     -moz-hyphens: auto;
     -ms-hyphens: auto;
     -webkit-hyphens: auto;
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
-
 a.brackets:before,
 span.brackets > a:before{
     content: "[";
 }
 
 a.brackets:after,
 span.brackets > a:after {
     content: "]";
 }
 
+
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
 dt:hover > a.headerlink,
@@ -330,21 +330,19 @@
     clear: right;
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
-
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
-
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -424,18 +422,14 @@
     padding: 1px 8px 1px 5px;
     border-top: 0;
     border-left: 0;
     border-right: 0;
     border-bottom: 1px solid #aaa;
 }
 
-table.footnote td, table.footnote th {
-    border: 0 !important;
-}
-
 th {
     text-align: left;
     padding-right: 5px;
 }
 
 table.citation {
     border-left: solid 1px gray;
@@ -610,15 +604,14 @@
     margin-top: 0;
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
-
 dl.footnote > dt,
 dl.citation > dt {
     float: left;
     margin-right: 0.5em;
 }
 
 dl.footnote > dd,
@@ -639,19 +632,19 @@
 
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
-
 dl.field-list > dt:after {
     content: ":";
 }
 
+
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
 
@@ -753,14 +746,15 @@
 }
 
 span.pre {
     -moz-hyphens: none;
     -ms-hyphens: none;
     -webkit-hyphens: none;
     hyphens: none;
+    white-space: nowrap;
 }
 
 div[class*="highlight-"] {
     margin: 1em 0;
 }
 
 td.linenos pre {
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/badge_only.css` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold.woff` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-bold.woff2` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal.woff` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/fonts/lato-normal.woff2` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/css/theme.css` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/custom.css` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/custom.css`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/jquery-3.5.1.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/jquery-3.6.0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 /*!
- * jQuery JavaScript Library v3.5.1
+ * jQuery JavaScript Library v3.6.0
  * https://jquery.com/
  *
  * Includes Sizzle.js
  * https://sizzlejs.com/
  *
- * Copyright JS Foundation and other contributors
+ * Copyright OpenJS Foundation and other contributors
  * Released under the MIT license
  * https://jquery.org/license
  *
- * Date: 2020-05-04T22:49Z
+ * Date: 2021-03-02T17:08Z
  */
 (function(global, factory) {
 
     "use strict";
 
     if (typeof module === "object" && typeof module.exports === "object") {
 
@@ -76,15 +76,19 @@
 
     var isFunction = function isFunction(obj) {
 
         // Support: Chrome <=57, Firefox <=52
         // In some browsers, typeof returns "function" for HTML <object> elements
         // (i.e., `typeof document.createElement( "object" ) === "function"`).
         // We don't want to classify *any* DOM node as a function.
-        return typeof obj === "function" && typeof obj.nodeType !== "number";
+        // Support: QtWeb <=3.8.5, WebKit <=534.34, wkhtmltopdf tool <=0.12.5
+        // Plus for old WebKit, typeof returns "function" for HTML collections
+        // (e.g., `typeof document.getElementsByTagName("div") === "function"`). (gh-4756)
+        return typeof obj === "function" && typeof obj.nodeType !== "number" &&
+            typeof obj.item !== "function";
     };
 
 
     var isWindow = function isWindow(obj) {
         return obj != null && obj === obj.window;
     };
 
@@ -143,15 +147,15 @@
     /* global Symbol */
     // Defining this global in .eslintrc.json would create a danger of using the global
     // unguarded in another place, it seems safer to define global only for this module
 
 
 
     var
-        version = "3.5.1",
+        version = "3.6.0",
 
         // Define a local copy of jQuery
         jQuery = function(selector, context) {
 
             // The jQuery object is actually just the init constructor 'enhanced'
             // Need init if jQuery is called (just allow error to be thrown if not included)
             return new jQuery.fn.init(selector, context);
@@ -515,22 +519,22 @@
         }
 
         return type === "array" || length === 0 ||
             typeof length === "number" && length > 0 && (length - 1) in obj;
     }
     var Sizzle =
         /*!
-         * Sizzle CSS Selector Engine v2.3.5
+         * Sizzle CSS Selector Engine v2.3.6
          * https://sizzlejs.com/
          *
          * Copyright JS Foundation and other contributors
          * Released under the MIT license
          * https://js.foundation/
          *
-         * Date: 2020-03-14
+         * Date: 2021-02-16
          */
         (function(window) {
             var i,
                 support,
                 Expr,
                 getText,
                 isXML,
@@ -1108,16 +1112,16 @@
 
             /**
              * Detects XML nodes
              * @param {Element|Object} elem An element or a document
              * @returns {Boolean} True iff elem is a non-HTML XML node
              */
             isXML = Sizzle.isXML = function(elem) {
-                var namespace = elem.namespaceURI,
-                    docElem = (elem.ownerDocument || elem).documentElement;
+                var namespace = elem && elem.namespaceURI,
+                    docElem = elem && (elem.ownerDocument || elem).documentElement;
 
                 // Support: IE <=8
                 // Assume HTML when documentElement doesn't yet exist, such as inside loading iframes
                 // https://bugs.jquery.com/ticket/4833
                 return !rhtml.test(namespace || docElem && docElem.nodeName || "HTML");
             };
 
@@ -3048,15 +3052,15 @@
 
 
 
     function nodeName(elem, name) {
 
         return elem.nodeName && elem.nodeName.toLowerCase() === name.toLowerCase();
 
-    };
+    }
     var rsingleTag = (/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i);
 
 
 
     // Implement the identical functionality for filter and not
     function winnow(elements, qualifier, not) {
         if (isFunction(qualifier)) {
@@ -4024,47 +4028,47 @@
                 // count of unprocessed arguments
                 i = remaining,
 
                 // subordinate fulfillment data
                 resolveContexts = Array(i),
                 resolveValues = slice.call(arguments),
 
-                // the master Deferred
-                master = jQuery.Deferred(),
+                // the primary Deferred
+                primary = jQuery.Deferred(),
 
                 // subordinate callback factory
                 updateFunc = function(i) {
                     return function(value) {
                         resolveContexts[i] = this;
                         resolveValues[i] = arguments.length > 1 ? slice.call(arguments) : value;
                         if (!(--remaining)) {
-                            master.resolveWith(resolveContexts, resolveValues);
+                            primary.resolveWith(resolveContexts, resolveValues);
                         }
                     };
                 };
 
             // Single- and empty arguments are adopted like Promise.resolve
             if (remaining <= 1) {
-                adoptValue(singleValue, master.done(updateFunc(i)).resolve, master.reject,
+                adoptValue(singleValue, primary.done(updateFunc(i)).resolve, primary.reject,
                     !remaining);
 
                 // Use .then() to unwrap secondary thenables (cf. gh-3000)
-                if (master.state() === "pending" ||
+                if (primary.state() === "pending" ||
                     isFunction(resolveValues[i] && resolveValues[i].then)) {
 
-                    return master.then();
+                    return primary.then();
                 }
             }
 
             // Multiple arguments are aggregated like Promise.all array elements
             while (i--) {
-                adoptValue(resolveValues[i], updateFunc(i), master.reject);
+                adoptValue(resolveValues[i], updateFunc(i), primary.reject);
             }
 
-            return master.promise();
+            return primary.promise();
         }
     });
 
 
     // These usually indicate a programmer mistake during development,
     // warn about them ASAP rather than swallowing them by default.
     var rerrorNames = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
@@ -5117,18 +5121,15 @@
             }
         }
 
         return fragment;
     }
 
 
-    var
-        rkeyEvent = /^key/,
-        rmouseEvent = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        rtypenamespace = /^([^.]*)(?:\.(.+)|)/;
+    var rtypenamespace = /^([^.]*)(?:\.(.+)|)/;
 
     function returnTrue() {
         return true;
     }
 
     function returnFalse() {
         return false;
@@ -5689,15 +5690,21 @@
                             result = {};
                         }
                         if (saved !== result) {
 
                             // Cancel the outer synthetic event
                             event.stopImmediatePropagation();
                             event.preventDefault();
-                            return result.value;
+
+                            // Support: Chrome 86+
+                            // In Chrome, if an element having a focusout handler is blurred by
+                            // clicking outside of it, it invokes the handler synchronously. If
+                            // that handler calls `.remove()` on the element, the data is cleared,
+                            // leaving `result` undefined. We need to guard against this.
+                            return result && result.value;
                         }
 
                         // If this is an inner synthetic event for an event with a bubbling surrogate
                         // (focus or blur), assume that the surrogate already propagated from triggering the
                         // native event and prevent that from happening again here.
                         // This technically gets the ordering wrong w.r.t. to `.trigger()` (in which the
                         // bubbling surrogate propagates *after* the non-bubbling base), but that seems
@@ -5854,42 +5861,15 @@
         pointerId: true,
         pointerType: true,
         screenX: true,
         screenY: true,
         targetTouches: true,
         toElement: true,
         touches: true,
-
-        which: function(event) {
-            var button = event.button;
-
-            // Add which for key events
-            if (event.which == null && rkeyEvent.test(event.type)) {
-                return event.charCode != null ? event.charCode : event.keyCode;
-            }
-
-            // Add which for click: 1 === left; 2 === middle; 3 === right
-            if (!event.which && button !== undefined && rmouseEvent.test(event.type)) {
-                if (button & 1) {
-                    return 1;
-                }
-
-                if (button & 2) {
-                    return 3;
-                }
-
-                if (button & 4) {
-                    return 2;
-                }
-
-                return 0;
-            }
-
-            return event.which;
-        }
+        which: true
     }, jQuery.event.addProp);
 
     jQuery.each({
         focus: "focusin",
         blur: "focusout"
     }, function(type, delegateType) {
         jQuery.event.special[type] = {
@@ -5910,14 +5890,20 @@
                 // Force setup before trigger
                 leverageNative(this, type);
 
                 // Return non-false to allow normal event-path propagation
                 return true;
             },
 
+            // Suppress native focus or blur as it's already being fired
+            // in leverageNative.
+            _default: function() {
+                return true;
+            },
+
             delegateType: delegateType
         };
     });
 
     // Create mouseenter/leave events using mouseover/out and event-time checks
     // so that event delegation works in jQuery.
     // Do the same for pointerenter/pointerleave and pointerover/pointerout
@@ -6581,32 +6567,51 @@
             },
 
             // Support: IE 9 - 11+, Edge 15 - 18+
             // IE/Edge misreport `getComputedStyle` of table rows with width/height
             // set in CSS while `offset*` properties report correct values.
             // Behavior in IE 9 is more subtle than in newer versions & it passes
             // some versions of this test; make sure not to make it pass there!
+            //
+            // Support: Firefox 70+
+            // Only Firefox includes border widths
+            // in computed dimensions. (gh-4529)
             reliableTrDimensions: function() {
                 var table, tr, trChild, trStyle;
                 if (reliableTrDimensionsVal == null) {
                     table = document.createElement("table");
                     tr = document.createElement("tr");
                     trChild = document.createElement("div");
 
-                    table.style.cssText = "position:absolute;left:-11111px";
+                    table.style.cssText = "position:absolute;left:-11111px;border-collapse:separate";
+                    tr.style.cssText = "border:1px solid";
+
+                    // Support: Chrome 86+
+                    // Height set through cssText does not get applied.
+                    // Computed height then comes back as 0.
                     tr.style.height = "1px";
                     trChild.style.height = "9px";
 
+                    // Support: Android 8 Chrome 86+
+                    // In our bodyBackground.html iframe,
+                    // display for all div elements is set to "inline",
+                    // which causes a problem only in Android 8 Chrome 86.
+                    // Ensuring the div is display: block
+                    // gets around this issue.
+                    trChild.style.display = "block";
+
                     documentElement
                         .appendChild(table)
                         .appendChild(tr)
                         .appendChild(trChild);
 
                     trStyle = window.getComputedStyle(tr);
-                    reliableTrDimensionsVal = parseInt(trStyle.height) > 3;
+                    reliableTrDimensionsVal = (parseInt(trStyle.height, 10) +
+                        parseInt(trStyle.borderTopWidth, 10) +
+                        parseInt(trStyle.borderBottomWidth, 10)) === tr.offsetHeight;
 
                     documentElement.removeChild(table);
                 }
                 return reliableTrDimensionsVal;
             }
         });
     })();
@@ -7813,14 +7818,15 @@
                     var anim = Animation(this, jQuery.extend({}, prop), optall);
 
                     // Empty animations, or finishing resolves immediately
                     if (empty || dataPriv.get(this, "finish")) {
                         anim.stop(true);
                     }
                 };
+
             doAnimation.finish = doAnimation;
 
             return empty || optall.queue === false ?
                 this.each(doAnimation) :
                 this.queue(optall.queue, doAnimation);
         },
         stop: function(type, clearQueue, gotoEnd) {
@@ -8764,17 +8770,15 @@
             while ((cur = eventPath[i++]) && !event.isPropagationStopped()) {
                 lastElement = cur;
                 event.type = i > 1 ?
                     bubbleType :
                     special.bindType || type;
 
                 // jQuery handler
-                handle = (
-                        dataPriv.get(cur, "events") || Object.create(null)
-                    )[event.type] &&
+                handle = (dataPriv.get(cur, "events") || Object.create(null))[event.type] &&
                     dataPriv.get(cur, "handle");
                 if (handle) {
                     handle.apply(cur, data);
                 }
 
                 // Native handler
                 handle = ontype && cur[ontype];
@@ -8917,29 +8921,34 @@
 
     var rquery = (/\?/);
 
 
 
     // Cross-browser xml parsing
     jQuery.parseXML = function(data) {
-        var xml;
+        var xml, parserErrorElem;
         if (!data || typeof data !== "string") {
             return null;
         }
 
         // Support: IE 9 - 11 only
         // IE throws on parseFromString with invalid input.
         try {
             xml = (new window.DOMParser()).parseFromString(data, "text/xml");
-        } catch (e) {
-            xml = undefined;
-        }
+        } catch (e) {}
 
-        if (!xml || xml.getElementsByTagName("parsererror").length) {
-            jQuery.error("Invalid XML: " + data);
+        parserErrorElem = xml && xml.getElementsByTagName("parsererror")[0];
+        if (!xml || parserErrorElem) {
+            jQuery.error("Invalid XML: " + (
+                parserErrorElem ?
+                jQuery.map(parserErrorElem.childNodes, function(el) {
+                    return el.textContent;
+                }).join("\n") :
+                data
+            ));
         }
         return xml;
     };
 
 
     var
         rbracket = /\[\]$/,
@@ -9029,47 +9038,45 @@
     jQuery.fn.extend({
         serialize: function() {
             return jQuery.param(this.serializeArray());
         },
         serializeArray: function() {
             return this.map(function() {
 
-                    // Can add propHook for "elements" to filter or add form elements
-                    var elements = jQuery.prop(this, "elements");
-                    return elements ? jQuery.makeArray(elements) : this;
-                })
-                .filter(function() {
-                    var type = this.type;
-
-                    // Use .is( ":disabled" ) so that fieldset[disabled] works
-                    return this.name && !jQuery(this).is(":disabled") &&
-                        rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
-                        (this.checked || !rcheckableType.test(type));
-                })
-                .map(function(_i, elem) {
-                    var val = jQuery(this).val();
+                // Can add propHook for "elements" to filter or add form elements
+                var elements = jQuery.prop(this, "elements");
+                return elements ? jQuery.makeArray(elements) : this;
+            }).filter(function() {
+                var type = this.type;
+
+                // Use .is( ":disabled" ) so that fieldset[disabled] works
+                return this.name && !jQuery(this).is(":disabled") &&
+                    rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
+                    (this.checked || !rcheckableType.test(type));
+            }).map(function(_i, elem) {
+                var val = jQuery(this).val();
 
-                    if (val == null) {
-                        return null;
-                    }
+                if (val == null) {
+                    return null;
+                }
 
-                    if (Array.isArray(val)) {
-                        return jQuery.map(val, function(val) {
-                            return {
-                                name: elem.name,
-                                value: val.replace(rCRLF, "\r\n")
-                            };
-                        });
-                    }
+                if (Array.isArray(val)) {
+                    return jQuery.map(val, function(val) {
+                        return {
+                            name: elem.name,
+                            value: val.replace(rCRLF, "\r\n")
+                        };
+                    });
+                }
 
-                    return {
-                        name: elem.name,
-                        value: val.replace(rCRLF, "\r\n")
-                    };
-                }).get();
+                return {
+                    name: elem.name,
+                    value: val.replace(rCRLF, "\r\n")
+                };
+            }).get();
         }
     });
 
 
     var
         r20 = /%20/g,
         rhash = /#.*$/,
@@ -9100,14 +9107,15 @@
         transports = {},
 
         // Avoid comment-prolog char sequence (#10098); must appease lint and evade compression
         allTypes = "*/".concat("*"),
 
         // Anchor tag for parsing the document origin
         originAnchor = document.createElement("a");
+
     originAnchor.href = location.href;
 
     // Base "constructor" for jQuery.ajaxPrefilter and jQuery.ajaxTransport
     function addToPrefiltersOrTransports(structure) {
 
         // dataTypeExpression is optional and defaults to "*"
         return function(dataTypeExpression, func) {
@@ -9797,16 +9805,18 @@
                 isSuccess = status >= 200 && status < 300 || status === 304;
 
                 // Get response data
                 if (responses) {
                     response = ajaxHandleResponses(s, jqXHR, responses);
                 }
 
-                // Use a noop converter for missing script
-                if (!isSuccess && jQuery.inArray("script", s.dataTypes) > -1) {
+                // Use a noop converter for missing script but not if jsonp
+                if (!isSuccess &&
+                    jQuery.inArray("script", s.dataTypes) > -1 &&
+                    jQuery.inArray("json", s.dataTypes) < 0) {
                     s.converters["text script"] = function() {};
                 }
 
                 // Convert no matter what (that way responseXXX fields are always set)
                 response = ajaxConvert(s, response, jqXHR, isSuccess);
 
                 // If successful, handle type chaining
@@ -10541,20 +10551,14 @@
                 props.left = (options.left - curOffset.left) + curLeft;
             }
 
             if ("using" in options) {
                 options.using.call(elem, props);
 
             } else {
-                if (typeof props.top === "number") {
-                    props.top += "px";
-                }
-                if (typeof props.left === "number") {
-                    props.left += "px";
-                }
                 curElem.css(props);
             }
         }
     };
 
     jQuery.fn.extend({
 
@@ -10728,59 +10732,58 @@
 
     // Create innerHeight, innerWidth, height, width, outerHeight and outerWidth methods
     jQuery.each({
         Height: "height",
         Width: "width"
     }, function(name, type) {
         jQuery.each({
-                padding: "inner" + name,
-                content: type,
-                "": "outer" + name
-            },
-            function(defaultExtra, funcName) {
-
-                // Margin is only for outerHeight, outerWidth
-                jQuery.fn[funcName] = function(margin, value) {
-                    var chainable = arguments.length && (defaultExtra || typeof margin !== "boolean"),
-                        extra = defaultExtra || (margin === true || value === true ? "margin" : "border");
-
-                    return access(this, function(elem, type, value) {
-                        var doc;
-
-                        if (isWindow(elem)) {
-
-                            // $( window ).outerWidth/Height return w/h including scrollbars (gh-1729)
-                            return funcName.indexOf("outer") === 0 ?
-                                elem["inner" + name] :
-                                elem.document.documentElement["client" + name];
-                        }
-
-                        // Get document width or height
-                        if (elem.nodeType === 9) {
-                            doc = elem.documentElement;
-
-                            // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height],
-                            // whichever is greatest
-                            return Math.max(
-                                elem.body["scroll" + name], doc["scroll" + name],
-                                elem.body["offset" + name], doc["offset" + name],
-                                doc["client" + name]
-                            );
-                        }
+            padding: "inner" + name,
+            content: type,
+            "": "outer" + name
+        }, function(defaultExtra, funcName) {
+
+            // Margin is only for outerHeight, outerWidth
+            jQuery.fn[funcName] = function(margin, value) {
+                var chainable = arguments.length && (defaultExtra || typeof margin !== "boolean"),
+                    extra = defaultExtra || (margin === true || value === true ? "margin" : "border");
+
+                return access(this, function(elem, type, value) {
+                    var doc;
+
+                    if (isWindow(elem)) {
+
+                        // $( window ).outerWidth/Height return w/h including scrollbars (gh-1729)
+                        return funcName.indexOf("outer") === 0 ?
+                            elem["inner" + name] :
+                            elem.document.documentElement["client" + name];
+                    }
+
+                    // Get document width or height
+                    if (elem.nodeType === 9) {
+                        doc = elem.documentElement;
+
+                        // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height],
+                        // whichever is greatest
+                        return Math.max(
+                            elem.body["scroll" + name], doc["scroll" + name],
+                            elem.body["offset" + name], doc["offset" + name],
+                            doc["client" + name]
+                        );
+                    }
 
-                        return value === undefined ?
+                    return value === undefined ?
 
-                            // Get width or height on the element, requesting but not forcing parseFloat
-                            jQuery.css(elem, type, extra) :
+                        // Get width or height on the element, requesting but not forcing parseFloat
+                        jQuery.css(elem, type, extra) :
 
-                            // Set width or height on the element
-                            jQuery.style(elem, type, value, extra);
-                    }, type, chainable ? margin : undefined, chainable);
-                };
-            });
+                        // Set width or height on the element
+                        jQuery.style(elem, type, value, extra);
+                }, type, chainable ? margin : undefined, chainable);
+            };
+        });
     });
 
 
     jQuery.each([
         "ajaxStart",
         "ajaxStop",
         "ajaxComplete",
@@ -10817,26 +10820,28 @@
         },
 
         hover: function(fnOver, fnOut) {
             return this.mouseenter(fnOver).mouseleave(fnOut || fnOver);
         }
     });
 
-    jQuery.each(("blur focus focusin focusout resize scroll click dblclick " +
+    jQuery.each(
+        ("blur focus focusin focusout resize scroll click dblclick " +
             "mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave " +
             "change select submit keydown keypress keyup contextmenu").split(" "),
         function(_i, name) {
 
             // Handle event binding
             jQuery.fn[name] = function(data, fn) {
                 return arguments.length > 0 ?
                     this.on(name, null, data, fn) :
                     this.trigger(name);
             };
-        });
+        }
+    );
 
 
 
 
     // Support: Android <=4.0 only
     // Make sure we trim BOM and NBSP
     var rtrim = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/jquery.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/jquery.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! jQuery v3.5.1 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+/*! jQuery v3.6.0 | (c) OpenJS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
     "use strict";
     "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
         if (!e.document) throw new Error("jQuery requires a window with a document");
         return t(e)
     } : t(e)
 }("undefined" != typeof window ? window : this, function(C, e) {
     "use strict";
@@ -19,15 +19,15 @@
         n = {},
         o = n.toString,
         v = n.hasOwnProperty,
         a = v.toString,
         l = a.call(Object),
         y = {},
         m = function(e) {
-            return "function" == typeof e && "number" != typeof e.nodeType
+            return "function" == typeof e && "number" != typeof e.nodeType && "function" != typeof e.item
         },
         x = function(e) {
             return null != e && e === e.window
         },
         E = C.document,
         c = {
             type: !0,
@@ -42,15 +42,15 @@
             for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
         n.head.appendChild(o).parentNode.removeChild(o)
     }
 
     function w(e) {
         return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
     }
-    var f = "3.5.1",
+    var f = "3.6.0",
         S = function(e, t) {
             return new S.fn.init(e, t)
         };
 
     function p(e) {
         var t = !!e && "length" in e && e.length,
             n = w(e);
@@ -182,18 +182,18 @@
             p = n.document,
             k = 0,
             r = 0,
             m = ue(),
             x = ue(),
             A = ue(),
             N = ue(),
-            D = function(e, t) {
+            j = function(e, t) {
                 return e === t && (l = !0), 0
             },
-            j = {}.hasOwnProperty,
+            D = {}.hasOwnProperty,
             t = [],
             q = t.pop,
             L = t.push,
             H = t.push,
             O = t.slice,
             P = function(e, t) {
                 for (var n = 0, r = e.length; n < r; n++)
@@ -360,16 +360,16 @@
             })
         }
 
         function ye(e) {
             return e && "undefined" != typeof e.getElementsByTagName && e
         }
         for (e in d = se.support = {}, i = se.isXML = function(e) {
-                var t = e.namespaceURI,
-                    n = (e.ownerDocument || e).documentElement;
+                var t = e && e.namespaceURI,
+                    n = e && (e.ownerDocument || e).documentElement;
                 return !Y.test(t || n && n.nodeName || "HTML")
             }, T = se.setDocument = function(e) {
                 var t, n, r = e ? e.ownerDocument || e : p;
                 return r != C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), p != C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.scope = ce(function(e) {
                     return a.appendChild(e).appendChild(C.createElement("div")), "undefined" != typeof e.querySelectorAll && !e.querySelectorAll(":scope fieldset div").length
                 }), d.attributes = ce(function(e) {
                     return e.className = "i", !e.getAttribute("className")
@@ -431,15 +431,15 @@
                         r = t && t.parentNode;
                     return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
                 } : function(e, t) {
                     if (t)
                         while (t = t.parentNode)
                             if (t === e) return !0;
                     return !1
-                }, D = t ? function(e, t) {
+                }, j = t ? function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
                     return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e == C || e.ownerDocument == p && y(p, e) ? -1 : t == C || t.ownerDocument == p && y(p, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
                 } : function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n, r = 0,
                         i = e.parentNode,
@@ -466,25 +466,25 @@
                 }
                 return 0 < se(t, C, null, [e]).length
             }, se.contains = function(e, t) {
                 return (e.ownerDocument || e) != C && T(e), y(e, t)
             }, se.attr = function(e, t) {
                 (e.ownerDocument || e) != C && T(e);
                 var n = b.attrHandle[t.toLowerCase()],
-                    r = n && j.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
+                    r = n && D.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
                 return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
             }, se.escape = function(e) {
                 return (e + "").replace(re, ie)
             }, se.error = function(e) {
                 throw new Error("Syntax error, unrecognized expression: " + e)
             }, se.uniqueSort = function(e) {
                 var t, n = [],
                     r = 0,
                     i = 0;
-                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(D), l) {
+                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(j), l) {
                     while (t = e[i++]) t === e[i] && (r = n.push(i));
                     while (r--) e.splice(n[r], 1)
                 }
                 return u = null, e
             }, o = se.getText = function(e) {
                 var t, n = "",
                     r = 0,
@@ -880,15 +880,15 @@
                     if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ye(t.parentNode) || t))) {
                         if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
                         break
                     }
                 }
             }
             return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-        }, d.sortStable = S.split("").sort(D).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
+        }, d.sortStable = S.split("").sort(j).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
             return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
         }), ce(function(e) {
             return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
         }) || fe("type|href|height|width", function(e, t, n) {
             if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
         }), d.attributes && ce(function(e) {
             return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
@@ -918,15 +918,15 @@
         k = S.expr.match.needsContext;
 
     function A(e, t) {
         return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
     }
     var N = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-    function D(e, n, r) {
+    function j(e, n, r) {
         return m(n) ? S.grep(e, function(e, t) {
             return !!n.call(e, t, e) !== r
         }) : n.nodeType ? S.grep(e, function(e) {
             return e === n !== r
         }) : "string" != typeof n ? S.grep(e, function(e) {
             return -1 < i.call(n, e) !== r
         }) : S.filter(n, e, r)
@@ -944,38 +944,38 @@
                 for (t = 0; t < r; t++)
                     if (S.contains(i[t], this)) return !0
             }));
             for (n = this.pushStack([]), t = 0; t < r; t++) S.find(e, i[t], n);
             return 1 < r ? S.uniqueSort(n) : n
         },
         filter: function(e) {
-            return this.pushStack(D(this, e || [], !1))
+            return this.pushStack(j(this, e || [], !1))
         },
         not: function(e) {
-            return this.pushStack(D(this, e || [], !0))
+            return this.pushStack(j(this, e || [], !0))
         },
         is: function(e) {
-            return !!D(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
+            return !!j(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
         }
     });
-    var j, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    var D, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
     (S.fn.init = function(e, t, n) {
         var r, i;
         if (!e) return this;
-        if (n = n || j, "string" == typeof e) {
+        if (n = n || D, "string" == typeof e) {
             if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : q.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
             if (r[1]) {
                 if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), N.test(r[1]) && S.isPlainObject(t))
                     for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
                 return this
             }
             return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
         }
         return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this)
-    }).prototype = S.fn, j = S(E);
+    }).prototype = S.fn, D = S(E);
     var L = /^(?:parents|prev(?:Until|All))/,
         H = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
@@ -1514,72 +1514,70 @@
             if (r && -1 < S.inArray(o, r)) i && i.push(o);
             else if (l = ie(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
             c = 0;
             while (o = a[c++]) he.test(o.type || "") && n.push(o)
         }
         return f
     }
-    var be = /^key/,
-        we = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        Te = /^([^.]*)(?:\.(.+)|)/;
+    var be = /^([^.]*)(?:\.(.+)|)/;
 
-    function Ce() {
+    function we() {
         return !0
     }
 
-    function Ee() {
+    function Te() {
         return !1
     }
 
-    function Se(e, t) {
+    function Ce(e, t) {
         return e === function() {
             try {
                 return E.activeElement
             } catch (e) {}
         }() == ("focus" === t)
     }
 
-    function ke(e, t, n, r, i, o) {
+    function Ee(e, t, n, r, i, o) {
         var a, s;
         if ("object" == typeof t) {
-            for (s in "string" != typeof n && (r = r || n, n = void 0), t) ke(e, s, n, r, t[s], o);
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ee(e, s, n, r, t[s], o);
             return e
         }
-        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Ee;
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Te;
         else if (!i) return e;
         return 1 === o && (a = i, (i = function(e) {
             return S().off(e), a.apply(this, arguments)
         }).guid = a.guid || (a.guid = S.guid++)), e.each(function() {
             S.event.add(this, t, i, r, n)
         })
     }
 
-    function Ae(e, i, o) {
+    function Se(e, i, o) {
         o ? (Y.set(e, i, !1), S.event.add(e, i, {
             namespace: !1,
             handler: function(e) {
                 var t, n, r = Y.get(this, i);
                 if (1 & e.isTrigger && this[i]) {
                     if (r.length)(S.event.special[i] || {}).delegateType && e.stopPropagation();
-                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
+                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n && n.value
                 } else r.length && (Y.set(this, i, {
                     value: S.event.trigger(S.extend(r[0], S.Event.prototype), r.slice(1), this)
                 }), e.stopImmediatePropagation())
             }
-        })) : void 0 === Y.get(e, i) && S.event.add(e, i, Ce)
+        })) : void 0 === Y.get(e, i) && S.event.add(e, i, we)
     }
     S.event = {
         global: {},
         add: function(t, e, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.get(t);
             if (V(t)) {
                 n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(re, i), n.guid || (n.guid = S.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(e) {
                     return "undefined" != typeof S && S.event.triggered !== e.type ? S.event.dispatch.apply(t, arguments) : void 0
                 }), l = (e = (e || "").match(P) || [""]).length;
-                while (l--) d = g = (s = Te.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
+                while (l--) d = g = (s = be.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
                     type: d,
                     origType: g,
                     data: r,
                     handler: n,
                     guid: n.guid,
                     selector: i,
                     needsContext: i && S.expr.match.needsContext.test(i),
@@ -1588,15 +1586,15 @@
             }
         },
         remove: function(e, t, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.hasData(e) && Y.get(e);
             if (v && (u = v.events)) {
                 l = (t = (t || "").match(P) || [""]).length;
                 while (l--)
-                    if (d = g = (s = Te.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                    if (d = g = (s = be.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
                         f = S.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
                         while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
                         a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || S.removeEvent(e, d, v.handle), delete u[d])
                     } else
                         for (d in u) S.event.remove(e, d + t[l], n, r, !0);
                 S.isEmptyObject(u) && Y.remove(e, "handle events")
             }
@@ -1658,19 +1656,19 @@
         special: {
             load: {
                 noBubble: !0
             },
             click: {
                 setup: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click", Ce), !1
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click", we), !1
                 },
                 trigger: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click"), !0
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click"), !0
                 },
                 _default: function(e) {
                     var t = e.target;
                     return pe.test(t.type) && t.click && A(t, "input") && Y.get(t, "click") || A(t, "a")
                 }
             },
             beforeunload: {
@@ -1679,32 +1677,32 @@
                 }
             }
         }
     }, S.removeEvent = function(e, t, n) {
         e.removeEventListener && e.removeEventListener(t, n)
     }, S.Event = function(e, t) {
         if (!(this instanceof S.Event)) return new S.Event(e, t);
-        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ce : Ee, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? we : Te, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
     }, S.Event.prototype = {
         constructor: S.Event,
-        isDefaultPrevented: Ee,
-        isPropagationStopped: Ee,
-        isImmediatePropagationStopped: Ee,
+        isDefaultPrevented: Te,
+        isPropagationStopped: Te,
+        isImmediatePropagationStopped: Te,
         isSimulated: !1,
         preventDefault: function() {
             var e = this.originalEvent;
-            this.isDefaultPrevented = Ce, e && !this.isSimulated && e.preventDefault()
+            this.isDefaultPrevented = we, e && !this.isSimulated && e.preventDefault()
         },
         stopPropagation: function() {
             var e = this.originalEvent;
-            this.isPropagationStopped = Ce, e && !this.isSimulated && e.stopPropagation()
+            this.isPropagationStopped = we, e && !this.isSimulated && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
             var e = this.originalEvent;
-            this.isImmediatePropagationStopped = Ce, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+            this.isImmediatePropagationStopped = we, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
         }
     }, S.each({
         altKey: !0,
         bubbles: !0,
         cancelable: !0,
         changedTouches: !0,
         ctrlKey: !0,
@@ -1729,28 +1727,28 @@
         pointerId: !0,
         pointerType: !0,
         screenX: !0,
         screenY: !0,
         targetTouches: !0,
         toElement: !0,
         touches: !0,
-        which: function(e) {
-            var t = e.button;
-            return null == e.which && be.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && we.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
-        }
+        which: !0
     }, S.event.addProp), S.each({
         focus: "focusin",
         blur: "focusout"
     }, function(e, t) {
         S.event.special[e] = {
             setup: function() {
-                return Ae(this, e, Se), !1
+                return Se(this, e, Ce), !1
             },
             trigger: function() {
-                return Ae(this, e), !0
+                return Se(this, e), !0
+            },
+            _default: function() {
+                return !0
             },
             delegateType: t
         }
     }), S.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
@@ -1763,95 +1761,95 @@
                 var t, n = e.relatedTarget,
                     r = e.handleObj;
                 return n && (n === this || S.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
             }
         }
     }), S.fn.extend({
         on: function(e, t, n, r) {
-            return ke(this, e, t, n, r)
+            return Ee(this, e, t, n, r)
         },
         one: function(e, t, n, r) {
-            return ke(this, e, t, n, r, 1)
+            return Ee(this, e, t, n, r, 1)
         },
         off: function(e, t, n) {
             var r, i;
             if (e && e.preventDefault && e.handleObj) return r = e.handleObj, S(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
             if ("object" == typeof e) {
                 for (i in e) this.off(i, t, e[i]);
                 return this
             }
-            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Ee), this.each(function() {
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Te), this.each(function() {
                 S.event.remove(this, e, n, t)
             })
         }
     });
-    var Ne = /<script|<style|<link/i,
-        De = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        je = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+    var ke = /<script|<style|<link/i,
+        Ae = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        Ne = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
-    function qe(e, t) {
+    function je(e, t) {
         return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
     }
 
-    function Le(e) {
+    function De(e) {
         return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
     }
 
-    function He(e) {
+    function qe(e) {
         return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
     }
 
-    function Oe(e, t) {
+    function Le(e, t) {
         var n, r, i, o, a, s;
         if (1 === t.nodeType) {
             if (Y.hasData(e) && (s = Y.get(e).events))
                 for (i in Y.remove(t, "handle events"), s)
                     for (n = 0, r = s[i].length; n < r; n++) S.event.add(t, i, s[i][n]);
             Q.hasData(e) && (o = Q.access(e), a = S.extend({}, o), Q.set(t, a))
         }
     }
 
-    function Pe(n, r, i, o) {
+    function He(n, r, i, o) {
         r = g(r);
         var e, t, a, s, u, l, c = 0,
             f = n.length,
             p = f - 1,
             d = r[0],
             h = m(d);
-        if (h || 1 < f && "string" == typeof d && !y.checkClone && De.test(d)) return n.each(function(e) {
+        if (h || 1 < f && "string" == typeof d && !y.checkClone && Ae.test(d)) return n.each(function(e) {
             var t = n.eq(e);
-            h && (r[0] = d.call(this, e, t.html())), Pe(t, r, i, o)
+            h && (r[0] = d.call(this, e, t.html())), He(t, r, i, o)
         });
         if (f && (t = (e = xe(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
-            for (s = (a = S.map(ve(e, "script"), Le)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
+            for (s = (a = S.map(ve(e, "script"), De)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
             if (s)
-                for (l = a[a.length - 1].ownerDocument, S.map(a, He), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
+                for (l = a[a.length - 1].ownerDocument, S.map(a, qe), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
                     nonce: u.nonce || u.getAttribute("nonce")
-                }, l) : b(u.textContent.replace(je, ""), u, l))
+                }, l) : b(u.textContent.replace(Ne, ""), u, l))
         }
         return n
     }
 
-    function Re(e, t, n) {
+    function Oe(e, t, n) {
         for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(ve(r)), r.parentNode && (n && ie(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
         return e
     }
     S.extend({
         htmlPrefilter: function(e) {
             return e
         },
         clone: function(e, t, n) {
             var r, i, o, a, s, u, l, c = e.cloneNode(!0),
                 f = ie(e);
             if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
                 for (a = ve(c), r = 0, i = (o = ve(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
             if (t)
                 if (n)
-                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Oe(o[r], a[r]);
-                else Oe(e, c);
+                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Le(o[r], a[r]);
+                else Le(e, c);
             return 0 < (a = ve(c, "script")).length && ye(a, !f && ve(e, "script")), c
         },
         cleanData: function(e) {
             for (var t, n, r, i = S.event.special, o = 0; void 0 !== (n = e[o]); o++)
                 if (V(n)) {
                     if (t = n[Y.expando]) {
                         if (t.events)
@@ -1859,46 +1857,46 @@
                         n[Y.expando] = void 0
                     }
                     n[Q.expando] && (n[Q.expando] = void 0)
                 }
         }
     }), S.fn.extend({
         detach: function(e) {
-            return Re(this, e, !0)
+            return Oe(this, e, !0)
         },
         remove: function(e) {
-            return Re(this, e)
+            return Oe(this, e)
         },
         text: function(e) {
             return $(this, function(e) {
                 return void 0 === e ? S.text(this) : this.empty().each(function() {
                     1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                 })
             }, null, e, arguments.length)
         },
         append: function() {
-            return Pe(this, arguments, function(e) {
-                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || qe(this, e).appendChild(e)
+            return He(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || je(this, e).appendChild(e)
             })
         },
         prepend: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var t = qe(this, e);
+                    var t = je(this, e);
                     t.insertBefore(e, t.firstChild)
                 }
             })
         },
         before: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this)
             })
         },
         after: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
             })
         },
         empty: function() {
             for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(ve(e, !1)), e.textContent = "");
             return this
         },
@@ -1909,27 +1907,27 @@
         },
         html: function(e) {
             return $(this, function(e) {
                 var t = this[0] || {},
                     n = 0,
                     r = this.length;
                 if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !Ne.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
+                if ("string" == typeof e && !ke.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
                     e = S.htmlPrefilter(e);
                     try {
                         for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(ve(t, !1)), t.innerHTML = e);
                         t = 0
                     } catch (e) {}
                 }
                 t && this.empty().append(e)
             }, null, e, arguments.length)
         },
         replaceWith: function() {
             var n = [];
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 var t = this.parentNode;
                 S.inArray(this, n) < 0 && (S.cleanData(ve(this)), t && t.replaceChild(e, this))
             }, n)
         }
     }), S.each({
         appendTo: "append",
         prependTo: "prepend",
@@ -1938,33 +1936,33 @@
         replaceAll: "replaceWith"
     }, function(e, a) {
         S.fn[e] = function(e) {
             for (var t, n = [], r = S(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), S(r[o])[a](t), u.apply(n, t.get());
             return this.pushStack(n)
         }
     });
-    var Me = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
-        Ie = function(e) {
+    var Pe = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
+        Re = function(e) {
             var t = e.ownerDocument.defaultView;
             return t && t.opener || (t = C), t.getComputedStyle(e)
         },
-        We = function(e, t, n) {
+        Me = function(e, t, n) {
             var r, i, o = {};
             for (i in t) o[i] = e.style[i], e.style[i] = t[i];
             for (i in r = n.call(e), t) e.style[i] = o[i];
             return r
         },
-        Fe = new RegExp(ne.join("|"), "i");
+        Ie = new RegExp(ne.join("|"), "i");
 
-    function Be(e, t, n) {
+    function We(e, t, n) {
         var r, i, o, a, s = e.style;
-        return (n = n || Ie(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Me.test(a) && Fe.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
+        return (n = n || Re(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Pe.test(a) && Ie.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
     }
 
-    function $e(e, t) {
+    function Fe(e, t) {
         return {
             get: function() {
                 if (!e()) return (this.get = t).apply(this, arguments);
                 delete this.get
             }
         }
     }! function() {
@@ -1995,79 +1993,79 @@
                 return e(), s
             },
             scrollboxSize: function() {
                 return e(), i
             },
             reliableTrDimensions: function() {
                 var e, t, n, r;
-                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px", t.style.height = "1px", n.style.height = "9px", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = 3 < parseInt(r.height), re.removeChild(e)), a
+                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = parseInt(r.height, 10) + parseInt(r.borderTopWidth, 10) + parseInt(r.borderBottomWidth, 10) === t.offsetHeight, re.removeChild(e)), a
             }
         }))
     }();
-    var _e = ["Webkit", "Moz", "ms"],
-        ze = E.createElement("div").style,
-        Ue = {};
-
-    function Xe(e) {
-        var t = S.cssProps[e] || Ue[e];
-        return t || (e in ze ? e : Ue[e] = function(e) {
+    var Be = ["Webkit", "Moz", "ms"],
+        $e = E.createElement("div").style,
+        _e = {};
+
+    function ze(e) {
+        var t = S.cssProps[e] || _e[e];
+        return t || (e in $e ? e : _e[e] = function(e) {
             var t = e[0].toUpperCase() + e.slice(1),
-                n = _e.length;
+                n = Be.length;
             while (n--)
-                if ((e = _e[n] + t) in ze) return e
+                if ((e = Be[n] + t) in $e) return e
         }(e) || e)
     }
-    var Ve = /^(none|table(?!-c[ea]).+)/,
-        Ge = /^--/,
-        Ye = {
+    var Ue = /^(none|table(?!-c[ea]).+)/,
+        Xe = /^--/,
+        Ve = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Qe = {
+        Ge = {
             letterSpacing: "0",
             fontWeight: "400"
         };
 
-    function Je(e, t, n) {
+    function Ye(e, t, n) {
         var r = te.exec(t);
         return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
     }
 
-    function Ke(e, t, n, r, i, o) {
+    function Qe(e, t, n, r, i, o) {
         var a = "width" === t ? 1 : 0,
             s = 0,
             u = 0;
         if (n === (r ? "border" : "content")) return 0;
         for (; a < 4; a += 2) "margin" === n && (u += S.css(e, n + ne[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + ne[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + ne[a] + "Width", !0, i))) : (u += S.css(e, "padding" + ne[a], !0, i), "padding" !== n ? u += S.css(e, "border" + ne[a] + "Width", !0, i) : s += S.css(e, "border" + ne[a] + "Width", !0, i));
         return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
     }
 
-    function Ze(e, t, n) {
-        var r = Ie(e),
+    function Je(e, t, n) {
+        var r = Re(e),
             i = (!y.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, r),
             o = i,
-            a = Be(e, t, r),
+            a = We(e, t, r),
             s = "offset" + t[0].toUpperCase() + t.slice(1);
-        if (Me.test(a)) {
+        if (Pe.test(a)) {
             if (!n) return a;
             a = "auto"
         }
-        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Ke(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Qe(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
     }
 
-    function et(e, t, n, r, i) {
-        return new et.prototype.init(e, t, n, r, i)
+    function Ke(e, t, n, r, i) {
+        return new Ke.prototype.init(e, t, n, r, i)
     }
     S.extend({
         cssHooks: {
             opacity: {
                 get: function(e, t) {
                     if (t) {
-                        var n = Be(e, "opacity");
+                        var n = We(e, "opacity");
                         return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
             animationIterationCount: !0,
@@ -2091,152 +2089,152 @@
             zIndex: !0,
             zoom: !0
         },
         cssProps: {},
         style: function(e, t, n, r) {
             if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
                 var i, o, a, s = X(t),
-                    u = Ge.test(t),
+                    u = Xe.test(t),
                     l = e.style;
-                if (u || (t = Xe(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                if (u || (t = ze(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
                 "string" === (o = typeof n) && (i = te.exec(n)) && i[1] && (n = se(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
             }
         },
         css: function(e, t, n, r) {
             var i, o, a, s = X(t);
-            return Ge.test(t) || (t = Xe(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Be(e, t, r)), "normal" === i && t in Qe && (i = Qe[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+            return Xe.test(t) || (t = ze(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = We(e, t, r)), "normal" === i && t in Ge && (i = Ge[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
         }
     }), S.each(["height", "width"], function(e, u) {
         S.cssHooks[u] = {
             get: function(e, t, n) {
-                if (t) return !Ve.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Ze(e, u, n) : We(e, Ye, function() {
-                    return Ze(e, u, n)
+                if (t) return !Ue.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Je(e, u, n) : Me(e, Ve, function() {
+                    return Je(e, u, n)
                 })
             },
             set: function(e, t, n) {
-                var r, i = Ie(e),
+                var r, i = Re(e),
                     o = !y.scrollboxSize() && "absolute" === i.position,
                     a = (o || n) && "border-box" === S.css(e, "boxSizing", !1, i),
-                    s = n ? Ke(e, u, n, a, i) : 0;
-                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Ke(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Je(0, t, s)
+                    s = n ? Qe(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Qe(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Ye(0, t, s)
             }
         }
-    }), S.cssHooks.marginLeft = $e(y.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(Be(e, "marginLeft")) || e.getBoundingClientRect().left - We(e, {
+    }), S.cssHooks.marginLeft = Fe(y.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(We(e, "marginLeft")) || e.getBoundingClientRect().left - Me(e, {
             marginLeft: 0
         }, function() {
             return e.getBoundingClientRect().left
         })) + "px"
     }), S.each({
         margin: "",
         padding: "",
         border: "Width"
     }, function(i, o) {
         S.cssHooks[i + o] = {
             expand: function(e) {
                 for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + ne[t] + o] = r[t] || r[t - 2] || r[0];
                 return n
             }
-        }, "margin" !== i && (S.cssHooks[i + o].set = Je)
+        }, "margin" !== i && (S.cssHooks[i + o].set = Ye)
     }), S.fn.extend({
         css: function(e, t) {
             return $(this, function(e, t, n) {
                 var r, i, o = {},
                     a = 0;
                 if (Array.isArray(t)) {
-                    for (r = Ie(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
+                    for (r = Re(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
                     return o
                 }
                 return void 0 !== n ? S.style(e, t, n) : S.css(e, t)
             }, e, t, 1 < arguments.length)
         }
-    }), ((S.Tween = et).prototype = {
-        constructor: et,
+    }), ((S.Tween = Ke).prototype = {
+        constructor: Ke,
         init: function(e, t, n, r, i, o) {
             this.elem = e, this.prop = n, this.easing = i || S.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (S.cssNumber[n] ? "" : "px")
         },
         cur: function() {
-            var e = et.propHooks[this.prop];
-            return e && e.get ? e.get(this) : et.propHooks._default.get(this)
+            var e = Ke.propHooks[this.prop];
+            return e && e.get ? e.get(this) : Ke.propHooks._default.get(this)
         },
         run: function(e) {
-            var t, n = et.propHooks[this.prop];
-            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : et.propHooks._default.set(this), this
+            var t, n = Ke.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : Ke.propHooks._default.set(this), this
         }
-    }).init.prototype = et.prototype, (et.propHooks = {
+    }).init.prototype = Ke.prototype, (Ke.propHooks = {
         _default: {
             get: function(e) {
                 var t;
                 return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = S.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
             },
             set: function(e) {
-                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[Xe(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
+                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[ze(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
             }
         }
-    }).scrollTop = et.propHooks.scrollLeft = {
+    }).scrollTop = Ke.propHooks.scrollLeft = {
         set: function(e) {
             e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
         }
     }, S.easing = {
         linear: function(e) {
             return e
         },
         swing: function(e) {
             return .5 - Math.cos(e * Math.PI) / 2
         },
         _default: "swing"
-    }, S.fx = et.prototype.init, S.fx.step = {};
-    var tt, nt, rt, it, ot = /^(?:toggle|show|hide)$/,
-        at = /queueHooks$/;
+    }, S.fx = Ke.prototype.init, S.fx.step = {};
+    var Ze, et, tt, nt, rt = /^(?:toggle|show|hide)$/,
+        it = /queueHooks$/;
 
-    function st() {
-        nt && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(st) : C.setTimeout(st, S.fx.interval), S.fx.tick())
+    function ot() {
+        et && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(ot) : C.setTimeout(ot, S.fx.interval), S.fx.tick())
     }
 
-    function ut() {
+    function at() {
         return C.setTimeout(function() {
-            tt = void 0
-        }), tt = Date.now()
+            Ze = void 0
+        }), Ze = Date.now()
     }
 
-    function lt(e, t) {
+    function st(e, t) {
         var n, r = 0,
             i = {
                 height: e
             };
         for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = ne[r])] = i["padding" + n] = e;
         return t && (i.opacity = i.width = e), i
     }
 
-    function ct(e, t, n) {
-        for (var r, i = (ft.tweeners[t] || []).concat(ft.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+    function ut(e, t, n) {
+        for (var r, i = (lt.tweeners[t] || []).concat(lt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
             if (r = i[o].call(n, t, e)) return r
     }
 
-    function ft(o, e, t) {
+    function lt(o, e, t) {
         var n, a, r = 0,
-            i = ft.prefilters.length,
+            i = lt.prefilters.length,
             s = S.Deferred().always(function() {
                 delete u.elem
             }),
             u = function() {
                 if (a) return !1;
-                for (var e = tt || ut(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                for (var e = Ze || at(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
                 return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
             },
             l = s.promise({
                 elem: o,
                 props: S.extend({}, e),
                 opts: S.extend(!0, {
                     specialEasing: {},
                     easing: S.easing._default
                 }, t),
                 originalProperties: e,
                 originalOptions: t,
-                startTime: tt || ut(),
+                startTime: Ze || at(),
                 duration: t.duration,
                 tweens: [],
                 createTween: function(e, t) {
                     var n = S.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
                     return l.tweens.push(n), n
                 },
                 stop: function(e) {
@@ -2251,31 +2249,31 @@
         for (! function(e, t) {
                 var n, r, i, o, a;
                 for (n in e)
                     if (i = t[r = X(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
                         for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
                     else t[r] = i
             }(c, l.opts.specialEasing); r < i; r++)
-            if (n = ft.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
-        return S.map(c, ct, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
+            if (n = lt.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return S.map(c, ut, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
             elem: o,
             anim: l,
             queue: l.opts.queue
         })), l
     }
-    S.Animation = S.extend(ft, {
+    S.Animation = S.extend(lt, {
         tweeners: {
             "*": [function(e, t) {
                 var n = this.createTween(e, t);
                 return se(n.elem, e, te.exec(t), n), n
             }]
         },
         tweener: function(e, t) {
             m(e) ? (t = e, e = ["*"]) : e = e.match(P);
-            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], ft.tweeners[n] = ft.tweeners[n] || [], ft.tweeners[n].unshift(t)
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], lt.tweeners[n] = lt.tweeners[n] || [], lt.tweeners[n].unshift(t)
         },
         prefilters: [function(e, t, n) {
             var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
                 p = this,
                 d = {},
                 h = e.style,
                 g = e.nodeType && ae(e),
@@ -2283,33 +2281,33 @@
             for (r in n.queue || (null == (a = S._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
                     a.unqueued || s()
                 }), a.unqueued++, p.always(function() {
                     p.always(function() {
                         a.unqueued--, S.queue(e, "fx").length || a.empty.fire()
                     })
                 })), t)
-                if (i = t[r], ot.test(i)) {
+                if (i = t[r], rt.test(i)) {
                     if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
                         if ("show" !== i || !v || void 0 === v[r]) continue;
                         g = !0
                     }
                     d[r] = v && v[r] || S.style(e, r)
                 } if ((u = !S.isEmptyObject(t)) || !S.isEmptyObject(d))
                 for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Y.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (le([e], !0), l = e.style.display || l, c = S.css(e, "display"), le([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done(function() {
                         h.display = l
                     }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
                         h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
                     })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Y.access(e, "fxshow", {
                     display: l
                 }), o && (v.hidden = !g), g && le([e], !0), p.done(function() {
                     for (r in g || le([e]), Y.remove(e, "fxshow"), d) S.style(e, r, d[r])
-                })), u = ct(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+                })), u = ut(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
         }],
         prefilter: function(e, t) {
-            t ? ft.prefilters.unshift(e) : ft.prefilters.push(e)
+            t ? lt.prefilters.unshift(e) : lt.prefilters.push(e)
         }
     }), S.speed = function(e, t, n) {
         var r = e && "object" == typeof e ? S.extend({}, e) : {
             complete: n || !n && t || m(e) && e,
             duration: e,
             easing: n && t || t && !m(t) && t
         };
@@ -2322,15 +2320,15 @@
                 opacity: t
             }, e, n, r)
         },
         animate: function(t, e, n, r) {
             var i = S.isEmptyObject(t),
                 o = S.speed(e, n, r),
                 a = function() {
-                    var e = ft(this, S.extend({}, t), o);
+                    var e = lt(this, S.extend({}, t), o);
                     (i || Y.get(this, "finish")) && e.stop(!0)
                 };
             return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
         },
         stop: function(i, e, o) {
             var a = function(e) {
                 var t = e.stop;
@@ -2339,15 +2337,15 @@
             return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
                 var e = !0,
                     t = null != i && i + "queueHooks",
                     n = S.timers,
                     r = Y.get(this);
                 if (t) r[t] && r[t].stop && a(r[t]);
                 else
-                    for (t in r) r[t] && r[t].stop && at.test(t) && a(r[t]);
+                    for (t in r) r[t] && r[t].stop && it.test(t) && a(r[t]);
                 for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
                 !e && o || S.dequeue(this, i)
             })
         },
         finish: function(a) {
             return !1 !== a && (a = a || "fx"), this.each(function() {
                 var e, t = Y.get(this),
@@ -2359,20 +2357,20 @@
                 for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
                 delete t.finish
             })
         }
     }), S.each(["toggle", "show", "hide"], function(e, r) {
         var i = S.fn[r];
         S.fn[r] = function(e, t, n) {
-            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(lt(r, !0), e, t, n)
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(st(r, !0), e, t, n)
         }
     }), S.each({
-        slideDown: lt("show"),
-        slideUp: lt("hide"),
-        slideToggle: lt("toggle"),
+        slideDown: st("show"),
+        slideUp: st("hide"),
+        slideToggle: st("toggle"),
         fadeIn: {
             opacity: "show"
         },
         fadeOut: {
             opacity: "hide"
         },
         fadeToggle: {
@@ -2381,48 +2379,48 @@
     }, function(e, r) {
         S.fn[e] = function(e, t, n) {
             return this.animate(r, e, t, n)
         }
     }), S.timers = [], S.fx.tick = function() {
         var e, t = 0,
             n = S.timers;
-        for (tt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-        n.length || S.fx.stop(), tt = void 0
+        for (Ze = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || S.fx.stop(), Ze = void 0
     }, S.fx.timer = function(e) {
         S.timers.push(e), S.fx.start()
     }, S.fx.interval = 13, S.fx.start = function() {
-        nt || (nt = !0, st())
+        et || (et = !0, ot())
     }, S.fx.stop = function() {
-        nt = null
+        et = null
     }, S.fx.speeds = {
         slow: 600,
         fast: 200,
         _default: 400
     }, S.fn.delay = function(r, e) {
         return r = S.fx && S.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
             var n = C.setTimeout(e, r);
             t.stop = function() {
                 C.clearTimeout(n)
             }
         })
-    }, rt = E.createElement("input"), it = E.createElement("select").appendChild(E.createElement("option")), rt.type = "checkbox", y.checkOn = "" !== rt.value, y.optSelected = it.selected, (rt = E.createElement("input")).value = "t", rt.type = "radio", y.radioValue = "t" === rt.value;
-    var pt, dt = S.expr.attrHandle;
+    }, tt = E.createElement("input"), nt = E.createElement("select").appendChild(E.createElement("option")), tt.type = "checkbox", y.checkOn = "" !== tt.value, y.optSelected = nt.selected, (tt = E.createElement("input")).value = "t", tt.type = "radio", y.radioValue = "t" === tt.value;
+    var ct, ft = S.expr.attrHandle;
     S.fn.extend({
         attr: function(e, t) {
             return $(this, S.attr, e, t, 1 < arguments.length)
         },
         removeAttr: function(e) {
             return this.each(function() {
                 S.removeAttr(this, e)
             })
         }
     }), S.extend({
         attr: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? pt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? ct : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
         },
         attrHooks: {
             type: {
                 set: function(e, t) {
                     if (!y.radioValue && "radio" === t && A(e, "input")) {
                         var n = e.value;
                         return e.setAttribute("type", t), n && (e.value = n), t
@@ -2432,37 +2430,37 @@
         },
         removeAttr: function(e, t) {
             var n, r = 0,
                 i = t && t.match(P);
             if (i && 1 === e.nodeType)
                 while (n = i[r++]) e.removeAttribute(n)
         }
-    }), pt = {
+    }), ct = {
         set: function(e, t, n) {
             return !1 === t ? S.removeAttr(e, n) : e.setAttribute(n, n), n
         }
     }, S.each(S.expr.match.bool.source.match(/\w+/g), function(e, t) {
-        var a = dt[t] || S.find.attr;
-        dt[t] = function(e, t, n) {
+        var a = ft[t] || S.find.attr;
+        ft[t] = function(e, t, n) {
             var r, i, o = t.toLowerCase();
-            return n || (i = dt[o], dt[o] = r, r = null != a(e, t, n) ? o : null, dt[o] = i), r
+            return n || (i = ft[o], ft[o] = r, r = null != a(e, t, n) ? o : null, ft[o] = i), r
         }
     });
-    var ht = /^(?:input|select|textarea|button)$/i,
-        gt = /^(?:a|area)$/i;
+    var pt = /^(?:input|select|textarea|button)$/i,
+        dt = /^(?:a|area)$/i;
 
-    function vt(e) {
+    function ht(e) {
         return (e.match(P) || []).join(" ")
     }
 
-    function yt(e) {
+    function gt(e) {
         return e.getAttribute && e.getAttribute("class") || ""
     }
 
-    function mt(e) {
+    function vt(e) {
         return Array.isArray(e) ? e : "string" == typeof e && e.match(P) || []
     }
     S.fn.extend({
         prop: function(e, t) {
             return $(this, S.prop, e, t, 1 < arguments.length)
         },
         removeProp: function(e) {
@@ -2475,15 +2473,15 @@
             var r, i, o = e.nodeType;
             if (3 !== o && 8 !== o && 2 !== o) return 1 === o && S.isXMLDoc(e) || (t = S.propFix[t] || t, i = S.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
         },
         propHooks: {
             tabIndex: {
                 get: function(e) {
                     var t = S.find.attr(e, "tabindex");
-                    return t ? parseInt(t, 10) : ht.test(e.nodeName) || gt.test(e.nodeName) && e.href ? 0 : -1
+                    return t ? parseInt(t, 10) : pt.test(e.nodeName) || dt.test(e.nodeName) && e.href ? 0 : -1
                 }
             }
         },
         propFix: {
             "for": "htmlFor",
             "class": "className"
         }
@@ -2498,77 +2496,77 @@
         }
     }), S.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
         S.propFix[this.toLowerCase()] = this
     }), S.fn.extend({
         addClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).addClass(t.call(this, e, yt(this)))
+                S(this).addClass(t.call(this, e, gt(this)))
             });
-            if ((e = mt(t)).length)
+            if ((e = vt(t)).length)
                 while (n = this[u++])
-                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
+                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
                         a = 0;
                         while (o = e[a++]) r.indexOf(" " + o + " ") < 0 && (r += o + " ");
-                        i !== (s = vt(r)) && n.setAttribute("class", s)
+                        i !== (s = ht(r)) && n.setAttribute("class", s)
                     } return this
         },
         removeClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).removeClass(t.call(this, e, yt(this)))
+                S(this).removeClass(t.call(this, e, gt(this)))
             });
             if (!arguments.length) return this.attr("class", "");
-            if ((e = mt(t)).length)
+            if ((e = vt(t)).length)
                 while (n = this[u++])
-                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
+                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
                         a = 0;
                         while (o = e[a++])
                             while (-1 < r.indexOf(" " + o + " ")) r = r.replace(" " + o + " ", " ");
-                        i !== (s = vt(r)) && n.setAttribute("class", s)
+                        i !== (s = ht(r)) && n.setAttribute("class", s)
                     } return this
         },
         toggleClass: function(i, t) {
             var o = typeof i,
                 a = "string" === o || Array.isArray(i);
             return "boolean" == typeof t && a ? t ? this.addClass(i) : this.removeClass(i) : m(i) ? this.each(function(e) {
-                S(this).toggleClass(i.call(this, e, yt(this), t), t)
+                S(this).toggleClass(i.call(this, e, gt(this), t), t)
             }) : this.each(function() {
                 var e, t, n, r;
                 if (a) {
-                    t = 0, n = S(this), r = mt(i);
+                    t = 0, n = S(this), r = vt(i);
                     while (e = r[t++]) n.hasClass(e) ? n.removeClass(e) : n.addClass(e)
-                } else void 0 !== i && "boolean" !== o || ((e = yt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
+                } else void 0 !== i && "boolean" !== o || ((e = gt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
             })
         },
         hasClass: function(e) {
             var t, n, r = 0;
             t = " " + e + " ";
             while (n = this[r++])
-                if (1 === n.nodeType && -1 < (" " + vt(yt(n)) + " ").indexOf(t)) return !0;
+                if (1 === n.nodeType && -1 < (" " + ht(gt(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var xt = /\r/g;
+    var yt = /\r/g;
     S.fn.extend({
         val: function(n) {
             var r, e, i, t = this[0];
             return arguments.length ? (i = m(n), this.each(function(e) {
                 var t;
                 1 === this.nodeType && (null == (t = i ? n.call(this, e, S(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = S.map(t, function(e) {
                     return null == e ? "" : e + ""
                 })), (r = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
-            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(xt, "") : null == e ? "" : e : void 0
+            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(yt, "") : null == e ? "" : e : void 0
         }
     }), S.extend({
         valHooks: {
             option: {
                 get: function(e) {
                     var t = S.find.attr(e, "value");
-                    return null != t ? t : vt(S.text(e))
+                    return null != t ? t : ht(S.text(e))
                 }
             },
             select: {
                 get: function(e) {
                     var t, n, r, i = e.options,
                         o = e.selectedIndex,
                         a = "select-one" === e.type,
@@ -2594,31 +2592,31 @@
             set: function(e, t) {
                 if (Array.isArray(t)) return e.checked = -1 < S.inArray(S(e).val(), t)
             }
         }, y.checkOn || (S.valHooks[this].get = function(e) {
             return null === e.getAttribute("value") ? "on" : e.value
         })
     }), y.focusin = "onfocusin" in C;
-    var bt = /^(?:focusinfocus|focusoutblur)$/,
-        wt = function(e) {
+    var mt = /^(?:focusinfocus|focusoutblur)$/,
+        xt = function(e) {
             e.stopPropagation()
         };
     S.extend(S.event, {
         trigger: function(e, t, n, r) {
             var i, o, a, s, u, l, c, f, p = [n || E],
                 d = v.call(e, "type") ? e.type : e,
                 h = v.call(e, "namespace") ? e.namespace.split(".") : [];
-            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !bt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !mt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
                 if (!r && !c.noBubble && !x(n)) {
-                    for (s = c.delegateType || d, bt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    for (s = c.delegateType || d, mt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
                     a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
                 }
                 i = 0;
                 while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Y.get(o, "events") || Object.create(null))[e.type] && Y.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && V(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
-                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, wt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, wt), S.event.triggered = void 0, a && (n[u] = a)), e.result
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, xt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, xt), S.event.triggered = void 0, a && (n[u] = a)), e.result
             }
         },
         simulate: function(e, t, n) {
             var r = S.extend(new S.Event, n, {
                 type: e,
                 isSimulated: !0
             });
@@ -2650,135 +2648,135 @@
             teardown: function() {
                 var e = this.ownerDocument || this.document || this,
                     t = Y.access(e, r) - 1;
                 t ? Y.access(e, r, t) : (e.removeEventListener(n, i, !0), Y.remove(e, r))
             }
         }
     });
-    var Tt = C.location,
-        Ct = {
+    var bt = C.location,
+        wt = {
             guid: Date.now()
         },
-        Et = /\?/;
+        Tt = /\?/;
     S.parseXML = function(e) {
-        var t;
+        var t, n;
         if (!e || "string" != typeof e) return null;
         try {
             t = (new C.DOMParser).parseFromString(e, "text/xml")
-        } catch (e) {
-            t = void 0
-        }
-        return t && !t.getElementsByTagName("parsererror").length || S.error("Invalid XML: " + e), t
+        } catch (e) {}
+        return n = t && t.getElementsByTagName("parsererror")[0], t && !n || S.error("Invalid XML: " + (n ? S.map(n.childNodes, function(e) {
+            return e.textContent
+        }).join("\n") : e)), t
     };
-    var St = /\[\]$/,
-        kt = /\r?\n/g,
-        At = /^(?:submit|button|image|reset|file)$/i,
-        Nt = /^(?:input|select|textarea|keygen)/i;
+    var Ct = /\[\]$/,
+        Et = /\r?\n/g,
+        St = /^(?:submit|button|image|reset|file)$/i,
+        kt = /^(?:input|select|textarea|keygen)/i;
 
-    function Dt(n, e, r, i) {
+    function At(n, e, r, i) {
         var t;
         if (Array.isArray(e)) S.each(e, function(e, t) {
-            r || St.test(n) ? i(n, t) : Dt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+            r || Ct.test(n) ? i(n, t) : At(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
         });
         else if (r || "object" !== w(e)) i(n, e);
         else
-            for (t in e) Dt(n + "[" + t + "]", e[t], r, i)
+            for (t in e) At(n + "[" + t + "]", e[t], r, i)
     }
     S.param = function(e, t) {
         var n, r = [],
             i = function(e, t) {
                 var n = m(t) ? t() : t;
                 r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
             };
         if (null == e) return "";
         if (Array.isArray(e) || e.jquery && !S.isPlainObject(e)) S.each(e, function() {
             i(this.name, this.value)
         });
         else
-            for (n in e) Dt(n, e[n], t, i);
+            for (n in e) At(n, e[n], t, i);
         return r.join("&")
     }, S.fn.extend({
         serialize: function() {
             return S.param(this.serializeArray())
         },
         serializeArray: function() {
             return this.map(function() {
                 var e = S.prop(this, "elements");
                 return e ? S.makeArray(e) : this
             }).filter(function() {
                 var e = this.type;
-                return this.name && !S(this).is(":disabled") && Nt.test(this.nodeName) && !At.test(e) && (this.checked || !pe.test(e))
+                return this.name && !S(this).is(":disabled") && kt.test(this.nodeName) && !St.test(e) && (this.checked || !pe.test(e))
             }).map(function(e, t) {
                 var n = S(this).val();
                 return null == n ? null : Array.isArray(n) ? S.map(n, function(e) {
                     return {
                         name: t.name,
-                        value: e.replace(kt, "\r\n")
+                        value: e.replace(Et, "\r\n")
                     }
                 }) : {
                     name: t.name,
-                    value: n.replace(kt, "\r\n")
+                    value: n.replace(Et, "\r\n")
                 }
             }).get()
         }
     });
-    var jt = /%20/g,
-        qt = /#.*$/,
-        Lt = /([?&])_=[^&]*/,
-        Ht = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        Ot = /^(?:GET|HEAD)$/,
-        Pt = /^\/\//,
-        Rt = {},
-        Mt = {},
-        It = "*/".concat("*"),
-        Wt = E.createElement("a");
+    var Nt = /%20/g,
+        jt = /#.*$/,
+        Dt = /([?&])_=[^&]*/,
+        qt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Lt = /^(?:GET|HEAD)$/,
+        Ht = /^\/\//,
+        Ot = {},
+        Pt = {},
+        Rt = "*/".concat("*"),
+        Mt = E.createElement("a");
 
-    function Ft(o) {
+    function It(o) {
         return function(e, t) {
             "string" != typeof e && (t = e, e = "*");
             var n, r = 0,
                 i = e.toLowerCase().match(P) || [];
             if (m(t))
                 while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
         }
     }
 
-    function Bt(t, i, o, a) {
+    function Wt(t, i, o, a) {
         var s = {},
-            u = t === Mt;
+            u = t === Pt;
 
         function l(e) {
             var r;
             return s[e] = !0, S.each(t[e] || [], function(e, t) {
                 var n = t(i, o, a);
                 return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
             }), r
         }
         return l(i.dataTypes[0]) || !s["*"] && l("*")
     }
 
-    function $t(e, t) {
+    function Ft(e, t) {
         var n, r, i = S.ajaxSettings.flatOptions || {};
         for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
         return r && S.extend(!0, e, r), e
     }
-    Wt.href = Tt.href, S.extend({
+    Mt.href = bt.href, S.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
-            url: Tt.href,
+            url: bt.href,
             type: "GET",
-            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),
+            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(bt.protocol),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": It,
+                "*": Rt,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
                 xml: /\bxml\b/,
@@ -2798,18 +2796,18 @@
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(e, t) {
-            return t ? $t($t(e, S.ajaxSettings), t) : $t(S.ajaxSettings, e)
+            return t ? Ft(Ft(e, S.ajaxSettings), t) : Ft(S.ajaxSettings, e)
         },
-        ajaxPrefilter: Ft(Rt),
-        ajaxTransport: Ft(Mt),
+        ajaxPrefilter: It(Ot),
+        ajaxTransport: It(Pt),
         ajax: function(e, t) {
             "object" == typeof e && (t = e, e = void 0), t = t || {};
             var c, f, p, n, d, r, h, g, i, o, v = S.ajaxSetup({}, t),
                 y = v.context || v,
                 m = v.context && (y.nodeType || y.jquery) ? S(y) : S.event,
                 x = S.Deferred(),
                 b = S.Callbacks("once memory"),
@@ -2820,15 +2818,15 @@
                 T = {
                     readyState: 0,
                     getResponseHeader: function(e) {
                         var t;
                         if (h) {
                             if (!n) {
                                 n = {};
-                                while (t = Ht.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
+                                while (t = qt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
                             }
                             t = n[e.toLowerCase() + " "]
                         }
                         return null == t ? null : t.join(", ")
                     },
                     getAllResponseHeaders: function() {
                         return h ? p : null
@@ -2848,26 +2846,26 @@
                         return this
                     },
                     abort: function(e) {
                         var t = e || u;
                         return c && c.abort(t), l(0, t), this
                     }
                 };
-            if (x.promise(T), v.url = ((e || v.url || Tt.href) + "").replace(Pt, Tt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
+            if (x.promise(T), v.url = ((e || v.url || bt.href) + "").replace(Ht, bt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
                 r = E.createElement("a");
                 try {
-                    r.href = v.url, r.href = r.href, v.crossDomain = Wt.protocol + "//" + Wt.host != r.protocol + "//" + r.host
+                    r.href = v.url, r.href = r.href, v.crossDomain = Mt.protocol + "//" + Mt.host != r.protocol + "//" + r.host
                 } catch (e) {
                     v.crossDomain = !0
                 }
             }
-            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Bt(Rt, v, t, T), h) return T;
-            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Ot.test(v.type), f = v.url.replace(qt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(jt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Et.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Lt, "$1"), o = (Et.test(f) ? "&" : "?") + "_=" + Ct.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + It + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
+            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Wt(Ot, v, t, T), h) return T;
+            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Lt.test(v.type), f = v.url.replace(jt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Nt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Tt.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Dt, "$1"), o = (Tt.test(f) ? "&" : "?") + "_=" + wt.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + Rt + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
             if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
-            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Bt(Mt, v, t, T)) {
+            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Wt(Pt, v, t, T)) {
                 if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
                 v.async && 0 < v.timeout && (d = C.setTimeout(function() {
                     T.abort("timeout")
                 }, v.timeout));
                 try {
                     h = !1, c.send(a, l)
                 } catch (e) {
@@ -2895,15 +2893,15 @@
                                 break
                             }
                             a || (a = i)
                         }
                         o = o || a
                     }
                     if (o) return o !== u[0] && u.unshift(o), n[o]
-                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
+                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && S.inArray("json", v.dataTypes) < 0 && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
                     var i, o, a, s, u, l = {},
                         c = e.dataTypes.slice();
                     if (c[1])
                         for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
                     o = c.shift();
                     while (o)
                         if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
@@ -3001,30 +2999,30 @@
     }, S.expr.pseudos.visible = function(e) {
         return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
     }, S.ajaxSettings.xhr = function() {
         try {
             return new C.XMLHttpRequest
         } catch (e) {}
     };
-    var _t = {
+    var Bt = {
             0: 200,
             1223: 204
         },
-        zt = S.ajaxSettings.xhr();
-    y.cors = !!zt && "withCredentials" in zt, y.ajax = zt = !!zt, S.ajaxTransport(function(i) {
+        $t = S.ajaxSettings.xhr();
+    y.cors = !!$t && "withCredentials" in $t, y.ajax = $t = !!$t, S.ajaxTransport(function(i) {
         var o, a;
-        if (y.cors || zt && !i.crossDomain) return {
+        if (y.cors || $t && !i.crossDomain) return {
             send: function(e, t) {
                 var n, r = i.xhr();
                 if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
                     for (n in i.xhrFields) r[n] = i.xhrFields[n];
                 for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
                 o = function(e) {
                     return function() {
-                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(_t[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Bt[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
                             binary: r.response
                         } : {
                             text: r.responseText
                         }, r.getAllResponseHeaders()))
                     }
                 }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
                     4 === r.readyState && C.setTimeout(function() {
@@ -3069,38 +3067,38 @@
                 }), E.head.appendChild(r[0])
             },
             abort: function() {
                 i && i()
             }
         }
     });
-    var Ut, Xt = [],
-        Vt = /(=)\?(?=&|$)|\?\?/;
+    var _t, zt = [],
+        Ut = /(=)\?(?=&|$)|\?\?/;
     S.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var e = Xt.pop() || S.expando + "_" + Ct.guid++;
+            var e = zt.pop() || S.expando + "_" + wt.guid++;
             return this[e] = !0, e
         }
     }), S.ajaxPrefilter("json jsonp", function(e, t, n) {
-        var r, i, o, a = !1 !== e.jsonp && (Vt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Vt.test(e.data) && "data");
-        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Vt, "$1" + r) : !1 !== e.jsonp && (e.url += (Et.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+        var r, i, o, a = !1 !== e.jsonp && (Ut.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Ut.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Ut, "$1" + r) : !1 !== e.jsonp && (e.url += (Tt.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
             return o || S.error(r + " was not called"), o[0]
         }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
             o = arguments
         }, n.always(function() {
-            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Xt.push(r)), o && m(i) && i(o[0]), o = i = void 0
+            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, zt.push(r)), o && m(i) && i(o[0]), o = i = void 0
         }), "script"
-    }), y.createHTMLDocument = ((Ut = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Ut.childNodes.length), S.parseHTML = function(e, t, n) {
+    }), y.createHTMLDocument = ((_t = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === _t.childNodes.length), S.parseHTML = function(e, t, n) {
         return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = N.exec(e)) ? [t.createElement(i[1])] : (i = xe([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
         var r, i, o
     }, S.fn.load = function(e, t, n) {
         var r, i, o, a = this,
             s = e.indexOf(" ");
-        return -1 < s && (r = vt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
+        return -1 < s && (r = ht(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
             url: e,
             type: i || "GET",
             dataType: "html",
             data: t
         }).done(function(e) {
             o = arguments, a.html(r ? S("<div>").append(S.parseHTML(e)).find(r) : e)
         }).always(n && function(e, t) {
@@ -3113,15 +3111,15 @@
             return t === e.elem
         }).length
     }, S.offset = {
         setOffset: function(e, t, n) {
             var r, i, o, a, s, u, l = S.css(e, "position"),
                 c = S(e),
                 f = {};
-            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : ("number" == typeof f.top && (f.top += "px"), "number" == typeof f.left && (f.left += "px"), c.css(f))
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
         }
     }, S.fn.extend({
         offset: function(t) {
             if (arguments.length) return void 0 === t ? this : this.each(function(e) {
                 S.offset.setOffset(this, t, e)
             });
             var e, n, r = this[0];
@@ -3168,16 +3166,16 @@
             return $(this, function(e, t, n) {
                 var r;
                 if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
                 r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
             }, t, e, arguments.length)
         }
     }), S.each(["top", "left"], function(e, n) {
-        S.cssHooks[n] = $e(y.pixelPosition, function(e, t) {
-            if (t) return t = Be(e, n), Me.test(t) ? S(e).position()[n] + "px" : t
+        S.cssHooks[n] = Fe(y.pixelPosition, function(e, t) {
+            if (t) return t = We(e, n), Pe.test(t) ? S(e).position()[n] + "px" : t
         })
     }), S.each({
         Height: "height",
         Width: "width"
     }, function(a, s) {
         S.each({
             padding: "inner" + a,
@@ -3214,29 +3212,29 @@
             return this.mouseenter(e).mouseleave(t || e)
         }
     }), S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
         S.fn[n] = function(e, t) {
             return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
         }
     });
-    var Gt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    var Xt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
     S.proxy = function(e, t) {
         var n, r, i;
         if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
             return e.apply(t || this, r.concat(s.call(arguments)))
         }).guid = e.guid = e.guid || S.guid++, i
     }, S.holdReady = function(e) {
         e ? S.readyWait++ : S.ready(!0)
     }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = A, S.isFunction = m, S.isWindow = x, S.camelCase = X, S.type = w, S.now = Date.now, S.isNumeric = function(e) {
         var t = S.type(e);
         return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
     }, S.trim = function(e) {
-        return null == e ? "" : (e + "").replace(Gt, "")
+        return null == e ? "" : (e + "").replace(Xt, "")
     }, "function" == typeof define && define.amd && define("jquery", [], function() {
         return S
     });
-    var Yt = C.jQuery,
-        Qt = C.$;
+    var Vt = C.jQuery,
+        Gt = C.$;
     return S.noConflict = function(e) {
-        return C.$ === S && (C.$ = Qt), e && C.jQuery === S && (C.jQuery = Yt), S
+        return C.$ === S && (C.$ = Gt), e && C.jQuery === S && (C.jQuery = Vt), S
     }, "undefined" == typeof e && (C.jQuery = C.$ = S), S
 });
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/badge_only.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/html5shiv-printshiv.min.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/html5shiv.min.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/js/theme.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/pygments.css` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/underscore-1.13.1.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/_static/underscore.js` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/genindex.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/genindex.html`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
@@ -131,18 +132,14 @@
 
 <h2 id="S">S</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="scripting/image_embedder.html#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.server_url">server_url (orangecontrib.imageanalytics.image_embedder.ImageEmbedder attribute)</a>
 </li>
   </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="scripting/image_embedder.html#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.set_canceled">set_canceled() (orangecontrib.imageanalytics.image_embedder.ImageEmbedder method)</a>
-</li>
-  </ul></td>
 </tr></table>
 
 
 
            </div>
           </div>
           <footer>
```

#### html2text {}

```diff
@@ -32,15 +32,14 @@
 ***** M *****
     * model_(orangecontrib.imageanalytics.image_embedder.ImageEmbedder
       attribute)
 ***** P *****
     * prepare_output_data()_
       (orangecontrib.imageanalytics.image_embedder.ImageEmbedder_static_method)
 ***** S *****
-    * server_url_                                                    * set_canceled()_
-      (orangecontrib.imageanalytics.image_embedder.ImageEmbedder       (orangecontrib.imageanalytics.image_embedder.ImageEmbedder
-      attribute)                                                       method)
+    * server_url_(orangecontrib.imageanalytics.image_embedder.ImageEmbedder
+      attribute)
 
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/index.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Welcome to Orange3 Image Analytics documentation! &mdash; Orange3 Image Analytics  documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Import Images" href="widgets/importimages.html" /> 
 </head>
 
@@ -68,45 +68,45 @@
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="welcome-to-orange3-image-analytics-documentation">
-<h1>Welcome to Orange3 Image Analytics documentation!<a class="headerlink" href="#welcome-to-orange3-image-analytics-documentation" title="Permalink to this headline"></a></h1>
-<section id="widgets">
-<h2>Widgets<a class="headerlink" href="#widgets" title="Permalink to this headline"></a></h2>
+  <div class="section" id="welcome-to-orange3-image-analytics-documentation">
+<h1>Welcome to Orange3 Image Analytics documentation!<a class="headerlink" href="#welcome-to-orange3-image-analytics-documentation" title="Permalink to this heading"></a></h1>
+<div class="section" id="widgets">
+<h2>Widgets<a class="headerlink" href="#widgets" title="Permalink to this heading"></a></h2>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="widgets/importimages.html">Import Images</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/imageviewer.html">Image Viewer</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/imageembedding.html">Image Embedding</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/imagegrid.html">Image Grid</a></li>
 <li class="toctree-l1"><a class="reference internal" href="widgets/saveimages.html">Save Images</a></li>
 </ul>
 </div>
-</section>
-<section id="scripting">
-<h2>Scripting<a class="headerlink" href="#scripting" title="Permalink to this headline"></a></h2>
+</div>
+<div class="section" id="scripting">
+<h2>Scripting<a class="headerlink" href="#scripting" title="Permalink to this heading"></a></h2>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="scripting/image_embedder.html">Image Embedding module</a></li>
 </ul>
 </div>
-</section>
-</section>
-<section id="indices-and-tables">
-<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this headline"></a></h1>
+</div>
+</div>
+<div class="section" id="indices-and-tables">
+<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
 <ul class="simple">
 <li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
 <li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
 <li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
 </ul>
-</section>
+</div>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="widgets/importimages.html" class="btn btn-neutral float-right" title="Import Images" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
```

#### html2text {}

```diff
@@ -21,18 +21,16 @@
 ****** Welcome to Orange3 Image Analytics documentation!ï ******
 ***** Widgetsï *****
     * Import_Images
     * Image_Viewer
     * Image_Embedding
     * Image_Grid
     * Save_Images
-
 ***** Scriptingï *****
     * Image_Embedding_module
-
 ****** Indices and tablesï ******
     * Index
     * Module_Index
     * Search_Page
 Next
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/scripting/image_embedder.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/scripting/image_embedder.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Image Embedding module &mdash; Orange3 Image Analytics  documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
+        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="prev" title="Save Images" href="../widgets/saveimages.html" /> 
 </head>
 
@@ -68,16 +68,16 @@
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="image-embedding-module">
-<h1>Image Embedding module<a class="headerlink" href="#image-embedding-module" title="Permalink to this headline"></a></h1>
+  <div class="section" id="image-embedding-module">
+<h1>Image Embedding module<a class="headerlink" href="#image-embedding-module" title="Permalink to this heading"></a></h1>
 <dl class="py class">
 <dt class="sig sig-object py" id="orangecontrib.imageanalytics.image_embedder.ImageEmbedder">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">orangecontrib.imageanalytics.image_embedder.</span></span><span class="sig-name descname"><span class="pre">ImageEmbedder</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">model</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'inception-v3'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">server_url</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'https://api.garaza.io/'</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder" title="Permalink to this definition"></a></dt>
 <dd><p>Client side functionality for accessing a remote image embedding backend.</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="orangecontrib.imageanalytics.image_embedder.ImageEmbedder.model">
 <span class="sig-name descname"><span class="pre">model</span></span><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.model" title="Permalink to this definition"></a></dt>
@@ -113,35 +113,32 @@
 <dd><p>Function clear cache for the selected embedder. If embedder is loaded
 cache is cleaned from its dict otherwise we load cache and clean it
 from file.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="orangecontrib.imageanalytics.image_embedder.ImageEmbedder.construct_output_data_table">
-<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">construct_output_data_table</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">embedded_images</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Orange.data.table.Table</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">embeddings_</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">numpy.ndarray</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Orange.data.table.Table</span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.construct_output_data_table"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.construct_output_data_table" title="Permalink to this definition"></a></dt>
+<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">construct_output_data_table</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">embedded_images</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Table</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">embeddings_</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ndarray</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Table</span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.construct_output_data_table"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.construct_output_data_table" title="Permalink to this definition"></a></dt>
 <dd><p>Join the orange table with embeddings.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>embedded_images</strong> – Table with images that were successfully embedded</p></li>
 <li><p><strong>embeddings</strong> – Embeddings for images from table</p></li>
 </ul>
 </dd>
-<dt class="field-even">Returns</dt>
-<dd class="field-even"><p></p>
-</dd>
-<dt class="field-odd">Return type</dt>
-<dd class="field-odd"><p>Table with added embeddings to data.</p>
+<dt class="field-even">Return type</dt>
+<dd class="field-even"><p>Table with added embeddings to data.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="orangecontrib.imageanalytics.image_embedder.ImageEmbedder.from_table">
-<span class="sig-name descname"><span class="pre">from_table</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Orange.data.table.Table</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">col</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Orange.data.variable.Variable</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'image'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">callback</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Orange.data.table.Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Orange.data.table.Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">int</span><span class="p"><span class="pre">]</span></span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.from_table"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.from_table" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">from_table</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Table</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">col</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Variable</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'image'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">callback</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">int</span><span class="p"><span class="pre">]</span></span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.from_table"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.from_table" title="Permalink to this definition"></a></dt>
 <dd><p>Calls embedding when data are provided as a Orange Table.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>data</strong> – Data table with image paths</p></li>
 <li><p><strong>col</strong> – The column with image paths</p></li>
 <li><p><strong>callback</strong> – Optional callback - function that is called for every embedded
@@ -155,15 +152,15 @@
 <dt class="sig sig-object py" id="orangecontrib.imageanalytics.image_embedder.ImageEmbedder.is_local_embedder">
 <span class="sig-name descname"><span class="pre">is_local_embedder</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.is_local_embedder"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.is_local_embedder" title="Permalink to this definition"></a></dt>
 <dd><p>Tells whether selected embedder is local or not.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="orangecontrib.imageanalytics.image_embedder.ImageEmbedder.prepare_output_data">
-<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">prepare_output_data</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">input_data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Orange.data.table.Table</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">embeddings_</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">float</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Orange.data.table.Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Orange.data.table.Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">int</span><span class="p"><span class="pre">]</span></span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.prepare_output_data"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.prepare_output_data" title="Permalink to this definition"></a></dt>
+<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">prepare_output_data</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">input_data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Table</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">embeddings_</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">float</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Table</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">int</span><span class="p"><span class="pre">]</span></span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.prepare_output_data"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.prepare_output_data" title="Permalink to this definition"></a></dt>
 <dd><p>Prepare output data when data table on input.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>input_data</strong> – The table with original data that are joined with embeddings</p></li>
 <li><p><strong>embeddings</strong> – List with embeddings</p></li>
 </ul>
@@ -174,23 +171,17 @@
 <li><p><em>table with skipped images and third the number of skipped images.</em></p></li>
 </ul>
 </p>
 </dd>
 </dl>
 </dd></dl>
 
-<dl class="py method">
-<dt class="sig sig-object py" id="orangecontrib.imageanalytics.image_embedder.ImageEmbedder.set_canceled">
-<span class="sig-name descname"><span class="pre">set_canceled</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="reference internal" href="../_modules/orangecontrib/imageanalytics/image_embedder.html#ImageEmbedder.set_canceled"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#orangecontrib.imageanalytics.image_embedder.ImageEmbedder.set_canceled" title="Permalink to this definition"></a></dt>
-<dd><p>Cancel the embedding</p>
 </dd></dl>
 
-</dd></dl>
-
-</section>
+</div>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="../widgets/saveimages.html" class="btn btn-neutral float-left" title="Save Images" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
     </div>
```

#### html2text {}

```diff
@@ -37,51 +37,44 @@
       >>> table = Orange.data.Table('Table_with_image_path.csv')
       >>> with ImageEmbedder(model='model_name') as emb:
       ...    embeddings = emb(table, col="image_path_column")
         clear_cache() &#x2192; None[source]ï
             Function clear cache for the selected embedder. If embedder is
             loaded cache is cleaned from its dict otherwise we load cache and
             clean it from file.
-        staticconstruct_output_data_table(embedded_images:
-        Orange.data.table.Table, embeddings_: numpy.ndarray) &#x2192;
-        Orange.data.table.Table[source]ï
+        staticconstruct_output_data_table(embedded_images: Table, embeddings_:
+        ndarray) &#x2192; Table[source]ï
             Join the orange table with embeddings.
               Parameters
                       * embedded_images â Table with images that were
                         successfully embedded
                       * embeddings â Embeddings for images from table
-              Returns
               Return type
                   Table with added embeddings to data.
-        from_table(data: Orange.data.table.Table, col: Union[str,
-        Orange.data.variable.Variable] = 'image', callback: Optional[Callable]
-        = None) &#x2192; Tuple[Orange.data.table.Table,
-        Orange.data.table.Table, int][source]ï
+        from_table(data: Table, col: Union[str, Variable] = 'image', callback:
+        Optional[Callable] = None) &#x2192; Tuple[Table, Table, int][source]ï
             Calls embedding when data are provided as a Orange Table.
               Parameters
                       * data â Data table with image paths
                       * col â The column with image paths
                       * callback â Optional callback - function that is
                         called for every embedded image and is used to report
                         the progress.
         is_local_embedder() &#x2192; bool[source]ï
             Tells whether selected embedder is local or not.
-        staticprepare_output_data(input_data: Orange.data.table.Table,
-        embeddings_: List[List[float]]) &#x2192; Tuple[Orange.data.table.Table,
-        Orange.data.table.Table, int][source]ï
+        staticprepare_output_data(input_data: Table, embeddings_: List[List
+        [float]]) &#x2192; Tuple[Table, Table, int][source]ï
             Prepare output data when data table on input.
               Parameters
                       * input_data â The table with original data that are
                         joined with embeddings
                       * embeddings â List with embeddings
               Returns
                       * Tuple where first parameter is table with embedded
                         images, the second
                       * table with skipped images and third the number of
                         skipped images.
-        set_canceled() &#x2192; None[source]ï
-            Cancel the embedding
 Previous
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/search.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" /> 
 </head>
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/imageembedding.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/imageembedding.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Image Embedding &mdash; Orange3 Image Analytics  documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
+        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Image Grid" href="imagegrid.html" />
     <link rel="prev" title="Image Viewer" href="imageviewer.html" /> 
 </head>
@@ -73,16 +73,16 @@
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="image-embedding">
-<h1>Image Embedding<a class="headerlink" href="#image-embedding" title="Permalink to this headline"></a></h1>
+  <div class="section" id="image-embedding">
+<h1>Image Embedding<a class="headerlink" href="#image-embedding" title="Permalink to this heading"></a></h1>
 <p>Image embedding through deep neural networks.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Images: List of images.</p></li>
 </ul>
 <p><strong>Outputs</strong></p>
 <ul class="simple">
@@ -110,32 +110,32 @@
 </ul>
 </li>
 </ul>
 </li>
 <li><p>Tick the box on the left to start the embedding automatically. Alternatively, click <em>Apply</em>. To cancel the embedding, click <em>Cancel</em>.</p></li>
 <li><p>Access help.</p></li>
 </ol>
-<section id="embedders">
-<h2>Embedders<a class="headerlink" href="#embedders" title="Permalink to this headline"></a></h2>
+<div class="section" id="embedders">
+<h2>Embedders<a class="headerlink" href="#embedders" title="Permalink to this heading"></a></h2>
 <p><strong>InceptionV3</strong> is Google’s deep neural network for image recognition. It is trained on the ImageNet data set. The model we are using is available <a class="reference external" href="http://download.tensorflow.org/models/image/imagenet/inception-2015-12-05.tgz">here</a>. For the embedding, we use the activations of the penultimate layer of the model, which represents images with vectors.</p>
 <p><strong>SqueezeNet</strong> is a deep model for image recognition that achieves AlexNet-level accuracy on ImageNet with 50x fewer parameters. The model is trained on the ImageNet dataset. We re-implemented the SqueezeNet by using weights from the <a class="reference external" href="https://github.com/DeepScale/SqueezeNet">author’s pretrained model</a>. We use activations from pre-softmax (<code class="docutils literal notranslate"><span class="pre">flatten10</span></code>) layer as an embedding.</p>
 <p><strong>VGG16</strong> and <strong>VGG19</strong> are deep neural networks for image recognition proposed by Visual Geometry Group from the University of Oxford. They are trained on the ImageNet data set. We use a <a class="reference external" href="https://github.com/machrisaa/tensorflow-vgg">community implementation</a> of networks with original weights. As an embedding, we use activations of the penultimate layer - <code class="docutils literal notranslate"><span class="pre">fc7</span></code>.</p>
 <p>Image Embedding also includes <a class="reference external" href="https://github.com/inejc/painters"><strong>Painters</strong></a>, an embedder that was trained on 79,433 images of paintings by 1,584 painters and won Kaggle’s Painter by Numbers competition. Activations of the penultimate layer of the network are used as an embedding.</p>
 <p><strong>DeepLoc</strong> is a convolutional network trained on 21,882 images of single cells that were manually assigned to one of 15 localization compartments. We use the pre-trained network proposed by <a class="reference external" href="https://github.com/okraus/DeepLoc">authors</a>. The embeddings are activations of penultimate layer <code class="docutils literal notranslate"><span class="pre">fc_2</span></code>.</p>
 <p>An <a class="reference external" href="https://www.nature.com/articles/s41467-019-12397-x">article</a> by Godec et al. (2019) explains how the embeddings work and how to use it in Orange.</p>
-</section>
-<section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline"></a></h2>
+</div>
+<div class="section" id="example">
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
 <p>Let us first import images from a folder with <a class="reference internal" href="importimages.html"><span class="doc">Import Images</span></a>. We have three images of an orange, a banana and a strawberry in a folder called Fruits. From <strong>Import Images</strong> we will send a data table containing a column with image paths to <strong>Image Embedding</strong>.</p>
 <p>We will use the default embedder <em>SqueezeNet</em>. The widget will automatically start retrieving image vectors from the server.</p>
 <p><img alt="../_images/ImageEmbedding-Example1.png" src="../_images/ImageEmbedding-Example1.png" /></p>
 <p>Once the computation is done, you can observe the enhanced data in a <strong>Data Table</strong>. With the retrieved embeddings, you can continue with any machine learning method Orange offers. Below is an example for clustering.</p>
 <p><img alt="../_images/ImageEmbedding-Example2.png" src="../_images/ImageEmbedding-Example2.png" /></p>
-</section>
-</section>
+</div>
+</div>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="imageviewer.html" class="btn btn-neutral float-left" title="Image Viewer" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="imagegrid.html" class="btn btn-neutral float-right" title="Image Grid" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
```

#### html2text {}

```diff
@@ -79,26 +79,24 @@
 embedding.
 DeepLoc is a convolutional network trained on 21,882 images of single cells
 that were manually assigned to one of 15 localization compartments. We use the
 pre-trained network proposed by authors. The embeddings are activations of
 penultimate layer fc_2.
 An article by Godec et al. (2019) explains how the embeddings work and how to
 use it in Orange.
-
 ***** Exampleï *****
 Let us first import images from a folder with Import_Images. We have three
 images of an orange, a banana and a strawberry in a folder called Fruits. From
 Import Images we will send a data table containing a column with image paths to
 Image Embedding.
 We will use the default embedder SqueezeNet. The widget will automatically
 start retrieving image vectors from the server.
 [../_images/ImageEmbedding-Example1.png]
 Once the computation is done, you can observe the enhanced data in a Data
 Table. With the retrieved embeddings, you can continue with any machine
 learning method Orange offers. Below is an example for clustering.
 [../_images/ImageEmbedding-Example2.png]
-
 Previous Next
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/imagegrid.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/imagegrid.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Image Grid &mdash; Orange3 Image Analytics  documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
+        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Save Images" href="saveimages.html" />
     <link rel="prev" title="Image Embedding" href="imageembedding.html" /> 
 </head>
@@ -72,16 +72,16 @@
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="image-grid">
-<h1>Image Grid<a class="headerlink" href="#image-grid" title="Permalink to this headline"></a></h1>
+  <div class="section" id="image-grid">
+<h1>Image Grid<a class="headerlink" href="#image-grid" title="Permalink to this heading"></a></h1>
 <p>Displays images in a similarity grid.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Embeddings: Image embeddings from Image Embedding widget.</p></li>
 <li><p>Data Subset: A subset of embeddings or images.</p></li>
 </ul>
 <p><strong>Outputs</strong></p>
@@ -95,22 +95,22 @@
 <li><p><em>Image Filename Attribute</em>: Attribute containing paths to images.</p></li>
 <li><p><em>Image cell fit</em>: Resize scales the images to grid, while Crop crops them to squares.</p></li>
 <li><p><em>Grid size</em>: Set the size of the grid. Click <em>Set size automatically</em> to optimize the projection.</p></li>
 <li><p>Tick the box to commit the changes automatically. Alternatively, click <em>Apply</em>.</p></li>
 <li><p>Information on the input.</p></li>
 <li><p>Access help, save image, and report (in that order).</p></li>
 </ol>
-<section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline"></a></h2>
+<div class="section" id="example">
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
 <p><strong>Image Grid</strong> can be used to visualize similarity of images in a 2D projection. We have used 5 images of fruits and vegetables, namely orange, banana, strawberry, broccoli and cauliflower.</p>
 <p>We loaded the images with <a class="reference internal" href="importimages.html"><span class="doc">Import Images</span></a> and embedded them with Inception v3 embedder in <a class="reference internal" href="imageembedding.html"><span class="doc">Image Embedding</span></a>.</p>
 <p>Finally, we visualized the images in <strong>Image Grid</strong>. It is obvious that broccoli and cauliflower and much more alike than strawberry and banana.</p>
 <p><img alt="../_images/ImageGrid-Example.png" src="../_images/ImageGrid-Example.png" /></p>
-</section>
-</section>
+</div>
+</div>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="imageembedding.html" class="btn btn-neutral float-left" title="Image Embedding" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="saveimages.html" class="btn btn-neutral float-right" title="Save Images" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
```

#### html2text {}

```diff
@@ -50,13 +50,12 @@
 have used 5 images of fruits and vegetables, namely orange, banana, strawberry,
 broccoli and cauliflower.
 We loaded the images with Import_Images and embedded them with Inception v3
 embedder in Image_Embedding.
 Finally, we visualized the images in Image Grid. It is obvious that broccoli
 and cauliflower and much more alike than strawberry and banana.
 [../_images/ImageGrid-Example.png]
-
 Previous Next
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/imageviewer.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/imageviewer.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Image Viewer &mdash; Orange3 Image Analytics  documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
+        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Image Embedding" href="imageembedding.html" />
     <link rel="prev" title="Import Images" href="importimages.html" /> 
 </head>
@@ -72,16 +72,16 @@
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="image-viewer">
-<h1>Image Viewer<a class="headerlink" href="#image-viewer" title="Permalink to this headline"></a></h1>
+  <div class="section" id="image-viewer">
+<h1>Image Viewer<a class="headerlink" href="#image-viewer" title="Permalink to this heading"></a></h1>
 <p>Displays images that come with a data set.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Data: A data set with images.</p></li>
 </ul>
 <p><strong>Outputs</strong></p>
 <ul class="simple">
@@ -96,22 +96,22 @@
 <li><p>Select the column with image data (links).</p></li>
 <li><p>Select the column with image titles.</p></li>
 <li><p>Zoom in or out.</p></li>
 <li><p>Saves the visualization in a file.</p></li>
 <li><p>Tick the box on the left to commit changes automatically.
 Alternatively, click <em>Send</em>.</p></li>
 </ol>
-<section id="examples">
-<h2>Examples<a class="headerlink" href="#examples" title="Permalink to this headline"></a></h2>
+<div class="section" id="examples">
+<h2>Examples<a class="headerlink" href="#examples" title="Permalink to this heading"></a></h2>
 <p>A very simple way to use this widget is to connect the <strong>File</strong> widget with <strong>Image Viewer</strong> and see all the images that come with your data set. You can also visualize images from <a class="reference internal" href="importimages.html"><span class="doc">Import Images</span></a>.</p>
 <p><img alt="../_images/image-viewer-example1.png" src="../_images/image-viewer-example1.png" /></p>
 <p>Alternatively, you can visualize only selected instances, as shown in the example below.</p>
 <p><img alt="../_images/image-viewer-example2.png" src="../_images/image-viewer-example2.png" /></p>
-</section>
-</section>
+</div>
+</div>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="importimages.html" class="btn btn-neutral float-left" title="Import Images" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="imageembedding.html" class="btn btn-neutral float-right" title="Image Embedding" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
```

#### html2text {}

```diff
@@ -44,13 +44,12 @@
 A very simple way to use this widget is to connect the File widget with Image
 Viewer and see all the images that come with your data set. You can also
 visualize images from Import_Images.
 [../_images/image-viewer-example1.png]
 Alternatively, you can visualize only selected instances, as shown in the
 example below.
 [../_images/image-viewer-example2.png]
-
 Previous Next
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/importimages.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/importimages.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Import Images &mdash; Orange3 Image Analytics  documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
+        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Image Viewer" href="imageviewer.html" />
     <link rel="prev" title="Welcome to Orange3 Image Analytics documentation!" href="../index.html" /> 
 </head>
@@ -72,16 +72,16 @@
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="import-images">
-<h1>Import Images<a class="headerlink" href="#import-images" title="Permalink to this headline"></a></h1>
+  <div class="section" id="import-images">
+<h1>Import Images<a class="headerlink" href="#import-images" title="Permalink to this heading"></a></h1>
 <p>Import images from a directory(s).</p>
 <p><strong>Outputs</strong></p>
 <ul class="simple">
 <li><p>Data: Dataset describing one image in each row.</p></li>
 </ul>
 <p><strong>Import Images</strong> walks through a directory and returs one row per located image. Columns include image name, path to image, width, height and image size. Column with image path is later used as an attribute for image visualization and embedding.</p>
 <p><img alt="../_images/ImportImages-stamped.png" src="../_images/ImportImages-stamped.png" /></p>
@@ -90,23 +90,23 @@
 <li><p>Select the folder to load.</p></li>
 <li><p>Click <em>Reload</em> to update imported images.</p></li>
 <li><p>Information on the input.</p></li>
 <li><p>Access help.</p></li>
 </ol>
 <p><img alt="../_images/ImportImages-class.png" src="../_images/ImportImages-class.png" /></p>
 <p>You can load a folder containing subfolders. In this case Orange will consider each folder as a class value. In the example above, <strong>Import Images</strong> loaded 26 images belonging to two categories. These two categories will be used as class values.</p>
-<section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline"></a></h2>
+<div class="section" id="example">
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
 <p><strong>Import Images</strong> is likely the first widget you will use in image analysis. It loads images and creates class values from folders. In this example we used <strong>Import Images</strong> to load 26 painting belonging to either Monet or Manet.</p>
 <p>We can observe the result in a <strong>Data Table</strong>. See how Orange added an extra class attribute with values Monet and Manet?</p>
 <p>Now we can proceed with standard machine learning methods. We will send images to <a class="reference internal" href="imageembedding.html"><span class="doc">Image Embedding</span></a>, where we will use <em>Painters</em> embedder to retrieve image vectors.</p>
 <p>Then we will use <strong>Test &amp; Score</strong> and <strong>Logistic Regression</strong>, to build a model for predicting the author of a painting. We get a perfect score? How come? It turns out, these were the images the <em>Painters</em> embedder was trained on, so a high accuracy is expected.</p>
 <p><img alt="../_images/ImportImages-Example.png" src="../_images/ImportImages-Example.png" /></p>
-</section>
-</section>
+</div>
+</div>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="../index.html" class="btn btn-neutral float-left" title="Welcome to Orange3 Image Analytics documentation!" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="imageviewer.html" class="btn btn-neutral float-right" title="Image Viewer" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
```

#### html2text {}

```diff
@@ -49,13 +49,12 @@
 to Image_Embedding, where we will use Painters embedder to retrieve image
 vectors.
 Then we will use Test & Score and Logistic Regression, to build a model for
 predicting the author of a painting. We get a perfect score? How come? It turns
 out, these were the images the Painters embedder was trained on, so a high
 accuracy is expected.
 [../_images/ImportImages-Example.png]
-
 Previous Next
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/_build/html/widgets/saveimages.html` & `Orange3-ImageAnalytics-0.9.0/doc/_build/html/widgets/saveimages.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.17: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Save Images &mdash; Orange3 Image Analytics  documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/jquery.js"></script>
         <script src="../_static/underscore.js"></script>
+        <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="../_static/doctools.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="Image Embedding module" href="../scripting/image_embedder.html" />
     <link rel="prev" title="Image Grid" href="imagegrid.html" /> 
 </head>
@@ -73,16 +73,16 @@
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="save-images">
-<h1>Save Images<a class="headerlink" href="#save-images" title="Permalink to this headline"></a></h1>
+  <div class="section" id="save-images">
+<h1>Save Images<a class="headerlink" href="#save-images" title="Permalink to this heading"></a></h1>
 <p>Save images in the directory structure.</p>
 <p><strong>Inputs</strong></p>
 <ul class="simple">
 <li><p>Data: images to save.</p></li>
 </ul>
 <p><strong>Save Images</strong> is a simple widget that saves images sent to its input. Images will be saved as separate files in their own directory. When a class is present in the data, images will be saved in subdirectories based on the class variable.</p>
 <p><img alt="../_images/SaveImages.png" src="../_images/SaveImages.png" /></p>
@@ -98,34 +98,34 @@
 <li><p>DeepLoc: 64x64</p></li>
 <li><p>openface: 256x256</p></li>
 </ul>
 </li>
 <li><p>File format to save images in. See the next section for information on supported formats.</p></li>
 <li><p>If <em>Autosave when receiving new data or settings change</em> is on, images will be saved upon every change. <em>Save</em> will save images, while <em>Save as…</em> enables the user to set the name and the folder where to save the images.</p></li>
 </ol>
-<section id="supported-formats">
-<h2>Supported Formats<a class="headerlink" href="#supported-formats" title="Permalink to this headline"></a></h2>
+<div class="section" id="supported-formats">
+<h2>Supported Formats<a class="headerlink" href="#supported-formats" title="Permalink to this heading"></a></h2>
 <p><strong>Save Images</strong> can save images in the following formats:</p>
 <ul class="simple">
 <li><p>.png</p></li>
 <li><p>.jpeg</p></li>
 <li><p>.gif</p></li>
 <li><p>.tiff</p></li>
 <li><p>.pdf</p></li>
 <li><p>.bmp</p></li>
 <li><p>.eps</p></li>
 <li><p>.ico</p></li>
 </ul>
-</section>
-<section id="example">
-<h2>Example<a class="headerlink" href="#example" title="Permalink to this headline"></a></h2>
+</div>
+<div class="section" id="example">
+<h2>Example<a class="headerlink" href="#example" title="Permalink to this heading"></a></h2>
 <p>Here is a simple example how to use <strong>Save Images</strong>. We loaded 14 paintings from Picasso, sent them to <a class="reference internal" href="imageembedding.html"><span class="doc">Image Embedding</span></a> using <em>Painters</em> embedder, then to <a class="reference external" href="https://orange-visual-programming.readthedocs.io/widgets/unsupervised/distances.html">Distances</a> using cosine distance and finally to <a class="reference external" href="https://orange-visual-programming.readthedocs.io/widgets/unsupervised/hierarchicalclustering.html">Hierarchical Clustering</a> to construct a dendrogram. Then we selected a cluster from the plot and saved the images belonging to the selected cluster with <strong>Save Images</strong>.</p>
 <p><img alt="../_images/SaveImages-Example.png" src="../_images/SaveImages-Example.png" /></p>
-</section>
-</section>
+</div>
+</div>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="imagegrid.html" class="btn btn-neutral float-left" title="Image Grid" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="../scripting/image_embedder.html" class="btn btn-neutral float-right" title="Image Embedding module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
```

#### html2text {}

```diff
@@ -50,21 +50,19 @@
     * .jpeg
     * .gif
     * .tiff
     * .pdf
     * .bmp
     * .eps
     * .ico
-
 ***** Exampleï *****
 Here is a simple example how to use Save Images. We loaded 14 paintings from
 Picasso, sent them to Image_Embedding using Painters embedder, then to
 Distances using cosine distance and finally to Hierarchical_Clustering to
 construct a dendrogram. Then we selected a cluster from the plot and saved the
 images belonging to the selected cluster with Save Images.
 [../_images/SaveImages-Example.png]
-
 Previous Next
 ===============================================================================
 © Copyright 2016, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/conf.py` & `Orange3-ImageAnalytics-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/make.bat` & `Orange3-ImageAnalytics-0.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/image-embedding.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/image-embedding.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/image-grid.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/image-grid.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/image-viewer.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/image-viewer.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/icons/import-images.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/icons/import-images.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/imageembedding.md` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/imageembedding.md`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/imagegrid.md` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/imagegrid.md`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageEmbedding-Example1.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageEmbedding-Example1.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageEmbedding-Example2.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageEmbedding-Example2.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageEmbedding-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageEmbedding-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageGrid-Example.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageGrid-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageGrid-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageGrid-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageViewer-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageViewer-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImageViewer.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImageViewer.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImportImages-Example.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImportImages-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImportImages-class.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImportImages-class.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/ImportImages-stamped.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/ImportImages-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/SaveImages-Example.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/SaveImages-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/SaveImages.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/SaveImages.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/header-example.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/header-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/image-viewer-example1.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/image-viewer-example1.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/images/image-viewer-example2.png` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/images/image-viewer-example2.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/imageviewer.md` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/imageviewer.md`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/importimages.md` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/importimages.md`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets/saveimages.md` & `Orange3-ImageAnalytics-0.9.0/doc/widgets/saveimages.md`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/doc/widgets.json` & `Orange3-ImageAnalytics-0.9.0/doc/widgets.json`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/image_embedder.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/image_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from Orange.data import ContinuousVariable, Domain, Table, Variable
 from Orange.misc.utils.embedder_utils import EmbedderCache
+from Orange.util import dummy_callback
 
 from orangecontrib.imageanalytics.local_embedder import LocalEmbedder
 from orangecontrib.imageanalytics.server_embedder import ServerEmbedder
 from orangecontrib.imageanalytics.utils.image_utils import extract_paths
 
 MODELS = {
     "inception-v3": {
@@ -149,15 +150,15 @@
                 self._model_settings["target_image_size"]
             )
 
     def __call__(
         self,
         data: Union[Table, List[str], np.array],
         col: Optional[Union[str, Variable]] = None,
-        callback: Optional[Callable] = None,
+        callback: Optional[Callable] = dummy_callback,
     ) -> Union[Tuple[Table, Table, int], List[List[float]]]:
         """
         Embedd images.
 
         Parameters
         ----------
         data
@@ -184,17 +185,15 @@
         self._init_embedder()
         if isinstance(data, Table):
             assert col is not None, "Please provide a column for image path"
             # if table on input tables on output
             return self.from_table(data, col=col, callback=callback)
         elif isinstance(data, (np.ndarray, list)):
             # if array-like on input array-like on output
-            return self._embedder.embedd_data(
-                data, processed_callback=callback
-            )
+            return self._embedder.embedd_data(data, callback=callback)
 
     def from_table(
         self,
         data: Table,
         col: Union[str, Variable] = "image",
         callback: Callable = None,
     ) -> Tuple[Table, Table, int]:
@@ -208,22 +207,22 @@
         col
             The column with image paths
         callback
             Optional callback - function that is called for every embedded
             image and is used to report the progress.
         """
         file_paths = extract_paths(data, data.domain[col])
-        embeddings_ = self._embedder.embedd_data(file_paths, callback)
+        embeddings_ = self._embedder.embedd_data(file_paths, callback=callback)
         return ImageEmbedder.prepare_output_data(data, embeddings_)
 
     def __enter__(self) -> "ImageEmbedder":
         return self
 
-    def __exit__(self, exception_type, exception_value, traceback) -> None:
-        self.set_canceled()
+    def __exit__(self, _, __, ___) -> None:
+        pass
 
     def __del__(self) -> None:
         self.__exit__(None, None, None)
 
     @staticmethod
     def construct_output_data_table(
             embedded_images: Table, embeddings_: np.ndarray
@@ -319,21 +318,14 @@
             # embedder is loaded so we clean its cache
             self._embedder.clear_cache()
         else:
             # embedder is not initialized yet - clear it cache from file
             cache = EmbedderCache(self.model)
             cache.clear_cache()
 
-    def set_canceled(self) -> None:
-        """
-        Cancel the embedding
-        """
-        if self._embedder is not None:
-            self._embedder.set_cancelled()
-
 
 if __name__ == "__main__":
     image_file_paths = ["tests/test_images/example_image_0.jpg"]
     # with ImageEmbedder(model='inception-v3') as embedder:
     with ImageEmbedder(model="squeezenet") as embedder:
         embedder.clear_cache()
         print(embedder(image_file_paths))
```

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/image_grid.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/image_grid.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/import_images.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/import_images.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/local_embedder.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/local_embedder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from os.path import join
 
 import cachecontrol.caches
 import requests
 from ndf.example_models import squeezenet
 
 from Orange.canvas.config import cache_dir
-from Orange.misc.utils.embedder_utils import (EmbedderCache,
-                                              EmbeddingCancelledException)
+from Orange.misc.utils.embedder_utils import EmbedderCache
+from Orange.util import dummy_callback
 from orangecontrib.imageanalytics.utils.embedder_utils import ImageLoader
 
 
 class LocalEmbedder:
 
     embedder = None
 
@@ -23,41 +23,34 @@
         self._session = cachecontrol.CacheControl(
             requests.session(),
             cache=cachecontrol.caches.FileCache(
                 join(cache_dir(), __name__ + ".ImageEmbedder.httpcache")
             ),
         )
 
-        self._cancelled = False
-
         self._image_loader = ImageLoader()
         self._cache = EmbedderCache(model)
 
     def _load_model(self):
         self.embedder = squeezenet(include_softmax=False)
 
-    def embedd_data(self, file_paths, processed_callback=None):
+    def embedd_data(self, file_paths, callback=dummy_callback):
         all_embeddings = []
 
-        for row in file_paths:
+        for i, row in enumerate(file_paths, start=1):
             all_embeddings.append(self._embed(row))
-            if processed_callback:
-                processed_callback(success=True)
+            callback(i / len(file_paths))
 
         self._cache.persist_cache()
-
         return all_embeddings
 
     def _embed(self, file_path):
         """ Load images and compute cache keys and send requests to
         an http2 server for valid ones.
         """
-        if self._cancelled:
-            raise EmbeddingCancelledException()
-
         image = self._image_loader.load_image_or_none(
             file_path, self._target_image_size
         )
         if image is None:
             return None
         image = self._image_loader.preprocess_squeezenet(image)
 
@@ -67,10 +60,7 @@
             return cached_im
 
         embedded_image = self.embedder.predict([image])
         embedded_image = embedded_image[0][0]
 
         self._cache.add(cache_key, embedded_image)
         return embedded_image
-
-    def set_cancelled(self):
-        self._cancelled = True
```

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/server_embedder.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/server_embedder.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_image_embedder.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_image_embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class DummyResponse:
     def __init__(self, content):
         self.content = content
 
 
 def make_dummy_post(response, sleep=0):
     @staticmethod
-    async def dummy_post(url, headers, data):
+    async def dummy_post(url, headers, data=None, content=None):
         await asyncio.sleep(sleep)
         return DummyResponse(content=response)
 
     return dummy_post
 
 
 regular_dummy_sr = make_dummy_post(b'{"embedding": [0, 1]}')
```

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_image_grid.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_image_grid.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_0.jpg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_0.jpg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_1.tiff` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_1.tiff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.bmp` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.bmp`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.gif` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.gif`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpeg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpeg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.jpg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pbm` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pbm`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pgm` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pgm`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.png` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.png`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pnm` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.pnm`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.ppm` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.ppm`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tif` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tif`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tiff` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.tiff`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xbm` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xbm`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xpm` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_2.xpm`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_images/example_image_3.svg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_images/example_image_3.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/tests/test_import_images.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/tests/test_import_images.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/embedder_utils.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/embedder_utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/image_utils.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/tests/test_embedder_utils.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/tests/test_embedder_utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/utils/tests/test_image_utils.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/utils/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/__init__.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/Category-ImageAnalytics.svg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/Category-ImageAnalytics.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImageEmbedding.svg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImageEmbedding.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImageGrid.svg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImageGrid.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImageViewer.svg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImageViewer.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/ImportImages.svg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/ImportImages.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/icons/SaveImages.svg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/icons/SaveImages.svg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimageembedding.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimageembedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,36 +48,25 @@
     Returns
     -------
     The object that holds embedded images, skipped images, and number
     of skipped images.
     """
     embedder = ImageEmbedder(model=embedder_name)
 
-    # init progress bar and fuction
-    ticks = iter(np.linspace(0.0, 100.0, len(images)))
-
-    def advance(success=True):
+    def callback(s):
         if state.is_interruption_requested():
-            embedder.set_canceled()
-        if success:
-            state.set_progress_value(next(ticks))
+            raise Exception()
+        state.set_progress_value(s * 100)
 
     try:
-        emb, skip, n_skip = embedder(
-            images, col=file_paths_attr, callback=advance
-        )
+        emb, skip, n_skip = embedder(images, col=file_paths_attr, callback=callback)
     except EmbeddingConnectionError:
-        # recompute ticks to go from current state to 100
-        ticks = iter(np.linspace(next(ticks), 100.0, len(images)))
-
         state.set_partial_result("squeezenet")
         embedder = ImageEmbedder(model="squeezenet")
-        emb, skip, n_skip = embedder(
-            images, col=file_paths_attr, callback=advance
-        )
+        emb, skip, n_skip = embedder(images, col=file_paths_attr, callback=callback)
 
     return Result(embedding=emb, skip_images=skip, num_skipped=n_skip)
 
 
 class OWImageEmbedding(OWWidget, ConcurrentWidgetMixin):
     name = "Image Embedding"
     description = "Image embedding through deep neural networks."
```

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimagegrid.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimagegrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     QShortcut,
     QLabel,
 )
 from Orange.widgets import widget, gui, settings
 from Orange.widgets.settings import ContextSetting
 from Orange.widgets.utils.annotated_data import (
     create_annotated_table, create_groups_table)
-from Orange.widgets.utils.colorpalette import ColorPaletteGenerator
+from Orange.widgets.utils.colorpalettes import LimitedDiscretePalette
 from Orange.widgets.utils.itemmodels import VariableListModel, DomainModel
 from Orange.widgets.utils.overlay import proxydoc
 from Orange.widgets.widget import Input, Output, OWWidget, Msg
 
 from orangecontrib.imageanalytics.image_grid import ImageGrid
 from orangecontrib.imageanalytics.utils.image_utils import (
     extract_image_path,
@@ -479,15 +479,15 @@
     # Adapted from Scatter Plot Graph (change brush instead of pen)
     def compute_colors(self):
         no_brush = DEFAULT_SELECTION_BRUSH
         sels = np.max(self.selection)
         if sels == 1:
             brushes = [no_brush, no_brush]
         else:
-            palette = ColorPaletteGenerator(number_of_colors=sels + 1)
+            palette = LimitedDiscretePalette(number_of_colors=sels + 1)
             brushes = [no_brush] + [QBrush(palette[i]) for i in range(sels)]
         brush = [brushes[a] for a in self.selection]
 
         pen = [DEFAULT_SELECTION_PEN] * len(self.items)
         return pen, brush
 
     def send_report(self):
@@ -918,16 +918,15 @@
         columns = max(layout.columnCount(), 1)
         for i, item in enumerate(items, layout.count()):
             layout.addItem(item, i // columns, i % columns)
 
     def __scheduleLayout(self):
         if not self.__reflowPending:
             self.__reflowPending = True
-            QApplication.postEvent(
-                self, QEvent(QEvent.LayoutRequest), Qt.HighEventPriority)
+            QApplication.postEvent(self, QEvent(QEvent.LayoutRequest))
 
     def event(self, event):
         if event.type() == QEvent.LayoutRequest:
             if self.__layoutMode == GraphicsThumbnailGrid.AutoReflow:
                 self.__reflow()
             else:
                 self.__gridlayout()
@@ -1282,15 +1281,15 @@
 
 
 class GraphicsScene(QGraphicsScene):
     selectionRectPointChanged = Signal(QPointF)
 
     # override the default signal since it should only be emitted when a
     # selection is finished
-    selectionChanged = Signal(set, int)
+    selectionChanged = Signal(set, Qt.KeyboardModifier)
 
     def __init__(self, *args):
         QGraphicsScene.__init__(self, *args)
         self.selectionRect = None
 
     # TODO figure out how to keep items highlighted and prevent redrawing
     #  during selection without disabling this method
```

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimageimport.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimageimport.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owimageviewer.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owimageviewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,15 +697,15 @@
         request = QNetworkRequest(url)
         request.setRawHeader(b"User-Agent", b"OWImageViewer/1.0")
         request.setAttribute(
             QNetworkRequest.CacheLoadControlAttribute,
             QNetworkRequest.PreferCache
         )
         request.setAttribute(
-            QNetworkRequest.FollowRedirectsAttribute, True
+            QNetworkRequest.RedirectPolicyAttribute, True
         )
         request.setMaximumRedirectsAllowed(5)
 
         # Future yielding a QNetworkReply when finished.
         reply = self._netmanager.get(request)
         future._reply = reply
```

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/owsaveimages.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/owsaveimages.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/afternoon-4175917_640.jpg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/afternoon-4175917_640.jpg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/atomium-4179270_640.jpg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/atomium-4179270_640.jpg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/kittens-4020199_640.jpg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/kittens-4020199_640.jpg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_images/landscape-2130524_640.jpg` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_images/landscape-2130524_640.jpg`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimageembedding.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimageembedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
-from unittest import mock, skipIf
+from unittest import mock
 from unittest.mock import patch
 
 import numpy as np
-import pkg_resources
 
 from Orange.data import Table
 from Orange.misc.utils.embedder_utils import EmbeddingConnectionError
 from Orange.widgets.tests.base import WidgetTest
 from Orange.widgets.tests.utils import simulate
 from orangecontrib.imageanalytics.tests.test_image_embedder import (
     HTTPX_POST_METHOD, regular_dummy_sr)
@@ -106,33 +105,28 @@
         self.assertEqual(w.cb_embedder.currentText(), "SqueezeNet (local)")
 
         output = self.get_output(self.widget.Outputs.embeddings)
         self.assertIsInstance(output, Table)
         self.assertEqual(len(output), len(table))
         self.assertEqual(output.X.shape[1], 1000)
 
-    def test_embedder_changed(self):
+    @patch("orangecontrib.imageanalytics.widgets.owimageembedding.ImageEmbedder")
+    def test_embedder_changed(self, _):
         """
         We will check whether embedder changes correctly.
         """
         w = self.widget
         table = load_images()
 
         self.assertEqual(w.cb_embedder.currentText(), "Inception v3")
         self.send_signal(w.Inputs.images, table)
-        cbox = self.widget.controls.cb_embedder_current_id
-        simulate.combobox_activate_index(cbox, 3)
 
-        self.assertEqual(w.cb_embedder.currentText(), "VGG-19")
-
-        output = self.get_output(self.widget.Outputs.embeddings, wait=10000)
-        self.assertIsInstance(output, Table)
-        self.assertEqual(len(output), len(table))
-        # 4096 shows that output is really by VGG-19
-        self.assertEqual(output.X.shape[1], 4096)
+        simulate.combobox_activate_index(self.widget.controls.cb_embedder_current_id, 3)
+        self.assertEqual("VGG-19", w.cb_embedder.currentText())
+        self.assertEqual("vgg19", w.embedders[w.cb_embedder_current_id])
 
     def test_not_image_data_attributes(self):
         """
         Test change of the attributes when data not images
         """
         w = self.widget
         table = Table("iris")
```

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimagegrid.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimagegrid.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimageimport.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimageimport.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owimageviewer.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owimageviewer.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/test_owsaveimages.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/test_owsaveimages.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/tests/utils.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/imagepreview.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/imagepreview.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/tests/test_imagepreview.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/tests/test_imagepreview.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/tests/test_thumnbnailview.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/tests/test_thumnbnailview.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/orangecontrib/imageanalytics/widgets/utils/thumbnailview.py` & `Orange3-ImageAnalytics-0.9.0/orangecontrib/imageanalytics/widgets/utils/thumbnailview.py`

 * *Files identical despite different names*

### Comparing `Orange3-ImageAnalytics-0.8.0/setup.py` & `Orange3-ImageAnalytics-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with io.open('README.pypi', 'r', encoding='utf-8') as f:
     ABOUT = f.read()
 
 NAME = 'Orange3-ImageAnalytics'
 
 MAJOR = 0
-MINOR = 8
+MINOR = 9
 MICRO = 0
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 AUTHOR = 'Bioinformatics Laboratory, FRI UL'
 AUTHOR_EMAIL = 'contact@orange.biolab.si'
 
 URL = 'http://orange.biolab.si/download'
@@ -41,19 +41,14 @@
 
 PACKAGE_DATA = {
     'orangecontrib.imageanalytics.widgets': ['icons/*.svg'],
     'orangecontrib.imageanalytics.widgets.tests': ['test_images/*'],
     'orangecontrib.imageanalytics.tests': ['test_images/*']
 }
 
-INSTALL_REQUIRES = sorted(set(
-    line.partition('#')[0].strip()
-    for line in open(os.path.join(os.path.dirname(__file__), 'requirements.txt'))
-) - {''})
-
 ENTRY_POINTS = {
     'orange.widgets':
         ('Image Analytics = orangecontrib.imageanalytics.widgets',),
     'orange3.addon':
         ('Orange3-Imageanalytics = orangecontrib.imageanalytics',),
     # Register widget help
     "orange.canvas.help": (
@@ -92,15 +87,25 @@
         long_description_content_type='text/markdown',
         license=LICENSE,
         packages=PACKAGES,
         data_files=DATA_FILES,
         package_data=PACKAGE_DATA,
         keywords=KEYWORDS,
         classifiers=CLASSIFIERS,
-        install_requires=INSTALL_REQUIRES,
+        install_requires=[
+            "lockfile",
+            "cachecontrol",
+            "ndf >=0.1.4",
+            "numpy >=1.16",
+            "orange-widget-base",
+            "Orange3 >=3.32",
+            "pillow >=6.2.0",
+            "requests",
+            "scipy",
+        ],
         extras_require={
             'test': ['coverage', ],
             'doc': ['sphinx', 'recommonmark', 'sphinx_rtd_theme', ],
         },
         namespace_packages=['orangecontrib'],
         entry_points=ENTRY_POINTS,
     )
```

### Comparing `Orange3-ImageAnalytics-0.8.0/tox.ini` & `Orange3-ImageAnalytics-0.9.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 deps =
     pyqt5==5.12.*
     pyqtwebengine==5.12.*
     oldest: scikit-learn~=0.23.1
     oldest: orange3==3.31.1
     oldest: orange-canvas-core==0.1.24
     oldest: orange-widget-base==4.16.1
-    latest: git+git://github.com/biolab/orange3.git#egg=orange3
-    latest: git+git://github.com/biolab/orange-canvas-core.git#egg=orange-canvas-core
-    latest: git+git://github.com/biolab/orange-widget-base.git#egg=orange-widget-base
+    latest: https://github.com/biolab/orange3/archive/refs/heads/master.zip#egg=orange3
+    latest: https://github.com/biolab/orange-canvas-core/archive/refs/heads/master.zip#egg=orange-canvas-core
+    latest: https://github.com/biolab/orange-widget-base/archive/refs/heads/master.zip#egg=orange-widget-base
 commands_pre =
     # Verify installed packages have compatible dependencies
     pip check
     # freeze environment
     pip freeze
 commands =
     coverage run -m unittest discover -v --start-directory orangecontrib/imageanalytics
```


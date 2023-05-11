# Comparing `tmp/xgi-0.5.7.tar.gz` & `tmp/xgi-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgi-0.5.7.tar", last modified: Thu Apr 13 18:56:33 2023, max compression
+gzip compressed data, was "xgi-0.5.8.tar", last modified: Thu May 11 13:17:56 2023, max compression
```

## Comparing `xgi-0.5.7.tar` & `xgi-0.5.8.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.293846 xgi-0.5.7/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      541 2023-04-13 18:54:30.000000 xgi-0.5.7/CITATION.cff
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    13449 2023-04-13 15:46:50.000000 xgi-0.5.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3123 2023-04-13 15:46:50.000000 xgi-0.5.7/CONTRIBUTING.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5426 2023-03-17 19:59:13.000000 xgi-0.5.7/LICENSE.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      373 2023-01-03 14:13:27.000000 xgi-0.5.7/MANIFEST.in
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3204 2023-04-13 18:56:33.293714 xgi-0.5.7/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5531 2023-04-13 15:46:50.000000 xgi-0.5.7/README.md
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.283970 xgi-0.5.7/logo/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.5.7/logo/logo.pdf
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.5.7/logo/logo.png
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.5.7/logo/logo.svg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2438 2023-04-13 15:46:50.000000 xgi-0.5.7/long_description.rst
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.5.7/pytest.ini
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.284826 xgi-0.5.7/requirements/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.5.7/requirements/README.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.5.7/requirements/benchmarks.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-03-17 19:59:30.000000 xgi-0.5.7/requirements/default.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-03-17 19:59:22.000000 xgi-0.5.7/requirements/developer.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       95 2022-10-13 17:38:17.000000 xgi-0.5.7/requirements/documentation.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.5.7/requirements/release.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       27 2023-04-13 15:46:50.000000 xgi-0.5.7/requirements/test.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2022-10-13 17:38:17.000000 xgi-0.5.7/requirements/tutorial.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-04-13 18:56:33.293885 xgi-0.5.7/setup.cfg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1805 2023-04-13 18:47:46.000000 xgi-0.5.7/setup.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.286970 xgi-0.5.7/tutorials/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-03-14 19:28:19.000000 xgi-0.5.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-03-14 19:28:19.000000 xgi-0.5.7/tutorials/Tutorial 2 - Read and Write.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-01-03 14:13:27.000000 xgi-0.5.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2022-10-13 17:38:17.000000 xgi-0.5.7/tutorials/Tutorial 4 - Generative_Models.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)  1036142 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/Tutorial 5 - Plotting.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57352 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/Tutorial 6 - Statistics.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   214665 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-03-28 14:59:38.000000 xgi-0.5.7/tutorials/case_study_zhang2022.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    21289 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/quickstart.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-03-14 19:28:19.000000 xgi-0.5.7/tutorials/simplicial_kuramoto_example.ipynb
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.287457 xgi-0.5.7/xgi/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.5.7/xgi/__init__.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.288813 xgi-0.5.7/xgi/algorithms/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      169 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/algorithms/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4552 2023-03-27 20:55:15.000000 xgi-0.5.7/xgi/algorithms/assortativity.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9027 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/algorithms/centrality.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7198 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/algorithms/clustering.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5425 2022-10-13 17:38:17.000000 xgi-0.5.7/xgi/algorithms/connected.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.289681 xgi-0.5.7/xgi/classes/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      151 2023-03-17 19:59:13.000000 xgi-0.5.7/xgi/classes/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    25479 2023-04-11 13:26:40.000000 xgi-0.5.7/xgi/classes/function.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    41403 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/classes/hypergraph.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2729 2023-03-28 13:51:25.000000 xgi-0.5.7/xgi/classes/hypergraphviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    22713 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/classes/reportviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    26351 2023-04-11 13:26:40.000000 xgi-0.5.7/xgi/classes/simplicialcomplex.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    20902 2023-04-08 17:36:23.000000 xgi-0.5.7/xgi/convert.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.290126 xgi-0.5.7/xgi/drawing/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-03-22 23:23:15.000000 xgi-0.5.7/xgi/drawing/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    42809 2023-04-08 17:36:59.000000 xgi-0.5.7/xgi/drawing/draw.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10608 2023-03-28 14:59:38.000000 xgi-0.5.7/xgi/drawing/layout.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.290386 xgi-0.5.7/xgi/dynamics/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.5.7/xgi/dynamics/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8872 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/dynamics/synchronization.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.5.7/xgi/exception.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.291593 xgi-0.5.7/xgi/generators/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      227 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2616 2023-04-05 18:46:03.000000 xgi-0.5.7/xgi/generators/classic.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1410 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/lattice.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10635 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/random.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2749 2023-04-05 18:49:06.000000 xgi-0.5.7/xgi/generators/simple.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7754 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/simplicial_complexes.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10033 2023-04-08 17:36:59.000000 xgi-0.5.7/xgi/generators/uniform.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.292104 xgi-0.5.7/xgi/linalg/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      183 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/linalg/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7016 2023-04-05 18:50:00.000000 xgi-0.5.7/xgi/linalg/hodge_matrix.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8403 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/linalg/hypergraph_matrix.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6711 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/linalg/laplacian_matrix.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.292806 xgi-0.5.7/xgi/readwrite/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      179 2022-10-13 17:38:17.000000 xgi-0.5.7/xgi/readwrite/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6002 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/bipartite.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/edgelist.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2177 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/incidence.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1904 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/json.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5235 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/readwrite/xgi_data.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.293210 xgi-0.5.7/xgi/stats/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    17825 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/stats/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6527 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/stats/edgestats.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    12556 2023-04-13 13:41:14.000000 xgi-0.5.7/xgi/stats/nodestats.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.293507 xgi-0.5.7/xgi/utils/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.5.7/xgi/utils/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3858 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/utils/utilities.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.288120 xgi-0.5.7/xgi.egg-info/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3204 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2018 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      741 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/requires.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.910927 xgi-0.5.8/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      541 2023-05-11 13:14:18.000000 xgi-0.5.8/CITATION.cff
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    13449 2023-05-09 12:29:44.000000 xgi-0.5.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3123 2023-05-09 12:29:44.000000 xgi-0.5.8/CONTRIBUTING.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5426 2023-04-14 16:11:20.000000 xgi-0.5.8/LICENSE.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      373 2023-05-05 16:04:30.000000 xgi-0.5.8/MANIFEST.in
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4030 2023-05-11 13:17:56.910790 xgi-0.5.8/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5643 2023-05-09 12:29:44.000000 xgi-0.5.8/README.md
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.901151 xgi-0.5.8/logo/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.5.8/logo/logo.pdf
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.5.8/logo/logo.png
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.5.8/logo/logo.svg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3264 2023-05-09 12:29:44.000000 xgi-0.5.8/long_description.rst
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.5.8/pytest.ini
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.902058 xgi-0.5.8/requirements/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.5.8/requirements/README.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.5.8/requirements/benchmarks.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-05-09 12:29:44.000000 xgi-0.5.8/requirements/default.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-05-11 12:53:09.000000 xgi-0.5.8/requirements/developer.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       93 2023-05-09 12:29:44.000000 xgi-0.5.8/requirements/documentation.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.5.8/requirements/release.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       27 2023-05-09 12:29:44.000000 xgi-0.5.8/requirements/test.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       58 2023-05-09 12:29:44.000000 xgi-0.5.8/requirements/tutorial.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-05-11 13:17:56.910967 xgi-0.5.8/setup.cfg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1855 2023-05-11 13:14:23.000000 xgi-0.5.8/setup.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.904578 xgi-0.5.8/tutorials/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-05-05 16:04:30.000000 xgi-0.5.8/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-05-05 16:04:30.000000 xgi-0.5.8/tutorials/Tutorial 2 - Read and Write.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-05-05 16:04:30.000000 xgi-0.5.8/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2023-05-05 16:04:30.000000 xgi-0.5.8/tutorials/Tutorial 4 - Generative_Models.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)  1036142 2023-05-09 12:29:44.000000 xgi-0.5.8/tutorials/Tutorial 5 - Plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57352 2023-05-09 12:29:44.000000 xgi-0.5.8/tutorials/Tutorial 6 - Statistics.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   214665 2023-05-09 12:29:44.000000 xgi-0.5.8/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-05-09 12:29:44.000000 xgi-0.5.8/tutorials/case_study_zhang2022.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   987944 2023-05-09 12:29:44.000000 xgi-0.5.8/tutorials/quickstart.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-05-05 16:04:30.000000 xgi-0.5.8/tutorials/simplicial_kuramoto_example.ipynb
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.905058 xgi-0.5.8/xgi/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.5.8/xgi/__init__.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.906247 xgi-0.5.8/xgi/algorithms/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      169 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/algorithms/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4775 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/algorithms/assortativity.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9335 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/algorithms/centrality.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7621 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/algorithms/clustering.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5393 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/algorithms/connected.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.907123 xgi-0.5.8/xgi/classes/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      151 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/classes/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    25904 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/classes/function.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    41486 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/classes/hypergraph.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2759 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/classes/hypergraphviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    23875 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/classes/reportviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    26648 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/classes/simplicialcomplex.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    22000 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/convert.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.907573 xgi-0.5.8/xgi/drawing/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/drawing/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    44099 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/drawing/draw.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10642 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/drawing/layout.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.907825 xgi-0.5.8/xgi/dynamics/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.5.8/xgi/dynamics/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8892 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/dynamics/synchronization.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.5.8/xgi/exception.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.908722 xgi-0.5.8/xgi/generators/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      227 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/generators/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6310 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/generators/classic.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1411 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/generators/lattice.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10637 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/generators/random.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2749 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/generators/simple.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8505 2023-05-11 12:53:43.000000 xgi-0.5.8/xgi/generators/simplicial_complexes.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10058 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/generators/uniform.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.909214 xgi-0.5.8/xgi/linalg/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      183 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/linalg/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7002 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/linalg/hodge_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8447 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/linalg/hypergraph_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6715 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/linalg/laplacian_matrix.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.909904 xgi-0.5.8/xgi/readwrite/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      179 2022-10-13 17:38:17.000000 xgi-0.5.8/xgi/readwrite/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6048 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/readwrite/bipartite.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.5.8/xgi/readwrite/edgelist.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2181 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/readwrite/incidence.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1892 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/readwrite/json.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5273 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/readwrite/xgi_data.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.910248 xgi-0.5.8/xgi/stats/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    17777 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/stats/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6527 2023-05-09 12:29:44.000000 xgi-0.5.8/xgi/stats/edgestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    12555 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/stats/nodestats.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.910574 xgi-0.5.8/xgi/utils/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.5.8/xgi/utils/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4781 2023-05-11 12:53:09.000000 xgi-0.5.8/xgi/utils/utilities.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-11 13:17:56.905633 xgi-0.5.8/xgi.egg-info/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4030 2023-05-11 13:17:56.000000 xgi-0.5.8/xgi.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2018 2023-05-11 13:17:56.000000 xgi-0.5.8/xgi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-05-11 13:17:56.000000 xgi-0.5.8/xgi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      769 2023-05-11 13:17:56.000000 xgi-0.5.8/xgi.egg-info/requires.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-05-11 13:17:56.000000 xgi-0.5.8/xgi.egg-info/top_level.txt
```

### Comparing `xgi-0.5.7/CITATION.cff` & `xgi-0.5.8/CITATION.cff`

 * *Files 19% similar despite different names*

```diff
@@ -22,8 +22,8 @@
   - family-names: Schwarze
     given-names: Alice
 
 cff-version: "1.1.0"
 license: "BSD-3"
 message: "If you use this software, please cite it using these metadata."
 title: XGI
-version: "0.5.7"
+version: "0.5.8"
```

### Comparing `xgi-0.5.7/CODE_OF_CONDUCT.md` & `xgi-0.5.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/CONTRIBUTING.md` & `xgi-0.5.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/LICENSE.md` & `xgi-0.5.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/README.md` & `xgi-0.5.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 * [**Documentation**](https://xgi.readthedocs.io/en/latest/)
 
 Sign up for our [mailing list](http://eepurl.com/igE6ez) and follow XGI on [Twitter](https://twitter.com/xginets) or [Mastodon](https://mathstodon.xyz/@xginets)!
 
 ## Table of Contents:
   - [Installation](#installation)
   - [Getting Started](#getting-started)
-  - [Documentation](#documentation)
+  - [How to Contribute](#contributing)
   - [Corresponding Data](#corresponding-data)
-  - [Contributing](#contributing)
   - [How to Cite](#how-to-cite)
-  - [Code of Conduct](#code-of-conduct)
   - [License](#license)
   - [Funding](#funding)
   - [Other Resources](#other-resources)
 
+
 ## Installation
 XGI runs on Python 3.8 or higher.
 
 To install the latest version of XGI, run the following command:
 ```sh
 pip install xgi
 ```
@@ -41,73 +40,60 @@
 pip install -e .["all"]
 ```
 * If that command does not work, you may try the following instead
 ````zsh
 pip install -e .\[all\]
 ````
 
-## Getting Started
 
+## Getting Started
 To get started, take a look at the [tutorials](/tutorials/) illustrating the library's basic functionality.
 
-## Documentation
-
-For more documentation, see our [Read The Docs](https://xgi.readthedocs.io/en/latest/) page.
 
 ## Corresponding Data
-
 A number of higher-order datasets are available in the [XGI-DATA repository](https://gitlab.com/complexgroupinteractions/xgi-data) and can be easily accessed with the `load_xgi_data()` function.
 
-## Contributing
+
+## How to Contribute
 If you want to contribute to this project, please make sure to read the
-[code of conduct](CODE_OF_CONDUCT.md)
-and the [contributing guidelines](CONTRIBUTING.md).
+[contributing guidelines](CONTRIBUTING.md). We expect respectful and kind interactions by all contributors and users as laid out in our [code of conduct](CODE_OF_CONDUCT.md).
 
-The best way to contribute to XGI is by submitting a bug or request a new feature by
-opening a [new issue](https://github.com/xgi-org/xgi/issues/new).
+The XGI community always welcomes contributions, no matter how small. We're happy to help troubleshoot XGI issues you run into, assist you if you would like to add functionality or fixes to the codebase, or answer any questions you may have.
 
-To get more actively involved, you are invited to browse the [issues page](../../issues) and choose one that you can
-work on.  The core developers will be happy to help you understand the codebase and any
-other doubts you may have while working on your contribution.
+Some concrete ways that you can get involved:
 
-If you are interested in the daily goings-on of XGI, you are invited to join our [Zulip
-channel](https://xgi.zulipchat.com/join/7agfwo7dh7jo56ppnk5kc23r/).
+* **Get XGI updates** by following the XGI [Twitter](https://twitter.com/xginets) account, signing up for our [mailing list](http://eepurl.com/igE6ez), or starring this repository.
+* **Spread the word** when you use XGI by sharing with your colleagues and friends.
+* **Request a new feature or report a bug** by raising a [new issue](https://github.com/xgi-org/xgi/issues/new).
+* **Create a Pull Request (PR)** to address an [open issue](../../issues) or add a feature.
+* **Join our [Zulip channel](https://xgi.zulipchat.com/join/7agfwo7dh7jo56ppnk5kc23r/)** to be a part of the daily goings-on of XGI.
 
-## How to Cite
 
+## How to Cite
 We acknowledge the importance of good software to support research, and we note
 that research becomes more valuable when it is communicated effectively. To
 demonstrate the value of XGI, we ask that you cite XGI in your work.
 Currently, the best way to cite XGI is to go to our
 [repository page](../../) (if you haven't already) and
 click the "cite this repository" button on the right sidebar. This will generate
 a citation in your preferred format, and will also integrate well with citation managers.
 
-## Code of Conduct
-
-Our full code of conduct, and how we enforce it, can be read in [our repository](CODE_OF_CONDUCT.md).
 
 ## License
 Released under the 3-Clause BSD license (see [`LICENSE.md`](LICENSE.md))
 
 Copyright (C) 2021-2023 XGI Developers
 
-Nicholas Landry <nicholas.landry@uvm.edu>
-
-Leo Torres <leo@leotrs.com>
-
-Iacopo Iacopini <iacopiniiacopo@gmail.com>
-
-Maxime Lucas <maxime.lucas@centai.eu>
-
-Giovanni Petri <giovanni.petri@centai.eu>
-
-Alice Patania <apatania@uvm.edu>
-
-Alice Schwarze <alice.c.schwarze@dartmouth.edu>
+* Nicholas Landry <nicholas.landry@uvm.edu>
+* Leo Torres <leo@leotrs.com>
+* Iacopo Iacopini <iacopiniiacopo@gmail.com>
+* Maxime Lucas <maxime.lucas@centai.eu>
+* Giovanni Petri <giovanni.petri@centai.eu>
+* Alice Patania <apatania@uvm.edu>
+* Alice Schwarze <alice.c.schwarze@dartmouth.edu>
 
 The XGI library has copied or modified code from the HyperNetX and NetworkX libraries, the licenses of which can be found in our [license file](LICENSE.md)
 
 ## Funding
 The XGI package has been supported by NSF Grant 2121905, ["HNDS-I: Using Hypergraphs to Study Spreading Processes in Complex Social Networks"](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2121905).
 
 ## Other Resources
```

### Comparing `xgi-0.5.7/logo/logo.pdf` & `xgi-0.5.8/logo/logo.pdf`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/logo/logo.png` & `xgi-0.5.8/logo/logo.png`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/logo/logo.svg` & `xgi-0.5.8/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/requirements/README.md` & `xgi-0.5.8/requirements/README.md`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/setup.py` & `xgi-0.5.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import sys
 
 import setuptools
 from setuptools import setup
 
-__version__ = "0.5.7"
+__version__ = "0.5.8"
 
 if sys.version_info < (3, 8):
     sys.exit("XGI requires Python 3.8 or later.")
 
 name = "xgi"
 
 version = __version__
 
-authors = "Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze"
+authors = (
+    "Nicholas Landry, "
+    "Leo Torres, "
+    "Maxime Lucas, "
+    "Iacopo Iacopini, "
+    "Giovanni Petri, "
+    "Alice Patania, "
+    "and Alice Schwarze"
+)
 
 author_email = "nicholas.landry@uvm.edu"
 
 project_urls = {
     "Documentation": "https://xgi.readthedocs.io/en/latest/",
     "Bug Reports": "https://github.com/xgi-org/xgi/issues",
     "Source": "https://github.com/xgi-org/xgi",
```

### Comparing `xgi-0.5.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb` & `xgi-0.5.8/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/Tutorial 2 - Read and Write.ipynb` & `xgi-0.5.8/tutorials/Tutorial 2 - Read and Write.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb` & `xgi-0.5.8/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/Tutorial 4 - Generative_Models.ipynb` & `xgi-0.5.8/tutorials/Tutorial 4 - Generative_Models.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/Tutorial 5 - Plotting.ipynb` & `xgi-0.5.8/tutorials/Tutorial 5 - Plotting.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/Tutorial 6 - Statistics.ipynb` & `xgi-0.5.8/tutorials/Tutorial 6 - Statistics.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb` & `xgi-0.5.8/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/case_study_zhang2022.ipynb` & `xgi-0.5.8/tutorials/case_study_zhang2022.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/tutorials/simplicial_kuramoto_example.ipynb` & `xgi-0.5.8/tutorials/simplicial_kuramoto_example.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/xgi/algorithms/assortativity.py` & `xgi-0.5.8/xgi/algorithms/assortativity.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         Hypergraph of interest
 
     Returns
     -------
     float
         The dynamical assortativity
 
+    See Also
+    --------
+    degree_assortativity
+
     Raises
     ------
     XGIError
         If the hypergraph is not uniform, or if there are no nodes
         or no edges
 
     References
@@ -66,33 +70,38 @@
 def degree_assortativity(H, kind="uniform", exact=False, num_samples=1000):
     """Computes the degree assortativity of a hypergraph
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest
-    kind : str, default: "uniform"
+    kind : str, optional
         the type of degree assortativity. valid choices are
-        "uniform", "top-2", and "top-bottom".
-    exact : bool, default: False
-        whether to compute over all edges or
-        sample randomly from the set of edges
-    num_samples : int, default: 1000
+        "uniform", "top-2", and "top-bottom". By default, "uniform".
+    exact : bool, optional
+        whether to compute over all edges or sample randomly from the
+        set of edges. By default, False.
+    num_samples : int, optional
         if not exact, specify the number of samples for the computation.
+        By default, 1000.
 
     Returns
     -------
     float
         the degree assortativity
 
     Raises
     ------
     XGIError
         If there are no nodes or no edges
 
+    See Also
+    --------
+    dynamical_assortativity
+
     References
     ----------
     Phil Chodrow,
     Configuration models of random hypergraphs,
     Journal of Complex Networks 2020.
     DOI: 10.1093/comnet/cnaa018
     """
@@ -101,54 +110,58 @@
         raise XGIError("Hypergraph must contain nodes")
     elif H.num_edges == 0:
         raise XGIError("Hypergraph must contain edges!")
 
     degs = H.degree()
     if exact:
         k1k2 = [
-            choose_degrees(H.edges.members(e), degs, kind)
+            _choose_degrees(H.edges.members(e), degs, kind)
             for e in H.edges
             if len(H.edges.members(e)) > 1
         ]
     else:
         edges = [e for e in H.edges if len(H.edges.members(e)) > 1]
         k1k2 = [
-            choose_degrees(H.edges.members(random.choice(edges)), degs, kind)
+            _choose_degrees(H.edges.members(random.choice(edges)), degs, kind)
             for _ in range(num_samples)
         ]
 
     rho = np.corrcoef(np.array(k1k2).T)[0, 1]
     if np.isnan(rho):
         return 0
     return rho
 
 
-def choose_degrees(e, k, kind="uniform"):
+def _choose_degrees(e, k, kind="uniform"):
     """Choose the degrees of two nodes in a hyperedge.
 
     Parameters
     ----------
     e : iterable
         the members in a hyperedge
     k : dict
         the degrees where keys are node IDs and values are degrees
-    kind : str, default: "uniform"
-        the type of degree assortativity, options are
-        "uniform", "top-2", and "top-bottom".
+    kind : str, optional
+        the type of degree assortativity, options are "uniform", "top-2",
+        and "top-bottom". By default, "uniform".
 
     Returns
     -------
     tuple
         two degrees selected from the edge
 
     Raises
     ------
     XGIError
         if invalid assortativity function chosen
 
+    See Also
+    --------
+    degree_assortativity
+
     References
     ----------
     Phil Chodrow,
     Configuration models of random hypergraphs,
     Journal of Complex Networks 2020.
     DOI: 10.1093/comnet/cnaa018
     """
```

### Comparing `xgi-0.5.7/xgi/algorithms/centrality.py` & `xgi-0.5.8/xgi/algorithms/centrality.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,27 @@
 def clique_eigenvector_centrality(H, tol=1e-6):
     """Compute the clique motif eigenvector centrality of a hypergraph.
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest.
-    tol : float, default: 1e-6
-        The tolerance when computing the eigenvector.
+    tol : float, optional
+        The tolerance when computing the eigenvector. By default, 1e-6.
 
     Returns
     -------
     dict
         Centrality, where keys are node IDs and values are centralities. The
         centralities are 1-normalized.
 
+    See Also
+    --------
+    h_eigenvector_centrality
+
     References
     ----------
     Three Hypergraph Eigenvector Centralities,
     Austin R. Benson,
     https://doi.org/10.1137/18M1203031
     """
     from ..algorithms import is_connected
@@ -61,30 +65,35 @@
 def h_eigenvector_centrality(H, max_iter=100, tol=1e-6):
     """Compute the H-eigenvector centrality of a uniform hypergraph.
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest.
-    max_iter : int, default: 100
+    max_iter : int, optional
         The maximum number of iterations before the algorithm terminates.
-    tol : float > 0, default: 1e-6
-        The desired L2 error in the centrality vector.
+        By default, 100.
+    tol : float > 0, optional
+        The desired L2 error in the centrality vector. By default, 1e-6.
 
     Returns
     -------
     dict
         Centrality, where keys are node IDs and values are centralities. The
         centralities are 1-normalized.
 
     Raises
     ------
     XGIError
         If the hypergraph is not uniform.
 
+    See Also
+    --------
+    clique_eigenvector_centrality
+
     References
     ----------
     Three Hypergraph Eigenvector Centralities,
     Austin R. Benson,
     https://doi.org/10.1137/18M1203031
     """
     from ..algorithms import is_connected
@@ -99,16 +108,16 @@
 
     m = is_uniform(H)
     if not m:
         raise XGIError("This method is not defined for non-uniform hypergraphs.")
 
     new_H = convert_labels_to_integers(H, "old-label")
 
-    f = lambda v, m: np.power(v, 1.0 / m)
-    g = lambda v, x: np.prod(v[list(x)])
+    f = lambda v, m: np.power(v, 1.0 / m)  # noqa: E731
+    g = lambda v, x: np.prod(v[list(x)])  # noqa: E731
 
     x = np.random.uniform(size=(new_H.num_nodes))
     x = x / norm(x, 1)
 
     for iter in range(max_iter):
         new_x = apply(new_H, x, g)
         new_x = f(new_x, m)
@@ -127,16 +136,16 @@
 
     Parameters
     ----------
     H : Hypergraph
         Hypergraph of interest.
     x : 1D numpy array
         1D vector
-    g : lambda function, default: sum
-        function to apply
+    g : lambda function, optional
+        function to apply. By default, sum.
 
     Returns
     -------
     1D numpy array
         vector post application
     """
     new_x = np.zeros(H.num_nodes)
@@ -159,31 +168,32 @@
 ):
     """Computes the node and edge centralities
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest
-    f : lambda function, default: x^2
+    f : lambda function, optional
         The function f as described in Tudisco and Higham.
-        Must accept a numpy array.
-    g : lambda function, default: x^0.5
+        Must accept a numpy array. By default, $x^2$.
+    g : lambda function, optional
         The function g as described in Tudisco and Higham.
-        Must accept a numpy array.
-    phi : lambda function, default: x^2
+        Must accept a numpy array. By default, $\sqrt{x}$.
+    phi : lambda function, optional
         The function phi as described in Tudisco and Higham.
-        Must accept a numpy array.
-    psi : lambda function, default: x^0.5
+        Must accept a numpy array. By default $x^2$.
+    psi : lambda function, optional
         The function psi as described in Tudisco and Higham.
-        Must accept a numpy array.
-    max_iter : int, default: 100
+        Must accept a numpy array. By default: $\sqrt{x}$.
+    max_iter : int, optional
         Number of iterations at which the algorithm terminates
-        if convergence is not reached.
-    tol : float > 0, default: 1e-6
+        if convergence is not reached. By default, 100.
+    tol : float > 0, optional
         The total allowable error in the node and edge centralities.
+        By default, 1e-6.
 
     Returns
     -------
     dict, dict
         The node centrality where keys are node IDs and values are associated
         centralities and the edge centrality where keys are the edge IDs and
         values are associated centralities. The centralities of both the nodes
@@ -249,18 +259,19 @@
     Returns
     -------
     dict
         Centrality, where keys are node IDs and values are lists of centralities.
 
     References
     ----------
-    Vector centrality in hypergraphs,
-    K. Kovalenko, M. Romance, E. Vasilyeva, D. Aleja, R. Criado, D. Musatov,
-    A.M. Raigorodskii, J. Flores, I. Samoylenko, K. Alfaro-Bittner, M. Perc, S. Boccaletti,
+    "Vector centrality in hypergraphs", K. Kovalenko, M. Romance, E. Vasilyeva,
+    D. Aleja, R. Criado, D. Musatov, A.M. Raigorodskii, J. Flores, I. Samoylenko,
+    K. Alfaro-Bittner, M. Perc, S. Boccaletti,
     https://doi.org/10.1016/j.chaos.2022.112397
+
     """
     from ..algorithms import is_connected
 
     # If the hypergraph is empty, then return an empty dictionary
     if H.num_nodes == 0:
         return dict()
```

### Comparing `xgi-0.5.7/xgi/algorithms/clustering.py` & `xgi-0.5.8/xgi/algorithms/clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import numpy as np
 
 from ..exception import XGIError
 from ..linalg import adjacency_matrix
 
 __all__ = [
-    "local_clustering_coefficient",
     "clustering_coefficient",
+    "local_clustering_coefficient",
     "two_node_clustering_coefficient",
 ]
 
 
 def clustering_coefficient(H):
     """Return the clustering coefficients for
     each node in a Hypergraph.
 
     This clustering coefficient is defined as the
     clustering coefficient of the unweighted pairwise
     projection of the hypergraph, i.e., `num / denom`,
-    where `num` equals `A^3[n, n]` and `denom` equals
-    `k*(k-1)/2`.  Here `A` is the adjacency matrix
-    of the network and `k` is the pairwise
-    degree of `n`.
+    where `num` equals $A^3_{i,i}$ and `denom` equals
+    $\binom{k}{2}$.  Here $A$ is the adjacency matrix
+    of the network and $k$ is the pairwise
+    degree of $i$.
 
     Parameters
     ----------
     H : Hypergraph
         Hypergraph
 
     Returns
@@ -35,14 +35,19 @@
     Notes
     -----
     The clustering coefficient is undefined when the number of
     neighbors is 0 or 1, but we set the clustering coefficient
     to 0 in these cases. For more discussion, see
     https://arxiv.org/abs/0802.2512
 
+    See Also
+    --------
+    local_clustering_coefficient
+    two_node_clustering_coefficient
+
     References
     ----------
     "Clustering Coefficients in Protein Interaction Hypernetworks"
     by Suzanne Gallagher and Debra Goldberg.
     DOI: 10.1145/2506583.2506635
 
     Example
@@ -87,31 +92,37 @@
     Notes
     -----
     The clustering coefficient is undefined when the number of
     neighbors is 0 or 1, but we set the clustering coefficient
     to 0 in these cases. For more discussion, see
     https://arxiv.org/abs/0802.2512
 
+    See Also
+    --------
+    clustering_coefficient
+    two_node_clustering_coefficient
+
     References
     ----------
-    "Properties of metabolic graphs: biological organization or representation artifacts?"
-    by Wanding Zhou and Luay Nakhleh.
+    "Properties of metabolic graphs: biological organization or representation
+    artifacts?"  by Wanding Zhou and Luay Nakhleh.
     https://doi.org/10.1186/1471-2105-12-132
 
     "Hypergraphs for predicting essential genes using multiprotein complex data"
     by Florian Klimm, Charlotte M. Deane, and Gesine Reinert.
     https://doi.org/10.1093/comnet/cnaa028
 
     Example
     -------
     >>> import xgi
     >>> H = xgi.random_hypergraph(3, [1, 1])
     >>> cc = xgi.local_clustering_coefficient(H)
     >>> cc
     {0: 1.0, 1: 1.0, 2: 1.0}
+
     """
     result = {}
 
     memberships = H.nodes.memberships()
     members = H.edges.members()
 
     for n in H.nodes:
@@ -133,15 +144,15 @@
                     if len(D1.union(D2)) == 0:
                         eo = 0
                     else:
                         # otherwise we have to look at their neighbours
                         # the neighbours of D1 and D2, respectively.
                         neighD1 = {i for d in D1 for i in H.nodes.neighbors(d)}
                         neighD2 = {i for d in D2 for i in H.nodes.neighbors(d)}
-                        # compute the extra overlap [len() is used for cardinality of edges]
+                        # compute extra overlap [len() is used for cardinality of edges]
                         eo = (
                             len(neighD1.intersection(D2))
                             + len(neighD2.intersection(D1))
                         ) / len(
                             D1.union(D2)
                         )  # add it up
                     # add it up
@@ -159,27 +170,35 @@
     This definition averages over all of the
     two-node clustering coefficients involving the node.
 
     Parameters
     ----------
     H : Hypergraph
         Hypergraph
+    kind : string, optional
+        The type of two node clustering coefficient. Options
+        are "union", "max", and "min". By default, "union".
 
     Returns
     -------
     dict
         nodes are keys, clustering coefficients are values.
 
     Notes
     -----
     The clustering coefficient is undefined when the number of
     neighbors is 0 or 1, but we set the clustering coefficient
     to 0 in these cases. For more discussion, see
     https://arxiv.org/abs/0802.2512
 
+    See Also
+    --------
+    clustering_coefficient
+    local_clustering_coefficient
+
     References
     ----------
     "Clustering Coefficients in Protein Interaction Hypernetworks"
     by Suzanne Gallagher and Debra Goldberg.
     DOI: 10.1145/2506583.2506635
 
     Example
```

### Comparing `xgi-0.5.7/xgi/algorithms/connected.py` & `xgi-0.5.8/xgi/algorithms/connected.py`

 * *Files 14% similar despite different names*

```diff
@@ -133,25 +133,23 @@
     Returns
     -------
     set
         The largest connected component (a set of nodes) of the hypergraph.
 
     See Also
     --------
-    is_connected
     connected_components
-    number_connected_components
     largest_connected_hypergraph
 
     Example
     -------
     >>> import xgi
     >>> H = xgi.random_hypergraph(50, [0.1, 0.01], seed=1)
-    >>> print(xgi.number_connected_components(H))
-    1
+    >>> print(len(xgi.largest_connected_component(H)))
+    50
 
     """
     return max(connected_components(H), key=len)
 
 
 def node_connected_component(H, n):
     """
@@ -209,38 +207,38 @@
     A function to find the largest connected hypergraph from a data set.
 
     Parameters
     ----------
     H: Hypergraph
         The hypergraph of interest
     in_place: bool, optional
-        If False, creates a copy; if True, modifies the existing hypergraph
+        If False, creates a copy; if True, modifies the existing hypergraph.
+        By default, True.
 
     Returns
     -------
     None
         If in_place: modifies the existing hypergraph
 
     Hypergraph
         If not in_place: the hypergraph induced on the nodes of the
         largest connected component.
 
     See Also
     --------
-    is_connected
     connected_components
-    number_connected_components
     largest_connected_component
 
     Example
     -------
     >>> import xgi
-    >>> H = xgi.random_hypergraph(50, [0.1, 0.01], seed=1)
-    >>> print(xgi.number_connected_components(H))
-    1
+    >>> H = xgi.random_hypergraph(10, [0.1, 0.01], seed=1)
+    >>> H_gcc = xgi.largest_connected_hypergraph(H)
+    >>> print(H_gcc.num_nodes)
+    8
 
     """
     connected_nodes = max(connected_components(H), key=len)
     if not in_place:
         return subhypergraph(H, nodes=connected_nodes).copy()
     else:
         H.remove_nodes_from(set(H.nodes).difference(connected_nodes))
```

### Comparing `xgi-0.5.7/xgi/classes/function.py` & `xgi-0.5.8/xgi/classes/function.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,17 +39,26 @@
     """The number of edges of order d.
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest.
 
-    d : int | None, optional
+    d : int, optional
         The order of edges to count. If None (default), counts
         for all orders.
+
+    Returns
+    -------
+    int
+        The number of edges of order d
+
+    See Also
+    --------
+    max_edge_order
     """
 
     if d is not None:
         return len(H.edges.filterby("order", d))
     else:
         return H.num_edges
 
@@ -63,24 +72,27 @@
         The hypergraph of interest.
 
     Returns
     -------
     int
         Maximum order of edges in hypergraph.
 
+    See Also
+    --------
+    num_edges_order
     """
     if H._edge:
         d_max = max(len(edge) for edge in H._edge.values()) - 1
     else:
         d_max = 0 if H._node else None
     return d_max
 
 
 def is_possible_order(H, d):
-    """Whether the specified order is between 1 and the maximum order.
+    """Whether the specified order is between 0 (singletons) and the maximum order.
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest.
     d : int
         Order for which to check.
@@ -88,15 +100,15 @@
     Returns
     -------
     bool
         Whether `d` is a possible order.
 
     """
     d_max = max_edge_order(H)
-    return (d >= 1) and (d <= d_max)
+    return (d >= 0) and (d <= d_max)
 
 
 def is_uniform(H):
     """Order of uniformity if the hypergraph is uniform, or False.
 
     A hypergraph is uniform if all its edges have the same order.
 
@@ -117,41 +129,41 @@
     >>> H = xgi.Hypergraph([(0, 1, 2), (1, 2, 3), (2, 3, 4)])
     >>> xgi.is_uniform(H)
     2
     >>> if xgi.is_uniform(H): print('H is uniform!')
     H is uniform!
 
     """
-    edge_sizes = {len(members) for _, members in H._edge.items()}
+    edge_sizes = unique_edge_sizes(H)
     if 1 in edge_sizes:
         edge_sizes.remove(1)  # discard singleton edges
 
     if not edge_sizes or len(edge_sizes) != 1:
         return False
 
     return edge_sizes.pop() - 1  # order of all edges
 
 
 def edge_neighborhood(H, n, include_self=False):
     """The edge neighborhood of the specified node.
 
-    The edge neighborhood of a node `n` in a hypergraph `H` is an edgelist of all the edges
-    containing `n` and its edges are all the edges in `H` that contain
-    `n`.  Usually, the edge neighborhood does not include `n` itself.  This can be controlled
+    The edge neighborhood of a node `n` in a hypergraph `H` is an edgelist of all the
+    edges containing `n` and its edges are all the edges in `H` that contain `n`.
+    Usually, the edge neighborhood does not include `n` itself.  This can be controlled
     with `include_self`.
 
     Parameters
     ----------
     H : Hypergraph
         THe hypergraph of interest
     n : node
         Node whose edge_neighborhood is needed.
-    include_self : bool (default False)
+    include_self : bool, optional
         Whether the edge_neighborhood contains `n`.
-
+        By default, False.
     Returns
     -------
     list
         An edgelist of the edge_neighborhood of `n`.
 
     See Also
     --------
@@ -261,15 +273,15 @@
         The hypergraph of interest
 
     Returns
     -------
     list()
         The unique edge sizes in ascending order by size.
     """
-    return sorted({len(H.edges.members(edge)) for edge in H.edges})
+    return sorted(set(H.edges.size.asnumpy()))
 
 
 def frozen(*args, **kwargs):
     """Dummy method that raises an error when trying to modify frozen hypergraphs
 
     Raises
     ------
@@ -377,15 +389,15 @@
     hypergraph.
 
     Parameters
     ----------
     H : Hypergraph object
         The hypergraph to copy
     with_data : bool, optional
-        Whether to keep the node and hypergraph data, by default True
+        Whether to keep the node and hypergraph data, by default True.
 
     Returns
     -------
     Hypergraph object
         A hypergraph with the same nodes but without edges
 
     See Also
@@ -428,21 +440,22 @@
         will be reflected in the node attribute for every node.
         The attribute name will be `name`.
 
         If `values` is a dict or a dict of dict, it should be keyed
         by node to either an attribute value or a dict of attribute key/value
         pairs used to update the node's attributes.
     name : string, optional
-        Name of the node attribute to set if values is a scalar, by default None
+        Name of the node attribute to set if values is a scalar, by default None.
 
     See Also
     --------
     get_node_attributes
     set_edge_attributes
-    get_edge_attributes
+    ~xgi.classes.hypergraph.Hypergraph.add_node
+    ~xgi.classes.hypergraph.Hypergraph.add_nodes_from
 
     Notes
     -----
     After computing some property of the nodes of a hypergraph, you may
     want to assign a node attribute to store the value of that property
     for each node.
 
@@ -493,15 +506,14 @@
     -------
     dict of dict
         Dictionary of attributes keyed by node.
 
     See Also
     --------
     set_node_attributes
-    set_edge_attributes
     get_edge_attributes
 
     """
     if name is None:
         return dict(H._node_attr)
     else:
         return {n: d[name] for n, d in H._node_attr.items() if name in d}
@@ -520,22 +532,23 @@
         that is then applied to every edge in `H`.  This means that if
         you provide a mutable object, like a list, updates to that object
         will be reflected in the edge attribute for each edge.  The attribute
         name will be `name`.
         If `values` is a dict or a dict of dict, it should be keyed
         by edge ID to either an attribute value or a dict of attribute
         key/value pairs used to update the edge's attributes.
-    name : string (optional, default=None)
-        Name of the edge attribute to set if values is a scalar.
+    name : string, optional
+        Name of the edge attribute to set if values is a scalar. By default, None.
 
     See Also
     --------
     set_node_attributes
-    get_node_attributes
     get_edge_attributes
+    ~xgi.classes.hypergraph.Hypergraph.add_edge
+    ~xgi.classes.hypergraph.Hypergraph.add_edges_from
 
     Notes
     -----
     Note that if the dict contains edge IDs that are not in `H`, they are
     silently ignored.
 
     """
@@ -556,27 +569,28 @@
             for e, d in values.items():
                 try:
                     H._edge_attr[e].update(d)
                 except IDNotFound:
                     warn(f"Edge {e} does not exist!")
         except AttributeError:
             raise XGIError(
-                "name property has not been set and a dict-of-dicts has not been provided."
+                "name property has not been set and a "
+                "dict-of-dicts has not been provided."
             )
 
 
 def get_edge_attributes(H, name=None):
     """Get the edge attributes of the hypergraph
 
     Parameters
     ----------
     H : Hypergraph object
         The hypergraph to get edge attributes from
     name : string, optional
-       Attribute name. If None, then return the entire attribute dictionary.
+       Attribute name. If None (default), then return the entire attribute dictionary.
 
     Returns
     -------
     dict
         Dictionary of attributes keyed by edge ID.
 
     See Also
@@ -691,23 +705,25 @@
     * `density(H, max_order=1) =` :math:`\frac{a}{{n \choose 1} + {n \choose 2}}`,
     * `density(H, max_order=1, ignore_singletons=True) =` :math:`\frac{a}{{n \choose 2}}`,
     * `density(H, max_order=2) =` :math:`\frac{m}{{n \choose 1} + {n \choose 2} + {n \choose 3}}`,
     * `density(H, max_order=2, ignore_singletons=True) =` :math:`\frac{m}{{n \choose 2} + {n \choose 3}}`,
 
     Parameters
     ---------
-    order : int or None (default)
+    order : int, optional
         If not None, only count edges of the specified order.
+        By default, None.
 
-    max_order : int or None (default)
+    max_order : int, optional
         If not None, only count edges of order up to this value, inclusive.
+        By default, None.
 
-    ignore_singletons : bool (default False)
+    ignore_singletons : bool, optional
         Whether to consider singleton edges.  Ignored if `order` is not None and
-        different from :math:`0`.
+        different from :math:`0`. By default, False.
 
     See Also
     --------
     :func:`incidence_density`
 
     Notes
     -----
@@ -759,23 +775,25 @@
     The incidence matrix of a hypergraph contains one row per node nad one column per
     edge.  An entry is non-zero when the corresponding node is a member of the
     corresponding edge.  The density of this matrix is the number of non-zero entries
     divided by the total number of entries.
 
     Parameters
     ---------
-    order : int or None (default)
+    order : int, optional
         If not None, only count edges of the specified order.
+        By default, None.
 
-    max_order : int or None (default)
+    max_order : int, optional
         If not None, only count edges of order up to this value, inclusive.
+        By default, None.
 
-    ignore_singletons : bool (default False)
+    ignore_singletons : bool, optional
         Whether to consider singleton edges.  Ignored if `order` is not None and
-        different from :math:`0`.
+        different from :math:`0`. By default, False.
 
     See Also
     --------
     :func:`density`
 
     Notes
     -----
@@ -821,20 +839,21 @@
 
 
 def subfaces(edges, order=None):
     """Returns the subfaces of a list of hyperedges
 
     Parameters
     ---------
-    edges: list of edges, default: None
+    edges: list of edges
         Edges to consider, as tuples of nodes
-    order: {None, -1, int}, default: None
+    order: {None, -1, int}, optional
         If None, compute subfaces recursively down to nodes.
         If -1, compute subfaces the order below (e.g. edges for a triangle).
         If d > 0, compute the subfaces of order d.
+        By default, None.
 
     Returns
     -------
     faces: list of sets
         List of hyperedges that are subfaces of input hyperedges.
 
     Raises
@@ -860,15 +879,16 @@
     [(1, 2, 3), (1, 2, 4), (1, 3, 4), (2, 3, 4), (3, 4, 5)]
 
     """
 
     max_order = len(max(edges, key=len)) - 1
     if order and order > max_order:
         raise XGIError(
-            f"order must be less or equal to the maximum order among the edges: {max_order}."
+            "order must be less or equal to the maximum "
+            f"order among the edges: {max_order}."
         )
 
     faces = []
     for edge in edges:
         size = len(edge)
 
         if size <= 1:  # down from a node is an empty tuple
```

### Comparing `xgi-0.5.7/xgi/classes/hypergraph.py` & `xgi-0.5.8/xgi/classes/hypergraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,49 +2,20 @@
 from collections import defaultdict
 from collections.abc import Hashable, Iterable
 from copy import copy, deepcopy
 from itertools import count
 from warnings import warn
 
 from ..exception import IDNotFound, XGIError
-from ..utils.utilities import update_uid_counter
+from ..utils.utilities import IDDict, update_uid_counter
 from .reportviews import EdgeView, NodeView
 
 __all__ = ["Hypergraph"]
 
 
-class IDDict(dict):
-    """A dict that holds (node or edge) IDs.
-
-    For internal use only.  Adds input validation functionality to the internal dicts
-    that hold nodes and edges in a network.
-
-    """
-
-    def __getitem__(self, item):
-        try:
-            return dict.__getitem__(self, item)
-        except KeyError as e:
-            raise IDNotFound(f"ID {item} not found") from e
-
-    def __setitem__(self, item, value):
-        if item is None:
-            raise XGIError("None cannot be a node or edge")
-        try:
-            return dict.__setitem__(self, item, value)
-        except TypeError as e:
-            raise TypeError(f"ID {item} not a valid type") from e
-
-    def __delitem__(self, item):
-        try:
-            return dict.__delitem__(self, item)
-        except KeyError as e:
-            raise IDNotFound(f"ID {item} not found") from e
-
-
 class Hypergraph:
     r"""A hypergraph is a collection of subsets of a set of *nodes* or *vertices*.
 
     A hypergraph is a pair :math:`(V, E)`, where :math:`V` is a set of elements called
     *nodes* or *vertices*, and :math:`E` is a set whose elements are subsets of
     :math:`V`, that is, each :math:`e \in E` satisfies :math:`e \subset V`.  The
     elements of :math:`E` are called *hyperedges* or simply *edges*.
@@ -53,27 +24,28 @@
     attributes to each node, edge, or the hypergraph itself, in the form of key/value
     pairs.
 
     Multiedges and self-loops are allowed.
 
     Parameters
     ----------
-    incoming_data : input hypergraph data (optional, default: None)
+    incoming_data : input hypergraph data, optional
         Data to initialize the hypergraph. If None (default), an empty
         hypergraph is created, i.e. one with no nodes or edges.
         The data can be in the following formats:
 
         * hyperedge list
         * hyperedge dictionary
         * 2-column Pandas dataframe (bipartite edges)
         * Scipy/Numpy incidence matrix
         * Hypergraph object.
 
-    **attr : dict, optional, default: None
+    **attr : dict, optional
         Attributes to add to the hypergraph as key, value pairs.
+        By default, None.
 
     Notes
     -----
     Unique IDs are assigned to each node and edge internally and are used to refer to
     them throughout.
 
     The `attr` keyword arguments are added as hypergraph attributes. To add node or edge
@@ -173,17 +145,23 @@
         Returns
         -------
         string
             Hypergraph information
 
         """
         try:
-            return f"{type(self).__name__} named {self['name']} with {self.num_nodes} nodes and {self.num_edges} hyperedges"
+            return (
+                f"{type(self).__name__} named {self['name']} "
+                f"with {self.num_nodes} nodes and {self.num_edges} hyperedges"
+            )
         except XGIError:
-            return f"Unnamed {type(self).__name__} with {self.num_nodes} nodes and {self.num_edges} hyperedges"
+            return (
+                f"Unnamed {type(self).__name__} with "
+                f"{self.num_nodes} nodes and {self.num_edges} hyperedges"
+            )
 
     def __iter__(self):
         """Iterate over the nodes.
 
         Returns
         -------
         iterator
@@ -241,15 +219,16 @@
         word = "nodes"
         if stat is None:
             stat = getattr(self.edges, attr, None)
             word = "edges"
         if stat is None:
             word = None
             raise AttributeError(
-                f"{attr} is not a method of Hypergraph or a recognized NodeStat or EdgeStat"
+                f"{attr} is not a method of Hypergraph or a "
+                "recognized NodeStat or EdgeStat"
             )
 
         def func(node=None, *args, **kwargs):
             val = stat(*args, **kwargs).asdict()
             return val if node is None else val[node]
 
         func.__doc__ = f"""Equivalent to H.{word}.{attr}.asdict(). For accepted *args and
@@ -373,16 +352,16 @@
             A node can be any hashable Python object except None.
         attr : keyword arguments, optional
             Set or change node attributes using key=value.
 
         See Also
         --------
         add_nodes_from
-        set_node_attributes
-        get_node_attributes
+        ~xgi.classes.function.set_node_attributes
+        ~xgi.classes.function.get_node_attributes
 
         Notes
         -----
         If node is already in the hypergraph, its attributes are still updated.
 
         """
         if node not in self._node:
@@ -404,16 +383,16 @@
             Update attributes for all nodes in nodes.
             Node attributes specified in nodes as a tuple take
             precedence over attributes specified via keyword arguments.
 
         See Also
         --------
         add_node
-        set_node_attributes
-        get_node_attributes
+        ~xgi.classes.function.set_node_attributes
+        ~xgi.classes.function.get_node_attributes
         """
         for n in nodes_for_adding:
             try:
                 newnode = n not in self._node
                 newdict = attr
             except TypeError:
                 n, ndict = n
@@ -434,16 +413,16 @@
         node are removed, regardless of size.
 
         Parameters
         ----------
         n : node
             A node in the hypergraph
 
-        strong : bool (default False)
-            Whether to execute weak or strong removal.
+        strong : bool, optional
+            Whether to execute weak or strong removal. By default, False.
 
         Raises
         ------
         XGIError
            If n is not in the hypergraph.
 
         See Also
@@ -488,29 +467,29 @@
     def add_edge(self, members, id=None, **attr):
         """Add one edge with optional attributes.
 
         Parameters
         ----------
         members : Iterable
             An iterable of the ids of the nodes contained in the new edge.
-        id : hashable, default None
-            Id of the new edge. If None, a unique numeric ID will be created.
+        id : hashable, optional
+            Id of the new edge. If None (default), a unique numeric ID will be created.
         **attr : dict, optional
             Attributes of the new edge.
 
         Raises
         -----
         XGIError
             If `members` is empty.
 
         See Also
         --------
         add_edges_from : Add a collection of edges.
-        set_edge_attributes
-        get_edge_attributes
+        ~xgi.classes.function.set_edge_attributes
+        ~xgi.classes.function.get_edge_attributes
 
         Examples
         --------
 
         Add edges with or without specifying an edge id.
 
         >>> import xgi
@@ -552,48 +531,48 @@
         self._edge_attr[uid] = self._hyperedge_attr_dict_factory()
         self._edge_attr[uid].update(attr)
 
         if id:  # set self._edge_uid correctly
             update_uid_counter(self, id)
 
     def add_edges_from(self, ebunch_to_add, **attr):
-        """Add multiple edges with optional attributes.
+        r"""Add multiple edges with optional attributes.
 
         Parameters
         ----------
         ebunch_to_add : Iterable
 
             An iterable of edges.  This may be an iterable of iterables (Format 1),
-            where each element contains the members of the edge specified as valid node IDs.
-            Alternatively, each element could also be a tuple in any of the following
-            formats:
+            where each element contains the members of the edge specified as valid node
+            IDs.  Alternatively, each element could also be a tuple in any of the
+            following formats:
 
             * Format 2: 2-tuple (members, edge_id), or
             * Format 3: 2-tuple (members, attr), or
             * Format 4: 3-tuple (members, edge_id, attr),
 
             where `members` is an iterable of node IDs, `edge_id` is a hashable to use
-            as edge ID, and `attr` is a dict of attributes. Finally, `ebunch_to_add`
-            may be a dict of the form `{edge_id: edge_members}` (Format 5).
+            as edge ID, and `attr` is a dict of attributes. Finally, `ebunch_to_add` may
+            be a dict of the form `{edge_id: edge_members}` (Format 5).
 
-            Formats 2 and 3 are unambiguous because `attr` dicts are not hashable, while `id`s must be.
-            In Formats 2-4, each element of `ebunch_to_add` must have the same length,
-            i.e. you cannot mix different formats.  The iterables containing edge
-            members cannot be strings.
+            Formats 2 and 3 are unambiguous because `attr` dicts are not hashable, while
+            `id`s must be.  In Formats 2-4, each element of `ebunch_to_add` must have
+            the same length, i.e. you cannot mix different formats.  The iterables
+            containing edge members cannot be strings.
 
         attr : \*\*kwargs, optional
             Additional attributes to be assigned to all edges. Attribues specified via
             `ebunch_to_add` take precedence over `attr`.
 
         See Also
         --------
         add_edge : Add a single edge.
         add_weighted_edges_from : Convenient way to add weighted edges.
-        set_edge_attributes
-        get_edge_attributes
+        ~xgi.classes.function.set_edge_attributes
+        ~xgi.classes.function.get_edge_attributes
 
         Notes
         -----
         Adding the same edge twice will create a multi-edge. Currently
         cannot add empty edges; the method skips over them.
 
         Examples
@@ -748,17 +727,18 @@
 
         Parameters
         ----------
         ebunch_to_add : iterable of edges
             Each edge given in the list or container will be added
             to the graph. The edges must be given as tuples of
             the form (node1, node2, ..., noden, weight).
-        weight : string, optional (default= 'weight')
-            The attribute name for the edge weights to be added.
-        attr : keyword arguments, optional (default= no attributes)
+        weight : string, optional
+            The attribute name for the edge weights to be added,
+            by default "weight".
+        attr : keyword arguments, optional
             Edge attributes to add/update for all edges.
 
         See Also
         --------
         add_edge : Add a single edge.
         add_edges_from : Add multiple edges.
         set_edge_attributes
@@ -797,58 +777,73 @@
         e_id1 : hashable
             The ID of the first edge.
         e_id2 : hashable
             The ID of the second edge.
 
         Raises
         ------
-        XGIError
-            If loopy hyperedges are created
         IDNotFound
             If user specifies nodes or edges that do not exist or
             nodes that are not part of edges.
+        XGIError
+            If the swap does not preserve edge sizes.
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph([[1, 2, 3], [3, 4]])
         >>> H.double_edge_swap(1, 4, 0, 1)
         >>> H.edges.members()
         [{2, 3, 4}, {1, 3}]
 
         """
         # Assign edges to modify
         try:
-            temp_memberships1 = list(self._node[n_id1])
-            temp_memberships1[temp_memberships1.index(e_id1)] = e_id2
-
-            temp_memberships2 = list(self._node[n_id2])
-            temp_memberships2[temp_memberships2.index(e_id2)] = e_id1
-
-            temp_members1 = list(self._edge[e_id1])
-            temp_members1[temp_members1.index(n_id1)] = n_id2
+            # Initialize temporary copies to modify
+            temp_memberships1 = self._node[n_id1].copy()
+            temp_memberships2 = self._node[n_id2].copy()
+            temp_members1 = self._edge[e_id1].copy()
+            temp_members2 = self._edge[e_id2].copy()
+
+            # remove old nodes from edges
+            temp_members1.remove(n_id1)
+            temp_members2.remove(n_id2)
+
+            # swap nodes
+            temp_members1.add(n_id2)
+            temp_members2.add(n_id1)
+
+            # Now we handle the memberships
+            # remove old nodes from edges
+            temp_memberships1.remove(e_id1)
+            temp_memberships2.remove(e_id2)
+
+            # swap nodes
+            temp_memberships1.add(e_id2)
+            temp_memberships2.add(e_id1)
 
-            temp_members2 = list(self._edge[e_id2])
-            temp_members2[temp_members2.index(n_id2)] = n_id1
+        except KeyError as e:
 
-        except ValueError as e:
-            raise XGIError(
+            raise IDNotFound(
                 "One of the nodes specified doesn't belong to the specified edge."
             ) from e
 
-        if len(set(temp_members1)) < len(set(self._edge[e_id1])) or len(
-            set(temp_members2)
-        ) < len(set(self._edge[e_id2])):
-            raise XGIError("This will create a loopy hyperedge.")
+        if (
+            len(temp_memberships1) != len(self._node[n_id1])
+            or len(temp_memberships2) != len(self._node[n_id2])
+            or len(temp_members1) != len(self._edge[e_id1])
+            or len(temp_members2) != len(self._edge[e_id2])
+        ):
+            raise XGIError("This swap does not preserve edge sizes.")
 
-        self._node[n_id1] = set(temp_memberships1)
-        self._node[n_id2] = set(temp_memberships2)
+        self._node[n_id1] = temp_memberships1
+        self._node[n_id2] = temp_memberships2
 
-        self._edge[e_id1] = set(temp_members1)
-        self._edge[e_id2] = set(temp_members2)
+        self._edge[e_id1] = temp_members1
+        self._edge[e_id2] = temp_members2
 
     def add_node_to_edge(self, edge, node):
         """Add one node to an existing edge.
 
         If the node or edge IDs do not exist, they are created.
 
         Parameters
@@ -858,14 +853,15 @@
         node : hashable
             node ID
 
         See Also
         --------
         add_node
         add_edge
+        remove_node_from_edge
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph()
         >>> H.add_edge(['apple', 'banana'], 'fruits')
         >>> H.add_node_to_edge('fruits', 'pear')
@@ -942,14 +938,20 @@
             The node ID
 
         Raises
         ------
         XGIError
             If either the node or edge does not exist.
 
+        See Also
+        --------
+        remove_node
+        remove_edge
+        add_node_to_edge
+
         Notes
         -----
         If edge is left empty as a result of removing node from it, the edge is also
         removed.
 
         """
         try:
@@ -972,17 +974,17 @@
 
     def update(self, *, edges=None, nodes=None):
         """Add nodes or edges to the hypergraph.
 
         Parameters
         ----------
         edges : Iterable, optional
-            Edges to be added.
+            Edges to be added. By default, None.
         nodes : Iterable, optional
-            Nodes to be added.
+            Nodes to be added. By default, None.
 
         See Also
         --------
         add_edges_from: Add multiple edges.
         add_nodes_from: Add multiple nodes.
 
         """
@@ -994,16 +996,17 @@
     def clear(self, hypergraph_attr=True):
         """Remove all nodes and edges from the graph.
 
         Also removes node and edge attribues, and optionally hypergraph attributes.
 
         Parameters
         ----------
-        hypergraph_attr : bool, default True
-            Whether to remove hypergraph attributes as well
+        hypergraph_attr : bool, optional
+            Whether to remove hypergraph attributes as well.
+            By default, True.
 
         """
         self._node.clear()
         self._node_attr.clear()
         self._edge.clear()
         self._edge_attr.clear()
         if hypergraph_attr:
@@ -1020,26 +1023,26 @@
         self, rename="first", merge_rule="first", multiplicity=None
     ):
         """Merges edges which have the same members.
 
         Parameters
         ----------
         rename : str, optional
-            Either "first", "tuple", or "new", by default "first"
+            Either "first" (default), "tuple", or "new".
             If "first", the new edge ID is the first of the sorted
             duplicate edge IDs. If "tuple", the new edge ID is a
             tuple of the sorted duplicate edge IDs. If "new", a
             new ID will be selected automatically.
         merge_rule : str, optional
-            Either "first" or "union", by default "first"
+            Either "first" (default) or "union".
             If "first", takes the attributes of the first duplicate.
             If "union", takes the set of attributes of all the duplicates.
         multiplicity : str, optional
             The attribute in which to store the multiplicity of the hyperedge,
-            by default None
+            by default None.
 
         Raises
         ------
         XGIError
             If invalid rename or merge_rule specified.
 
         Warns
@@ -1172,15 +1175,16 @@
                     new_attrs[multiplicity] = len(dup_ids)
                 new_edges.append((members, new_id, new_attrs))
         self.remove_edges_from(dups)
         self.add_edges_from(new_edges)
 
         if merge_rule == "union":
             warn(
-                "You will not be able to color/draw by merged attributes with xgi.draw()!"
+                "You will not be able to color/draw by "
+                "merged attributes with xgi.draw()!"
             )
 
     def copy(self):
         """A deep copy of the hypergraph.
 
         A deep copy of the hypergraph, including node, edge, and hypergraph attributes.
 
@@ -1235,23 +1239,26 @@
         in_place=True,
     ):
         """Removes potentially undesirable artifacts from the hypergraph.
 
         Parameters
         ----------
         isolates : bool, optional
-            Whether isolated nodes are allowed, by default False
+            Whether isolated nodes are allowed, by default False.
         singletons : bool, optional
-            Whether singleton edges are allowed, by default False
+            Whether singleton edges are allowed, by default False.
         multiedges : bool, optional
-            Whether multiedges are allowed, by default False
+            Whether multiedges are allowed, by default False.
         relabel : bool, optional
-            Whether to convert all node and edge labels to sequential integers, by default True
+            Whether to convert all node and edge labels to sequential integers, by
+            default True.
         in_place : bool, optional
-            Whether to modify the current hypergraph or output a new one, by default True
+            Whether to modify the current hypergraph or output a new one, by default
+            True.
+
         """
         if in_place:
             if not multiedges:
                 self.merge_duplicate_edges()
             if not singletons:
                 self.remove_edges_from(self.edges.singletons())
             if not isolates:
```

### Comparing `xgi-0.5.7/xgi/classes/hypergraphviews.py` & `xgi-0.5.8/xgi/classes/hypergraphviews.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """View of Hypergraphs as a subhypergraph or read-only.
 
-In some algorithms it is convenient to temporarily morph
-a hypergraph to exclude some nodes or edges. It should be better
-to do that via a view than to remove and then re-add. This module provides those graph views.
+In some algorithms it is convenient to temporarily morph a hypergraph to exclude some
+nodes or edges. It should be better to do that via a view than to remove and then
+re-add. This module provides those graph views.
 
-The resulting views are essentially read-only graphs that
-report data from the original graph object.
+The resulting views are essentially read-only graphs that report data from the original
+graph object.
 
 Note: Since hypergraphviews look like hypergraphs, one can end up with
 view-of-view-of-view chains. Be careful with chains because they become very slow with
 about 15 nested views. Often it is easiest to use .copy() to avoid chains.
 
 """
 
@@ -19,39 +19,40 @@
 
 
 def subhypergraph(H, nodes=None, edges=None, keep_isolates=True):
     """View of `H` applying a filter on nodes and edges.
 
     `subhypergraph_view` provides a read-only view of the induced subhypergraph that
     includes nodes, edges, or both based on what the user specifies. This function
-    automatically filters out edges that are not subsets of the nodes. This function
-    may create isolated nodes.
+    automatically filters out edges that are not subsets of the nodes. This function may
+    create isolated nodes.
 
-    If the user only specifies the nodes to include, the function returns
-    an induced subhypergraph on the nodes.
+    If the user only specifies the nodes to include, the function returns an induced
+    subhypergraph on the nodes.
 
-    If the user only specifies the edges to include, the function returns all of the nodes
-    and the specified edges.
+    If the user only specifies the edges to include, the function returns all of the
+    nodes and the specified edges.
 
     If the user specifies both nodes and edges to include in the subhypergraph, then the
-    function returns a subhypergraph with the specified nodes and edges from the list of specified
-    hyperedges that are induced by the specified nodes.
+    function returns a subhypergraph with the specified nodes and edges from the list of
+    specified hyperedges that are induced by the specified nodes.
 
     Parameters
     ----------
     H : hypergraph.Hypergraph
         A hypergraph
-    nodes : list or set, default: None
+    nodes : list or set, optional
         A list of the nodes desired for the subhypergraph.
-        If None, uses all the nodes.
-    edges : list or set, default: None
+        If None (default), uses all the nodes.
+    edges : list or set, optional
         A list of the edges desired for the subhypergraph.
-        If None, uses all the edges.
-    keep_isolates : bool, default : True
+        If None (default), uses all the edges.
+    keep_isolates : bool, optional
         Whether to keep isolated nodes in the subhypergraph.
+        By default, True.
 
     Returns
     -------
     Hypergraph object
         A read-only hypergraph view of the input hypergraph.
 
     """
```

### Comparing `xgi-0.5.7/xgi/classes/reportviews.py` & `xgi-0.5.8/xgi/classes/reportviews.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,61 +41,58 @@
 
     """
 
     _id_kind = None
 
     __slots__ = (
         "_net",
-        "_id_dict",
-        "_id_attr",
-        "_bi_id_dict",
-        "_bi_id_attr",
         "_ids",
     )
 
     def __getstate__(self):
         """Function that allows pickling.
 
         Returns
         -------
         dict
             The keys access the IDs and their attributes respectively
             and the values are dictionarys from the Hypergraph class.
 
         """
         return {
-            "_id_dict": self._id_dict,
-            "_id_attr": self._id_attr,
-            "_bi_id_dict": self._bi_id_dict,
-            "_bi_id_attr": self._bi_id_attr,
+            "_net": self._net,
             "_ids": self._ids,
         }
 
     def __setstate__(self, state):
         """Function that allows unpickling.
 
         Parameters
         ----------
         dict
             The keys access the IDs and their attributes respectively
             and the values are dictionarys from the Hypergraph class.
 
         """
-        self._id_dict = state["_id_dict"]
-        self._id_attr = state["_id_attr"]
-        self._bi_id_dict = state["_bi_id_dict"]
-        self._bi_id_attr = state["_bi_id_attr"]
-        self._ids = state["_ids"]
+        self._net = state["_net"]
+        self._id_kind = state["_id_kind"]
 
-    def __init__(self, network, id_dict, id_attr, bi_id_dict, bi_id_attr, ids=None):
+    def __init__(self, network, ids=None):
         self._net = network
-        self._id_dict = id_dict
-        self._id_attr = id_attr
-        self._bi_id_dict = bi_id_dict
-        self._bi_id_attr = bi_id_attr
+
+        if self._id_kind == "node":
+            self._id_dict = None if self._net is None else network._node
+            self._id_attr = None if self._net is None else network._node_attr
+            self._bi_id_dict = None if self._net is None else network._edge
+            self._bi_id_attr = None if self._net is None else network._edge_attr
+        elif self._id_kind == "edge":
+            self._id_dict = None if self._net is None else network._edge
+            self._id_attr = None if self._net is None else network._edge_attr
+            self._bi_id_dict = None if self._net is None else network._node
+            self._bi_id_attr = None if self._net is None else network._node_attr
 
         if ids is None:
             self._ids = self._id_dict
         else:
             self._ids = ids
 
     def __getattr__(self, attr):
@@ -112,24 +109,24 @@
 
         Notes
         -----
         Do not use this property for membership check. Instead of `x in view.ids`,
         always use `x in view`.  The latter is always faster.
 
         """
-        return set(self._id_dict.keys()) if self._ids is None else self._ids
+        return set(self._id_dict) if self._ids is None else self._ids
 
     def __len__(self):
         """The number of IDs."""
         return len(self._id_dict) if self._ids is None else len(self._ids)
 
     def __iter__(self):
         """Returns an iterator over the IDs."""
         if self._ids is None:
-            return iter({}) if self._id_dict is None else iter(self._id_dict.keys())
+            return iter({}) if self._id_dict is None else iter(self._id_dict)
         else:
             return iter(self._ids)
 
     def __getitem__(self, id):
         """Get the attributes of the ID.
 
         Parameters
@@ -187,29 +184,29 @@
         Parameters
         ----------
         stat : str or :class:`xgi.stats.NodeStat`
             `NodeStat` object, or name of a `NodeStat`.
         val : Any
             Value of the statistic.  Usually a single numeric value.  When mode is
             'between', must be a tuple of exactly two values.
-        mode : str
+        mode : str, optional
             How to compare each value to `val`.  Can be one of the following.
 
             * 'eq' (default): Return IDs whose value is exactly equal to `val`.
             * 'neq': Return IDs whose value is not equal to `val`.
             * 'lt': Return IDs whose value is less than `val`.
             * 'gt': Return IDs whose value is greater than `val`.
             * 'leq': Return IDs whose value is less than or equal to `val`.
             * 'geq': Return IDs whose value is greater than or equal to `val`.
             * 'between': In this mode, `val` must be a tuple `(val1, val2)`.  Return IDs
               whose value `v` satisfies `val1 <= v <= val2`.
 
         See Also
         --------
-        For more details, see the `tutorial
+        IDView.filterby_attr : For more details, see the `tutorial
         <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
         Examples
         --------
         By default, return the IDs whose value of the statistic is exactly equal to
         `val`.
 
@@ -261,38 +258,39 @@
             bunch = [idx for idx in self if values[idx] <= val]
         elif mode == "geq":
             bunch = [idx for idx in self if values[idx] >= val]
         elif mode == "between":
             bunch = [node for node in self if val[0] <= values[node] <= val[1]]
         else:
             raise ValueError(
-                f"Unrecognized mode {mode}. mode must be one of 'eq', 'neq', 'lt', 'gt', 'leq', 'geq', or 'between'."
+                f"Unrecognized mode {mode}. mode must be one of "
+                "'eq', 'neq', 'lt', 'gt', 'leq', 'geq', or 'between'."
             )
         return type(self).from_view(self, bunch)
 
     def filterby_attr(self, attr, val, mode="eq", missing=None):
         """Filter the IDs in this view by an attribute.
 
         Parameters
         ----------
         attr : string
             The name of the attribute
         val : Any
             A single value or, in the case of 'between', a list of length 2
-        mode : str, default: "eq"
-            Comparison mode. Valid options are 'eq', 'neq', 'lt', 'gt',
+        mode : str, optional
+            Comparison mode. Valid options are 'eq' (default), 'neq', 'lt', 'gt',
             'leq', 'geq', or 'between'.
-        missing : Any, default: None
-            The default value if the attribute is missing. If None,
+        missing : Any, optional
+            The default value if the attribute is missing. If None (default),
             ignores those IDs.
 
 
         See Also
         --------
-        Works identically to `filterby`.  For more details, see the `tutorial
+        IDView.filterby : Identical method.  For more details, see the `tutorial
         <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
         Notes
         -----
         Beware of using comparison modes ("lt", "gt", "leq", "geq")
         when the attribute is a string. For example, the string comparison
         `'10' < '9'` evaluates to `True`.
@@ -328,15 +326,16 @@
             bunch = [
                 idx
                 for idx in self
                 if values[idx] is not None and val[0] <= values[idx] <= val[1]
             ]
         else:
             raise ValueError(
-                f"Unrecognized mode {mode}. mode must be one of 'eq', 'neq', 'lt', 'gt', 'leq', 'geq', or 'between'."
+                f"Unrecognized mode {mode}. mode must be one of "
+                "'eq', 'neq', 'lt', 'gt', 'leq', 'geq', or 'between'."
             )
         return type(self).from_view(self, bunch)
 
     def neighbors(self, id):
         """Find the neighbors of an ID.
 
         The neighbors of an ID are those IDs that share at least one bipartite ID.
@@ -348,15 +347,15 @@
         Returns
         -------
         set
             A set of the neighboring IDs
 
         See Also
         --------
-        edge_neighborhood
+        ~xgi.classes.function.edge_neighborhood
 
         Examples
         --------
         >>> import xgi
         >>> hyperedge_list = [[1, 2], [2, 3, 4]]
         >>> H = xgi.Hypergraph(hyperedge_list)
         >>> H.nodes.neighbors(1)
@@ -493,15 +492,15 @@
         """
         newview = cls(None)
         newview._net = view._net
         newview._id_dict = view._id_dict
         newview._id_attr = view._id_attr
         newview._bi_id_dict = view._bi_id_dict
         newview._bi_id_attr = view._bi_id_attr
-        all_ids = set(view._id_dict.keys())
+        all_ids = set(view._id_dict)
         if bunch is None:
             newview._ids = all_ids
         else:
             bunch = set(bunch)
             wrong = bunch - all_ids
             if wrong:
                 raise IDNotFound(f"Nodes {wrong} not in the hypergraph")
@@ -524,41 +523,45 @@
     Parameters
     ----------
     hypergraph : Hypergraph
         The hypergraph whose nodes this view will keep track of.
     bunch : optional iterable, default None
         The node ids to keep track of.  If None (default), keep track of all node ids.
 
+    See Also
+    --------
+    IDView
+
     Notes
     -----
     In addition to the methods listed in this page, other methods defined in the `stats`
     package are also accessible via the `NodeView` class.  For more details, see the
     `tutorial
     <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
     _id_kind = "node"
 
     def __init__(self, H, bunch=None):
         if H is None:
-            super().__init__(None, None, None, None, None, bunch)
+            super().__init__(None, bunch)
         else:
-            super().__init__(H, H._node, H._node_attr, H._edge, H._edge_attr, bunch)
+            super().__init__(H, bunch)
 
     def memberships(self, n=None):
         """Get the edge ids of which a node is a member.
 
         Gets all the node memberships for all nodes in the view if n
         not specified.
 
         Parameters
         ----------
-        n : hashable
-            Node ID.
+        n : hashable, optional
+            Node ID. By default, None.
 
         Returns
         -------
         dict of sets if n is None, otherwise a set
             Edge memberships.
 
         Raises
@@ -572,26 +575,27 @@
             if n is None
             else self._id_dict[n].copy()
         )
 
     def isolates(self, ignore_singletons=False):
         """Nodes that belong to no edges.
 
-        When ignore_singletons is True, a node is considered isolated from the
-        rest of the hypergraph when it is included in no edges of size two or more.  In
+        When ignore_singletons is True, a node is considered isolated from the rest of
+        the hypergraph when it is included in no edges of size two or more.  In
         particular, whether the node is part of any singleton edges is irrelevant to
         determine whether it is isolated.
 
-        When ignore_singletons is False (default), a node is isolated only when it is a member of
-        exactly zero edges, including singletons.
+        When ignore_singletons is False (default), a node is isolated only when it is a
+        member of exactly zero edges, including singletons.
 
         Parameters
         ----------
-        ignore_singletons : bool, default False
+        ignore_singletons : bool, optional
             Whether to consider singleton edges.
+            By default, False.
 
         Returns
         -------
         NodeView containing the isolated nodes.
 
         See Also
         --------
@@ -616,40 +620,45 @@
     Parameters
     ----------
     hypergraph : Hypergraph
         The hypergraph whose edges this view will keep track of.
     bunch : optional iterable, default None
         The edge ids to keep track of.  If None (default), keep track of all edge ids.
 
+    See Also
+    --------
+    IDView
+
     Notes
     -----
     In addition to the methods listed in this page, other methods defined in the `stats`
     package are also accessible via the `EdgeView` class.  For more details, see the
     `tutorial
     <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
     _id_kind = "edge"
 
     def __init__(self, H, bunch=None):
         if H is None:
-            super().__init__(None, None, None, None, None, bunch)
+            super().__init__(None, bunch)
         else:
-            super().__init__(H, H._edge, H._edge_attr, H._node, H._node_attr, bunch)
+            super().__init__(H, bunch)
 
     def members(self, e=None, dtype=list):
         """Get the node ids that are members of an edge.
 
         Parameters
         ----------
-        e : hashable
-            Edge ID.
-        dtype : type, default list
+        e : hashable, optional
+            Edge ID. By default, None.
+        dtype : {list, dict}, optional
             Specify the type of the return value.
+            By default, list.
 
         Returns
         -------
         list (if dtype is list, default)
             Edge members.
         dict (if dtype is dict)
             Edge members.
@@ -689,29 +698,46 @@
         See Also
         --------
         :meth:`NodeView.isolates`
 
         """
         return self.filterby("size", 1)
 
-    def maximal(self):
-        """Returns the maximal edges as an EdgeView. Maximal edges are those that are not subsets of any other edges in the hypergraph.
+    def maximal(self, strict=False):
+        """Returns the maximal edges as an EdgeView.
 
+        Maximal edges are those that are not subsets
+        of any other edges in the hypergraph. The strict
+        keyword determines whether the subsets
+        are strict or non-strict.
+
+        Parameters
+        ----------
+        strict : bool, optional
+            Whether maximal edges must strictly include all of its
+            subsets (`strict=True`) or whether maximal multiedges
+            are permitted (`strict=False`), by default False.
+            See Notes for more details.
         Returns
         -------
         EdgeView
             The maximal edges
 
         Notes
         -----
-        When there are maximal edges that are also multi-edges,
-        `maximal()` returns all of these multi-edges rather than
-        choosing one of them to return. There are methods for
-        eliminating these duplicates by running `H.cleanup()`
-        or `H.remove_edges_from(H.edges.duplicates())`
+        This function implements two definitions of maximal
+        hyperedges: strict and non-strict. For the strict case
+        (`strict=True`), we enforce that a maximal edge must
+        strictly include all of its subsets and by this
+        definition, multiedges can't be included. For the non-strict
+        case (`strict=False`), then we add all the maximal multiedges
+        with non-strict inclusion.
+
+        There are methods for eliminating these duplicates by
+        running `H.cleanup()` or `H.remove_edges_from(H.edges.duplicates())`
 
         References
         ----------
         https://stackoverflow.com/questions/14106121/efficient-algorithm-for-finding-all-maximal-subsets
 
         Example
         -------
@@ -723,24 +749,27 @@
         >>> H.edges.maximal().members()
         [{1, 2, 3}, {3, 4}, {1, 2, 3}]
         """
         edges = self._id_dict
         nodes = self._bi_id_dict
         max_edges = set()
 
-        # This data structure so that the algorithm can handle multi-edges
-        dups = defaultdict(list)
-        for idx, members in edges.items():
-            dups[frozenset(members)].append(idx)
-
-        _intersection = lambda x, y: x & y
-
-        for i, e in edges.items():
-            # If a multi-edge has already been added to the set of
-            # maximal edges, we don't need to check.
-            if i not in max_edges:
-                in_common = reduce(_intersection, (nodes[n] for n in e))
-
-                if in_common == set(dups[frozenset(e)]):
-                    max_edges.update(in_common)
+        if strict:
+            for i, e in edges.items():
+                if reduce(lambda x, y: x & y, (nodes[n] for n in e)) == {i}:
+                    max_edges.add(i)
+        else:
+            # This data structure so that the algorithm can handle multi-edges
+            dups = defaultdict(list)
+            for idx, members in edges.items():
+                dups[frozenset(members)].append(idx)
+
+            for i, e in edges.items():
+                # If a multi-edge has already been added to the set of
+                # maximal edges, we don't need to check.
+                if i not in max_edges:
+                    if reduce(lambda x, y: x & y, (nodes[n] for n in e)) == set(
+                        dups[frozenset(e)]
+                    ):
+                        max_edges.update(dups[frozenset(e)])
 
         return self.from_view(self, bunch=max_edges)
```

### Comparing `xgi-0.5.7/xgi/classes/simplicialcomplex.py` & `xgi-0.5.8/xgi/classes/simplicialcomplex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Base class for undirected simplicial complexes.
 
-The SimplicialComplex class allows any hashable object as a node
-and can associate key/value attribute pairs with each undirected simplex and node.
+The SimplicialComplex class allows any hashable object as a node and can associate
+key/value attribute pairs with each undirected simplex and node.
 
 Multi-simplices are not allowed.
+
 """
 
 from collections.abc import Hashable, Iterable
 from itertools import combinations, count
 from warnings import warn
 
 from ..exception import XGIError
@@ -18,41 +19,45 @@
 __all__ = ["SimplicialComplex"]
 
 
 class SimplicialComplex(Hypergraph):
     r"""A class to represent undirected simplicial complexes.
 
     A simplicial complex is a collection of subsets of a set of *nodes* or *vertices*.
-    It is a pair :math:`(V, E)`, where :math:`V` is a set of elements called
-    *nodes* or *vertices*, and :math:`E` is a set whose elements are subsets of
-    :math:`V`, that is, each :math:`e \in E` satisfies :math:`e \subset V`.  The
-    elements of :math:`E` are called *simplices*. Additionally, if a simplex is part of
-    a simplicial complex, all its faces must be too. This makes simplicial complexes
-    a special case of hypergraphs.
+    It is a pair :math:`(V, E)`, where :math:`V` is a set of elements called *nodes* or
+    *vertices*, and :math:`E` is a set whose elements are subsets of :math:`V`, that is,
+    each :math:`e \in E` satisfies :math:`e \subset V`.  The elements of :math:`E` are
+    called *simplices*. Additionally, if a simplex is part of a simplicial complex, all
+    its faces must be too. This makes simplicial complexes a special case of
+    hypergraphs.
 
     The SimplicialComplex class allows any hashable object as a node and can associate
-    attributes to each node, simplex, or the simplicial complex itself, in the form of key/value
-    pairs.
-
+    attributes to each node, simplex, or the simplicial complex itself, in the form of
+    key/value pairs.
 
     Parameters
     ----------
-    incoming_data : input simplicial complex data (optional, default: None)
+    incoming_data : input simplicial complex data, optional
         Data to initialize the simplicial complex. If None (default), an empty
-        simplicial complex is created, i.e. one with no nodes or simplices.
-        The data can be in the following formats:
+        simplicial complex is created, i.e. one with no nodes or simplices.  The data
+        can be in the following formats:
 
         * simplex list
         * simplex dictionary
         * 2-column Pandas dataframe (bipartite edges)
         * Scipy/Numpy incidence matrix
         * SimplicialComplex object.
 
-    **attr : dict, optional, default: None
+    **attr : dict, optional
         Attributes to add to the simplicial complex as key, value pairs.
+        By default, None.
+
+    See Also
+    --------
+    ~xgi.classes.hypergraph.Hypergraph
 
     Notes
     -----
     Unique IDs are assigned to each node and simplex internally and are used to refer to
     them throughout.
 
     The `attr` keyword arguments are added as simplicial complex attributes. To add node
@@ -101,52 +106,62 @@
         >>> import xgi
         >>> H = xgi.SimplicialComplex(name="foo")
         >>> str(H)
         "SimplicialComplex named 'foo' with 0 nodes and 0 simplices"
 
         """
         try:
-            return f"{type(self).__name__} named '{self['name']}' with {self.num_nodes} nodes and {self.num_edges} simplices"
+            return (
+                f"{type(self).__name__} named '{self['name']}' "
+                f"with {self.num_nodes} nodes and {self.num_edges} simplices"
+            )
         except XGIError:
-            return f"Unnamed {type(self).__name__} with {self.num_nodes} nodes and {self.num_edges} simplices"
+            return (
+                f"Unnamed {type(self).__name__} with {self.num_nodes}"
+                f" nodes and {self.num_edges} simplices"
+            )
 
     def add_edge(self, edge, id=None, **attr):
-        """add_edge is deprecated in SimplicialComplex. Use add_simplex instead"""
+        """Deprecated in SimplicialComplex. Use add_simplex instead"""
         warn("add_edge is deprecated in SimplicialComplex. Use add_simplex instead")
         return self.add_simplex(edge, id=None, **attr)
 
     def add_edges_from(self, ebunch_to_add, max_order=None, **attr):
-        """add_edges_from is deprecated in SimplicialComplex. Use add_simplices_from instead"""
+        """Deprecated in SimplicialComplex. Use add_simplices_from instead"""
         warn(
-            "add_edges_from is deprecated in SimplicialComplex. Use add_simplices_from instead"
+            "add_edges_from is deprecated in SimplicialComplex. "
+            "Use add_simplices_from instead"
         )
         return self.add_simplices_from(ebunch_to_add, max_order=None, **attr)
 
     def add_weighted_edges_from(
         self, ebunch_to_add, max_order=None, weight="weight", **attr
     ):
-        """add_weighted_edges_from is deprecated in SimplicialComplex. Use add_weighted_simplices_from instead"""
+        """Deprecated in SimplicialComplex. Use add_weighted_simplices_from instead"""
         warn(
-            "add_weighted_edges_from is deprecated in SimplicialComplex. Use add_weighted_simplices_from instead"
+            "add_weighted_edges_from is deprecated in SimplicialComplex."
+            " Use add_weighted_simplices_from instead"
         )
         return self.add_weighted_simplices_from(
-            ebunch_to_add, max_order=None, weight="weight", **attr
+            ebunch_to_add, max_order=max_order, weight=weight, **attr
         )
 
     def remove_edge(self, id):
-        """remove_edge is deprecated in SimplicialComplex. Use remove_simplex_id instead"""
+        """Deprecated in SimplicialComplex. Use remove_simplex_id instead"""
         warn(
-            "remove_edge is deprecated in SimplicialComplex. Use remove_simplex_id instead"
+            "remove_edge is deprecated in SimplicialComplex. "
+            "Use remove_simplex_id instead"
         )
-        return self.remove_simplex_id(id, **attr)
+        return self.remove_simplex_id(id)
 
     def remove_edges_from(self, ebunch):
-        """remove_edges_from is deprecated in SimplicialComplex. Use remove_simplex_ids_from instead"""
+        """Deprecated in SimplicialComplex. Use remove_simplex_ids_from instead"""
         warn(
-            "remove_edges_from is deprecated in SimplicialComplex. Use remove_simplex_ids_from instead"
+            "remove_edges_from is deprecated in SimplicialComplex. "
+            "Use remove_simplex_ids_from instead"
         )
         return self.remove_simplex_ids_from(ebunch)
 
     def add_node_to_edge(self, edge, node):
         """add_node_to_edge is not implemented in SimplicialComplex."""
         raise XGIError("add_node_to_edge is not implemented in SimplicialComplex.")
 
@@ -194,16 +209,17 @@
         accessing the simplex's attribute dictionary. The attributes do not propagate
         to the subfaces.
 
         Parameters
         ----------
         members : Iterable
             An iterable of the ids of the nodes contained in the new simplex.
-        id : hashable, default None
-            Id of the new simplex. If None, a unique numeric ID will be created.
+        id : hashable, optional
+            Id of the new simplex. If None (default), a unique numeric ID will be
+            created.
         **attr : dict, optional
             Attributes of the new simplex.
 
         Raises
         -----
         XGIError
             If `members` is empty.
@@ -236,14 +252,15 @@
         >>> S.edges[0]
         {}
         >>> S.add_simplex([1, 4], color='red', place='peru')
         >>> S.edges
         EdgeView((0, 1, 2, 3, 'myedge', 4))
         >>> S.edges[4]
         {'color': 'red', 'place': 'peru'}
+
         """
 
         try:
             members = frozenset(members)
         except TypeError:
             raise XGIError("The simplex cannot be cast to a frozenset.")
 
@@ -277,17 +294,17 @@
     def _subfaces(self, simplex, all=True):
         """Returns list of subfaces of simplex.
 
         Parameters
         ----------
         simplex: an iterable of hashables
             A list of node ids
-        all: bool, default: True
+        all: bool, optional
             Whether to return all of the subfaces or just
-            those of the order below
+            those of the order below. By default, True.
 
         Returns
         -------
         faces: list of iterables
             The list containing the subfaces of the
             given simplex
 
@@ -315,40 +332,40 @@
 
     def add_simplices_from(self, ebunch_to_add, max_order=None, **attr):
         """Add multiple edges with optional attributes.
 
         Parameters
         ----------
         ebunch_to_add : Iterable
-
             An iterable of simplices.  This may be an iterable of iterables (Format 1),
-            where each element contains the members of the simplex specified as valid node IDs.
-            Alternatively, each element could also be a tuple in any of the following
-            formats:
+            where each element contains the members of the simplex specified as valid
+            node IDs.  Alternatively, each element could also be a tuple in any of the
+            following formats:
 
             * Format 2: 2-tuple (members, simplex_id), or
             * Format 3: 2-tuple (members, attr), or
             * Format 4: 3-tuple (members, simplex_id, attr),
 
-            where `members` is an iterable of node IDs, `simplex_id` is a hashable to use
-            as simplex ID, and `attr` is a dict of attributes. Finally, `ebunch_to_add`
-            may be a dict of the form `{simplex_id: simplex_members}` (Format 5).
-
-            Formats 2 and 3 are unambiguous because `attr` dicts are not hashable, while `id`s must be.
-            In Formats 2-4, each element of `ebunch_to_add` must have the same length,
-            i.e. you cannot mix different formats.  The iterables containing simplex
-            members cannot be strings.
-
-        max_order : None or int
-            Maximal dimension of simplices to add. If None (default), adds all simplices.
-            If int, and `ebunch_to_add` contains simplices of order > `max_order`, creates
-            and adds all its subfaces up to `max_order`.
+            where `members` is an iterable of node IDs, `simplex_id` is a hashable to
+            use as simplex ID, and `attr` is a dict of attributes. Finally,
+            `ebunch_to_add` may be a dict of the form `{simplex_id: simplex_members}`
+            (Format 5).
+
+            Formats 2 and 3 are unambiguous because `attr` dicts are not hashable, while
+            `id`s must be.  In Formats 2-4, each element of `ebunch_to_add` must have
+            the same length, i.e. you cannot mix different formats.  The iterables
+            containing simplex members cannot be strings.
+
+        max_order : int, optional
+            Maximal dimension of simplices to add. If None (default), adds all
+            simplices.  If int, and `ebunch_to_add` contains simplices of order >
+            `max_order`, creates and adds all its subfaces up to `max_order`.
         attr : \*\*kwargs, optional
-            Additional attributes to be assigned to all simplices. Attribues specified via
-            `ebunch_to_add` take precedence over `attr`.
+            Additional attributes to be assigned to all simplices. Attribues specified
+            via `ebunch_to_add` take precedence over `attr`.
 
         See Also
         --------
         add_simplex : add a single simplex
         add_weighted_simplices_from : convenient way to add weighted simplices
 
         Notes
@@ -357,16 +374,16 @@
         cannot add empty simplices; the method skips over them.
 
         Examples
         --------
         >>> import xgi
         >>> S = xgi.SimplicialComplex()
 
-        When specifying simplices by their members only, numeric simplex IDs will be assigned
-        automatically.
+        When specifying simplices by their members only, numeric simplex IDs will be
+        assigned automatically.
 
         >>> S.add_simplices_from([[0, 1], [1, 2], [2, 3, 4]])
         >>> S.edges.members(dtype=dict) # doctest: +SKIP
         {0: frozenset({0, 1}), 1: frozenset({1, 2}), 2: frozenset({2, 3, 4}), 3: frozenset({2, 3}), 4: frozenset({2, 4}), 5: frozenset({3, 4})}
 
         Custom simplex ids can be specified using a dict.
 
@@ -424,15 +441,15 @@
                 if not members or self.has_simplex(members):
                     continue
 
                 if id in self._edge.keys():  # check that uid is not present yet
                     warn(f"uid {id} already exists, cannot add simplex {members}.")
                     continue
 
-                if max_order != None:
+                if max_order is not None:
                     if len(members) > max_order + 1:
                         combos = powerset(members, include_singletons=False)
                         faces += list(combos)
 
                         continue
 
                 try:
@@ -518,15 +535,15 @@
                 continue
 
             # needs to go after the check for existence, otherwise
             # we're skipping ID numbers when edges already exist
             if format1 or format3:
                 id = next(self._edge_uid)
 
-            if max_order != None:
+            if max_order is not None:
                 if len(members) > max_order + 1:
                     combos = powerset(members, include_singletons=False)
                     faces += list(combos)  # store faces
 
                     try:
                         e = next(new_edges)
                     except StopIteration:
@@ -586,14 +603,15 @@
         add_simplex : add a single simplex
         add_weighted_simplices_from : convenient way to add weighted simplices
 
         Notes
         -----
         Adding the same simplex twice will add it only once. Currently
         cannot add empty simplices; the method skips over them.
+
         """
         ebunch_to_close = list(map(list, self.edges.members()))
         for simplex in ebunch_to_close:
             if isinstance(simplex[-1], dict):
                 dd = simplex[-1]
                 simplex = simplex[:-1]
             else:
@@ -610,16 +628,19 @@
 
         Parameters
         ----------
         ebunch_to_add : iterable of simplices
             Each simplex given in the list or container will be added
             to the graph. The simplices must be given as tuples of
             the form (node1, node2, ..., noden, weight).
-        weight : string, optional (default= 'weight')
+        max_order : int, optional
+            The maximum order simplex to add, by default None.
+        weight : string, optional
             The attribute name for the simplex weights to be added.
+            By default, "weight".
         attr : keyword arguments, optional (default= no attributes)
             simplex attributes to add/update for all simplices.
 
         See Also
         --------
         add_simplex : add a single simplex
         add_simplices_from : add multiple simplices
```

### Comparing `xgi-0.5.7/xgi/convert.py` & `xgi-0.5.8/xgi/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,49 +49,61 @@
     The preferred way to call this is automatically from the class constructor.
 
     Parameters
     ----------
     data : object to be converted
         Current known types are:
          * a Hypergraph object
+         * a SimplicialComplex object
          * list-of-iterables
          * dict-of-iterables
          * Pandas DataFrame (bipartite edgelist)
          * numpy matrix
          * numpy ndarray
          * scipy sparse matrix
     create_using : Hypergraph constructor, optional (default=Hypergraph)
-        Hypergraph type to create. If hypergraph instance, then cleared before populated.
+        Hypergraph type to create. If hypergraph instance, then cleared before
+        populated.
 
     Returns
     -------
     Hypergraph object
         A hypergraph constructed from the data
 
     """
     if data is None:
         return empty_hypergraph(create_using)
 
-    elif isinstance(data, Hypergraph):
+    elif isinstance(data, Hypergraph) and not isinstance(data, SimplicialComplex):
         H = empty_hypergraph(create_using)
         H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
         ee = data.edges
         H.add_edges_from((ee.members(e), e, deepcopy(attr)) for e, attr in ee.items())
         H._hypergraph = deepcopy(data._hypergraph)
+        return H
+
+    elif isinstance(data, SimplicialComplex):
+        return from_max_simplices(data)
 
     elif isinstance(data, list):
         # edge list
-        from_hyperedge_list(data, create_using)
+        result = from_hyperedge_list(data, create_using)
+        if not isinstance(create_using, Hypergraph):
+            return result
 
     elif isinstance(data, pd.DataFrame):
-        from_bipartite_pandas_dataframe(data, create_using)
+        result = from_bipartite_pandas_dataframe(data, create_using)
+        if not isinstance(create_using, Hypergraph):
+            return result
 
     elif isinstance(data, dict):
         # edge dict in the form we need
-        from_hyperedge_dict(data, create_using)
+        result = from_hyperedge_dict(data, create_using)
+        if not isinstance(create_using, Hypergraph):
+            return result
 
     elif isinstance(
         data,
         (
             ndarray,
             matrix,
             csr_array,
@@ -149,19 +161,19 @@
     Returns
     -------
     LG : networkx.Graph
          The line graph associated to the Hypergraph
 
     References
     ----------
-    "Hypernetwork science via high-order hypergraph walks"
-    by Sinan G. Aksoy, Cliff Joslyn, Carlos Ortiz Marrero, Brenda Praggastis & Emilie Purvine.
+    "Hypernetwork science via high-order hypergraph walks", by Sinan G. Aksoy, Cliff
+    Joslyn, Carlos Ortiz Marrero, Brenda Praggastis & Emilie Purvine.
     https://doi.org/10.1140/epjds/s13688-020-00231-0
-    """
 
+    """
     LG = nx.Graph()
 
     edge_label_dict = {tuple(edge): index for index, edge in H._edge.items()}
 
     LG.add_nodes_from(H.edges)
 
     for edge1, edge2 in combinations(H.edges.members(), 2):
@@ -176,48 +188,65 @@
     The preferred way to call this is automatically
     from the class constructor.
 
     Parameters
     ----------
     data : object to be converted
         Current known types are:
+         * a SimplicialComplex object
          * a Hypergraph object
          * list-of-iterables
          * dict-of-iterables
          * Pandas DataFrame (bipartite edgelist)
          * numpy matrix
          * numpy ndarray
          * scipy sparse matrix
     create_using : Hypergraph graph constructor, optional (default=Hypergraph)
-        Hypergraph type to create. If hypergraph instance, then cleared before populated.
+        Hypergraph type to create. If hypergraph instance, then cleared before
+        populated.
 
     Returns
     -------
     Hypergraph object
         A hypergraph constructed from the data
+
     """
 
     if data is None:
-        return empty_hypergraph(create_using)
+        return empty_simplicial_complex(create_using)
 
     elif isinstance(data, SimplicialComplex):
         H = empty_simplicial_complex(create_using)
         H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
         ee = data.edges
         H.add_simplices_from(
             (ee.members(e), e, deepcopy(attr)) for e, attr in ee.items()
         )
         H._hypergraph = deepcopy(data._hypergraph)
+        return H
+
+    elif isinstance(data, Hypergraph):
+        H = empty_simplicial_complex(create_using)
+        H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
+        ee = data.edges
+        H.add_simplices_from(
+            (ee.members(e), e, deepcopy(attr)) for e, attr in ee.items()
+        )
+        return H
 
     elif isinstance(data, list):
         # edge list
-        from_hyperedge_list(data, create_using)
+        result = from_hyperedge_list(data, create_using)
+        if not isinstance(create_using, SimplicialComplex):
+            return convert_to_simplicial_complex(result)
 
     elif isinstance(data, pd.DataFrame):
-        from_bipartite_pandas_dataframe(data, create_using)
+        result = from_bipartite_pandas_dataframe(data, create_using)
+        if not isinstance(create_using, SimplicialComplex):
+            return convert_to_simplicial_complex(result)
 
     elif isinstance(data, dict):
         # edge dict in the form we need
         raise XGIError("Cannot generate SimplicialComplex from simplex dictionary")
     elif isinstance(
         data,
         (
```

### Comparing `xgi-0.5.7/xgi/drawing/draw.py` & `xgi-0.5.8/xgi/drawing/draw.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,61 +45,68 @@
 ):
     """Draw hypergraph or simplicial complex.
 
     Parameters
     ----
     H : Hypergraph or SimplicialComplex.
         Hypergraph to draw
-    pos : dict (default=None)
-        If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
-        If None (default), use the `barycenter_spring_layout` to compute the positions.
-    ax : matplotlib.pyplot.axes (default=None)
-        Axis to draw on
-    dyad_color : str, dict, iterable, or EdgeStat (default='black')
-        Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
-        contain (edge_id: color_str) pairs.  If iterable, assume the colors are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
-        (specified with dyad_color_cmap) associated to it.
-    dyad_lw : int, float, dict, iterable, or EdgeStat (default=1.5)
-        Line width of edges of order 1 (dyadic links).  If int or float, use the same width for all edges.
-        If a dict, must contain (edge_id: width) pairs.  If iterable, assume the widths are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a monotonic
-        linear interpolation defined between min_dyad_lw and max_dyad_lw.
-    edge_fc : str, dict, iterable, or EdgeStat (default=None)
-        Color of the hyperedges.  If str, use the same color for all nodes.  If a dict, must
-        contain (edge_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the hyperedges are found in H.edges. If EdgeStat,
-        use the colormap specified with edge_fc_cmap. If None (default),
-        use the H.edges.size.
-    node_fc : str, dict, iterable, or NodeStat (default='white')
+    pos : dict, optional
+        If passed, this dictionary of positions node_id:(x,y) is used for placing the
+        0-simplices.  If None (default), use the `barycenter_spring_layout` to compute
+        the positions.
+    ax : matplotlib.pyplot.axes, optional
+        Axis to draw on. If None (default), get the current axes.
+    dyad_color : str, dict, iterable, or EdgeStat, optional
+        Color of the dyadic links.  If str, use the same color for all edges. If a dict,
+        must contain (edge_id: color_str) pairs.  If iterable, assume the colors are
+        specified in the same order as the edges are found in H.edges. If EdgeStat, use
+        a colormap (specified with dyad_color_cmap) associated to it. By default,
+        "black".
+    dyad_lw : int, float, dict, iterable, or EdgeStat, optional
+        Line width of edges of order 1 (dyadic links).  If int or float, use the same
+        width for all edges.  If a dict, must contain (edge_id: width) pairs.  If
+        iterable, assume the widths are specified in the same order as the edges are
+        found in H.edges. If EdgeStat, use a monotonic linear interpolation defined
+        between min_dyad_lw and max_dyad_lw. By default, 1.5.
+    edge_fc : str, dict, iterable, or EdgeStat, optional
+        Color of the hyperedges.  If str, use the same color for all nodes.  If a dict,
+        must contain (edge_id: color_str) pairs.  If other iterable, assume the colors
+        are specified in the same order as the hyperedges are found in H.edges. If
+        EdgeStat, use the colormap specified with edge_fc_cmap. If None (default), use
+        the H.edges.size.
+    node_fc : str, dict, iterable, or NodeStat, optional
         Color of the nodes.  If str, use the same color for all nodes.  If a dict, must
         contain (node_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat,
-        use the colormap specified with node_fc_cmap.
-    node_ec : str, dict, iterable, or NodeStat (default='black')
-        Color of node borders.  If str, use the same color for all nodes.  If a dict, must
-        contain (node_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat,
-        use the colormap specified with node_ec_cmap.
-    node_lw : int, float, dict, iterable, or NodeStat (default=1)
-        Line width of the node borders in pixels.  If int or float, use the same width for all node borders.
-        If a dict, must contain (node_id: width) pairs.  If iterable, assume the widths are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
-        linear interpolation defined between min_node_lw and max_node_lw.
-    node_size : int, float, dict, iterable, or NodeStat (default=15)
-        Radius of the nodes in pixels.  If int or float, use the same radius for all nodes.
-        If a dict, must contain (node_id: radius) pairs.  If iterable, assume the radiuses are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
-        linear interpolation defined between min_node_size and max_node_size.
-    max_order : int (default=None)
+        specified in the same order as the nodes are found in H.nodes. If NodeStat, use
+        the colormap specified with node_fc_cmap. By default, "white".
+    node_ec : str, dict, iterable, or NodeStat, optional
+        Color of node borders.  If str, use the same color for all nodes.  If a dict,
+        must contain (node_id: color_str) pairs.  If other iterable, assume the colors
+        are specified in the same order as the nodes are found in H.nodes. If NodeStat,
+        use the colormap specified with node_ec_cmap. By default, "black".
+    node_lw : int, float, dict, iterable, or NodeStat, optional
+        Line width of the node borders in pixels.  If int or float, use the same width
+        for all node borders.  If a dict, must contain (node_id: width) pairs.  If
+        iterable, assume the widths are specified in the same order as the nodes are
+        found in H.nodes. If NodeStat, use a monotonic linear interpolation defined
+        between min_node_lw and max_node_lw. By default, 1.
+    node_size : int, float, dict, iterable, or NodeStat, optional
+        Radius of the nodes in pixels.  If int or float, use the same radius for all
+        nodes.  If a dict, must contain (node_id: radius) pairs.  If iterable, assume
+        the radiuses are specified in the same order as the nodes are found in
+        H.nodes. If NodeStat, use a monotonic linear interpolation defined between
+        min_node_size and max_node_size. By default, 15.
+    max_order : int, optional
         Maximum of hyperedges to plot. If None (default), plots all orders.
-    node_labels : bool, or dict (default=False)
+    node_labels : bool or dict, optional
         If True, draw ids on the nodes. If a dict, must contain (node_id: label) pairs.
-    hyperedge_labels : bool, or dict (default=False)
-        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label) pairs.
+        By default, False.
+    hyperedge_labels : bool or dict, optional
+        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label)
+        pairs.  By default, False.
     **kwargs : optional args
         Alternate default values. Values that can be overwritten are the following:
         * min_node_size
         * max_node_size
         * min_node_lw
         * max_node_lw
         * min_dyad_lw
@@ -119,14 +126,15 @@
     See Also
     --------
     draw_nodes
     draw_hyperedges
     draw_simplices
     draw_node_labels
     draw_hyperedge_labels
+
     """
     settings = {
         "min_node_size": 10.0,
         "max_node_size": 30.0,
         "min_dyad_lw": 2.0,
         "max_dyad_lw": 10.0,
         "min_node_lw": 1.0,
@@ -219,42 +227,45 @@
 ):
     """Draw the nodes of a hypergraph
 
     Parameters
     ----------
     H : Hypergraph or SimplicialComplex
         Higher-order network to plot.
-    ax : matplotlib.pyplot.axes
-        Axis to draw on
-    pos : dict (default=None)
-        If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
-        If None (default), use the `barycenter_spring_layout` to compute the positions.
-    node_fc : str, dict, iterable, or NodeStat (default='white')
+    ax : matplotlib.pyplot.axes, optional
+        Axis to draw on. If None (default), get the current axes.
+    pos : dict, optional
+        If passed, this dictionary of positions node_id:(x,y) is used for placing the
+        0-simplices.  If None (default), use the `barycenter_spring_layout` to compute
+        the positions.
+    node_fc : str, dict, iterable, or NodeStat, optional
         Color of the nodes.  If str, use the same color for all nodes.  If a dict, must
         contain (node_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat,
-        use the colormap specified with node_fc_cmap.
-    node_ec : str, dict, iterable, or NodeStat (default='black')
-        Color of node borders.  If str, use the same color for all nodes.  If a dict, must
-        contain (node_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat,
-        use the colormap specified with node_ec_cmap.
-    node_lw : int, float, dict, iterable, or EdgeStat (default=1)
-        Line width of the node borders in pixels.  If int or float, use the same width for all node borders.
-        If a dict, must contain (node_id: width) pairs.  If iterable, assume the widths are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
-        linear interpolation defined between min_node_lw and max_node_lw.
-    node_size : int, float, dict, iterable, or NodeStat (default=15)
-        Radius of the nodes in pixels.  If int or float, use the same radius for all nodes.
-        If a dict, must contain (node_id: radius) pairs.  If iterable, assume the radiuses are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
-        linear interpolation defined between min_node_size and max_node_size.
+        specified in the same order as the nodes are found in H.nodes. If NodeStat, use
+        the colormap specified with node_fc_cmap. By default, "white".
+    node_ec : str, dict, iterable, or NodeStat, optional
+        Color of node borders.  If str, use the same color for all nodes.  If a dict,
+        must contain (node_id: color_str) pairs.  If other iterable, assume the colors
+        are specified in the same order as the nodes are found in H.nodes. If NodeStat,
+        use the colormap specified with node_ec_cmap. By default, "black".
+    node_lw : int, float, dict, iterable, or EdgeStat, optional
+        Line width of the node borders in pixels.  If int or float, use the same width
+        for all node borders.  If a dict, must contain (node_id: width) pairs.  If
+        iterable, assume the widths are specified in the same order as the nodes are
+        found in H.nodes. If NodeStat, use a monotonic linear interpolation defined
+        between min_node_lw and max_node_lw. By default, 1.
+    node_size : int, float, dict, iterable, or NodeStat, optional
+        Radius of the nodes in pixels.  If int or float, use the same radius for all
+        nodes.  If a dict, must contain (node_id: radius) pairs.  If iterable, assume
+        the radiuses are specified in the same order as the nodes are found in
+        H.nodes. If NodeStat, use a monotonic linear interpolation defined between
+        min_node_size and max_node_size. By default, 15.
     zorder : int
         The layer on which to draw the nodes.
-    node_labels : bool, or dict
+    node_labels : bool or dict
         If True, draw ids on the nodes. If a dict, must contain (node_id: label) pairs.
     settings : dict
         Default parameters. Keys that may be useful to override default settings:
         * min_node_size
         * max_node_size
         * min_node_lw
         * max_node_lw
@@ -266,14 +277,15 @@
     See Also
     --------
     draw
     draw_hyperedges
     draw_simplices
     draw_node_labels
     draw_hyperedge_labels
+
     """
 
     if settings is None:
         settings = {
             "min_node_size": 10.0,
             "max_node_size": 30.0,
             "min_node_lw": 1.0,
@@ -352,38 +364,43 @@
     **kwargs,
 ):
     """Draw hyperedges.
 
     Parameters
     ----------
     H : Hypergraph
-    ax : matplotlib.pyplot.axes
-        Axis to draw on
-    pos : dict (default=None)
-        If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
-        If None (default), use the `barycenter_spring_layout` to compute the positions.
-    dyad_color : str, dict, iterable, or EdgeStat (default='black')
-        Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
-        contain (edge_id: color_str) pairs.  If iterable, assume the colors are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
-        (specified with dyad_color_cmap) associated to it.
-    dyad_lw : int, float, dict, iterable, or EdgeStat (default=1.5)
-        Line width of edges of order 1 (dyadic links).  If int or float, use the same width for all edges.
-        If a dict, must contain (edge_id: width) pairs.  If iterable, assume the widths are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a monotonic
-        linear interpolation defined between min_dyad_lw and max_dyad_lw.
-    edge_fc : str, dict, iterable, or EdgeStat (default=None)
-        Color of the hyperedges.  If str, use the same color for all nodes.  If a dict, must
-        contain (edge_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the hyperedges are found in H.edges. If EdgeStat,
-        use the colormap specified with edge_fc_cmap.
-    max_order : int (default=None)
-        Maximum of hyperedges to plot.
-    hyperedge_labels : bool, or dict (default=False)
-        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label) pairs.
+    ax : matplotlib.pyplot.axes, optional
+        Axis to draw on. If None (default), get the current axes.
+    pos : dict, optional
+        If passed, this dictionary of positions node_id:(x,y) is used for placing the
+        0-simplices.  If None (default), use the `barycenter_spring_layout` to compute
+        the positions.
+    dyad_color : str, dict, iterable, or EdgeStat, optional
+        Color of the dyadic links.  If str, use the same color for all edges. If a dict,
+        must contain (edge_id: color_str) pairs.  If iterable, assume the colors are
+        specified in the same order as the edges are found in H.edges. If EdgeStat, use
+        a colormap (specified with dyad_color_cmap) associated to it. By default,
+        "black".
+    dyad_lw : int, float, dict, iterable, or EdgeStat, optional
+        Line width of edges of order 1 (dyadic links).  If int or float, use the same
+        width for all edges.  If a dict, must contain (edge_id: width) pairs.  If
+        iterable, assume the widths are specified in the same order as the edges are
+        found in H.edges. If EdgeStat, use a monotonic linear interpolation defined
+        between min_dyad_lw and max_dyad_lw. By default, 1.5.
+    edge_fc : str, dict, iterable, or EdgeStat, optional
+        Color of the hyperedges.  If str, use the same color for all nodes.  If a dict,
+        must contain (edge_id: color_str) pairs.  If other iterable, assume the colors
+        are specified in the same order as the hyperedges are found in H.edges. If
+        EdgeStat, use the colormap specified with edge_fc_cmap. If None (default), color
+        by edge size.
+    max_order : int, optional
+        Maximum of hyperedges to plot. By default, None.
+    hyperedge_labels : bool or dict, optional
+        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label)
+        pairs.  By default, None.
     settings : dict
         Default parameters. Keys that may be useful to override default settings:
         * min_dyad_lw
         * max_dyad_lw
         * dyad_color_cmap
         * edge_fc_cmap
     kwargs : optional keywords
@@ -397,14 +414,15 @@
     See Also
     --------
     draw
     draw_nodes
     draw_simplices
     draw_node_labels
     draw_hyperedge_labels
+
     """
 
     if pos is None:
         pos = barycenter_spring_layout(H)
 
     if ax is None:
         ax = plt.gca()
@@ -432,15 +450,16 @@
     dyad_color = _color_arg_to_dict(dyad_color, H.edges, settings["dyad_color_cmap"])
     dyad_lw = _scalar_arg_to_dict(
         dyad_lw, H.edges, settings["min_dyad_lw"], settings["max_dyad_lw"]
     )
 
     edge_fc = _color_arg_to_dict(edge_fc, H.edges, settings["edge_fc_cmap"])
 
-    # Looping over the hyperedges of different order (reversed) -- nodes will be plotted separately
+    # Looping over the hyperedges of different order (reversed) -- nodes will be plotted
+    # separately
     for id, he in H.edges.members(dtype=dict).items():
         d = len(he) - 1
         if d > max_order:
             continue
         if d == 1:
             # Drawing the edges
             he = list(he)
@@ -499,41 +518,46 @@
 ):
     """Draw maximal simplices and pairwise faces.
 
     Parameters
     ----------
     SC : SimplicialComplex
         Simplicial complex to draw
-    ax : matplotlib.pyplot.axes
-        Axis to draw on
-    pos : dict (default=None)
-        If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
-        If None (default), use the `barycenter_spring_layout` to compute the positions.
-    dyad_color : str, dict, iterable, or EdgeStat
-        Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
-        contain (edge_id: color_str) pairs.  If iterable, assume the colors are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
-        (specified with dyad_color_cmap) associated to it.
-    dyad_lw : int, float, dict, iterable, or EdgeStat
-        Line width of edges of order 1 (dyadic links).  If int or float, use the same width for all edges.
-        If a dict, must contain (edge_id: width) pairs.  If iterable, assume the widths are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a monotonic
-        linear interpolation defined between min_dyad_lw and max_dyad_lw.
-    edge_fc : str, dict, iterable, or EdgeStat (default=None)
-        Color of the hyperedges.  If str, use the same color for all nodes.  If a dict, must
-        contain (edge_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the hyperedges are found in H.edges. If EdgeStat,
-        use the colormap specified with edge_fc_cmap.
-    max_order : int
-        Maximum of hyperedges to plot.
-    hyperedge_labels : bool, or dict
-        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label) pairs.
-        Note, we plot only the maximal simplices so if you pass a dict be careful to match its keys
-        with the new edge ids in the converted SimplicialComplex. These may differ from the
-        edge ids in the given SC.
+    ax : matplotlib.pyplot.axes, optional
+        Axis to draw on. If None (default), get the current axes.
+    pos : dict, optional
+        If passed, this dictionary of positions node_id:(x,y) is used for placing the
+        0-simplices.  If None (default), use the `barycenter_spring_layout` to compute
+        the positions.
+    dyad_color : str, dict, iterable, or EdgeStat, optional
+        Color of the dyadic links.  If str, use the same color for all edges. If a dict,
+        must contain (edge_id: color_str) pairs.  If iterable, assume the colors are
+        specified in the same order as the edges are found in H.edges. If EdgeStat, use
+        a colormap (specified with dyad_color_cmap) associated to it. By default,
+        "black".
+    dyad_lw : int, float, dict, iterable, or EdgeStat, optional
+        Line width of edges of order 1 (dyadic links).  If int or float, use the same
+        width for all edges.  If a dict, must contain (edge_id: width) pairs.  If
+        iterable, assume the widths are specified in the same order as the edges are
+        found in H.edges. If EdgeStat, use a monotonic linear interpolation defined
+        between min_dyad_lw and max_dyad_lw. By default, 1.5.
+    edge_fc : str, dict, iterable, or EdgeStat, optional
+        Color of the hyperedges.  If str, use the same color for all nodes.  If a dict,
+        must contain (edge_id: color_str) pairs.  If other iterable, assume the colors
+        are specified in the same order as the hyperedges are found in H.edges. If
+        EdgeStat, use the colormap specified with edge_fc_cmap. If None (default), color
+        by simplex size.
+    max_order : int, optional
+        Maximum of hyperedges to plot. By default, None.
+    hyperedge_labels : bool or dict, optional
+        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label)
+        pairs.  Note, we plot only the maximal simplices so if you pass a dict be
+        careful to match its keys with the new edge ids in the converted
+        SimplicialComplex. These may differ from the edge ids in the given SC. By
+        default, False.
     settings : dict
         Default parameters. Keys that may be useful to override default settings:
         * min_dyad_lw
         * max_dyad_lw
         * dyad_color_cmap
         * edge_fc_cmap
     kwargs : optional keywords
@@ -548,14 +572,15 @@
     See Also
     --------
     draw
     draw_nodes
     draw_hyperedges
     draw_node_labels
     draw_hyperedge_labels
+
     """
 
     if max_order:
         max_edges = SC.edges.filterby("order", max_order, "leq").members()
         SC = SimplicialComplex(max_edges)  # SC without simplices larger than max_order
 
     # Plot only the maximal simplices, thus let's convert the SC to H
@@ -593,15 +618,16 @@
         H_.edges,
         settings["min_dyad_lw"],
         settings["max_dyad_lw"],
     )
 
     edge_fc = _color_arg_to_dict(edge_fc, H_.edges, settings["edge_fc_cmap"])
 
-    # Looping over the hyperedges of different order (reversed) -- nodes will be plotted separately
+    # Looping over the hyperedges of different order (reversed) -- nodes will be plotted
+    # separately
     for id, he in H_.edges.members(dtype=dict).items():
         d = len(he) - 1
 
         if d == 1:
             # Drawing the edges
             he = list(he)
             x_coords = [pos[he[0]][0], pos[he[1]][0]]
@@ -680,28 +706,30 @@
     Raises
     ------
     TypeError
         If a int, float, list, dict, or NodeStat/EdgeStat is not passed.
     """
     if isinstance(arg, str):
         raise TypeError(
-            f"Argument must be int, float, dict, iterable, or NodeStat/EdgeStat. Received {type(arg)}"
+            "Argument must be int, float, dict, iterable, "
+            f"or NodeStat/EdgeStat. Received {type(arg)}"
         )
     elif isinstance(arg, dict):
         return {id: arg[id] for id in arg if id in ids}
     elif type(arg) in [int, float]:
         return {id: arg for id in ids}
     elif isinstance(arg, NodeStat) or isinstance(arg, EdgeStat):
         vals = np.interp(arg.asnumpy(), [arg.min(), arg.max()], [min_val, max_val])
         return dict(zip(ids, vals))
     elif isinstance(arg, Iterable):
         return {id: arg[idx] for idx, id in enumerate(ids)}
     else:
         raise TypeError(
-            f"Argument must be int, float, dict, iterable, or NodeStat/EdgeStat. Received {type(arg)}"
+            "Argument must be int, float, dict, iterable, "
+            f"or NodeStat/EdgeStat. Received {type(arg)}"
         )
 
 
 def _color_arg_to_dict(arg, ids, cmap):
     """Map different types of arguments for drawing style to a dict with color values.
 
     Parameters
@@ -723,28 +751,29 @@
     TypeError
         If a string, dict, iterable, or NodeStat/EdgeStat is not passed.
     """
     if isinstance(arg, dict):
         return {id: arg[id] for id in arg if id in ids}
     elif isinstance(arg, str):
         return {id: arg for id in ids}
-    elif isinstance(arg, NodeStat) or isinstance(arg, EdgeStat):
+    elif isinstance(arg, (NodeStat, EdgeStat)):
         if isinstance(cmap, ListedColormap):
             vals = np.interp(arg.asnumpy(), [arg.min(), arg.max()], [0, cmap.N])
         elif isinstance(cmap, LinearSegmentedColormap):
             vals = np.interp(arg.asnumpy(), [arg.min(), arg.max()], [0.1, 0.9])
         else:
             raise XGIError("Invalid colormap!")
 
         return {id: np.array(cmap(vals[i])).reshape(1, -1) for i, id in enumerate(ids)}
     elif isinstance(arg, Iterable):
         return {id: arg[idx] for idx, id in enumerate(ids)}
     else:
         raise TypeError(
-            f"Argument must be str, dict, iterable, or NodeStat/EdgeStat. Received {type(arg)}"
+            "Argument must be str, dict, iterable, or "
+            f"NodeStat/EdgeStat. Received {type(arg)}"
         )
 
 
 def _CCW_sort(p):
     """
     Sort the input 2D points counterclockwise.
     """
@@ -773,36 +802,42 @@
     """Draw node labels on the hypergraph or simplicial complex.
 
     Parameters
     ----------
     H : Hypergraph or SimplicialComplex.
     pos : dict
         Dictionary of positions node_id:(x,y).
-    node_labels : bool, or dict (default=False)
+    node_labels : bool or dict, optional
         If True, draw ids on the nodes. If a dict, must contain (node_id: label) pairs.
-    font_size_nodes : int (default=10)
-        Font size for text labels.
-    font_color_nodes : str (default='black')
-        Font color string.
-    font_family_nodes : str (default='sans-serif')
-        Font family.
+        By default, False.
+    font_size_nodes : int, optional
+        Font size for text labels, by default 10.
+    font_color_nodes : str, optional
+        Font color string, by default "black".
+    font_family_nodes : str, optional
+        Font family, by default "sans-serif".
     font_weight_nodes : str (default='normal')
         Font weight.
-    alpha_nodes : float (default=None)
-        The text transparency.
-    bbox_nodes : Matplotlib bbox (default is Matplotlib's ax.text default)
+    alpha_nodes : float, optional
+        The text transparency, by default None.
+    bbox_nodes : Matplotlib bbox, optional
         Specify text box properties (e.g. shape, color etc.) for node labels.
-    horizontalalignment_nodes : str (default='center')
+        When it is None (default), use Matplotlib's ax.text default
+    horizontalalignment_nodes : str, optional
         Horizontal alignment {'center', 'right', 'left'}.
-    verticalalignment_nodes : str (default='center')
+        By default, "center".
+    verticalalignment_nodes : str, optional
         Vertical alignment {'center', 'top', 'bottom', 'baseline', 'center_baseline'}.
-    ax_nodes : matplotlib.pyplot.axes (default=None)
+        By default, "center".
+    ax_nodes : matplotlib.pyplot.axes, optional
         Draw the graph in the specified Matplotlib axes.
-    clip_on_nodes : bool (default=True)
+        By default, None.
+    clip_on_nodes : bool, optional
         Turn on clipping of node labels at axis boundaries.
+        By default, True.
 
     Returns
     -------
     dict
         `dict` of labels keyed by node id.
 
     See Also
@@ -821,16 +856,16 @@
     if node_labels is True:
         node_labels = {id: id for id in H.nodes}
 
     # Plot the labels in the last layer
     zorder = max_edge_order(H) + 1
 
     text_items = {}
-    for id, label in node_labels.items():
-        (x, y) = pos[id]
+    for idx, label in node_labels.items():
+        (x, y) = pos[idx]
 
         if not isinstance(label, str):
             label = str(label)
 
         t = ax.text(
             x,
             y,
@@ -843,15 +878,15 @@
             horizontalalignment=horizontalalignment_nodes,
             verticalalignment=verticalalignment_nodes,
             transform=ax.transData,
             bbox=bbox_nodes,
             clip_on=clip_on_nodes,
             zorder=zorder,
         )
-        text_items[id] = t
+        text_items[idx] = t
 
     return text_items
 
 
 def draw_hyperedge_labels(
     H,
     pos,
@@ -871,51 +906,56 @@
     """Draw hyperedge labels on the hypegraph or simplicial complex.
 
     Parameters
     ----------
     H : Hypergraph.
     pos : dict
         Dictionary of positions node_id:(x,y).
-    hyperedge_labels : bool, or dict (default=False)
-        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label) pairs.
-    font_size_edges : int (default=10)
-        Font size for text labels.
-    font_color_edges : str (default='black')
-        Font color string.
+    hyperedge_labels : bool or dict, optional
+        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label)
+        pairs.  By default, False.
+    font_size_edges : int, optional
+        Font size for text labels, by default 10.
+    font_color_edges : str, optional
+        Font color string, by default "black".
     font_family_edges : str (default='sans-serif')
         Font family.
     font_weight_edges : str (default='normal')
         Font weight.
-    alpha_edges : float (default=None)
-        The text transparency.
-    bbox_edges : Matplotlib bbox (default={boxstyle='round', ec=(1.0, 1.0, 1.0), fc=(1.0, 1.0, 1.0)})
+    alpha_edges : float, optional
+        The text transparency, by default None.
+    bbox_edges : Matplotlib bbox, optional
         Specify text box properties (e.g. shape, color etc.) for edge labels.
-    horizontalalignment_edges : str (default='center')
+        By default, {boxstyle='round', ec=(1.0, 1.0, 1.0), fc=(1.0, 1.0, 1.0)}
+    horizontalalignment_edges : str, optional
         Horizontal alignment {'center', 'right', 'left'}.
-    verticalalignment_edges: str (default='center')
+        By default, "center".
+    verticalalignment_edges: str, optional
         Vertical alignment {'center', 'top', 'bottom', 'baseline', 'center_baseline'}.
-    ax_edges : matplotlib.pyplot.axes (default=None)
-        Draw the graph in the specified Matplotlib axes.
-    rotate_edges : bool (default=False)
-        Rotate edge labels for dyadic links to lie parallel to edges.
-    clip_on_edges: bool (default=True)
-        Turn on clipping of hyperedge labels at axis boundaries.
+        By default, "center".
+    ax_edges : matplotlib.pyplot.axes, optional
+        Draw the graph in the specified Matplotlib axes. By default, None.
+    rotate_edges : bool, optional
+        Rotate edge labels for dyadic links to lie parallel to edges, by default False.
+    clip_on_edges: bool, optional
+        Turn on clipping of hyperedge labels at axis boundaries, by default True.
 
     Returns
     -------
     dict
         `dict` of labels keyed by hyperedge id.
 
     See Also
     --------
     draw
     draw_nodes
     draw_hyperedges
     draw_simplices
     draw_node_labels
+
     """
     if ax_edges is None:
         ax = plt.gca()
     else:
         ax = ax_edges
 
     if hyperedge_labels is True:
@@ -1057,64 +1097,70 @@
 ):
     """Draw hypergraphs displaying the hyperedges of order k>1 as convex hulls
 
 
     Parameters
     ----------
     H : Hypergraph
-    pos : dict (default=None)
-        If passed, this dictionary of positions node_id:(x,y) is used for placing the nodes.
-        If None (default), use the `barycenter_spring_layout` to compute the positions.
-    ax : matplotlib.pyplot.axes (default=None)
-    dyad_color : str, dict, iterable, or EdgeStat (default='black')
-        Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
-        contain (edge_id: color_str) pairs.  If iterable, assume the colors are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
-        (specified with dyad_color_cmap) associated to it.
-    edge_fc : str, dict, iterable, or EdgeStat (default=None)
-        str, dict, iterable, or EdgeStat (default=None)
-        Color of the hyperedges of order k>1.  If str, use the same color for all hyperedges of order k>1.  If a dict, must
-        contain (edge_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the hyperedges are found in H.edges. If EdgeStat,
-        use the colormap specified with edge_fc_cmap. If None (default),
-        use the H.edges.size.
-    edge_ec : str, dict, iterable, or EdgeStat (default=None)
-        Color of the borders of the hyperdges of order k>1.  If str, use the same color for all edges. If a dict, must
-        contain (edge_id: color_str) pairs.  If iterable, assume the colors are
-        specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
-        (specified with edge_ec_cmap) associated to it. If None (default),
-        use the H.edges.size.
-    node_fc : node_fc : str, dict, iterable, or NodeStat (default='tab:blue')
+    pos : dict, optional
+        If passed, this dictionary of positions node_id:(x,y) is used for placing the
+        nodes.  If None (default), use the `barycenter_spring_layout` to compute the
+        positions.
+    ax : matplotlib.pyplot.axes, optional
+        Axis to draw on. If None (default), get the current axes.
+    dyad_color : str, dict, iterable, or EdgeStat, optional
+        Color of the dyadic links.  If str, use the same color for all edges. If a dict,
+        must contain (edge_id: color_str) pairs.  If iterable, assume the colors are
+        specified in the same order as the edges are found in H.edges. If EdgeStat, use
+        a colormap (specified with dyad_color_cmap) associated to it. By default,
+        "black".
+    edge_fc : str, dict, iterable, or EdgeStat, optional
+        Color of the hyperedges of order k>1.  If str, use the same color for all
+        hyperedges of order k>1.  If a dict, must contain (edge_id: color_str) pairs.
+        If other iterable, assume the colors are specified in the same order as the
+        hyperedges are found in H.edges. If EdgeStat, use the colormap specified with
+        edge_fc_cmap. If None (default), use the H.edges.size.
+    edge_ec : str, dict, iterable, or EdgeStat, optional
+        Color of the borders of the hyperdges of order k>1.  If str, use the same color
+        for all edges. If a dict, must contain (edge_id: color_str) pairs.  If iterable,
+        assume the colors are specified in the same order as the edges are found in
+        H.edges. If EdgeStat, use a colormap (specified with edge_ec_cmap) associated to
+        it. If None (default), use the H.edges.size.
+    node_fc : node_fc : str, dict, iterable, or NodeStat, optional
         Color of the nodes.  If str, use the same color for all nodes.  If a dict, must
         contain (node_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat,
-        use the colormap specified with node_fc_cmap.
-    node_ec : str, dict, iterable, or NodeStat (default='black')
-        Color of node borders.  If str, use the same color for all nodes.  If a dict, must
-        contain (node_id: color_str) pairs.  If other iterable, assume the colors are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat,
-        use the colormap specified with node_ec_cmap.
-    node_lw : int, float, dict, iterable, or EdgeStat (default=1)
-        Line width of the node borders in pixels.  If int or float, use the same width for all node borders.
-        If a dict, must contain (node_id: width) pairs.  If iterable, assume the widths are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
-        linear interpolation defined between min_node_lw and max_node_lw.
-    node_size : int, float, dict, iterable, or NodeStat (default=7)
-        Radius of the nodes in pixels.  If int or float, use the same radius for all nodes.
-        If a dict, must contain (node_id: radius) pairs.  If iterable, assume the radiuses are
-        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
-        linear interpolation defined between min_node_size and max_node_size.
-    max_order : int (default=None)
+        specified in the same order as the nodes are found in H.nodes. If NodeStat, use
+        the colormap specified with node_fc_cmap. By default, "tab:blue".
+    node_ec : str, dict, iterable, or NodeStat, optional
+        Color of node borders.  If str, use the same color for all nodes.  If a dict,
+        must contain (node_id: color_str) pairs.  If other iterable, assume the colors
+        are specified in the same order as the nodes are found in H.nodes. If NodeStat,
+        use the colormap specified with node_ec_cmap. By default, "black".
+    node_lw : int, float, dict, iterable, or EdgeStat, optional
+        Line width of the node borders in pixels.  If int or float, use the same width
+        for all node borders.  If a dict, must contain (node_id: width) pairs.  If
+        iterable, assume the widths are specified in the same order as the nodes are
+        found in H.nodes. If NodeStat, use a monotonic linear interpolation defined
+        between min_node_lw and max_node_lw. By default, 1.
+    node_size : int, float, dict, iterable, or NodeStat, optional
+        Radius of the nodes in pixels.  If int or float, use the same radius for all
+        nodes.  If a dict, must contain (node_id: radius) pairs.  If iterable, assume
+        the radiuses are specified in the same order as the nodes are found in
+        H.nodes. If NodeStat, use a monotonic linear interpolation defined between
+        min_node_size and max_node_size. By default, 7.
+    max_order : int, optional
         Maximum of hyperedges to plot. If None (default), plots all orders.
-    node_labels : bool, or dict (default=False)
+    node_labels : bool, or dict, optional
         If True, draw ids on the nodes. If a dict, must contain (node_id: label) pairs.
-    hyperedge_labels : bool, or dict (default=False)
-        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label) pairs.
-    radius : float (deafault=0.05)
-        Radius of the convex hull in the vicinity of the nodes.
+        By default, False
+    hyperedge_labels : bool, or dict, optional
+        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label)
+        pairs.  By default, False.
+    radius : float, optional
+        Radius of the convex hull in the vicinity of the nodes, by default 0.05.
     **kwargs : optional args
         Alternate default values. Values that can be overwritten are the following:
         * min_node_size
         * max_node_size
         * min_node_lw
         * max_node_lw
         * node_fc_cmap
@@ -1124,14 +1170,18 @@
         * edge_ec_cmap
         * alpha
 
     Returns
     -------
     ax : matplotlib.pyplot.axes
 
+    See Also
+    --------
+    draw
+
     """
 
     settings = {
         "min_node_size": 5.0,
         "max_node_size": 30.0,
         "min_node_lw": 1.0,
         "max_node_lw": 5.0,
```

### Comparing `xgi-0.5.7/xgi/drawing/layout.py` & `xgi-0.5.8/xgi/drawing/layout.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,47 +15,58 @@
     "barycenter_spring_layout",
     "weighted_barycenter_spring_layout",
     "pca_transform",
 ]
 
 
 def random_layout(H, center=None, dim=2, seed=None):
-    """Position nodes uniformly at random in the unit square. Exactly as networkx does.
-    For every node, a position is generated by choosing each of dim
-    coordinates uniformly at random on the interval [0.0, 1.0).
-    NumPy (http://scipy.org) is required for this function.
+    """Position nodes uniformly at random in the unit square.
+
+    For every node, a position is generated by choosing each of dim coordinates
+    uniformly at random on the interval [0.0, 1.0).  NumPy (http://scipy.org) is
+    required for this function.
 
     Parameters
     ----------
-    H : HyperGraph or list of nodes
+    H : Hypergraph or SimplicialComplex
         A position will be assigned to every node in HG.
-    center : array-like or None
+    center : array-like, optional
         Coordinate pair around which to center the layout.
-    dim : int
-        Dimension of layout.
-    seed : int, RandomState instance or None  optional (default=None)
+        If None (default), does not center the positions.
+    dim : int, optional
+        Dimension of layout, by default 2.
+    seed : int, optional
         Set the random state for deterministic node layouts.
         If int, `seed` is the seed used by the random number generator,
-        if numpy.random.RandomState instance, `seed` is the random
-        number generator,
-        if None, the random number generator is the RandomState instance used
-        by numpy.random.
+        If None (default), random numbers are sampled from the
+        numpy random number generator without initialization.
 
     Returns
     -------
     pos : dict
         A dictionary of positions keyed by node
 
+    See Also
+    --------
+    pairwise_spring_layout
+    barycenter_spring_layout
+    weighted_barycenter_spring_layout
+
+    Notes
+    -----
+    This function proceeds exactly as NetworkX does.
+
     Examples
     --------
     >>> import xgi
     >>> N = 50
     >>> ps = [0.1, 0.01]
     >>> H = xgi.random_hypergraph(N, ps)
     >>> pos = xgi.random_layout(H)
+
     """
     import numpy as np
 
     if isinstance(H, SimplicialComplex):
         H = convert.from_max_simplices(H)
 
     if seed is not None:
@@ -75,37 +86,36 @@
     algorithm using the graph projection of the hypergraph
     or the hypergraph constructed from the simplicial complex.
 
     Parameters
     ----------
     H : Hypergraph or SimplicialComplex
         A position will be assigned to every node in H.
-    seed : int, RandomState instance or None  optional (default=None)
+    seed : int, optional
         Set the random state for deterministic node layouts.
         If int, `seed` is the seed used by the random number generator,
-        if numpy.random.RandomState instance, `seed` is the random
-        number generator,
-        if None, the random number generator is the RandomState instance used
-        by numpy.random.
+        If None (default), random numbers are sampled from the
+        numpy random number generator without initialization.
 
     Returns
     -------
     pos : dict
         A dictionary of positions keyed by node
 
+    See Also
+    --------
+    random_layout
+    barycenter_spring_layout
+    weighted_barycenter_spring_layout
+
     Notes
     -----
     If a simplicial complex is provided the results will be based on the
     hypergraph constructed from its maximal simplices.
 
-    See also
-    --------
-    barycenter_spring_layout
-    weighted_barycenter_spring_layout
-
     Examples
     --------
     >>> import xgi
     >>> N = 50
     >>> ps = [0.1, 0.01]
     >>> H = xgi.random_hypergraph(N, ps)
     >>> pos = xgi.pairwise_spring_layout(H)
@@ -130,29 +140,28 @@
     If a simplicial complex is provided the results will be based on the
     hypergraph constructed from its maximal simplices.
 
     Parameters
     ----------
     H : xgi Hypergraph or SimplicialComplex
         A position will be assigned to every node in H.
-    seed : int, RandomState instance or None  optional (default=None)
+    seed : int, optional
         Set the random state for deterministic node layouts.
         If int, `seed` is the seed used by the random number generator,
-        if numpy.random.RandomState instance, `seed` is the random
-        number generator,
-        if None, the random number generator is the RandomState instance used
-        by numpy.random.
+        If None (default), random numbers are sampled from the
+        numpy random number generator without initialization.
 
     Returns
     -------
     pos : dict
         A dictionary of positions keyed by node
 
-    See also
+    See Also
     --------
+    random_layout
     pairwise_spring_layout
     weighted_barycenter_spring_layout
 
     Examples
     --------
     >>> import xgi
     >>> N = 50
@@ -169,15 +178,16 @@
 
     # Creating the projected networkx Graph, I will fill it manually
     G = nx.Graph()
 
     # Adding real nodes
     G.add_nodes_from(list(H.nodes))
 
-    # Adding links (edges composed by two nodes only, for which we don't use phantom nodes
+    # Adding links (edges composed by two nodes only),
+    # for which we don't use phantom nodes
     for i, j in H.edges.filterby("order", 1).members():
         G.add_edge(i, j)
 
     # Adding phantom nodes and connections therein
     # I will start from the first int node-label available
     try:
         phantom_node_id = max([n for n in H.nodes if isinstance(n, int)]) + 1
@@ -185,86 +195,88 @@
         # The list of node-labels has no integers, so I start from 0
         phantom_node_id = 0
 
     # Looping over the hyperedges of different order (from triples up)
     for d in range(2, max_edge_order(H) + 1):
         # Hyperedges of order d (d=2: triplets, etc.)
         for he in H.edges.filterby("order", d).members():
-            # Adding one phantom node for each hyperedge and linking it to the nodes of the hyperedge
+            # Adding one phantom node for each hyperedge and linking it to the nodes of
+            # the hyperedge
             for n in he:
                 G.add_edge(phantom_node_id, n)
             phantom_node_id += 1
 
-    # Creating a dictionary for the position of the nodes with the standard spring layout
+    # Creating a dictionary for the position of the nodes with the standard spring
+    # layout
     pos_with_phantom_nodes = nx.spring_layout(G, seed=seed)
 
     # Retaining only the positions of the real nodes
     pos = {k: pos_with_phantom_nodes[k] for k in list(H.nodes)}
 
     if return_phantom_graph:
         return pos, G
     else:
         return pos
 
 
 def weighted_barycenter_spring_layout(H, return_phantom_graph=False, seed=None):
-    """
-    Position the nodes using Fruchterman-Reingold force-directed
-    algorithm using an augmented version of the the graph projection
-    of the hypergraph (or simplicial complex), where phantom nodes (barycenters) are created
-    for each edge of order d>1 (composed by more than two nodes).
-    Weights are assigned to all hyperedges of order 1 (links) and
-    to all connections to phantom nodes within each hyperedge
-    to keep them together. Weights scale as the order d.
-    If a simplicial complex is provided the results will be based on the
-    hypergraph constructed from its maximal simplices.
+    """Position the nodes using Fruchterman-Reingold force-directed algorithm.
+
+    This uses an augmented version of the the graph projection of the hypergraph (or
+    simplicial complex), where phantom nodes (barycenters) are created for each edge of
+    order d>1 (composed by more than two nodes).  Weights are assigned to all hyperedges
+    of order 1 (links) and to all connections to phantom nodes within each hyperedge to
+    keep them together. Weights scale as the order d.  If a simplicial complex is
+    provided the results will be based on the hypergraph constructed from its maximal
+    simplices.
 
     Parameters
     ----------
     H : Hypergraph or SimplicialComplex
         A position will be assigned to every node in H.
-    seed : int, RandomState instance or None  optional (default=None)
+    seed : int, optional
         Set the random state for deterministic node layouts.
         If int, `seed` is the seed used by the random number generator,
-        if numpy.random.RandomState instance, `seed` is the random
-        number generator,
-        if None, the random number generator is the RandomState instance used
-        by numpy.random.
+        If None (default), random numbers are sampled from the
+        numpy random number generator without initialization.
 
     Returns
     -------
     pos : dict
         A dictionary of positions keyed by node
 
-    See also
+    See Also
     --------
+    random_layout
     pairwise_spring_layout
     barycenter_spring_layout
 
     Examples
     --------
     >>> import xgi
     >>> N = 50
     >>> ps = [0.1, 0.01]
     >>> H = xgi.random_hypergraph(N, ps)
     >>> pos = xgi.weighted_barycenter_spring_layout(H)
+
     """
     if seed is not None:
         random.seed(seed)
 
     if isinstance(H, SimplicialComplex):
         H = convert.from_max_simplices(H)
 
     # Creating the projected networkx Graph, I will fill it manually
     G = nx.Graph()
 
     # Adding real nodes
     G.add_nodes_from(list(H.nodes))
 
-    # Adding links (edges composed by two nodes only, for which we don't use phantom nodes)
+    # Adding links (edges composed by two nodes only),
+    # for which we don't use phantom nodes.
     d = 1
     for i, j in H.edges.filterby("order", d).members():
         G.add_edge(i, j, weight=d)
 
     # Adding phantom nodes and connections therein
     # I will start from the first int node-label available
     try:
@@ -273,20 +285,21 @@
         # The list of node-labels has no integers, so I start from 0
         phantom_node_id = 0
 
     # Looping over the hyperedges of different order (from triples up)
     for d in range(2, max_edge_order(H) + 1):
         # Hyperedges of order d (d=2: triplets, etc.)
         for he_id, members in H.edges.filterby("order", d).members(dtype=dict).items():
-            # Adding one phantom node for each hyperedge and linking it to the nodes of the hyperedge
+            # Adding one phantom node for each hyperedge and linking it to the nodes of
+            # the hyperedge
             for n in members:
                 G.add_edge(phantom_node_id, n, weight=d)
             phantom_node_id += 1
 
-    # Creating a dictionary for the position of the nodes with the standard spring layout
+    # Creating a dictionary for node position with the standard spring layout
     pos_with_phantom_nodes = nx.spring_layout(G, weight="weight", seed=seed)
 
     # Retaining only the positions of the real nodes
     pos = {k: pos_with_phantom_nodes[k] for k in list(H.nodes)}
 
     if return_phantom_graph:
         return pos, G
@@ -302,20 +315,28 @@
     ----------
     pos : dict of numpy arrays
         The output from any layout function
     theta : float, optional
         The angle between the horizontal axis and the principal axis
         measured counterclockwise, by default 0.
     degrees : bool, optional
-        Whether the angle specified is in degrees (True) or in radians (False), by default True.
+        Whether the angle specified is in degrees (True)
+        or in radians (False), by default True.
 
     Returns
     -------
-    dict of nump arrays
+    dict of numpy arrays
         The transformed positions.
+
+    See Also
+    --------
+    random_layout
+    pairwise_spring_layout
+    barycenter_spring_layout
+    weighted_barycenter_spring_layout
     """
     p = np.array(list(pos.values()))
     _, _, w = svd(p)
 
     pa = inv(w)
 
     if degrees:
```

### Comparing `xgi-0.5.7/xgi/dynamics/synchronization.py` & `xgi-0.5.8/xgi/dynamics/synchronization.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,19 @@
     H : Hypergraph object
         The hypergraph on which you run the Kuramoto model
     k2 : float
         The coupling strength for links
     k3 : float
         The coupling strength for triangles
     omega : numpy array of real values
-        The natural frequency of the nodes. If None (default), randomly drawn from a normal distribution
+        The natural frequency of the nodes. If None (default), randomly drawn from a
+        normal distribution
     theta : numpy array of real values
-        The initial phase distribution of nodes. If None (default), drawn from a random uniform distribution
-        on [0, 2pi[.
+        The initial phase distribution of nodes. If None (default), drawn from a random
+        uniform distribution on [0, 2pi[.
     timesteps : int greater than 1, default: 10000
         The number of timesteps for Euler Method.
     dt : float greater than 0, default: 0.002
         The size of timesteps for Euler Method.
 
     Returns
     -------
@@ -106,16 +107,17 @@
         theta_new = theta + d_theta * dt
         theta = theta_new
 
     return theta_time, times
 
 
 def compute_kuramoto_order_parameter(theta_time):
-    """This function calculates the order parameter for the Kuramoto model on hypergraphs,
-    from time series, which is a measure of synchrony.
+    """Calculate the order parameter for the Kuramoto model on hypergraphs.
+
+    Calculation proceeds from time series, and the output is a measure of synchrony.
 
     Parameters
     ----------
     theta_time: numpy array of floats
         Timeseries of phases from the Kuramoto model, of dimension (T, N)
 
     Returns
@@ -138,17 +140,16 @@
     omega=[],
     sigma=1,
     theta0=[],
     T=10,
     n_steps=10000,
     index=False,
 ):
-    """
-    This function simulates the simplicial Kuramoto model's dynamics on an oriented simplicial complex
-    using explicit Euler numerical integration scheme.
+    """Simulate the simplicial Kuramoto model's dynamics on an oriented simplicial
+    complex using explicit Euler numerical integration scheme.
 
     Parameters
     ----------
     S: simplicial complex object
         The simplicial complex on which you
         run the simplicial Kuramoto model
     orientations: dict, Default : None
@@ -162,18 +163,18 @@
         The coupling strength
     theta0: numpy.ndarray
         The initial phase distribution, has dimension
         (n_simplices of given order, 1)
     T: positive real value
         The final simulation time.
     n_steps: integer greater than 1
-        The number of integration timesteps for
-        the explicit Euler method.
+        The number of integration timesteps for the explicit Euler method.
     index: bool, default: False
-        Specifies whether to output dictionaries mapping the node and edge IDs to indices
+        Specifies whether to output dictionaries mapping the node and edge IDs to
+        indices.
 
     Returns
     -------
     theta: numpy.ndarray
         Timeseries of the simplicial oscillators' phases, has dimension
         (n_simplices of given order, n_steps)
     theta_minus: numpy array of floats
@@ -201,15 +202,16 @@
     # B_o - boundary matrix acting on (order)-simplices
     # D_o - adjoint boundary matrix acting on (order)-simplices
     # om1 = order - 1
     # op1 = order + 1
 
     if not isinstance(S, xgi.SimplicialComplex):
         raise XGIError(
-            "The simplicial Kuramoto model can be simulated only on a SimplicialComplex object"
+            "The simplicial Kuramoto model can be simulated "
+            "only on a SimplicialComplex object"
         )
 
     if index:
         B_o, om1_dict, o_dict = boundary_matrix(S, order, orientations, True)
     else:
         B_o = boundary_matrix(S, order, orientations, False)
     D_om1 = np.transpose(B_o)
```

### Comparing `xgi-0.5.7/xgi/generators/lattice.py` & `xgi-0.5.8/xgi/generators/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,17 @@
     Raises
     ------
     XGIError
         If k is negative.
 
     Notes
     -----
-    ring_lattice(n, 2, k, 0) is a ring lattice graph where each node has k//2 edges on either
-    side.
+    ring_lattice(n, 2, k, 0) is a ring lattice graph where each node has k//2 edges on
+    either side.
+
     """
     from ..classes import Hypergraph
 
     if k < 0:
         raise XGIError("Invalid k value!")
 
     if k < 2:
```

### Comparing `xgi-0.5.7/xgi/generators/random.py` & `xgi-0.5.8/xgi/generators/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,24 +248,25 @@
     if seed is not None:
         random.seed(seed)
 
     # sort dictionary by degree in decreasing order
     node_labels = [n for n, _ in sorted(k1.items(), key=lambda d: d[1], reverse=True)]
     edge_labels = [m for m, _ in sorted(k2.items(), key=lambda d: d[1], reverse=True)]
 
-    # these checks verify that the sum of node and edge degrees and the sum of node degrees
-    # and the sum of community connection matrix differ by less than a single edge.
+    # Verify that the sum of node and edge degrees and the sum of node degrees and the
+    # sum of community connection matrix differ by less than a single edge.
     if abs(sum(k1.values()) - sum(k2.values())) > 1:
         warnings.warn(
             "The sum of the degree sequence does not match the sum of the size sequence"
         )
 
     if abs(sum(k1.values()) - np.sum(omega)) > 1:
         warnings.warn(
-            "The sum of the degree sequence does not match the entries in the omega matrix"
+            "The sum of the degree sequence does not "
+            "match the entries in the omega matrix"
         )
 
     # get indices for each community
     community1_nodes = defaultdict(list)
     for label in node_labels:
         group = g1[label]
         community1_nodes[group].append(label)
```

### Comparing `xgi-0.5.7/xgi/generators/simple.py` & `xgi-0.5.8/xgi/generators/simple.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/xgi/generators/simplicial_complexes.py` & `xgi-0.5.8/xgi/generators/simplicial_complexes.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from itertools import combinations
 
 import networkx as nx
 import numpy as np
 from scipy.special import comb
 
 from ..classes import SimplicialComplex
-from ..classes.function import subfaces
 from ..utils.utilities import find_triangles
 
 __all__ = [
     "random_simplicial_complex",
     "random_flag_complex_d2",
     "random_flag_complex",
     "flag_complex",
@@ -126,34 +125,29 @@
     # defined.  Otherwise, a circular import error would happen.
     from ..classes import SimplicialComplex
 
     if seed is not None:
         random.seed(seed)
 
     nodes = G.nodes()
+    N = len(nodes)
     edges = G.edges()
 
-    # compute all maximal cliques to fill
-    max_cliques = list(nx.find_cliques(G))
+    cliques_to_add = _cliques_to_fill(G, max_order)
 
     S = SimplicialComplex()
     S.add_nodes_from(nodes)
     S.add_simplices_from(edges)
     if not ps:  # promote all cliques
-        S.add_simplices_from(max_cliques, max_order=max_order)
+        S.add_simplices_from(cliques_to_add, max_order=max_order)
         return S
 
-    if max_order:  # compute subfaces of order max_order (allowed max cliques)
-        max_cliques_to_add = subfaces(max_cliques, order=max_order)
-    else:
-        max_cliques_to_add = max_cliques
-
     # store max cliques per order
     cliques_d = defaultdict(list)
-    for x in max_cliques_to_add:
+    for x in cliques_to_add:
         cliques_d[len(x)].append(x)
 
     # promote cliques with a given probability
     for i, p in enumerate(ps[: max_order - 1]):
         d = i + 2  # simplex order
         cliques_d_to_add = [el for el in cliques_d[d + 1] if random.random() <= p]
         S.add_simplices_from(cliques_d_to_add, max_order=max_order)
@@ -210,16 +204,18 @@
 
     S.add_simplices_from(triangles)
 
     return S
 
 
 def random_flag_complex_d2(N, p, seed=None):
-    """Generate a maximal simplicial complex (up to order 2) from a
-    :math:`G_{N,p}` Erdős-Rényi random graph by filling all empty triangles with 2-simplices.
+    """Generate a maximal simplicial complex (up to order 2) from a :math:`G_{N,p}`
+    Erdős-Rényi random graph.
+
+    This proceeds by filling all empty triangles in the graph with 2-simplices.
 
     Parameters
     ----------
     N : int
         Number of nodes
     p : float
         Probabilities (between 0 and 1) to create an edge
@@ -230,29 +226,32 @@
     Returns
     -------
     SimplicialComplex
 
     Notes
     -----
     Computing all cliques quickly becomes heavy for large networks.
+
     """
     if seed is not None:
         random.seed(seed)
 
     if (p < 0) or (p > 1):
         raise ValueError("p must be between 0 and 1 included.")
 
     G = nx.fast_gnp_random_graph(N, p, seed=seed)
 
     return flag_complex_d2(G)
 
 
 def random_flag_complex(N, p, max_order=2, seed=None):
     """Generate a flag (or clique) complex from a
-    :math:`G_{N,p}` Erdős-Rényi random graph by filling all cliques up to dimension max_order.
+    :math:`G_{N,p}` Erdős-Rényi random graph.
+
+    This proceeds by filling all cliques up to dimension max_order.
 
     Parameters
     ----------
     N : int
         Number of nodes
     p : float
         Probability (between 0 and 1) to create an edge
@@ -265,25 +264,59 @@
     Returns
     -------
     SimplicialComplex
 
     Notes
     -----
     Computing all cliques quickly becomes heavy for large networks.
-    """
 
+    """
     if (p < 0) or (p > 1):
         raise ValueError("p must be between 0 and 1 included.")
 
     G = nx.fast_gnp_random_graph(N, p, seed=seed)
 
     nodes = G.nodes()
-    edges = list(G.edges())
 
-    # compute all triangles to fill
-    max_cliques = list(nx.find_cliques(G))
+    cliques = _cliques_to_fill(G, max_order)
 
     S = SimplicialComplex()
     S.add_nodes_from(nodes)
-    S.add_simplices_from(max_cliques, max_order=max_order)
+    S.add_simplices_from(cliques, max_order=max_order)
 
     return S
+
+
+def _cliques_to_fill(G, max_order):
+    """Return cliques to fill for flag complexes,
+    to be passed to `add_simplices_from`.
+
+    This function was written to speedup flag_complex functions
+    by avoiding adding redundant faces.
+
+    Parameters
+    ----------
+    G : networkx Graph
+        Graph to consider
+    max_order: int or None
+        If None, return maximal cliques. If int, return all cliques
+        up to max_order.
+
+    Returns
+    -------
+    cliques : list
+        List of cliques
+
+    """
+    if max_order is None:
+        cliques = list(nx.find_cliques(G))  # max cliques
+    else:  # avoid adding many unnecessary redundant cliques
+        cliques = []
+        for clique in nx.enumerate_all_cliques(G):  # sorted by size
+            if len(clique) == 1:
+                continue  # don't add singletons
+            if len(clique) <= max_order + 1:
+                cliques.append(clique)
+            else:
+                break  # dont go over whole list if not necessary
+
+    return cliques
```

### Comparing `xgi-0.5.7/xgi/generators/uniform.py` & `xgi-0.5.8/xgi/generators/uniform.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,16 @@
     if seed is not None:
         random.seed(seed)
 
     # Making sure we have the right number of stubs
     remainder = sum(k.values()) % m
     if remainder != 0:
         warnings.warn(
-            "This degree sequence is not realizable. Increasing the degree of random nodes so that it is."
+            "This degree sequence is not realizable. "
+            "Increasing the degree of random nodes so that it is."
         )
         random_ids = random.sample(list(k.keys()), int(round(m - remainder)))
         for id in random_ids:
             k[id] = k[id] + 1
 
     stubs = []
     # Creating the list to index through
@@ -361,15 +362,16 @@
     -------
     list
         The reconstructed hyperedge
 
     See Also
     --------
     _index_to_edge
+
     """
     try:
         return [
             int(index // np.prod(partition_sizes[r + 1 :]) % partition_sizes[r])
             for r in range(m)
         ]
-    except:
+    except KeyError:
         raise Exception("Invalid parameters")
```

### Comparing `xgi-0.5.7/xgi/linalg/hodge_matrix.py` & `xgi-0.5.8/xgi/linalg/hodge_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,18 @@
 __all__ = [
     "boundary_matrix",
     "hodge_laplacian",
 ]
 
 
 def boundary_matrix(S, order=1, orientations=None, index=False):
-    """
-    A function to generate the boundary matrices of an oriented simplicial complex.
-    The rows correspond to the (order-1)-simplices and the columns to the (order)-simplices.
+    """Generate the boundary matrices of an oriented simplicial complex.
+
+    The rows correspond to the (order-1)-simplices and the columns to the
+    (order)-simplices.
 
     Parameters
     ----------
     S: simplicial complex object
         The simplicial complex of interest
     order: int, default: 1
         Specifies the order of the boundary
@@ -118,16 +119,16 @@
         if order == 1:
             for u_simplex_id in simplices_u_ids:
                 u_simplex = list(S.edges.members(u_simplex_id))
                 u_simplex.sort(
                     key=lambda e: (isinstance(e, str), e)
                 )  # Sort the simplex's vertices to get a reference orientation
                 # The key is needed to sort a mixed list of numbers and strings:
-                #   it ensures that node labels which are numbers are put before strings,
-                #   thus giving a list [sorted numbers, sorted strings]
+                #   it ensures that node labels which are numbers are put before
+                #   strings, thus giving a list [sorted numbers, sorted strings]
                 matrix_id = simplices_u_dict[u_simplex_id]
                 head_idx = u_simplex[1]
                 tail_idx = u_simplex[0]
                 B[simplices_d_dict[head_idx], matrix_id] = (-1) ** orientations[
                     u_simplex_id
                 ]
                 B[simplices_d_dict[tail_idx], matrix_id] = -(
@@ -136,16 +137,16 @@
         else:
             for u_simplex_id in simplices_u_ids:
                 u_simplex = list(S.edges.members(u_simplex_id))
                 u_simplex.sort(
                     key=lambda e: (isinstance(e, str), e)
                 )  # Sort the simplex's vertices to get a reference orientation
                 # The key is needed to sort a mixed list of numbers and strings:
-                #   it ensures that node labels which are numbers are put before strings,
-                #   thus giving a list [sorted numbers, sorted strings]
+                #   it ensures that node labels which are numbers are put before
+                #   strings, thus giving a list [sorted numbers, sorted strings]
                 matrix_id = simplices_u_dict[u_simplex_id]
                 u_simplex_subfaces = S._subfaces(u_simplex, all=False)
                 subfaces_induced_orientation = [
                     (orientations[u_simplex_id] + order - i) % 2
                     for i in range(order + 1)
                 ]
                 for count, subf in enumerate(u_simplex_subfaces):
```

### Comparing `xgi-0.5.7/xgi/linalg/hypergraph_matrix.py` & `xgi-0.5.8/xgi/linalg/hypergraph_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,29 +56,29 @@
     "clique_motif_matrix",
 ]
 
 
 def incidence_matrix(
     H, order=None, sparse=True, index=False, weight=lambda node, edge, H: 1
 ):
-    """
-    A function to generate a weighted incidence matrix from a Hypergraph object,
+    """A function to generate a weighted incidence matrix from a Hypergraph object,
     where the rows correspond to nodes and the columns correspond to edges.
 
     Parameters
     ----------
     H: Hypergraph object
         The hypergraph of interest
     order: int, optional
         Order of interactions to use. If None (default), all orders are used. If int,
         must be >= 1.
     sparse: bool, default: True
         Specifies whether the output matrix is a scipy sparse matrix or a numpy matrix
     index: bool, default: False
-        Specifies whether to output dictionaries mapping the node and edge IDs to indices
+        Specifies whether to output dictionaries mapping the node and edge IDs to
+        indices.
     weight: lambda function, default=lambda function outputting 1
         A function specifying the weight, given a node and edge
 
     Returns
     -------
     I: numpy.ndarray or scipy csr_array
         The incidence matrix, has dimension (n_nodes, n_edges)
@@ -175,15 +175,16 @@
     A = I.dot(I.T)
 
     if sparse:
         with catch_warnings(record=True) as w:
             A.setdiag(0)
         if w:
             warn(
-                "Forming the adjacency matrix can be expensive when there are isolated nodes!"
+                "Forming the adjacency matrix can "
+                "be expensive when there are isolated nodes!"
             )
     else:
         np.fill_diagonal(A, 0)
 
     if not weighted:
         A = (A >= s) * 1
     else:
@@ -215,46 +216,47 @@
     -------
     if index is True:
         return P, rowdict, coldict
     else:
         return P
 
     """
-    I, _, coldict = incidence_matrix(H, order=order, sparse=sparse, index=True)
-    P = I.T.dot(I)
+    eye, _, coldict = incidence_matrix(H, order=order, sparse=sparse, index=True)
+    P = eye.T.dot(eye)
     return (P, coldict) if index else P
 
 
 def degree_matrix(H, order=None, index=False):
     """Returns the degree of each node as an array
 
     Parameters
     ----------
     H: Hypergraph object
         The hypergraph of interest
     order: int, optional
         Order of interactions to use. If None (default), all orders are used. If int,
         must be >= 1.
     index: bool, default: False
-        Specifies whether to output disctionaries mapping the node and edge IDs to indices
+        Specifies whether to output disctionaries mapping the node and edge IDs to
+        indices.
 
     Returns
     -------
     if index is True:
         return K, rowdict
     else:
         return K
 
     """
-    I, rowdict, _ = incidence_matrix(H, order=order, index=True)
+    eye, rowdict, _ = incidence_matrix(H, order=order, index=True)
 
-    if I.shape == (0, 0):
+    if eye.shape == (0, 0):
         K = np.zeros(H.num_nodes)
     else:
-        K = np.ravel(np.sum(I, axis=1))  # flatten
+        K = np.ravel(np.sum(eye, axis=1))  # flatten
 
     return (K, rowdict) if index else K
 
 
 def clique_motif_matrix(H, sparse=True, index=False):
     """
     A function to generate a weighted clique motif matrix
```

### Comparing `xgi-0.5.7/xgi/linalg/laplacian_matrix.py` & `xgi-0.5.8/xgi/linalg/laplacian_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,20 @@
 
     Parameters
     ----------
     HG : Hypergraph
         Hypergraph
     order : int
         Order of interactions to consider. If order=1 (default),
-        returns the usual graph Laplacian
+        returns the usual graph Laplacian.
     sparse: bool, default: False
-        Specifies whether the output matrix is a scipy sparse matrix or a numpy matrix
+        Specifies whether the output matrix is a scipy sparse matrix or a numpy matrix.
     index: bool, default: False
-        Specifies whether to output disctionaries mapping the node and edge IDs to indices
+        Specifies whether to output disctionaries mapping the node and edge IDs to
+        indices.
 
     Returns
     -------
     L_d : numpy array
         Array of dim (N, N)
     if index is True:
         return rowdict
@@ -126,15 +127,16 @@
     weights: list of float
         Weights associated to each order, i.e coupling strengths gamma_i in [1].
     sparse: bool, default: False
         Specifies whether the output matrix is a scipy sparse matrix or a numpy matrix
     rescale_per_node: bool, (default=False)
         Whether to rescale each Laplacian of order d by d (per node).
     index: bool, default: False
-        Specifies whether to output dictionaries mapping the node and edge IDs to indices
+        Specifies whether to output dictionaries mapping the node and edge IDs to
+        indices.
 
     Returns
     -------
     L_multi : numpy array
         Array of dim (N, N)
     if index is True:
         return rowdict
@@ -165,15 +167,16 @@
         L_multi = np.zeros((H.num_nodes, H.num_nodes))
 
     for L, K, w, d in zip(Ls, Ks, weights, orders):
         if np.all(K == 0):
             # avoid getting nans from dividing by 0
             # manually setting contribution to 0 as it should be
             warn(
-                f"No edges of order {d}. Contribution of that order is zero. Its weight is effectively zero."
+                f"No edges of order {d}. Contribution of "
+                "that order is zero. Its weight is effectively zero."
             )
         else:
             L_multi += L * w / np.mean(K)
 
     rowdict = {i: v for i, v in enumerate(H.nodes)}
 
     return (L_multi, rowdict) if index else L_multi
@@ -206,29 +209,27 @@
         If there are isolated nodes.
 
     References
     ----------
     "Learning with Hypergraphs: Clustering, Classification, and Embedding"
     by Dengyong Zhou, Jiayuan Huang, Bernhard Schölkopf
     Advances in Neural Information Processing Systems (2006)
-    """
-
-    from ..algorithms import is_connected
 
+    """
     if H.nodes.isolates():
         raise XGIError(
             "Every node must be a member of an edge to avoid divide by zero error!"
         )
 
     D = degree_matrix(H)
     A, rowdict = clique_motif_matrix(H, sparse=sparse, index=True)
 
     if sparse:
         Dinvsqrt = csr_array(diags(np.power(D, -0.5)))
-        I = csr_array((H.num_nodes, H.num_nodes))
-        I.setdiag(1)
+        eye = csr_array((H.num_nodes, H.num_nodes))
+        eye.setdiag(1)
     else:
         Dinvsqrt = np.diag(np.power(D, -0.5))
-        I = np.eye(H.num_nodes)
+        eye = np.eye(H.num_nodes)
 
-    L = 0.5 * (I - Dinvsqrt @ A @ Dinvsqrt)
+    L = 0.5 * (eye - Dinvsqrt @ A @ Dinvsqrt)
     return (L, rowdict) if index else L
```

### Comparing `xgi-0.5.7/xgi/readwrite/bipartite.py` & `xgi-0.5.8/xgi/readwrite/bipartite.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,25 +192,27 @@
 
         # convert node types
         if nodetype is not None:
             try:
                 node = nodetype(s[node_index])
             except ValueError as e:
                 raise TypeError(
-                    f"Failed to convert the node with ID {s[node_index]} to type {nodetype}."
+                    "Failed to convert the node with "
+                    f"ID {s[node_index]} to type {nodetype}."
                 ) from e
         else:
             node = s[node_index]
 
         # convert edge types
         if edgetype is not None:
             try:
                 edge = edgetype(s[edge_index])
             except ValueError as e:
                 raise TypeError(
-                    f"Failed to convert the edge with ID {s[edge_index]} to type {edgetype}."
+                    "Failed to convert the edge with "
+                    f"ID {s[edge_index]} to type {edgetype}."
                 ) from e
         else:
             edge = s[edge_index]
 
         H.add_node_to_edge(edge, node)
     return H
```

### Comparing `xgi-0.5.7/xgi/readwrite/edgelist.py` & `xgi-0.5.8/xgi/readwrite/edgelist.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/xgi/readwrite/incidence.py` & `xgi-0.5.8/xgi/readwrite/incidence.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,9 +74,9 @@
     Examples
     --------
     >>> import xgi
     >>> H = xgi.random_hypergraph(50, [0.01, 0.001])
     >>> # xgi.write_incidence_matrix(H, "test.csv", delimiter=",")
 
     """
-    I = incidence_matrix(H, sparse=False)
-    np.savetxt(path, I, delimiter=delimiter, newline="\n", encoding=encoding)
+    eye = incidence_matrix(H, sparse=False)
+    np.savetxt(path, eye, delimiter=delimiter, newline="\n", encoding=encoding)
```

### Comparing `xgi-0.5.7/xgi/readwrite/json.py` & `xgi-0.5.8/xgi/readwrite/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,32 +18,32 @@
     path: string
         The path of the file to read from
 
     """
     # initialize empty data
     data = {}
 
-    # get overall hypergraph attributes, name always gets written (default is an empty string)
-    data["hypergraph-data"] = dict()
+    # name always gets written (default is an empty string)
+    data["hypergraph-data"] = {}
     data["hypergraph-data"].update(H._hypergraph)
 
     # get node data
     try:
-        data["node-data"] = {str(id): H.nodes[id] for id in H.nodes}
-    except:
+        data["node-data"] = {str(idx): H.nodes[idx] for idx in H.nodes}
+    except KeyError:
         raise XGIError("Node attributes not saved!")
 
     try:
-        data["edge-data"] = {str(id): H.edges[id] for id in H.edges}
-    except:
+        data["edge-data"] = {str(idx): H.edges[idx] for idx in H.edges}
+    except KeyError:
         raise XGIError("Edge attributes not saved!")
 
     # hyperedge dict
     data["edge-dict"] = {
-        str(id): [str(n) for n in H.edges.members(id)] for id in H.edges
+        str(idx): [str(n) for n in H.edges.members(idx)] for idx in H.edges
     }
 
     datastring = json.dumps(data, indent=2)
 
     with open(path, "w") as output_file:
         output_file.write(datastring)
```

### Comparing `xgi-0.5.7/xgi/readwrite/xgi_data.py` & `xgi-0.5.8/xgi/readwrite/xgi_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,17 @@
             data = json.load(open(cfp, "r"))
 
             return convert.dict_to_hypergraph(
                 data, nodetype=nodetype, edgetype=edgetype, max_order=max_order
             )
         else:
             warn(
-                f"No local copy was found at {cfp}. The data is requested from the xgi-data repository instead. To download a local copy, use `download_xgi_data`."
+                f"No local copy was found at {cfp}. The data is requested "
+                "from the xgi-data repository instead. To download a local "
+                "copy, use `download_xgi_data`."
             )
     if cache:
         data = _request_from_xgi_data_cached(dataset)
     else:
         data = _request_from_xgi_data(dataset)
 
     return convert.dict_to_hypergraph(
```

### Comparing `xgi-0.5.7/xgi/stats/__init__.py` & `xgi-0.5.8/xgi/stats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,14 @@
 
 Many other features are available, including edge-statistics, and user-defined
 statistics.  For more details, see the `tutorial
 <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
 """
 
-from collections import defaultdict
-from typing import Callable
-
 import numpy as np
 import pandas as pd
 from scipy.stats import moment as spmoment
 
 from xgi.exception import IDNotFound
 
 from . import edgestats, nodestats
@@ -67,18 +64,18 @@
         self.args = () if args is None else args
         self.kwargs = {} if args is None else kwargs
         self.func = func
 
     def __call__(self, *args, **kwargs):
         return self.__class__(self.net, self.view, self.func, args=args, kwargs=kwargs)
 
-    def __getitem__(self, id):
-        if id not in self.view:
-            raise IDNotFound(f'ID "{id}" not in this view')
-        return self.func(self.net, [id], *self.args, **self.kwargs)[id]
+    def __getitem__(self, idx):
+        if idx not in self.view:
+            raise IDNotFound(f'ID "{idx}" not in this view')
+        return self.func(self.net, [idx], *self.args, **self.kwargs)[idx]
 
     def __repr__(self):
         cls = self.__class__.__name__
         fnc = self.func.__name__
         out = f"{cls}('{fnc}'"
         if self.args:
             out += f", args={self.args}"
@@ -351,15 +348,16 @@
         -----
         Equivalent to `np.array(self.aslist(inner=list))`.
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
-        >>> H.nodes.multi(['degree', 'clustering_coefficient']).asnumpy()  # doctest: +NORMALIZE_WHITESPACE
+        >>> H.nodes.multi(['degree', 'clustering_coefficient']).asnumpy()
+        ... # doctest: +NORMALIZE_WHITESPACE
         array([[1.        , 1.        ],
                [2.        , 0.66666667],
                [3.        , 0.66666667],
                [2.        , 1.        ],
                [2.        , 1.        ]])
 
         """
@@ -368,15 +366,16 @@
     def aspandas(self):
         """Output the stats as a pandas dataframe.
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
-        >>> H.nodes.multi(['degree', 'clustering_coefficient']).aspandas()  # doctest: +NORMALIZE_WHITESPACE
+        >>> H.nodes.multi(['degree', 'clustering_coefficient']).aspandas()
+        ... # doctest: +NORMALIZE_WHITESPACE
            degree  clustering_coefficient
         1       1    1.000000
         2       2    0.666667
         3       3    0.666667
         4       2    1.000000
         5       2    1.000000
 
@@ -436,28 +435,29 @@
 
 
 def dispatch_many_stats(kind, net, view, stats):
     return _dispatch_data[kind]["multistatclass"](net, view, stats)
 
 
 def nodestat_func(func):
-    """Decorator that allows arbitrary functions to behave like :class:`NodeStat` objects.
+    """Decorate arbitrary functions to behave like :class:`NodeStat` objects.
 
     Parameters
     ----------
     func : callable
         Function or callable with signature `func(net, bunch)`, where `net` is the
         network and `bunch` is an iterable of nodes in `net`.  The call `func(net,
-        bunch)` must return a dict with pairs of the form `(node: value)` where `node` is
-        in `bunch` and `value` is the value of the statistic at `node`.
+        bunch)` must return a dict with pairs of the form `(node: value)` where `node`
+        is in `bunch` and `value` is the value of the statistic at `node`.
 
     Returns
     -------
     callable
-        The decorated callable unmodified, after registering it in the `stats` framework.
+        The decorated callable unmodified, after registering it in the `stats`
+        framework.
 
     See Also
     --------
     :func:`edgestat_func`
 
     Notes
     -----
@@ -530,15 +530,15 @@
 
     """
     setattr(nodestats, func.__name__, func)
     return func
 
 
 def edgestat_func(func):
-    """Decorator that allows arbitrary functions to behave like :class:`EdgeStat` objects.
+    """Decorate arbitrary functions to behave like :class:`EdgeStat` objects.
 
     Works identically to :func:`nodestat`.  For extended documentation, see
     :func:`nodestat_func`.
 
     Parameters
     ----------
     func : callable
@@ -546,15 +546,16 @@
         network and `bunch` is an iterable of edges in `net`.  The call `func(net,
         bunch)` must return a dict with pairs of the form `(edge: value)` where `edge`
         is in `bunch` and `value` is the value of the statistic at `edge`.
 
     Returns
     -------
     callable
-        The decorated callable unmodified, after registering it in the `stats` framework.
+        The decorated callable unmodified, after registering it in the `stats`
+        framework.
 
     See Also
     --------
     :func:`nodestat_func`
 
     """
     setattr(edgestats, func.__name__, func)
```

### Comparing `xgi-0.5.7/xgi/stats/edgestats.py` & `xgi-0.5.8/xgi/stats/edgestats.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/xgi/stats/nodestats.py` & `xgi-0.5.8/xgi/stats/nodestats.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,28 +247,29 @@
     -------
     dict
         keys are node IDs and values are the
         clustering coefficients.
 
     References
     ----------
-    "Properties of metabolic graphs: biological organization or representation artifacts?"
-    by Wanding Zhou and Luay Nakhleh.
+    "Properties of metabolic graphs: biological organization or representation
+    artifacts?"  by Wanding Zhou and Luay Nakhleh.
     https://doi.org/10.1186/1471-2105-12-132
 
     "Hypergraphs for predicting essential genes using multiprotein complex data"
     by Florian Klimm, Charlotte M. Deane, and Gesine Reinert.
     https://doi.org/10.1093/comnet/cnaa028
 
     Example
     -------
     >>> import xgi
     >>> H = xgi.random_hypergraph(3, [1, 1])
     >>> H.nodes.local_clustering_coefficient.asdict()
     {0: 1.0, 1: 1.0, 2: 1.0}
+
     """
     cc = xgi.local_clustering_coefficient(net)
     return {n: cc[n] for n in cc if n in bunch}
 
 
 def two_node_clustering_coefficient(net, bunch, kind="union"):
     """Return the clustering coefficients for
@@ -283,18 +284,19 @@
         The network.
     bunch : Iterable
         Nodes in `net`.
     kind : str
         The type of two-node clustering coefficient.
         Types are:
 
-        - "union"
-        - "min"
-        - "max"
-        by default, "union".
+        * "union"
+        * "min"
+        * "max"
+
+    by default, "union".
 
     Returns
     -------
     dict
         nodes are keys, clustering coefficients are values.
 
     References
```

### Comparing `xgi-0.5.7/xgi/utils/utilities.py` & `xgi-0.5.8/xgi/utils/utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,80 @@
 """General utilities."""
 
 from collections import defaultdict
 from itertools import chain, combinations, count
 
+from xgi.exception import IDNotFound, XGIError
+
 __all__ = [
+    "IDDict",
     "dual_dict",
     "powerset",
     "update_uid_counter",
     "find_triangles",
 ]
 
 
+class IDDict(dict):
+    """A dict that holds (node or edge) IDs.
+
+    For internal use only.  Adds input validation functionality to the internal dicts
+    that hold nodes and edges in a network.
+
+    """
+
+    def __getitem__(self, item):
+        try:
+            return dict.__getitem__(self, item)
+        except KeyError as e:
+            raise IDNotFound(f"ID {item} not found") from e
+
+    def __setitem__(self, item, value):
+        if item is None:
+            raise XGIError("None cannot be a node or edge")
+        try:
+            return dict.__setitem__(self, item, value)
+        except TypeError as e:
+            raise TypeError(f"ID {item} not a valid type") from e
+
+    def __delitem__(self, item):
+        try:
+            return dict.__delitem__(self, item)
+        except KeyError as e:
+            raise IDNotFound(f"ID {item} not found") from e
+
+
 def dual_dict(edge_dict):
     """Given a dictionary with IDs as keys
-    and lists as values, return the dual.
+    and sets as values, return the dual.
 
     Parameters
     ----------
     edge_dict : dict
         A dictionary where the keys are
-        IDs and the values are lists of hashables
+        IDs and the values are sets of hashables
 
     Returns
     -------
     dict
         A dictionary with IDs as keys
-        and lists as values, but the reverse of
+        and sets as values, but the reverse of
         the original dict.
 
     Examples
     --------
     >>> import xgi
     >>> xgi.dual_dict({0 : [1, 2, 3], 1 : [0, 2]})
-    {1: [0], 2: [0, 1], 3: [0], 0: [1]}
+    {1: {0}, 2: {0, 1}, 3: {0}, 0: {1}}
 
     """
-    node_dict = defaultdict(list)
+    node_dict = defaultdict(set)
     for edge_id, members in edge_dict.items():
         for node in members:
-            node_dict[node].append(edge_id)
+            node_dict[node].add(edge_id)
 
     return dict(node_dict)
 
 
 def powerset(
     iterable, include_empty=False, include_full=False, include_singletons=True
 ):
```

### Comparing `xgi-0.5.7/xgi.egg-info/SOURCES.txt` & `xgi-0.5.8/xgi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xgi-0.5.7/xgi.egg-info/requires.txt` & `xgi-0.5.8/xgi.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,48 +2,49 @@
 scipy>=1.8
 pandas>=1.3
 networkx>=2.7
 requests>=2.0
 matplotlib>=3.4
 
 [all]
-github-changelog
-pytest>=7.2
 pre-commit>=2.12
-black[jupyter]==22.3.0
-sphinx-rtd-theme>=0.4.2
-sphinx_copybutton
-pylint>=2.10
-isort==5.10.1
 matplotlib>=3.3
-seaborn>=0.10
-pytest-cov>=4.0
+sphinx-rtd-theme>=1.2
 numpydoc>=1.1
+pylint>=2.10
+pytest>=7.2
 twine>=3.4
-sphinx~=4.0
-hypernetx>=1.0
-pillow>=8.2
-wheel>=0.36
 jupyter>=1.0
+sphinx~=6.0
+pillow>=8.2
+black[jupyter]==22.3.0
+isort==5.10.1
+seaborn>=0.10
 asv>=0.5
+wheel>=0.36
+pytest-cov>=4.0
+hypernetx>=1.0
+ipython<=8.12.0
+github-changelog
+sphinx_copybutton
 
 [benchmarks]
 hypernetx>=1.0
 asv>=0.5
 
 [developer]
 black[jupyter]==22.3.0
 pre-commit>=2.12
 isort==5.10.1
 pylint>=2.10
 
 [documentation]
-sphinx~=4.0
+sphinx~=6.0
 sphinx_copybutton
-sphinx-rtd-theme>=0.4.2
+sphinx-rtd-theme>=1.2
 numpydoc>=1.1
 pillow>=8.2
 matplotlib>=3.3
 
 [release]
 twine>=3.4
 wheel>=0.36
@@ -53,7 +54,8 @@
 pytest>=7.2
 pytest-cov>=4.0
 
 [tutorial]
 jupyter>=1.0
 matplotlib>=3.3
 seaborn>=0.10
+ipython<=8.12.0
```


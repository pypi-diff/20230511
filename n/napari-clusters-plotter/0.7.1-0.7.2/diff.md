# Comparing `tmp/napari-clusters-plotter-0.7.1.tar.gz` & `tmp/napari-clusters-plotter-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-clusters-plotter-0.7.1.tar", last modified: Mon May  1 07:37:46 2023, max compression
+gzip compressed data, was "napari-clusters-plotter-0.7.2.tar", last modified: Thu May 11 05:10:48 2023, max compression
```

## Comparing `napari-clusters-plotter-0.7.1.tar` & `napari-clusters-plotter-0.7.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.820173 napari-clusters-plotter-0.7.1/
--rw-rw-rw-   0        0        0     1642 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/LICENSE
--rw-rw-rw-   0        0        0      127 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0    15617 2023-05-01 07:37:46.820173 napari-clusters-plotter-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    14228 2023-04-29 17:52:49.000000 napari-clusters-plotter-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.776058 napari-clusters-plotter-0.7.1/napari_clusters_plotter/
--rw-rw-rw-   0        0        0    24305 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_Qt_code.py
--rw-rw-rw-   0        0        0      184 2023-05-01 07:35:45.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/__init__.py
--rw-rw-rw-   0        0        0    21295 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_clustering.py
--rw-rw-rw-   0        0        0    37507 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_dimensionality_reduction.py
--rw-rw-rw-   0        0        0      406 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_dock_widget.py
--rw-rw-rw-   0        0        0    33249 2023-04-29 17:16:06.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter.py
--rw-rw-rw-   0        0        0    17769 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter_utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.804131 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/
--rw-rw-rw-   0        0        0        0 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/__init__.py
--rw-rw-rw-   0        0        0     7838 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_clustering.py
--rw-rw-rw-   0        0        0     7373 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dimension_reduction.py
--rw-rw-rw-   0        0        0     2457 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dock_widget.py
--rw-rw-rw-   0        0        0     6619 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_plotter.py
--rw-rw-rw-   0        0        0     5256 2023-03-16 15:33:04.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_utils.py
--rw-rw-rw-   0        0        0    15576 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.819171 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/
--rw-rw-rw-   0        0        0     6680 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Back.png
--rw-rw-rw-   0        0        0     6951 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Customize.png
--rw-rw-rw-   0        0        0     6535 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Forward.png
--rw-rw-rw-   0        0        0     7143 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Home.png
--rw-rw-rw-   0        0        0     7114 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan.png
--rw-rw-rw-   0        0        0    11810 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan_checked.png
--rw-rw-rw-   0        0        0     7381 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Save.png
--rw-rw-rw-   0        0        0     6739 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Subplots.png
--rw-rw-rw-   0        0        0     8064 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom.png
--rw-rw-rw-   0        0        0    12372 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom_checked.png
-drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.797113 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/
--rw-rw-rw-   0        0        0    15617 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1384 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.1/requirements.txt
--rw-rw-rw-   0        0        0     1928 2023-05-01 07:37:46.822179 napari-clusters-plotter-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      117 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:10:48.335373 napari-clusters-plotter-0.7.2/
+-rw-rw-rw-   0        0        0     1717 2023-05-11 05:02:30.000000 napari-clusters-plotter-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    15626 2023-05-11 05:10:48.335373 napari-clusters-plotter-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14220 2023-05-11 05:02:30.000000 napari-clusters-plotter-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 05:10:48.288477 napari-clusters-plotter-0.7.2/napari_clusters_plotter/
+-rw-rw-rw-   0        0        0    24421 2023-05-11 05:02:30.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_Qt_code.py
+-rw-rw-rw-   0        0        0      184 2023-05-11 05:03:36.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/__init__.py
+-rw-rw-rw-   0        0        0    21295 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_clustering.py
+-rw-rw-rw-   0        0        0    37507 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_dimensionality_reduction.py
+-rw-rw-rw-   0        0        0      406 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_dock_widget.py
+-rw-rw-rw-   0        0        0    33494 2023-05-11 05:02:30.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_plotter.py
+-rw-rw-rw-   0        0        0    17769 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_plotter_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:10:48.320135 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/
+-rw-rw-rw-   0        0        0        0 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/__init__.py
+-rw-rw-rw-   0        0        0     7838 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_clustering.py
+-rw-rw-rw-   0        0        0     7373 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_dimension_reduction.py
+-rw-rw-rw-   0        0        0     2457 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_dock_widget.py
+-rw-rw-rw-   0        0        0     6619 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_plotter.py
+-rw-rw-rw-   0        0        0     5256 2023-03-16 15:33:04.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_utils.py
+-rw-rw-rw-   0        0        0    15576 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:10:48.335373 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/
+-rw-rw-rw-   0        0        0     6680 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Back.png
+-rw-rw-rw-   0        0        0     6951 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Customize.png
+-rw-rw-rw-   0        0        0     6535 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Forward.png
+-rw-rw-rw-   0        0        0     7143 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Home.png
+-rw-rw-rw-   0        0        0     7114 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Pan.png
+-rw-rw-rw-   0        0        0    11810 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Pan_checked.png
+-rw-rw-rw-   0        0        0     7381 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Save.png
+-rw-rw-rw-   0        0        0     6739 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Subplots.png
+-rw-rw-rw-   0        0        0     8064 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Zoom.png
+-rw-rw-rw-   0        0        0    12372 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Zoom_checked.png
+drwxrwxrwx   0        0        0        0 2023-05-11 05:10:48.320135 napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/
+-rw-rw-rw-   0        0        0    15626 2023-05-11 05:10:47.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1384 2023-05-11 05:10:48.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:10:47.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-11 05:10:47.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-05-11 05:10:47.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-11 05:10:48.000000 napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.2/requirements.txt
+-rw-rw-rw-   0        0        0     1945 2023-05-11 05:10:48.351000 napari-clusters-plotter-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      117 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.2/setup.py
```

### Comparing `napari-clusters-plotter-0.7.1/LICENSE` & `napari-clusters-plotter-0.7.2/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022, DFG Cluster of Excellence "Physics of Life" TU Dresden, Robert Haase, Laura Zigutyte, Marcello Zoccoler, Ryan Savill, Johannes Müller
+Copyright (c) 2022, DFG Cluster of Excellence "Physics of Life" TU Dresden: Robert Haase, Laura Zigutyte, Marcello Zoccoler, Ryan Savill, Johannes Müller and Max Planck Institute of Molecular Physiology Dortmund: Thorsten Wagner
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `napari-clusters-plotter-0.7.1/PKG-INFO` & `napari-clusters-plotter-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: napari-clusters-plotter
-Version: 0.7.1
+Version: 0.7.2
 Summary: A plugin to use with napari for clustering objects according to their properties
 Home-page: https://github.com/BiAPoL/napari-clusters-plotter
-Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Robert Haase
+Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Thorsten Wagner, Robert Haase
 Author-email: zigutyte@gmail.com, robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/BiAPoL/napari-clusters-plotter/issues
 Project-URL: Documentation, https://github.com/BiAPoL/napari-clusters-plotter
 Project-URL: Source Code, https://github.com/BiAPoL/napari-clusters-plotter
 Project-URL: User Support, https://github.com/BiAPoL/napari-clusters-plotter/issues
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -71,18 +71,18 @@
 in the napari plugin [napari-segment-blobs-and-things-with-membranes](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes).
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/starting_point.png)
 
 In case you have 2D time-lapse data you need to convert it into a suitable shape using the menu `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)` ([documentation](https://www.napari-hub.org/plugins/napari-time-slicer)).
 
 ### Measurements
-The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image. 
+The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image.
 Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget ([documentation](https://www.napari-hub.org/plugins/napari-skimage-regionprops)).
 Select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-A table with the measurements will open and afterwards, you can save and/or close the measurement table. 
+A table with the measurements will open and afterwards, you can save and/or close the measurement table.
 At this point it is recommended to close the table and the Measure widget to free space for following steps.
 
 You can also load your own measurements you can do this using the menu `Tools > Measurement tables > Load from CSV (nsr)`.
 If you load custom measurements, please make sure that there is a `label` column that specifies the which measurement belongs to which labeled object.
 Tables for time-lapse data need to include an additional column named `frame`.
 
 ### Plotting
@@ -142,33 +142,33 @@
 * [Uniform Manifold Approximation Projection (UMAP)](https://umap-learn.readthedocs.io/en/latest/)
 * [t-distributed stochastic neighbor embedding (t-SNE)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
 * [Principal Component Analysis (PCA)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
 * [Non-linear dimensionality reduction through Isometric Mapping (Isomap)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.Isomap.html)
 * [Multi-dimensional Scaling (MDS)](https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling)
 
 To apply them to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
-Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced. 
-By default, all measurements are selected in the box. 
-You can read more about parameters of both algorithms by hovering over question marks or by clicking on them. 
-When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset. 
+Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced.
+By default, all measurements are selected in the box.
+You can read more about parameters of both algorithms by hovering over question marks or by clicking on them.
+When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset.
 These columns are automatically saved in the labels layer and can be further processed by other plugins.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/umap.png)
 
 Afterwards, you can again save and/or close the table.
 
 ### Clustering
 If manual clustering, as shown above, is not an option, you can automatically cluster your data, using these implemented algorithms:
 * [k-means clustering (KMEANS)](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a)
 * [Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN)](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
 * [Gaussian Mixture Model (GMM)](https://scikit-learn.org/stable/modules/mixture.html)
 * [Mean Shift (MS)](https://scikit-learn.org/stable/auto_examples/cluster/plot_mean_shift.html#sphx-glr-auto-examples-cluster-plot-mean-shift-py)
 * [Agglomerative clustering (AC)](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
 
-Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`, 
+Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`,
 select the analysed labels layer.
 Select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
 Select the clustering method `KMeans` and click on `Run`.
 The table of measurements will reappear with an additional column `ALGORITHM_NAME_CLUSTERING_ID` containing the cluster
 ID of each datapoint.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/clustering.png)
@@ -186,15 +186,15 @@
 ### Devbio-napari installation
 
 The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) plugin collection. The napari-clusters-plotter is part of it.
 
 ### Minimal installation
 * Get a python environment, e.g. via [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
   If you never used mamba/conda environments before, please follow the instructions
-  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first. 
+  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first.
 
 * Create a new environment, for example, like this:
 
 ```
 mamba create --name ncp-env python=3.9
 ```
```

### Comparing `napari-clusters-plotter-0.7.1/README.md` & `napari-clusters-plotter-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 in the napari plugin [napari-segment-blobs-and-things-with-membranes](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes).
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/starting_point.png)
 
 In case you have 2D time-lapse data you need to convert it into a suitable shape using the menu `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)` ([documentation](https://www.napari-hub.org/plugins/napari-time-slicer)).
 
 ### Measurements
-The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image. 
+The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image.
 Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget ([documentation](https://www.napari-hub.org/plugins/napari-skimage-regionprops)).
 Select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-A table with the measurements will open and afterwards, you can save and/or close the measurement table. 
+A table with the measurements will open and afterwards, you can save and/or close the measurement table.
 At this point it is recommended to close the table and the Measure widget to free space for following steps.
 
 You can also load your own measurements you can do this using the menu `Tools > Measurement tables > Load from CSV (nsr)`.
 If you load custom measurements, please make sure that there is a `label` column that specifies the which measurement belongs to which labeled object.
 Tables for time-lapse data need to include an additional column named `frame`.
 
 ### Plotting
@@ -114,33 +114,33 @@
 * [Uniform Manifold Approximation Projection (UMAP)](https://umap-learn.readthedocs.io/en/latest/)
 * [t-distributed stochastic neighbor embedding (t-SNE)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
 * [Principal Component Analysis (PCA)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
 * [Non-linear dimensionality reduction through Isometric Mapping (Isomap)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.Isomap.html)
 * [Multi-dimensional Scaling (MDS)](https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling)
 
 To apply them to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
-Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced. 
-By default, all measurements are selected in the box. 
-You can read more about parameters of both algorithms by hovering over question marks or by clicking on them. 
-When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset. 
+Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced.
+By default, all measurements are selected in the box.
+You can read more about parameters of both algorithms by hovering over question marks or by clicking on them.
+When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset.
 These columns are automatically saved in the labels layer and can be further processed by other plugins.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/umap.png)
 
 Afterwards, you can again save and/or close the table.
 
 ### Clustering
 If manual clustering, as shown above, is not an option, you can automatically cluster your data, using these implemented algorithms:
 * [k-means clustering (KMEANS)](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a)
 * [Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN)](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
 * [Gaussian Mixture Model (GMM)](https://scikit-learn.org/stable/modules/mixture.html)
 * [Mean Shift (MS)](https://scikit-learn.org/stable/auto_examples/cluster/plot_mean_shift.html#sphx-glr-auto-examples-cluster-plot-mean-shift-py)
 * [Agglomerative clustering (AC)](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
 
-Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`, 
+Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`,
 select the analysed labels layer.
 Select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
 Select the clustering method `KMeans` and click on `Run`.
 The table of measurements will reappear with an additional column `ALGORITHM_NAME_CLUSTERING_ID` containing the cluster
 ID of each datapoint.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/clustering.png)
@@ -158,15 +158,15 @@
 ### Devbio-napari installation
 
 The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) plugin collection. The napari-clusters-plotter is part of it.
 
 ### Minimal installation
 * Get a python environment, e.g. via [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
   If you never used mamba/conda environments before, please follow the instructions
-  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first. 
+  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first.
 
 * Create a new environment, for example, like this:
 
 ```
 mamba create --name ncp-env python=3.9
 ```
```

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_Qt_code.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_Qt_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,14 +523,15 @@
         self.manual_clustering_method = manual_clustering_method
 
         self.axes = self.fig.add_subplot(111)
         self.histogram = None
 
         self.match_napari_layout()
         self.xylim = None
+        self.last_xy_labels = None
 
         super().__init__(self.fig)
         self.mpl_connect("draw_event", self.on_draw)
 
         self.pts = self.axes.scatter([], [])
         self.selector = SelectFromCollection(self, self.axes, self.pts)
         self.rectangle_selector = RectangleSelector(
@@ -550,14 +551,15 @@
 
     def reset_zoom(self):
         if self.xylim:
             self.axes.set_xlim(self.xylim[0])
             self.axes.set_ylim(self.xylim[1])
 
     def on_draw(self, event):
+        self.last_xy_labels = (self.axes.get_xlabel(), self.axes.get_ylabel())
         self.xylim = (self.axes.get_xlim(), self.axes.get_ylim())
 
     def draw_rectangle(self, eclick, erelease):
         """eclick and erelease are the press and release events"""
         x0, y0 = eclick.xdata, eclick.ydata
         x1, y1 = erelease.xdata, erelease.ydata
         self.xys = self.pts.get_offsets()
```

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_clustering.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_clustering.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_dimensionality_reduction.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,10 +783,15 @@
                         bin_number=number_bins,
                         log_scale=self.log_scale.isChecked(),
                     )
                     self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
                     self.graphics_widget.axes.set_ylabel(plot_y_axis_name)
 
             self.graphics_widget.match_napari_layout()
+            self.graphics_widget.draw()
+
+        if self.graphics_widget.last_xy_labels != (plot_x_axis_name, plot_y_axis_name):
+            # Additional redraw in case axis have changed, otherwise y-axis may not get updated. General redraw would
+            # resets the zoom, which needs to be avoided.
+            self.graphics_widget.draw()
 
-        self.graphics_widget.draw()  # Always redraws, oterwise y-axis may not get updated in histograms
         self.graphics_widget.reset_zoom()
```

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter_utilities.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_plotter_utilities.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_clustering.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dimension_reduction.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dock_widget.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_plotter.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_utils.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_utilities.py` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/_utilities.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Back.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Back.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Customize.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Customize.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Forward.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Forward.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Home.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Home.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Pan.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan_checked.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Save.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Save.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Subplots.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom_checked.png` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter/icons/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/PKG-INFO` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: napari-clusters-plotter
-Version: 0.7.1
+Version: 0.7.2
 Summary: A plugin to use with napari for clustering objects according to their properties
 Home-page: https://github.com/BiAPoL/napari-clusters-plotter
-Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Robert Haase
+Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Thorsten Wagner, Robert Haase
 Author-email: zigutyte@gmail.com, robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/BiAPoL/napari-clusters-plotter/issues
 Project-URL: Documentation, https://github.com/BiAPoL/napari-clusters-plotter
 Project-URL: Source Code, https://github.com/BiAPoL/napari-clusters-plotter
 Project-URL: User Support, https://github.com/BiAPoL/napari-clusters-plotter/issues
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -71,18 +71,18 @@
 in the napari plugin [napari-segment-blobs-and-things-with-membranes](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes).
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/starting_point.png)
 
 In case you have 2D time-lapse data you need to convert it into a suitable shape using the menu `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)` ([documentation](https://www.napari-hub.org/plugins/napari-time-slicer)).
 
 ### Measurements
-The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image. 
+The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image.
 Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget ([documentation](https://www.napari-hub.org/plugins/napari-skimage-regionprops)).
 Select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-A table with the measurements will open and afterwards, you can save and/or close the measurement table. 
+A table with the measurements will open and afterwards, you can save and/or close the measurement table.
 At this point it is recommended to close the table and the Measure widget to free space for following steps.
 
 You can also load your own measurements you can do this using the menu `Tools > Measurement tables > Load from CSV (nsr)`.
 If you load custom measurements, please make sure that there is a `label` column that specifies the which measurement belongs to which labeled object.
 Tables for time-lapse data need to include an additional column named `frame`.
 
 ### Plotting
@@ -142,33 +142,33 @@
 * [Uniform Manifold Approximation Projection (UMAP)](https://umap-learn.readthedocs.io/en/latest/)
 * [t-distributed stochastic neighbor embedding (t-SNE)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
 * [Principal Component Analysis (PCA)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
 * [Non-linear dimensionality reduction through Isometric Mapping (Isomap)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.Isomap.html)
 * [Multi-dimensional Scaling (MDS)](https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling)
 
 To apply them to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
-Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced. 
-By default, all measurements are selected in the box. 
-You can read more about parameters of both algorithms by hovering over question marks or by clicking on them. 
-When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset. 
+Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced.
+By default, all measurements are selected in the box.
+You can read more about parameters of both algorithms by hovering over question marks or by clicking on them.
+When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset.
 These columns are automatically saved in the labels layer and can be further processed by other plugins.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/umap.png)
 
 Afterwards, you can again save and/or close the table.
 
 ### Clustering
 If manual clustering, as shown above, is not an option, you can automatically cluster your data, using these implemented algorithms:
 * [k-means clustering (KMEANS)](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a)
 * [Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN)](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
 * [Gaussian Mixture Model (GMM)](https://scikit-learn.org/stable/modules/mixture.html)
 * [Mean Shift (MS)](https://scikit-learn.org/stable/auto_examples/cluster/plot_mean_shift.html#sphx-glr-auto-examples-cluster-plot-mean-shift-py)
 * [Agglomerative clustering (AC)](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
 
-Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`, 
+Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`,
 select the analysed labels layer.
 Select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
 Select the clustering method `KMeans` and click on `Run`.
 The table of measurements will reappear with an additional column `ALGORITHM_NAME_CLUSTERING_ID` containing the cluster
 ID of each datapoint.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/clustering.png)
@@ -186,15 +186,15 @@
 ### Devbio-napari installation
 
 The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) plugin collection. The napari-clusters-plotter is part of it.
 
 ### Minimal installation
 * Get a python environment, e.g. via [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
   If you never used mamba/conda environments before, please follow the instructions
-  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first. 
+  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first.
 
 * Create a new environment, for example, like this:
 
 ```
 mamba create --name ncp-env python=3.9
 ```
```

### Comparing `napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/SOURCES.txt` & `napari-clusters-plotter-0.7.2/napari_clusters_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/requirements.txt` & `napari-clusters-plotter-0.7.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.1/setup.cfg` & `napari-clusters-plotter-0.7.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,122 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 636c 7573 7465   = napari-cluste
 00000020: 7273 2d70 6c6f 7474 6572 0d0a 7665 7273  rs-plotter..vers
-00000030: 696f 6e20 3d20 302e 372e 310d 0a61 7574  ion = 0.7.1..aut
+00000030: 696f 6e20 3d20 302e 372e 320d 0a61 7574  ion = 0.7.2..aut
 00000040: 686f 7220 3d20 4c61 7572 6120 5a69 6775  hor = Laura Zigu
 00000050: 7479 7465 2c20 5279 616e 2053 6176 696c  tyte, Ryan Savil
 00000060: 6c2c 204a 6f68 616e 6e65 7320 4dc3 bc6c  l, Johannes M..l
 00000070: 6c65 722c 204d 6172 6365 6c6f 205a 6f63  ler, Marcelo Zoc
-00000080: 636f 6c65 722c 2052 6f62 6572 7420 4861  coler, Robert Ha
-00000090: 6173 650d 0a61 7574 686f 725f 656d 6169  ase..author_emai
-000000a0: 6c20 3d20 7a69 6775 7479 7465 4067 6d61  l = zigutyte@gma
-000000b0: 696c 2e63 6f6d 2c20 726f 6265 7274 2e68  il.com, robert.h
-000000c0: 6161 7365 4074 752d 6472 6573 6465 6e2e  aase@tu-dresden.
-000000d0: 6465 0d0a 7572 6c20 3d20 6874 7470 733a  de..url = https:
-000000e0: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6941  //github.com/BiA
-000000f0: 506f 4c2f 6e61 7061 7269 2d63 6c75 7374  PoL/napari-clust
-00000100: 6572 732d 706c 6f74 7465 720d 0a70 726f  ers-plotter..pro
-00000110: 6a65 6374 5f75 726c 7320 3d20 0d0a 0942  ject_urls = ...B
-00000120: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
-00000130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000140: 4269 4150 6f4c 2f6e 6170 6172 692d 636c  BiAPoL/napari-cl
-00000150: 7573 7465 7273 2d70 6c6f 7474 6572 2f69  usters-plotter/i
-00000160: 7373 7565 730d 0a09 446f 6375 6d65 6e74  ssues...Document
-00000170: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
-00000180: 6769 7468 7562 2e63 6f6d 2f42 6941 506f  github.com/BiAPo
-00000190: 4c2f 6e61 7061 7269 2d63 6c75 7374 6572  L/napari-cluster
-000001a0: 732d 706c 6f74 7465 720d 0a09 536f 7572  s-plotter...Sour
-000001b0: 6365 2043 6f64 6520 3d20 6874 7470 733a  ce Code = https:
-000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6941  //github.com/BiA
-000001d0: 506f 4c2f 6e61 7061 7269 2d63 6c75 7374  PoL/napari-clust
-000001e0: 6572 732d 706c 6f74 7465 720d 0a09 5573  ers-plotter...Us
-000001f0: 6572 2053 7570 706f 7274 203d 2068 7474  er Support = htt
-00000200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000210: 4269 4150 6f4c 2f6e 6170 6172 692d 636c  BiAPoL/napari-cl
-00000220: 7573 7465 7273 2d70 6c6f 7474 6572 2f69  usters-plotter/i
-00000230: 7373 7565 730d 0a6c 6963 656e 7365 203d  ssues..license =
-00000240: 2042 5344 2d33 2d43 6c61 7573 650d 0a64   BSD-3-Clause..d
-00000250: 6573 6372 6970 7469 6f6e 203d 2041 2070  escription = A p
-00000260: 6c75 6769 6e20 746f 2075 7365 2077 6974  lugin to use wit
-00000270: 6820 6e61 7061 7269 2066 6f72 2063 6c75  h napari for clu
-00000280: 7374 6572 696e 6720 6f62 6a65 6374 7320  stering objects 
-00000290: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
-000002a0: 6972 2070 726f 7065 7274 6965 730d 0a6c  ir properties..l
-000002b0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000002c0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000002d0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000002e0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000002f0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000300: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000310: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
-00000320: 7461 7475 7320 3a3a 2032 202d 2050 7265  tatus :: 2 - Pre
-00000330: 2d41 6c70 6861 0d0a 0949 6e74 656e 6465  -Alpha...Intende
-00000340: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000350: 7665 6c6f 7065 7273 0d0a 0946 7261 6d65  velopers...Frame
-00000360: 776f 726b 203a 3a20 6e61 7061 7269 0d0a  work :: napari..
-00000370: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
-00000380: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-00000390: 3a20 5465 7374 696e 670d 0a09 5072 6f67  : Testing...Prog
-000003a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000003b0: 203a 3a20 5079 7468 6f6e 0d0a 0950 726f   :: Python...Pro
-000003c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000003d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000003e0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000003f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000400: 6e20 3a3a 2033 2e37 0d0a 0950 726f 6772  n :: 3.7...Progr
-00000410: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000420: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000430: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000440: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000450: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
-00000460: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000470: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000480: 300d 0a09 4f70 6572 6174 696e 6720 5379  0...Operating Sy
-00000490: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000004a0: 656e 6465 6e74 0d0a 094c 6963 656e 7365  endent...License
-000004b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000004c0: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
-000004d0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-000004e0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-000004f0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000500: 3d20 3e3d 332e 370d 0a69 6e73 7461 6c6c  = >=3.7..install
-00000510: 5f72 6571 7569 7265 7320 3d20 0d0a 096e  _requires = ...n
-00000520: 6170 6172 692d 706c 7567 696e 2d65 6e67  apari-plugin-eng
-00000530: 696e 653e 3d30 2e31 2e34 0d0a 096e 756d  ine>=0.1.4...num
-00000540: 7079 3e3d 312e 3231 2c3c 3d31 2e32 332e  py>=1.21,<=1.23.
-00000550: 350d 0a09 7363 696b 6974 2d6c 6561 726e  5...scikit-learn
-00000560: 0d0a 096d 6174 706c 6f74 6c69 620d 0a09  ...matplotlib...
-00000570: 7061 6e64 6173 0d0a 0975 6d61 702d 6c65  pandas...umap-le
-00000580: 6172 6e0d 0a09 6e61 7061 7269 2d74 6f6f  arn...napari-too
-00000590: 6c73 2d6d 656e 750d 0a09 6e61 7061 7269  ls-menu...napari
-000005a0: 2d73 6b69 6d61 6765 2d72 6567 696f 6e70  -skimage-regionp
-000005b0: 726f 7073 3e3d 302e 332e 310d 0a09 6864  rops>=0.3.1...hd
-000005c0: 6273 6361 6e0d 0a09 6a6f 626c 6962 0d0a  bscan...joblib..
-000005d0: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
-000005e0: 5f70 6f69 6e74 735d 0d0a 6e61 7061 7269  _points]..napari
-000005f0: 2e70 6c75 6769 6e20 3d20 0d0a 096e 6170  .plugin = ...nap
-00000600: 6172 692d 636c 7573 7465 7273 2d70 6c6f  ari-clusters-plo
-00000610: 7474 6572 203d 206e 6170 6172 695f 636c  tter = napari_cl
-00000620: 7573 7465 7273 5f70 6c6f 7474 6572 0d0a  usters_plotter..
-00000630: 0d0a 5b66 6c61 6b65 385d 0d0a 6d61 782d  ..[flake8]..max-
-00000640: 6c69 6e65 2d6c 656e 6774 6820 3d20 3132  line-length = 12
-00000650: 300d 0a69 676e 6f72 6520 3d20 4532 3033  0..ignore = E203
-00000660: 2c57 3530 332c 4339 3031 2c46 3832 330d  ,W503,C901,F823.
-00000670: 0a6d 6178 2d63 6f6d 706c 6578 6974 7920  .max-complexity 
-00000680: 3d20 3138 0d0a 6275 696c 7469 6e73 203d  = 18..builtins =
-00000690: 2070 7974 6573 740d 0a65 7863 6c75 6465   pytest..exclude
-000006a0: 203d 206e 6170 6172 695f 636c 7573 7465   = napari_cluste
-000006b0: 7273 5f70 6c6f 7474 6572 2f5f 5f69 6e69  rs_plotter/__ini
-000006c0: 745f 5f2e 7079 2c20 6578 616d 706c 655f  t__.py, example_
-000006d0: 6461 7461 2c20 696d 6167 6573 2c20 6e61  data, images, na
-000006e0: 7061 7269 5f63 6c75 7374 6572 735f 706c  pari_clusters_pl
-000006f0: 6f74 7465 722f 5f67 6574 5f63 6f6c 6f72  otter/_get_color
-00000700: 6d61 702e 7079 0d0a 6261 6e6e 6564 2d6d  map.py..banned-m
-00000710: 6f64 756c 6573 203d 2050 7951 7435 203d  odules = PyQt5 =
-00000720: 2075 7365 2071 7470 790d 0a09 5079 5369   use qtpy...PySi
-00000730: 6465 3220 3d20 7573 6520 7174 7079 0d0a  de2 = use qtpy..
-00000740: 0d0a 5b69 736f 7274 5d0d 0a70 726f 6669  ..[isort]..profi
-00000750: 6c65 203d 2062 6c61 636b 0d0a 0d0a 5b65  le = black....[e
-00000760: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000770: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000780: 203d 2030 0d0a 0d0a                       = 0....
+00000080: 636f 6c65 722c 2054 686f 7273 7465 6e20  coler, Thorsten 
+00000090: 5761 676e 6572 2c20 526f 6265 7274 2048  Wagner, Robert H
+000000a0: 6161 7365 0d0a 6175 7468 6f72 5f65 6d61  aase..author_ema
+000000b0: 696c 203d 207a 6967 7574 7974 6540 676d  il = zigutyte@gm
+000000c0: 6169 6c2e 636f 6d2c 2072 6f62 6572 742e  ail.com, robert.
+000000d0: 6861 6173 6540 7475 2d64 7265 7364 656e  haase@tu-dresden
+000000e0: 2e64 650d 0a75 726c 203d 2068 7474 7073  .de..url = https
+000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4269  ://github.com/Bi
+00000100: 4150 6f4c 2f6e 6170 6172 692d 636c 7573  APoL/napari-clus
+00000110: 7465 7273 2d70 6c6f 7474 6572 0d0a 7072  ters-plotter..pr
+00000120: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+00000130: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
+00000140: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000150: 2f42 6941 506f 4c2f 6e61 7061 7269 2d63  /BiAPoL/napari-c
+00000160: 6c75 7374 6572 732d 706c 6f74 7465 722f  lusters-plotter/
+00000170: 6973 7375 6573 0d0a 0944 6f63 756d 656e  issues...Documen
+00000180: 7461 7469 6f6e 203d 2068 7474 7073 3a2f  tation = https:/
+00000190: 2f67 6974 6875 622e 636f 6d2f 4269 4150  /github.com/BiAP
+000001a0: 6f4c 2f6e 6170 6172 692d 636c 7573 7465  oL/napari-cluste
+000001b0: 7273 2d70 6c6f 7474 6572 0d0a 0953 6f75  rs-plotter...Sou
+000001c0: 7263 6520 436f 6465 203d 2068 7474 7073  rce Code = https
+000001d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4269  ://github.com/Bi
+000001e0: 4150 6f4c 2f6e 6170 6172 692d 636c 7573  APoL/napari-clus
+000001f0: 7465 7273 2d70 6c6f 7474 6572 0d0a 0955  ters-plotter...U
+00000200: 7365 7220 5375 7070 6f72 7420 3d20 6874  ser Support = ht
+00000210: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000220: 2f42 6941 506f 4c2f 6e61 7061 7269 2d63  /BiAPoL/napari-c
+00000230: 6c75 7374 6572 732d 706c 6f74 7465 722f  lusters-plotter/
+00000240: 6973 7375 6573 0d0a 6c69 6365 6e73 6520  issues..license 
+00000250: 3d20 4253 442d 332d 436c 6175 7365 0d0a  = BSD-3-Clause..
+00000260: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
+00000270: 706c 7567 696e 2074 6f20 7573 6520 7769  plugin to use wi
+00000280: 7468 206e 6170 6172 6920 666f 7220 636c  th napari for cl
+00000290: 7573 7465 7269 6e67 206f 626a 6563 7473  ustering objects
+000002a0: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
+000002b0: 6569 7220 7072 6f70 6572 7469 6573 0d0a  eir properties..
+000002c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000002d0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000002e0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000002f0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000300: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000310: 6e0d 0a63 6c61 7373 6966 6965 7273 203d  n..classifiers =
+00000320: 200d 0a09 4465 7665 6c6f 706d 656e 7420   ...Development 
+00000330: 5374 6174 7573 203a 3a20 3220 2d20 5072  Status :: 2 - Pr
+00000340: 652d 416c 7068 610d 0a09 496e 7465 6e64  e-Alpha...Intend
+00000350: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+00000360: 6576 656c 6f70 6572 730d 0a09 4672 616d  evelopers...Fram
+00000370: 6577 6f72 6b20 3a3a 206e 6170 6172 690d  ework :: napari.
+00000380: 0a09 546f 7069 6320 3a3a 2053 6f66 7477  ..Topic :: Softw
+00000390: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
+000003a0: 3a3a 2054 6573 7469 6e67 0d0a 0950 726f  :: Testing...Pro
+000003b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000003c0: 6520 3a3a 2050 7974 686f 6e0d 0a09 5072  e :: Python...Pr
+000003d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000003e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003f0: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
+00000400: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000410: 6f6e 203a 3a20 332e 370d 0a09 5072 6f67  on :: 3.7...Prog
+00000420: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000430: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000440: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+00000450: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000460: 6f6e 203a 3a20 332e 390d 0a09 5072 6f67  on :: 3.9...Prog
+00000470: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000480: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000490: 3130 0d0a 094f 7065 7261 7469 6e67 2053  10...Operating S
+000004a0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000004b0: 7065 6e64 656e 740d 0a09 4c69 6365 6e73  pendent...Licens
+000004c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000004d0: 6420 3a3a 2042 5344 204c 6963 656e 7365  d :: BSD License
+000004e0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+000004f0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000500: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000510: 203d 203e 3d33 2e37 0d0a 696e 7374 616c   = >=3.7..instal
+00000520: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
+00000530: 6e61 7061 7269 2d70 6c75 6769 6e2d 656e  napari-plugin-en
+00000540: 6769 6e65 3e3d 302e 312e 340d 0a09 6e75  gine>=0.1.4...nu
+00000550: 6d70 793e 3d31 2e32 312c 3c3d 312e 3233  mpy>=1.21,<=1.23
+00000560: 2e35 0d0a 0973 6369 6b69 742d 6c65 6172  .5...scikit-lear
+00000570: 6e0d 0a09 6d61 7470 6c6f 746c 6962 0d0a  n...matplotlib..
+00000580: 0970 616e 6461 730d 0a09 756d 6170 2d6c  .pandas...umap-l
+00000590: 6561 726e 0d0a 096e 6170 6172 692d 746f  earn...napari-to
+000005a0: 6f6c 732d 6d65 6e75 0d0a 096e 6170 6172  ols-menu...napar
+000005b0: 692d 736b 696d 6167 652d 7265 6769 6f6e  i-skimage-region
+000005c0: 7072 6f70 733e 3d30 2e33 2e31 0d0a 0968  props>=0.3.1...h
+000005d0: 6462 7363 616e 0d0a 096a 6f62 6c69 620d  dbscan...joblib.
+000005e0: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
+000005f0: 795f 706f 696e 7473 5d0d 0a6e 6170 6172  y_points]..napar
+00000600: 692e 706c 7567 696e 203d 200d 0a09 6e61  i.plugin = ...na
+00000610: 7061 7269 2d63 6c75 7374 6572 732d 706c  pari-clusters-pl
+00000620: 6f74 7465 7220 3d20 6e61 7061 7269 5f63  otter = napari_c
+00000630: 6c75 7374 6572 735f 706c 6f74 7465 720d  lusters_plotter.
+00000640: 0a0d 0a5b 666c 616b 6538 5d0d 0a6d 6178  ...[flake8]..max
+00000650: 2d6c 696e 652d 6c65 6e67 7468 203d 2031  -line-length = 1
+00000660: 3230 0d0a 6967 6e6f 7265 203d 2045 3230  20..ignore = E20
+00000670: 332c 5735 3033 2c43 3930 312c 4638 3233  3,W503,C901,F823
+00000680: 0d0a 6d61 782d 636f 6d70 6c65 7869 7479  ..max-complexity
+00000690: 203d 2031 380d 0a62 7569 6c74 696e 7320   = 18..builtins 
+000006a0: 3d20 7079 7465 7374 0d0a 6578 636c 7564  = pytest..exclud
+000006b0: 6520 3d20 6e61 7061 7269 5f63 6c75 7374  e = napari_clust
+000006c0: 6572 735f 706c 6f74 7465 722f 5f5f 696e  ers_plotter/__in
+000006d0: 6974 5f5f 2e70 792c 2065 7861 6d70 6c65  it__.py, example
+000006e0: 5f64 6174 612c 2069 6d61 6765 732c 206e  _data, images, n
+000006f0: 6170 6172 695f 636c 7573 7465 7273 5f70  apari_clusters_p
+00000700: 6c6f 7474 6572 2f5f 6765 745f 636f 6c6f  lotter/_get_colo
+00000710: 726d 6170 2e70 790d 0a62 616e 6e65 642d  rmap.py..banned-
+00000720: 6d6f 6475 6c65 7320 3d20 5079 5174 3520  modules = PyQt5 
+00000730: 3d20 7573 6520 7174 7079 0d0a 0950 7953  = use qtpy...PyS
+00000740: 6964 6532 203d 2075 7365 2071 7470 790d  ide2 = use qtpy.
+00000750: 0a0d 0a5b 6973 6f72 745d 0d0a 7072 6f66  ...[isort]..prof
+00000760: 696c 6520 3d20 626c 6163 6b0d 0a0d 0a5b  ile = black....[
+00000770: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000780: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000790: 6520 3d20 300d 0a0d 0a                   e = 0....
```


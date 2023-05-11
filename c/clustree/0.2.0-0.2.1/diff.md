# Comparing `tmp/clustree-0.2.0.tar.gz` & `tmp/clustree-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustree-0.2.0.tar", max compression
+gzip compressed data, was "clustree-0.2.1.tar", max compression
```

## Comparing `clustree-0.2.0.tar` & `clustree-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-01-20 09:22:00.300232 clustree-0.2.0/LICENSE
--rw-r--r--   0        0        0     5463 2023-03-17 13:32:09.262011 clustree-0.2.0/README.md
--rw-r--r--   0        0        0     1500 2023-03-17 13:32:09.264135 clustree-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-03-17 13:32:09.264526 clustree-0.2.0/src/clustree/__init__.py
--rw-r--r--   0        0        0      874 2023-03-17 13:32:09.264927 clustree-0.2.0/src/clustree/_clustree_typing.py
--rw-r--r--   0        0        0     7767 2023-03-17 13:32:09.265533 clustree-0.2.0/src/clustree/_config.py
--rw-r--r--   0        0        0     1268 2023-03-17 13:32:09.265943 clustree-0.2.0/src/clustree/_config_helpers.py
--rw-r--r--   0        0        0     7610 2023-03-17 13:32:09.266211 clustree-0.2.0/src/clustree/_draw.py
--rw-r--r--   0        0        0     7226 2023-03-17 13:32:09.266644 clustree-0.2.0/src/clustree/_graph.py
--rw-r--r--   0        0        0      957 2023-03-17 13:32:09.266930 clustree-0.2.0/src/clustree/_handle_pars.py
--rw-r--r--   0        0        0      251 2023-03-17 13:32:09.267203 clustree-0.2.0/src/clustree/_hash.py
--rw-r--r--   0        0        0        0 2023-03-02 16:01:16.422737 clustree-0.2.0/src/clustree/py.typed
--rw-r--r--   0        0        0     6460 1970-01-01 00:00:00.000000 clustree-0.2.0/setup.py
--rw-r--r--   0        0        0     6767 1970-01-01 00:00:00.000000 clustree-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-20 09:22:00.300232 clustree-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5614 2023-05-11 11:42:04.817353 clustree-0.2.1/README.md
+-rw-r--r--   0        0        0     1500 2023-05-11 11:42:04.819559 clustree-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-03-17 13:32:09.264526 clustree-0.2.1/src/clustree/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-11 11:42:04.819831 clustree-0.2.1/src/clustree/_clustree_typing.py
+-rw-r--r--   0        0        0     7767 2023-05-11 11:22:32.192524 clustree-0.2.1/src/clustree/_config.py
+-rw-r--r--   0        0        0     1268 2023-03-17 13:32:09.265943 clustree-0.2.1/src/clustree/_config_helpers.py
+-rw-r--r--   0        0        0     7610 2023-03-17 13:32:09.266211 clustree-0.2.1/src/clustree/_draw.py
+-rw-r--r--   0        0        0     7508 2023-05-11 11:42:04.820264 clustree-0.2.1/src/clustree/_graph.py
+-rw-r--r--   0        0        0      957 2023-03-17 13:32:09.266930 clustree-0.2.1/src/clustree/_handle_pars.py
+-rw-r--r--   0        0        0      251 2023-05-11 11:32:18.903696 clustree-0.2.1/src/clustree/_hash.py
+-rw-r--r--   0        0        0        0 2023-03-02 16:01:16.422737 clustree-0.2.1/src/clustree/py.typed
+-rw-r--r--   0        0        0     6611 1970-01-01 00:00:00.000000 clustree-0.2.1/setup.py
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 clustree-0.2.1/PKG-INFO
```

### Comparing `clustree-0.2.0/LICENSE` & `clustree-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clustree-0.2.0/README.md` & `clustree-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 * `node_color` : For continuous colormap, use 'samples' or the name of a metadata column to color nodes by. For discrete colors, use 'prefix' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set equal to value of prefix to color by resolution.
 * `node_color_aggr` : If node_color is a column name then a function or string giving the name of a function to aggregate that column for samples in each cluster.
 * `node_cmap` : If node_color is 'samples' or a column name then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).
 * `edge_color` : For continuous colormap, use 'samples'. For discrete colors, use 'prefix' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set to 'samples'.
 * `edge_cmap` : If edge_color is 'samples' then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).
 * `orientation` : Orientation of clustree drawing. Defaults to 'vertical'.
 * `layout_reingold_tilford` : Whether to use the Reingold-Tilford algorithm for node positioning. Defaults to True if (kk <= 12), False otherwise. Setting True not recommended if (kk > 12) due to memory bottleneck in igraph dependency.
-* `min_cluster_number` : 0 if cluster number is (0, ..., K-1) or 1 if (1, ..., K). Defaults to 1.
+* `min_cluster_number` : Cluster number can take values (0, ..., K-1) or (1, ..., K). If the former option is preferred, parameter should take value 0, and 1 otherwise. Defaults to None, in which case, minimum cluster number is found automatically.
 * `border_size` : Border width as proportion of image width. Defaults to 0.05.
 * `figsize` : Parsed to matplotlib to determine figure size. Defaults to (kk/2, kk/2), clipped to a minimum of (3,3) and maximum of (10,10).
 * `arrows` : Whether to add arrows to graph edges. Removing arrows alleviates appearance issue caused by arrows overlapping nodes. Defaults to True.
 * `node_size` : Size of nodes in clustree graph drawing. Parsed directly to networkx.draw_networkx_nodes. Default to 300.
 * `node_size_edge`: Controls edge start and end point. Parsed directly to networkx.draw_networkx_edges.
 * `dpi` : Controls resolution of output if saved to file.
 * `kk` : Choose custom depth of clustree graph.
```

### Comparing `clustree-0.2.0/pyproject.toml` & `clustree-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clustree"
-version = "0.2.0"
+version = "0.2.1"
 description = "Visualize relationship between clusterings at different resolutions"
 authors = ["Ben Barlow <ben-j-barlow.1@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/ben-j-barlow/clustree"
 repository = "https://github.com/ben-j-barlow/clustree"
 keywords = ["clustering", "visualization", "visualisation", "clustering-trees", "cluster-trees"]
```

### Comparing `clustree-0.2.0/src/clustree/_clustree_typing.py` & `clustree-0.2.1/src/clustree/_clustree_typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     int,  # (K, k_start, k_end) hashed
     dict[str, Any],  # 'color', 'samples', 'alpha', 'start', 'end', 'res'
 ]
 
 DATA_INPUT_TYPE = Union[str, Path, pd.DataFrame]
 IMAGE_INPUT_TYPE = Union[str, Path]
 ORIENTATION_INPUT_TYPE = Literal["vertical", "horizontal"]
-MIN_CLUSTER_NUMBER_TYPE = Literal[0, 1]
+MIN_CLUSTER_NUMBER_TYPE = Optional[Literal[0, 1]]
 CIRCLE_POS_TYPE = Optional[Literal["tl", "t", "tr", "l", "r", "bl", "b", "br"]]
 
 NODE_COLOR_TYPE = str  # e.g. 'samples', 'K', data col name
 EDGE_COLOR_TYPE = str
 COLOR_AGG_TYPE = Optional[Union[Callable, str]]
 CMAP_TYPE = Union[mpl.colors.Colormap, str]
```

### Comparing `clustree-0.2.0/src/clustree/_config.py` & `clustree-0.2.1/src/clustree/_config.py`

 * *Files identical despite different names*

### Comparing `clustree-0.2.0/src/clustree/_config_helpers.py` & `clustree-0.2.1/src/clustree/_config_helpers.py`

 * *Files identical despite different names*

### Comparing `clustree-0.2.0/src/clustree/_draw.py` & `clustree-0.2.1/src/clustree/_draw.py`

 * *Files identical despite different names*

### Comparing `clustree-0.2.0/src/clustree/_graph.py` & `clustree-0.2.1/src/clustree/_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     node_color: NODE_COLOR_TYPE = "prefix",
     node_color_aggr: COLOR_AGG_TYPE = None,
     node_cmap: CMAP_TYPE = "inferno",
     edge_color: EDGE_COLOR_TYPE = "samples",
     edge_cmap: CMAP_TYPE = "viridis",
     orientation: ORIENTATION_INPUT_TYPE = "vertical",
     layout_reingold_tilford: bool = None,
-    min_cluster_number: MIN_CLUSTER_NUMBER_TYPE = 1,
+    min_cluster_number: MIN_CLUSTER_NUMBER_TYPE = None,
     border_size: float = 0.05,
     figsize: tuple[float, float] = None,
     arrows: bool = None,
     node_size: float = 300,
     node_size_edge: Optional[float] = None,
     dpi: float = 500,
     kk: Optional[int] = None,
@@ -80,16 +80,18 @@
         tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).
     orientation : Literal["vertical", "horizontal"]
         Orientation of clustree drawing. Defaults to 'vertical'.
     layout_reingold_tilford : bool, optional
         Whether to use the Reingold-Tilford algorithm for node positioning. Defaults \
         to True if (kk <= 12), False otherwise. Setting True not recommended if \
         (kk > 12) due to memory bottleneck in igraph dependency.
-    min_cluster_number : Literal[0, 1]
-        0 if cluster number is (0, ..., K-1) or 1 if (1, ..., K). Defaults to 1.
+    min_cluster_number : Literal[0, 1], optional
+        Cluster number can take values (0, ..., K-1) or (1, ..., K). If the former \
+        option is preferred, parameter should take value 0, and 1 otherwise. \
+        Defaults to None, in which case, minimum cluster number is found automatically.
     border_size : float
         Border width as proportion of image width. Defaults to 0.05.
     figsize : tuple[float, float]
         Parsed to matplotlib to determine figure size. Defaults to (kk/2, kk/2), \
         clipped to a minimum of (3,3) and maximum of (10,10).
     arrows : bool
         Whether to add arrows to graph edges. Removing arrows alleviates appearance \
@@ -126,15 +128,18 @@
     _data = handle_data(data=data)
     kk = get_and_check_cluster_cols(cols=_data.columns, prefix=prefix, user_kk=kk)
 
     border_size = float(border_size)
     images = str(images)
     if images[-1] != "/":
         images = images + "/"
-    start_at_1 = bool(min_cluster_number)
+    if min_cluster_number:
+        start_at_1 = bool(min_cluster_number)
+    else:
+        start_at_1 = int(_data[f"{prefix}1"].min()) == 1
     if not figsize:
         if kk < 6:
             figsize = (3, 3)
         else:
             w = min([kk, 20]) / 2
             figsize = (w, w)
     if arrows is None:
```

### Comparing `clustree-0.2.0/src/clustree/_handle_pars.py` & `clustree-0.2.1/src/clustree/_handle_pars.py`

 * *Files identical despite different names*

### Comparing `clustree-0.2.0/setup.py` & `clustree-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'networkx>=3,<4',
  'opencv-python>=4.7.0.72,<5.0.0.0',
  'pairing-functions==0.2.1',
  'pandas>=1.5,<2.0']
 
 setup_kwargs = {
     'name': 'clustree',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Visualize relationship between clusterings at different resolutions',
-    'long_description': '# clustree\n\n## Status\n\n**Functionality: Implemented**\n\n* Directed graph representing clustree. Nodes are parsed images and node information is encoded by a border surrounding the image.\n* Loading: Data provided directly or through a path to parent directory. Images provided through a path to parent directory.\n* Appearance: Edge and node color can correspond to one of: #samples that pass through edge/node, cluster resolution `K`, or a fixed color. In the case of node color, a column name in the data and aggregate function can be used too. Use of column name and #samples creates a continuous colormap, whilst the other options result in discrete colors.\n* Layout: Reingold-Tilford algorithm used for node positioning. Not recommended for kk > 12 due to memory bottleneck in igraph dependency.\n* Legend: demonstration of node / edge color.\n\n\n**Functionality: To Add**\n\n* Legend: demonstration of transparency of edges.\n* Layout: Bespoke implementation of Reingold-Tilford algorithm to overcome dependency\'s memory bottleneck.\n\n## Usage\n\n### Installation\n\nInstall the package with pip:\n\n```\npip install clustree\n```\n\n### Quickstart\n\nThe powerhouse function of the library is `clustree`. Use\n\n```\nfrom clustree import clustree\n```\n\nto import the function. A detailed description of the parameters is provided below.\n\n```\ndef clustree(\n    data: Union[Path, str],\n    prefix: str,\n    images: Union[Path, str],\n    output_path: Optional[Union[Path, str]] = None,\n    draw: bool = True,\n    node_color: str = "prefix",\n    node_color_aggr: Optional[Union[Callable, str]] = None,\n    node_cmap: Union[mpl.colors.Colormap, str] = "inferno",\n    edge_color: str = "samples",\n    edge_cmap: Union[mpl.colors.Colormap, str] = "viridis",\n    orientation: Literal["vertical", "horizontal"] = "vertical",\n    layout_reingold_tilford: bool = None,\n    min_cluster_number: Literal[0, 1] = 1,\n    border_size: float = 0.05,\n    figsize: tuple[float, float] = None,\n    arrows: bool = None,\n    node_size: float = 300,\n    node_size_edge: Optional[float] = None,\n    dpi: float = 500,\n    kk: Optional[int] = None,\n) -> DiGraph:\n    """\n\n```\n\n* `data` : Path of csv or DataFrame object.\n* `prefix` : String indicating columns containing clustering information.\n* `images` : Path of directory that contains images.\n* `output_path` : Absolute path to save clustree drawing at. If file extension is supplied, must be .png. If None, then output not written to file.\n* `draw` : Whether to draw the clustree. Defaults to True. If False and output_path supplied, will be overridden.\n* `node_color` : For continuous colormap, use \'samples\' or the name of a metadata column to color nodes by. For discrete colors, use \'prefix\' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set equal to value of prefix to color by resolution.\n* `node_color_aggr` : If node_color is a column name then a function or string giving the name of a function to aggregate that column for samples in each cluster.\n* `node_cmap` : If node_color is \'samples\' or a column name then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).\n* `edge_color` : For continuous colormap, use \'samples\'. For discrete colors, use \'prefix\' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set to \'samples\'.\n* `edge_cmap` : If edge_color is \'samples\' then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).\n* `orientation` : Orientation of clustree drawing. Defaults to \'vertical\'.\n* `layout_reingold_tilford` : Whether to use the Reingold-Tilford algorithm for node positioning. Defaults to True if (kk <= 12), False otherwise. Setting True not recommended if (kk > 12) due to memory bottleneck in igraph dependency.\n* `min_cluster_number` : 0 if cluster number is (0, ..., K-1) or 1 if (1, ..., K). Defaults to 1.\n* `border_size` : Border width as proportion of image width. Defaults to 0.05.\n* `figsize` : Parsed to matplotlib to determine figure size. Defaults to (kk/2, kk/2), clipped to a minimum of (3,3) and maximum of (10,10).\n* `arrows` : Whether to add arrows to graph edges. Removing arrows alleviates appearance issue caused by arrows overlapping nodes. Defaults to True.\n* `node_size` : Size of nodes in clustree graph drawing. Parsed directly to networkx.draw_networkx_nodes. Default to 300.\n* `node_size_edge`: Controls edge start and end point. Parsed directly to networkx.draw_networkx_edges.\n* `dpi` : Controls resolution of output if saved to file.\n* `kk` : Choose custom depth of clustree graph.\n\n## Glossary\n\n* *cluster resolution*: Upper case `K`. For example, at cluster resolution `K=2` data is clustered into 2 distinct clusters.\n* *cluster number*: Lower case `k`. For example, at cluster resolution 2 data is clustered into 2 distinct clusters `k=1` and `k=2`.\n* *kk*: highest value of `K` (cluster resolution) shown in clustree.\n* *cluster membership*: The association between data points and cluster numbers for fixed cluster resolution. For example, `[1, 1, 2, 2, 2]` would mean the first 2 data points belong to cluster number `1` and the following 3 data points belong to cluster number `2`.',
+    'long_description': '# clustree\n\n## Status\n\n**Functionality: Implemented**\n\n* Directed graph representing clustree. Nodes are parsed images and node information is encoded by a border surrounding the image.\n* Loading: Data provided directly or through a path to parent directory. Images provided through a path to parent directory.\n* Appearance: Edge and node color can correspond to one of: #samples that pass through edge/node, cluster resolution `K`, or a fixed color. In the case of node color, a column name in the data and aggregate function can be used too. Use of column name and #samples creates a continuous colormap, whilst the other options result in discrete colors.\n* Layout: Reingold-Tilford algorithm used for node positioning. Not recommended for kk > 12 due to memory bottleneck in igraph dependency.\n* Legend: demonstration of node / edge color.\n\n\n**Functionality: To Add**\n\n* Legend: demonstration of transparency of edges.\n* Layout: Bespoke implementation of Reingold-Tilford algorithm to overcome dependency\'s memory bottleneck.\n\n## Usage\n\n### Installation\n\nInstall the package with pip:\n\n```\npip install clustree\n```\n\n### Quickstart\n\nThe powerhouse function of the library is `clustree`. Use\n\n```\nfrom clustree import clustree\n```\n\nto import the function. A detailed description of the parameters is provided below.\n\n```\ndef clustree(\n    data: Union[Path, str],\n    prefix: str,\n    images: Union[Path, str],\n    output_path: Optional[Union[Path, str]] = None,\n    draw: bool = True,\n    node_color: str = "prefix",\n    node_color_aggr: Optional[Union[Callable, str]] = None,\n    node_cmap: Union[mpl.colors.Colormap, str] = "inferno",\n    edge_color: str = "samples",\n    edge_cmap: Union[mpl.colors.Colormap, str] = "viridis",\n    orientation: Literal["vertical", "horizontal"] = "vertical",\n    layout_reingold_tilford: bool = None,\n    min_cluster_number: Literal[0, 1] = 1,\n    border_size: float = 0.05,\n    figsize: tuple[float, float] = None,\n    arrows: bool = None,\n    node_size: float = 300,\n    node_size_edge: Optional[float] = None,\n    dpi: float = 500,\n    kk: Optional[int] = None,\n) -> DiGraph:\n    """\n\n```\n\n* `data` : Path of csv or DataFrame object.\n* `prefix` : String indicating columns containing clustering information.\n* `images` : Path of directory that contains images.\n* `output_path` : Absolute path to save clustree drawing at. If file extension is supplied, must be .png. If None, then output not written to file.\n* `draw` : Whether to draw the clustree. Defaults to True. If False and output_path supplied, will be overridden.\n* `node_color` : For continuous colormap, use \'samples\' or the name of a metadata column to color nodes by. For discrete colors, use \'prefix\' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set equal to value of prefix to color by resolution.\n* `node_color_aggr` : If node_color is a column name then a function or string giving the name of a function to aggregate that column for samples in each cluster.\n* `node_cmap` : If node_color is \'samples\' or a column name then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).\n* `edge_color` : For continuous colormap, use \'samples\'. For discrete colors, use \'prefix\' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set to \'samples\'.\n* `edge_cmap` : If edge_color is \'samples\' then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).\n* `orientation` : Orientation of clustree drawing. Defaults to \'vertical\'.\n* `layout_reingold_tilford` : Whether to use the Reingold-Tilford algorithm for node positioning. Defaults to True if (kk <= 12), False otherwise. Setting True not recommended if (kk > 12) due to memory bottleneck in igraph dependency.\n* `min_cluster_number` : Cluster number can take values (0, ..., K-1) or (1, ..., K). If the former option is preferred, parameter should take value 0, and 1 otherwise. Defaults to None, in which case, minimum cluster number is found automatically.\n* `border_size` : Border width as proportion of image width. Defaults to 0.05.\n* `figsize` : Parsed to matplotlib to determine figure size. Defaults to (kk/2, kk/2), clipped to a minimum of (3,3) and maximum of (10,10).\n* `arrows` : Whether to add arrows to graph edges. Removing arrows alleviates appearance issue caused by arrows overlapping nodes. Defaults to True.\n* `node_size` : Size of nodes in clustree graph drawing. Parsed directly to networkx.draw_networkx_nodes. Default to 300.\n* `node_size_edge`: Controls edge start and end point. Parsed directly to networkx.draw_networkx_edges.\n* `dpi` : Controls resolution of output if saved to file.\n* `kk` : Choose custom depth of clustree graph.\n\n## Glossary\n\n* *cluster resolution*: Upper case `K`. For example, at cluster resolution `K=2` data is clustered into 2 distinct clusters.\n* *cluster number*: Lower case `k`. For example, at cluster resolution 2 data is clustered into 2 distinct clusters `k=1` and `k=2`.\n* *kk*: highest value of `K` (cluster resolution) shown in clustree.\n* *cluster membership*: The association between data points and cluster numbers for fixed cluster resolution. For example, `[1, 1, 2, 2, 2]` would mean the first 2 data points belong to cluster number `1` and the following 3 data points belong to cluster number `2`.',
     'author': 'Ben Barlow',
     'author_email': 'ben-j-barlow.1@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ben-j-barlow/clustree',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `clustree-0.2.0/PKG-INFO` & `clustree-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustree
-Version: 0.2.0
+Version: 0.2.1
 Summary: Visualize relationship between clusterings at different resolutions
 Home-page: https://github.com/ben-j-barlow/clustree
 License: GPL-3.0-or-later
 Keywords: clustering,visualization,visualisation,clustering-trees,cluster-trees
 Author: Ben Barlow
 Author-email: ben-j-barlow.1@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -101,15 +101,15 @@
 * `node_color` : For continuous colormap, use 'samples' or the name of a metadata column to color nodes by. For discrete colors, use 'prefix' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set equal to value of prefix to color by resolution.
 * `node_color_aggr` : If node_color is a column name then a function or string giving the name of a function to aggregate that column for samples in each cluster.
 * `node_cmap` : If node_color is 'samples' or a column name then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).
 * `edge_color` : For continuous colormap, use 'samples'. For discrete colors, use 'prefix' to color by resolution or specify a fixed color (see Specifying colors in Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colors.html). If None, default set to 'samples'.
 * `edge_cmap` : If edge_color is 'samples' then a colourmap to use (see Colormap Matplotlib tutorial here: https://matplotlib.org/stable/tutorials/colors/colormaps.html).
 * `orientation` : Orientation of clustree drawing. Defaults to 'vertical'.
 * `layout_reingold_tilford` : Whether to use the Reingold-Tilford algorithm for node positioning. Defaults to True if (kk <= 12), False otherwise. Setting True not recommended if (kk > 12) due to memory bottleneck in igraph dependency.
-* `min_cluster_number` : 0 if cluster number is (0, ..., K-1) or 1 if (1, ..., K). Defaults to 1.
+* `min_cluster_number` : Cluster number can take values (0, ..., K-1) or (1, ..., K). If the former option is preferred, parameter should take value 0, and 1 otherwise. Defaults to None, in which case, minimum cluster number is found automatically.
 * `border_size` : Border width as proportion of image width. Defaults to 0.05.
 * `figsize` : Parsed to matplotlib to determine figure size. Defaults to (kk/2, kk/2), clipped to a minimum of (3,3) and maximum of (10,10).
 * `arrows` : Whether to add arrows to graph edges. Removing arrows alleviates appearance issue caused by arrows overlapping nodes. Defaults to True.
 * `node_size` : Size of nodes in clustree graph drawing. Parsed directly to networkx.draw_networkx_nodes. Default to 300.
 * `node_size_edge`: Controls edge start and end point. Parsed directly to networkx.draw_networkx_edges.
 * `dpi` : Controls resolution of output if saved to file.
 * `kk` : Choose custom depth of clustree graph.
```


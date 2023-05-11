# Comparing `tmp/magnify-0.2.1.tar.gz` & `tmp/magnify-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.2.1.tar", max compression
+gzip compressed data, was "magnify-0.2.2.tar", max compression
```

## Comparing `magnify-0.2.1.tar` & `magnify-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.2.1/README.md
--rw-r--r--   0        0        0     1601 2023-04-11 21:33:19.187520 magnify-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      200 2023-04-11 21:33:12.099352 magnify-0.2.1/src/magnify/__init__.py
--rw-r--r--   0        0        0    24766 2023-04-11 21:20:33.945339 magnify-0.2.1/src/magnify/find.py
--rw-r--r--   0        0        0     1406 2023-04-08 03:43:27.466454 magnify-0.2.1/src/magnify/pipeline.py
--rw-r--r--   0        0        0      158 2023-04-07 22:03:32.255470 magnify-0.2.1/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1735 2023-04-11 21:20:43.805573 magnify-0.2.1/src/magnify/preprocess.py
--rw-r--r--   0        0        0    13646 2023-04-11 21:28:02.015984 magnify-0.2.1/src/magnify/reader.py
--rw-r--r--   0        0        0     3154 2023-04-08 03:43:33.554598 magnify-0.2.1/src/magnify/registry.py
--rw-r--r--   0        0        0     1121 2023-04-07 21:54:06.746151 magnify-0.2.1/src/magnify/stitch.py
--rw-r--r--   0        0        0     1583 2023-04-08 03:43:14.150139 magnify-0.2.1/src/magnify/utils.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 magnify-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.2.2/README.md
+-rw-r--r--   0        0        0     1601 2023-05-11 17:10:32.989687 magnify-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-05-11 17:10:39.829824 magnify-0.2.2/src/magnify/__init__.py
+-rw-r--r--   0        0        0     4586 2023-04-19 17:49:40.798430 magnify-0.2.2/src/magnify/filter.py
+-rw-r--r--   0        0        0    26017 2023-04-20 23:51:46.110906 magnify-0.2.2/src/magnify/find.py
+-rw-r--r--   0        0        0     1406 2023-04-14 21:30:07.711891 magnify-0.2.2/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      291 2023-04-14 03:25:12.785396 magnify-0.2.2/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     2348 2023-05-09 14:34:10.399616 magnify-0.2.2/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     1855 2023-05-11 01:21:29.027397 magnify-0.2.2/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     2488 2023-05-11 02:09:19.162200 magnify-0.2.2/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      650 2023-05-11 02:30:53.591879 magnify-0.2.2/src/magnify/plot/style.py
+-rw-r--r--   0        0        0     1033 2023-04-20 23:51:45.846900 magnify-0.2.2/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1736 2023-04-14 21:30:15.276066 magnify-0.2.2/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    14065 2023-04-19 01:42:37.155610 magnify-0.2.2/src/magnify/reader.py
+-rw-r--r--   0        0        0     3374 2023-04-19 18:59:40.761736 magnify-0.2.2/src/magnify/registry.py
+-rw-r--r--   0        0        0     1121 2023-04-07 21:54:06.746151 magnify-0.2.2/src/magnify/stitch.py
+-rw-r--r--   0        0        0     2644 2023-04-21 02:34:29.243260 magnify-0.2.2/src/magnify/utils.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 magnify-0.2.2/PKG-INFO
```

### Comparing `magnify-0.2.1/pyproject.toml` & `magnify-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.2.1"
+version = "0.2.2"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
```

### Comparing `magnify-0.2.1/src/magnify/find.py` & `magnify-0.2.2/src/magnify/find.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import math
 import logging
 
 from numpy.typing import ArrayLike
 import cv2 as cv
 import dask.array as da
 import numpy as np
 import scipy
@@ -19,141 +20,121 @@
 class ButtonFinder:
     def __init__(
         self,
         row_dist: float = 375 / 3.22,
         col_dist: float = 655 / 3.22,
         min_button_radius: int = 4,
         max_button_radius: int = 15,
-        cluster_penalty: float = 10,
+        cluster_penalty: float = 50,
         roi_length: int = 61,
         progress_bar: bool = False,
-        search_timesteps: list[int] | None = None,
+        search_timestep: list[int] | None = None,
+        search_channel: str | list[str] | None = None,
     ):
         self.row_dist = row_dist
         self.col_dist = col_dist
         self.min_button_radius = min_button_radius
         self.max_button_radius = max_button_radius
         self.cluster_penalty = cluster_penalty
         self.roi_length = roi_length
         self.progress_bar = progress_bar
-        self.search_timesteps = search_timesteps
+        self.search_timesteps = utils.to_list(search_timestep)
+        if search_channel == "all":
+            self.search_channels = assay.channel
+        else:
+            self.search_channels = utils.to_list(search_channel)
 
     def __call__(self, assay: xr.Dataset) -> xr.Dataset:
-        num_rows, num_cols = assay.id.shape
-        if isinstance(assay.search_channel, str):
-            if assay.search_channel in assay.channel:
-                search_channels = [assay.search_channel]
-            elif assay.search_channel == "all":
-                search_channels = assay.channel
-            else:
-                raise ValueError(f"{assay.search_channel} is not a channel name.")
-        else:
-            # We're searching across multiple channels.
-            search_channels = assay.search_channel
+        num_rows, num_cols = assay.mark_tag.shape
 
+        # Store all channels and timesteps for each marker in one chunk and set marker row/col
+        # sizes so each chunk ends up being at least 10MB.
+        chunk_bytes = 1e7
+        # Don't take into account dtype size since fg/bg bool arrays should also be 10MB.
+        mark_bytes = assay.dims["channel"] * assay.dims["time"] * self.roi_length**2
+        # Prioritize larger row chunks since we're more likely to want whole columns than rows.
+        row_chunk_size = min(math.ceil(chunk_bytes / mark_bytes), num_rows)
+        col_chunk_size = math.ceil(chunk_bytes / (mark_bytes * row_chunk_size))
         # Create the array of subimage regions.
         roi = da.empty(
             (
                 num_rows,
                 num_cols,
                 assay.dims["channel"],
                 assay.dims["time"],
                 self.roi_length,
                 self.roi_length,
             ),
             dtype=assay.image.dtype,
             chunks=(
-                1,
-                1,
+                row_chunk_size,
+                col_chunk_size,
                 assay.dims["channel"],
                 assay.dims["time"],
                 self.roi_length,
                 self.roi_length,
             ),
         )
         assay = assay.assign(
             roi=(
-                ("marker_row", "marker_col", "channel", "time", "roi_y", "roi_x"),
+                ("mark_row", "mark_col", "channel", "time", "roi_y", "roi_x"),
                 roi,
             ),
             fg=(
-                ("marker_row", "marker_col", "channel", "time", "roi_y", "roi_x"),
+                ("mark_row", "mark_col", "channel", "time", "roi_y", "roi_x"),
                 da.empty_like(
                     roi,
                     dtype=bool,
                 ),
             ),
             bg=(
-                ("marker_row", "marker_col", "channel", "time", "roi_y", "roi_x"),
+                ("mark_row", "mark_col", "channel", "time", "roi_y", "roi_x"),
                 da.empty_like(
                     roi,
                     dtype=bool,
                 ),
             ),
         )
         # Create the x and y coordinates arrays for each button.
         assay = assay.assign(
             x=(
-                ("marker_row", "marker_col", "time"),
+                ("mark_row", "mark_col", "time"),
                 np.empty((num_rows, num_cols, assay.dims["time"])),
             ),
             y=(
-                ("marker_row", "marker_col", "time"),
+                ("mark_row", "mark_col", "time"),
                 np.empty((num_rows, num_cols, assay.dims["time"])),
             ),
         )
 
         # Run the button finding algorithm for each timestep.
         for t, time in enumerate(tqdm.tqdm(assay.time, disable=not self.progress_bar)):
             # Preload all images for this timestep so we only read from disk once.
             images = assay.image.sel(time=time).compute()
             # Re-use the previous button locations if the user has specified that we should only
             # search on specific timesteps.
-            do_search = t == 0 or self.search_timesteps is None or t in self.search_timesteps
+            do_search = t == 0 or t in self.search_timesteps
 
             # Find button centers.
             if do_search:
                 assay.x[..., t], assay.y[..., t] = self.find_centers(
-                    images.sel(channel=search_channels), assay
+                    images.sel(channel=self.search_channels), assay
                 )
             else:
                 assay.x[..., t] = assay.x[..., t - 1]
                 assay.y[..., t] = assay.y[..., t - 1]
 
-            # Extract a region around each button.
-            offsets = np.empty((num_rows, num_cols, 2), dtype=int)
-            roi = xr.DataArray(
-                data=np.empty_like(assay.roi[:, :, :, t]), coords=assay.roi[:, :, :, t].coords
+            # Compute the roi, foreground and background masks for all buttons.
+            assay.roi[:, :, :, t], assay.fg[:, :, :, t], assay.bg[:, :, :, t] = self.find_rois(
+                images, t, do_search, assay
             )
-            for i in range(num_rows):
-                for j in range(num_cols):
-                    top, bottom, left, right = utils.bounding_box(
-                        round(float(assay.x[i, j, t])),
-                        round(float(assay.y[i, j, t])),
-                        self.roi_length,
-                        assay.sizes["im_y"],
-                        assay.sizes["im_x"],
-                    )
-                    roi[i, j] = images[:, top:bottom, left:right]
-                    offsets[i, j] = [left, top]
-            assay.roi[:, :, :, t] = roi
-
-            # Compute the foreground and background masks for all buttons.
-            if do_search:
-                assay.fg[:, :, :, t], assay.bg[:, :, :, t] = self.find_masks(
-                    roi.sel(channel=search_channels), offsets, t, assay
-                )
-            else:
-                assay.fg[:, :, :, t] = assay.fg[:, :, :, t - 1]
-                assay.bg[:, :, :, t] = assay.bg[:, :, :, t - 1]
-
-        # assay = assay.stack(marker=("marker_row", "marker_col"), create_index=True).transpose(
-        #     "marker", ...
+        # assay = assay.stack(mark=("mark_row", "mark_col"), create_index=True).transpose(
+        #     "mark", ...
         # )
-        # assay = assay.set_xindex("id")
+        # assay = assay.set_xindex("mark_tag")
 
         return assay
 
     def find_centers(self, images: xr.DataArray, assay: xr.Dataset):
         points = np.empty((0, 2))
         min_button_dist = round(min(self.row_dist, self.col_dist) / 2)
         if min_button_dist % 2 == 0:
@@ -198,17 +179,17 @@
             points = np.concatenate([points, new_points])
 
         # Split the points into x and y components.
         x = points[:, 0]
         y = points[:, 1]
 
         # Step 3: Cluster the points into distinct rows and columns.
-        points_per_row = (assay.id != "").sum(dim="marker_col")
-        points_per_col = (assay.id != "").sum(dim="marker_row")
-        num_rows, num_cols = assay.sizes["marker_row"], assay.sizes["marker_col"]
+        points_per_row = (assay.mark_tag != "").sum(dim="mark_col")
+        points_per_col = (assay.mark_tag != "").sum(dim="mark_row")
+        num_rows, num_cols = assay.sizes["mark_row"], assay.sizes["mark_col"]
         row_labels = cluster_1d(
             y,
             total_length=image.shape[0],
             num_clusters=num_rows,
             cluster_length=self.row_dist,
             ideal_num_points=points_per_row,
             penalty=self.cluster_penalty,
@@ -237,33 +218,54 @@
             x,
             labels=col_labels,
             num_clusters=num_cols,
             ideal_num_points=points_per_col,
         )
 
         # Step 5: Set button locations as the intersection of each line pair.
-        marker_y = (row_slope * col_intercepts[np.newaxis] + row_intercepts[:, np.newaxis]) / (
+        mark_y = (row_slope * col_intercepts[np.newaxis] + row_intercepts[:, np.newaxis]) / (
             1 - row_slope * col_slope
         )
-        marker_x = marker_y * col_slope + col_intercepts[np.newaxis]
+        mark_x = mark_y * col_slope + col_intercepts[np.newaxis]
+
+        return mark_x, mark_y
 
-        return marker_x, marker_y
+    def find_rois(self, images: xr.DataArray, t: int, do_search: bool, assay: xr.Dataset):
+        roi = xr.DataArray(
+            data=np.zeros_like(assay.roi[:, :, :, t]), coords=assay.roi[:, :, :, t].coords
+        )
+        num_rows, num_cols = assay.roi.shape[:2]
+        offsets = np.empty((num_rows, num_cols, 2), dtype=int)
+        # Initialize the roi images.
+        for i in range(num_rows):
+            for j in range(num_cols):
+                top, bottom, left, right = utils.bounding_box(
+                    round(float(assay.x[i, j, t])),
+                    round(float(assay.y[i, j, t])),
+                    self.roi_length,
+                    assay.sizes["im_y"],
+                    assay.sizes["im_x"],
+                )
+                roi[i, j] = images[..., top:bottom, left:right]
+                offsets[i, j] = left, top
+
+        if not do_search:
+            # If we're not searching just use the previous background/foreground masks.
+            return roi, assay.fg[:, :, :, t - 1].compute(), assay.bg[:, :, :, t - 1].compute()
 
-    def find_masks(self, roi: np.ndarray, offsets: np.ndarray, t: int, assay: xr.Dataset):
-        num_rows, num_cols = roi.shape[:2]
         fg = np.empty_like(roi, dtype=bool)
         bg = np.empty_like(fg)
         for i in range(num_rows):
             for j in range(num_cols):
                 # TODO: This step should occur over multiple channels.
-                subimage = utils.to_uint8(roi[i, j, 0].to_numpy())
+                subimage = utils.to_uint8(roi[i, j].sel(channel=self.search_channels[0]).to_numpy())
 
                 # Find circles to refine our button estimate unless we have a blank chamber.
                 circles = None
-                if assay.id[i, j] != "":
+                if assay.mark_tag[i, j] != "":
                     # Filter the subimage to smooth edges and remove noise.
                     filtered = cv.bilateralFilter(
                         subimage,
                         d=9,
                         sigmaColor=75,
                         sigmaSpace=75,
                         borderType=cv.BORDER_DEFAULT,
@@ -278,23 +280,40 @@
                         param1=20,
                         param2=5,
                         minRadius=self.min_button_radius,
                         maxRadius=self.max_button_radius,
                     )
 
                 # Update our estimate of the button position if we found some circles.
+                left, top = offsets[i, j]
                 if circles is not None:
                     circles = circles[0, :, :2]
-                    point = np.array([assay.x[i, j, t], assay.y[i, j, t]]) - offsets[i, j]
+                    # Change circle coordinates from roi to image coordinates.
+                    circles[:, 0] += left
+                    circles[:, 1] += top
+                    point = np.array([assay.x[i, j, t], assay.y[i, j, t]])
                     # Use the circle center closest to our previous estimate of the button.
                     closest_idx = np.argmin(np.linalg.norm(circles - point, axis=1))
-                    assay.x[i, j, t], assay.y[i, j, t] = circles[closest_idx] + offsets[i, j]
+                    assay.x[i, j, t], assay.y[i, j, t] = circles[closest_idx]
+                    # Move the roi bounding box to the center the new x, y values.
+                    top, bottom, left, right = utils.bounding_box(
+                        round(float(assay.x[i, j, t])),
+                        round(float(assay.y[i, j, t])),
+                        self.roi_length,
+                        assay.sizes["im_y"],
+                        assay.sizes["im_x"],
+                    )
+                    roi[i, j] = images[..., top:bottom, left:right]
+                    # TODO: This step should occur over multiple channels.
+                    subimage = utils.to_uint8(
+                        roi[i, j].sel(channel=self.search_channels[0]).to_numpy()
+                    )
 
-                x_rel = round(float(assay.x[i, j, t])) - offsets[i, j, 0]
-                y_rel = round(float(assay.y[i, j, t])) - offsets[i, j, 1]
+                x_rel = round(float(assay.x[i, j, t])) - left
+                y_rel = round(float(assay.y[i, j, t])) - top
 
                 # Set the foreground (the button) to be a circle of fixed radius.
                 fg_mask = utils.circle(
                     self.roi_length,
                     row=y_rel,
                     col=x_rel,
                     radius=self.max_button_radius,
@@ -317,46 +336,48 @@
                 )
                 dim_mask = ~cv.dilate(
                     bright_mask, np.ones((self.max_button_radius, self.max_button_radius))
                 )
                 bright_mask = bright_mask.astype(bool)
                 dim_mask = dim_mask.astype(bool)
 
-                # If part of the button is bright then set the foreground to that bright area.
+                # If enough of the button is bright then set the foreground to that bright area.
                 if np.any(fg_mask & bright_mask):
                     fg_mask &= bright_mask
 
                 # The background on the other hand should not be bright.
                 if np.any(bg_mask & dim_mask):
                     bg_mask &= dim_mask
 
                 fg[i, j] = fg_mask
                 bg[i, j] = bg_mask
 
-        return fg, bg
+        return roi, fg, bg
 
     @registry.components.register("find_buttons")
     def make(
         row_dist: float = 375 / 3.22,
         col_dist: float = 655 / 3.22,
         min_button_radius: int = 4,
         max_button_radius: int = 15,
-        cluster_penalty: float = 10,
+        cluster_penalty: float = 50,
         roi_length: int = 61,
         progress_bar: bool = False,
-        search_timesteps: list[int] | None = None,
+        search_timestep: list[int] | None = None,
+        search_channel: str | list[str] = "egfp",
     ):
         return ButtonFinder(
             row_dist=row_dist,
             col_dist=col_dist,
             min_button_radius=min_button_radius,
             cluster_penalty=cluster_penalty,
             roi_length=roi_length,
             progress_bar=progress_bar,
-            search_timesteps=search_timesteps,
+            search_timestep=search_timestep,
+            search_channel=search_channel,
         )
 
 
 class BeadFinder:
     def __init__(
         self,
         min_bead_radius: int = 10,
@@ -425,60 +446,60 @@
 
         # Update the assay object with the beads we found.
         if len(centers) > 0:
             num_beads = len(centers)
             # Create the array of subimage regions.
             assay = assay.assign(
                 roi=(
-                    ("marker", "channel", "time", "roi_y", "roi_x"),
+                    ("mark", "channel", "time", "roi_y", "roi_x"),
                     np.empty(
                         (
                             num_beads,
                             assay.dims["channel"],
                             assay.dims["time"],
                             self.roi_length,
                             self.roi_length,
                         ),
                         dtype=assay.image.dtype,
                     ),
                 ),
                 fg=(
-                    ("marker", "channel", "time", "roi_y", "roi_x"),
+                    ("mark", "channel", "time", "roi_y", "roi_x"),
                     np.empty(
                         (
                             num_beads,
                             assay.dims["channel"],
                             assay.dims["time"],
                             self.roi_length,
                             self.roi_length,
                         ),
                         dtype=bool,
                     ),
                 ),
                 bg=(
-                    ("marker", "channel", "time", "roi_y", "roi_x"),
+                    ("mark", "channel", "time", "roi_y", "roi_x"),
                     np.empty(
                         (
                             num_beads,
                             assay.dims["channel"],
                             assay.dims["time"],
                             self.roi_length,
                             self.roi_length,
                         ),
                         dtype=bool,
                     ),
                 ),
             )
             assay = assay.assign(
                 x=(
-                    ["marker", "time"],
+                    ["mark", "time"],
                     np.repeat(centers[:, np.newaxis, 0], assay.dims["time"], axis=1),
                 ),
                 y=(
-                    ["marker", "time"],
+                    ["mark", "time"],
                     np.repeat(centers[:, np.newaxis, 1], assay.dims["time"], axis=1),
                 ),
             )
 
             rois = np.empty(assay.roi.shape, dtype=assay.roi.dtype)
             fgs = np.empty(assay.roi.shape, dtype=bool)
             bgs = np.empty(assay.roi.shape, dtype=bool)
```

### Comparing `magnify-0.2.1/src/magnify/pipeline.py` & `magnify-0.2.2/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.1/src/magnify/preprocess.py` & `magnify-0.2.2/src/magnify/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 def horizontal_flip(assay: xr.Dataset):
     if "image" in assay:
         assay["image"] = assay.image.isel(im_x=slice(None, None, -1))
     else:
         assay["tile"] = assay.tile.isel(tile_x=slice(None, None, -1))
     return assay
 
+
 @registry.component("vertical_flip")
 def vertical_flip(assay: xr.Dataset):
     if "image" in assay:
         assay["image"] = assay.image.isel(im_y=slice(None, None, -1))
     else:
         assay["tile"] = assay.tile.isel(tile_y=slice(None, None, -1))
     return assay
```

### Comparing `magnify-0.2.1/src/magnify/reader.py` & `magnify-0.2.2/src/magnify/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -192,14 +192,18 @@
                 assay_info = info_dict[assay_name]
                 if assay_info:
                     info_idxs, time_idxs = (sorted(set(idx)) for idx in zip(*assay_info.keys()))
                     for info_idx in info_idxs:
                         info_vals = [assay_info[(info_idx, time_idx)] for time_idx in time_idxs]
                         coords[info_idx] = ("time", info_vals)
 
+                if "time" in coords:
+                    coords["time"] = pd.to_datetime(coords["time"])
+                    coords["time"] -= coords["time"][0]
+
                 # Put all our data into an xarray dataset.
                 assay = xr.Dataset(
                     {"tile": (dims_in_path + dims_in_file, tiles)},
                     coords=coords,
                     attrs={
                         "name": assay_name,
                         "search_channel": search_on,
@@ -239,15 +243,22 @@
     # Replace blanks with the empty string.
     df["MutantID"] = df["MutantID"].replace(blank, "")
     # Zero-index the indices.
     cols, rows = np.array(df["Indices"].to_list()).T - 1
     names = df["MutantID"].to_numpy(dtype=str, na_value="")
     names_array = np.empty((max(rows) + 1, max(cols) + 1), dtype=names.dtype)
     names_array[rows, cols] = names
-    assay = assay.assign_coords(id=(("marker_row", "marker_col"), names_array))
+    assay = assay.assign_coords(tag=np.unique(names_array))
+    assay = assay.assign_coords(mark_tag=(("mark_row", "mark_col"), names_array))
+    assay["valid"] = (
+        ("mark_row", "mark_col", "time"),
+        np.ones(
+            (assay.sizes["mark_row"], assay.sizes["mark_col"], assay.sizes["time"]), dtype=bool
+        ),
+    )
     return assay
 
 
 def extract_paths(pattern) -> dict[tuple[int, str, int, int], str]:
     pattern = os.path.expanduser(pattern)
 
     # Filter out special signifiers used for pattern matching.
```

### Comparing `magnify-0.2.1/src/magnify/registry.py` & `magnify-0.2.2/src/magnify/registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,17 +51,20 @@
     config = defaults.merge(confection.Config(kwargs))
     pipe = Pipeline("read", config=config)
     pipe.add_pipe("read_pinlist")
     # pipe.add_pipe("preprocessor")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("horizontal_flip")
-    pipe.add_pipe("vertical_flip")
     pipe.add_pipe("find_buttons")
     # pipe.add_pipe("background_filter")
+    pipe.add_pipe("filter_expression")
+    pipe.add_pipe("filter_nonround")
+    pipe.add_pipe("filter_leaky")
+    pipe.add_pipe("summarize_sum")
     pipe.add_pipe("squeeze")
 
     return pipe
 
 
 def pc_chip_pipeline(**kwargs):
     # Button centers are apart 412um vertically and 760um horizontally.
@@ -70,17 +73,20 @@
     config = defaults.merge(confection.Config(kwargs))
     pipe = Pipeline("read", config=config)
     pipe.add_pipe("read_pinlist")
     # pipe.add_pipe("preprocessor")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("horizontal_flip")
-    pipe.add_pipe("vertical_flip")
     pipe.add_pipe("find_buttons")
     # pipe.add_pipe("background_filter")
+    pipe.add_pipe("filter_expression")
+    pipe.add_pipe("filter_nonround")
+    pipe.add_pipe("filter_leaky")
+    pipe.add_pipe("summarize_sum")
     pipe.add_pipe("squeeze")
 
     return pipe
 
 
 def mrbles_pipeline(**kwargs):
     pipe = Pipeline("read", config=kwargs)
```

### Comparing `magnify-0.2.1/src/magnify/stitch.py` & `magnify-0.2.2/src/magnify/stitch.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.1/PKG-INFO` & `magnify-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.2.1
+Version: 0.2.2
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


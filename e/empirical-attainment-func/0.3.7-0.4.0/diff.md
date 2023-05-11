# Comparing `tmp/empirical_attainment_func-0.3.7-py3-none-any.whl.zip` & `tmp/empirical_attainment_func-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13741 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      545 b- defN 22-Sep-29 16:35 eaf/__init__.py
--rw-rw-r--  2.0 unx     7616 b- defN 22-Sep-10 18:50 eaf/eaf.py
--rw-rw-r--  2.0 unx    19011 b- defN 22-Sep-29 16:32 eaf/plot_surface.py
--rw-rw-r--  2.0 unx     7055 b- defN 22-Sep-12 17:31 eaf/utils.py
--rw-rw-r--  2.0 unx    10760 b- defN 22-Sep-29 16:36 empirical_attainment_func-0.3.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx      454 b- defN 22-Sep-29 16:36 empirical_attainment_func-0.3.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-29 16:36 empirical_attainment_func-0.3.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 22-Sep-29 16:36 empirical_attainment_func-0.3.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 22-Sep-29 16:36 empirical_attainment_func-0.3.7.dist-info/RECORD
-9 files, 46296 bytes uncompressed, 12425 bytes compressed:  73.2%
+Zip file size: 13804 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      545 b- defN 23-May-11 16:44 eaf/__init__.py
+-rw-rw-r--  2.0 unx     7680 b- defN 23-May-11 16:37 eaf/eaf.py
+-rw-rw-r--  2.0 unx    19195 b- defN 23-May-11 16:41 eaf/plot_surface.py
+-rw-rw-r--  2.0 unx     7055 b- defN 23-May-11 16:29 eaf/utils.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      432 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      759 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/RECORD
+9 files, 46522 bytes uncompressed, 12488 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: eaf/plot_surface.py
 Comment: 
 
 Filename: eaf/utils.py
 Comment: 
 
-Filename: empirical_attainment_func-0.3.7.dist-info/LICENSE
+Filename: empirical_attainment_func-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: empirical_attainment_func-0.3.7.dist-info/METADATA
+Filename: empirical_attainment_func-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: empirical_attainment_func-0.3.7.dist-info/WHEEL
+Filename: empirical_attainment_func-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: empirical_attainment_func-0.3.7.dist-info/top_level.txt
+Filename: empirical_attainment_func-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: empirical_attainment_func-0.3.7.dist-info/RECORD
+Filename: empirical_attainment_func-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eaf/__init__.py

```diff
@@ -1,14 +1,14 @@
 from eaf.eaf import get_empirical_attainment_surface
 from eaf.plot_surface import EmpiricalAttainmentFuncPlot
 from eaf.utils import pareto_front_to_surface
 
 
-__version__ = "0.3.7"
-__copyright__ = "Copyright (C) 2022 Shuhei Watanabe"
+__version__ = "0.4.0"
+__copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/empirical-attainment-func"
 
 
 __all__ = [
```

## eaf/eaf.py

```diff
@@ -21,16 +21,17 @@
     Returns:
         pf_set_list (List[np.ndarray]):
             The list of the Pareto front sets.
             The shape is (trial number, Pareto solution index, objective index).
             Note that each pareto front set is sorted based on the ascending order of
             the first objective.
     """
+    _cost_copy = costs.copy()
     pf_set_list: List[np.ndarray] = []
-    for _costs in costs:
+    for _costs in _cost_copy:
         # Sort by the first objective, then the second objective
         order = np.lexsort((-_costs[:, 1], _costs[:, 0]))
         _costs = _costs[order]
         pf_set_list.append(_costs[is_pareto_front(_costs, filter_duplication=True)])
     return pf_set_list
 
 
@@ -151,19 +152,20 @@
     if n_obj != 2:
         raise NotImplementedError("Three or more objectives are not supported.")
     if not all(1 <= level <= n_independent_runs for level in levels):
         raise ValueError(f"All elements in levels must be in [1, n_independent_runs], but got {levels}")
     if not np.all(np.maximum.accumulate(levels) == levels):
         raise ValueError(f"levels must be an increasing sequence, but got {levels}")
 
+    _costs = costs.copy()
     if larger_is_better_objectives is not None:
-        costs = _change_directions(costs, larger_is_better_objectives=larger_is_better_objectives)
+        _costs = _change_directions(_costs, larger_is_better_objectives=larger_is_better_objectives)
 
     log_scale = log_scale if log_scale is not None else []
-    pf_set_list = _get_pf_set_list(costs)
+    pf_set_list = _get_pf_set_list(_costs)
     pf_sols = np.vstack(pf_set_list)
     X = np.unique(np.hstack([LOGEPS if 0 in log_scale else -np.inf, pf_sols[:, 0], np.inf]))
 
     emp_att_surfs = _compute_emp_att_surf(X=X, pf_set_list=pf_set_list, levels=np.asarray(levels))
     if larger_is_better_objectives is not None:
         emp_att_surfs = _change_directions(emp_att_surfs, larger_is_better_objectives=larger_is_better_objectives)
     if larger_is_better_objectives is not None and 0 in larger_is_better_objectives:
```

## eaf/plot_surface.py

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from eaf.utils import (
     LOGEPS,
     _change_scale,
     _check_surface,
     _compute_hypervolume2d,
@@ -130,22 +131,23 @@
                 The label of the plot.
             kwargs:
                 The kwargs for scatter.
         """
         if len(surf.shape) != 2 or surf.shape[1] != 2:
             raise ValueError(f"The shape of surf must be (n_points, 2), but got {surf.shape}")
 
+        _surf = surf.copy()
         if transform:
-            surf = self._transform_surface_list(surfs_list=[surf])[0]
+            _surf = self._transform_surface_list(surfs_list=[_surf])[0]
             ax.set_xlim(self.x_min, self.x_max)
             ax.set_ylim(self.y_min, self.y_max)
 
         kwargs.update(drawstyle=f"steps-{self.step_dir}")
-        _check_surface(surf)
-        X, Y = surf[:, 0], surf[:, 1]
+        _check_surface(_surf)
+        X, Y = _surf[:, 0], _surf[:, 1]
         line = ax.plot(X, Y, color=color, label=label, linestyle=linestyle, marker=marker, **kwargs)[0]
         _change_scale(ax, self.log_scale)
         return line
 
     def plot_true_pareto_surface(
         self,
         ax: plt.Axes,
@@ -214,20 +216,21 @@
                 The colors of each plot
             labels (List[str]):
                 The labels of each plot.
             kwargs:
                 The kwargs for scatter.
         """
         lines: List[Any] = []
-        surfs = self._transform_surface_list(surfs)
+        _surfs = deepcopy(surfs)
+        _surfs = self._transform_surface_list(_surfs)
 
-        n_surfs = len(surfs)
+        n_surfs = len(_surfs)
         linestyles = linestyles if linestyles is not None else [None] * n_surfs
         markers = markers if markers is not None else [None] * n_surfs
-        for surf, color, label, linestyle, marker in zip(surfs, colors, labels, linestyles, markers):
+        for surf, color, label, linestyle, marker in zip(_surfs, colors, labels, linestyles, markers):
             kwargs.update(color=color, label=label, linestyle=linestyle, marker=marker)
             line = self.plot_surface(ax, surf, transform=False, **kwargs)
             lines.append(line)
 
         ax.set_xlim(self.x_min, self.x_max)
         ax.set_ylim(self.y_min, self.y_max)
         return lines
@@ -260,33 +263,35 @@
             label (str):
                 The label of the plot.
             kwargs:
                 The kwargs for scatter.
         """
         if surfs.shape[0] != 3:
             raise ValueError(f"plot_surface_with_band requires three levels, but got only {surfs.shape[0]} levels")
+
+        _surfs = deepcopy(surfs)
         if transform:
-            surfs = self._transform_surface_list(surfs_list=surfs)
+            _surfs = self._transform_surface_list(surfs_list=_surfs)
             ax.set_xlim(self.x_min, self.x_max)
             ax.set_ylim(self.y_min, self.y_max)
 
-        for surf in surfs:
+        for surf in _surfs:
             _check_surface(surf)
 
-        X = surfs[0, :, 0]
+        X = _surfs[0, :, 0]
 
         marker_kwargs, kwargs = _extract_marker_kwargs(**kwargs)
         kwargs.update(color=color)
         alpha = kwargs.pop("alpha", None)
-        ax.fill_between(X, surfs[0, :, 1], surfs[2, :, 1], alpha=0.2, step=self.step_dir, **kwargs)
+        ax.fill_between(X, _surfs[0, :, 1], _surfs[2, :, 1], alpha=0.2, step=self.step_dir, **kwargs)
         kwargs["alpha"] = alpha
 
         # marker and linestyle are only for plot
         kwargs.update(label=label, linestyle=linestyle, marker=marker, **marker_kwargs)
-        line = ax.plot(X, surfs[1, :, 1], drawstyle=f"steps-{self.step_dir}", **kwargs)[0]
+        line = ax.plot(X, _surfs[1, :, 1], drawstyle=f"steps-{self.step_dir}", **kwargs)[0]
         _change_scale(ax, self.log_scale)
         return line
 
     def plot_multiple_surface_with_band(
         self,
         ax: plt.Axes,
         surfs_list: Union[np.ndarray, List[np.ndarray]],
@@ -310,20 +315,21 @@
                 The colors of each plot
             labels (List[str]):
                 The labels of each plot.
             kwargs:
                 The kwargs for scatter.
         """
         lines: List[Any] = []
-        surfs_list = self._transform_surface_list(surfs_list)
+        _surfs_list = deepcopy(surfs_list)
+        _surfs_list = self._transform_surface_list(_surfs_list)
 
-        n_surfs = len(surfs_list)
+        n_surfs = len(_surfs_list)
         linestyles = linestyles if linestyles is not None else [None] * n_surfs
         markers = markers if markers is not None else [None] * n_surfs
-        for surf, color, label, linestyle, marker in zip(surfs_list, colors, labels, linestyles, markers):
+        for surf, color, label, linestyle, marker in zip(_surfs_list, colors, labels, linestyles, markers):
             kwargs.update(color=color, label=label, linestyle=linestyle, marker=marker)
             line = self.plot_surface_with_band(ax, surf, transform=False, **kwargs)
             lines.append(line)
 
         ax.set_xlim(self.x_min, self.x_max)
         ax.set_ylim(self.y_min, self.y_max)
         return lines
```

## Comparing `empirical_attainment_func-0.3.7.dist-info/LICENSE` & `empirical_attainment_func-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*


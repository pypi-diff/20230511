# Comparing `tmp/analysis_engine-2.0.8.tar.gz` & `tmp/analysis_engine-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/analysis_engine/analysis_engine/dist/tmp76efdwfd/analysis_engine-2.0.8.tar", last modified: Thu Oct 20 10:39:03 2022, max compression
+gzip compressed data, was "/home/runner/work/analysis_engine/analysis_engine/dist/tmpyssouc5i/analysis_engine-2.0.9.tar", last modified: Tue Oct 25 14:13:18 2022, max compression
```

## Comparing `analysis_engine-2.0.8.tar` & `analysis_engine-2.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4828 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4344 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine/
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3966 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/ar_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     6226 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/benefits.py
--rw-r--r--   0 runner    (1001) docker     (116)    39226 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/cdg_data.py
--rw-r--r--   0 runner    (1001) docker     (116)       89 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (116)     1720 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/colouring.py
--rw-r--r--   0 runner    (1001) docker     (116)    14550 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/core_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    21379 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/costs.py
--rw-r--r--   0 runner    (1001) docker     (116)    35856 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/dandelion.py
--rw-r--r--   0 runner    (1001) docker     (116)    27306 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (116)   304509 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/data.py
--rw-r--r--   0 runner    (1001) docker     (116)     9425 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/data_review.py
--rw-r--r--   0 runner    (1001) docker     (116)    13007 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/dca.py
--rw-r--r--   0 runner    (1001) docker     (116)     7725 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (116)     4334 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/error_msgs.py
--rw-r--r--   0 runner    (1001) docker     (116)    16614 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/gmpp_int.py
--rw-r--r--   0 runner    (1001) docker     (116)    39280 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     2627 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/merge.py
--rw-r--r--   0 runner    (1001) docker     (116)    36788 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/milestones.py
--rw-r--r--   0 runner    (1001) docker     (116)     3820 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/query.py
--rw-r--r--   0 runner    (1001) docker     (116)     7420 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/render_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3210 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/resourcing.py
--rw-r--r--   0 runner    (1001) docker     (116)    23031 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/risks.py
--rw-r--r--   0 runner    (1001) docker     (116)     7096 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (116)     6429 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     7003 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/speed_dials.py
--rw-r--r--   0 runner    (1001) docker     (116)    21332 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/summaries.py
--rw-r--r--   0 runner    (1001) docker     (116)    48047 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/analysis_engine/top35_data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4828 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1052 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       55 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       71 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/analysis_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-20 10:39:03.000000 analysis_engine-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1015 2022-10-20 10:38:52.000000 analysis_engine-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1067 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     4828 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4344 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine/
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3966 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/ar_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6226 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/benefits.py
+-rw-r--r--   0 runner    (1001) docker     (116)    39226 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/cdg_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)       89 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1720 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/colouring.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14550 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/core_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21557 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/costs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35772 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/dandelion.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27306 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (116)   304509 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9425 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/data_review.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13007 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/dca.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8100 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4334 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/error_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16614 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/gmpp_int.py
+-rw-r--r--   0 runner    (1001) docker     (116)    40525 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2627 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/merge.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36788 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/milestones.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3820 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/query.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7420 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/render_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3210 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/resourcing.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25921 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/risks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7096 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6429 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6959 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/speed_dials.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21331 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (116)    48047 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/analysis_engine/top35_data.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4828 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1052 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       55 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       71 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/analysis_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-25 14:13:18.000000 analysis_engine-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1015 2022-10-25 14:13:08.000000 analysis_engine-2.0.9/setup.py
```

### Comparing `analysis_engine-2.0.8/LICENSE` & `analysis_engine-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/PKG-INFO` & `analysis_engine-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis_engine
-Version: 2.0.8
+Version: 2.0.9
 Summary: Analysis for the UK Department for Transport's major projects portfolio
 Home-page: https://github.com/banillie/analysis_engine
 Author: Will Grant
 Author-email: will.granty@yahoo.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `analysis_engine-2.0.8/README.md` & `analysis_engine-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/ar_data.py` & `analysis_engine-2.0.9/analysis_engine/ar_data.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/benefits.py` & `analysis_engine-2.0.9/analysis_engine/benefits.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/cdg_data.py` & `analysis_engine-2.0.9/analysis_engine/cdg_data.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/colouring.py` & `analysis_engine-2.0.9/analysis_engine/colouring.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/core_data.py` & `analysis_engine-2.0.9/analysis_engine/core_data.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/costs.py` & `analysis_engine-2.0.9/analysis_engine/costs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 import numpy as np
 
 from analysis_engine.segmentation import (
     get_group,
     get_correct_p_data,
 )
 from analysis_engine.cleaning import convert_none_types
-from analysis_engine.dictionaries import STANDARDISE_COST_KEYS, YEAR_LIST, RDEL_FORECAST_COST_KEYS, \
-    CDEL_FORECAST_COST_KEYS, RDEL_BL_COST_KEYS, CDEL_BL_COST_KEYS
+from analysis_engine.dictionaries import (
+    STANDARDISE_COST_KEYS,
+    YEAR_LIST,
+    RDEL_FORECAST_COST_KEYS,
+    CDEL_FORECAST_COST_KEYS,
+    RDEL_BL_COST_KEYS,
+    CDEL_BL_COST_KEYS,
+)
 from analysis_engine.error_msgs import ProjectNameError, logger
 from analysis_engine.settings import get_remove_income
 from analysis_engine.render_utils import make_file_friendly
 from analysis_engine.render_utils import set_fig_size, get_chart_title
 
 
 class CostData:
@@ -183,41 +189,45 @@
                         except KeyError:
                             p_data = None
 
                     if p_data is None:
                         continue
 
                     for cat in COST_CAT:
-                        if cat == ' RDEL ':
+                        if cat == " RDEL ":
                             for k in RDEL_FORECAST_COST_KEYS.keys():
                                 # if y in ["16-17", "17-18", "18-19"]:
                                 #     try:
                                 #         rdel = convert_none_types(self.master.project_information[p][y + cat + k])
                                 #     except KeyError:
                                 #         rdel = 0
                                 #         print(y + cat + k + " not found.")
                                 # else:
                                 f_local_rdel = convert_none_types(p_data[y + cat + k])
                                 f_year_rdel += f_local_rdel
                             for k in RDEL_BL_COST_KEYS.keys():
                                 b_local_rdel = convert_none_types(p_data[y + cat + k])
                                 b_year_rdel += b_local_rdel
-                        if cat == ' CDEL ':
+                        if cat == " CDEL ":
                             for k in CDEL_FORECAST_COST_KEYS.keys():
                                 try:
-                                    f_local_cdel = convert_none_types(p_data[y + cat + k])
+                                    f_local_cdel = convert_none_types(
+                                        p_data[y + cat + k]
+                                    )
                                 except KeyError:
                                     # try:
                                     f_local_cdel = convert_none_types(p_data[y + k])
                                     # except KeyError:
                                     #     local_cdel = 0
                                 f_year_cdel += f_local_cdel
                             for k in CDEL_BL_COST_KEYS.keys():
                                 try:
-                                    b_local_cdel = convert_none_types(p_data[y + cat + k])
+                                    b_local_cdel = convert_none_types(
+                                        p_data[y + cat + k]
+                                    )
                                 except KeyError:
                                     # try:
                                     b_local_cdel = convert_none_types(p_data[y + k])
                                     # except KeyError:
                                     #     # user messaging if necessary
                                     #     # print(tp + " " + y + k + ' could not be found. Check')
                                     #     cdel = 0
@@ -239,15 +249,14 @@
                 "CDEL Forecast": f_cdel_list,
                 "RDEL Baseline": b_rdel_list,
                 "CDEL Baseline": b_cdel_list,
             }
 
         self.profiles = profile_dict
 
-
     # def get_baseline_cost_profile(self) -> None:
     #     COST_CAT = [" RDEL ", " CDEL "]
     #     # self.iter_list = get_iter_list(self.kwargs, self.master)
     #     self.iter_list = [self.master.current_quarter]
     #     tp_dict = {}
     #     for tp in self.iter_list:
     #         self.group = get_group(self.master, tp, self.kwargs)
```

### Comparing `analysis_engine-2.0.8/analysis_engine/dandelion.py` & `analysis_engine-2.0.9/analysis_engine/dandelion.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,18 +137,18 @@
         if kwargs["type"] == "near_spend":
             cost.get_forecast_cost_profile()
             return sum(cost.profiles[tp]["Total Forecast"][0:2])  # reliant on YEAR_LIST
         if kwargs["type"] == "benefits":
             benefits = BenefitsData(master, **kwargs)
             return benefits.b_totals[tp]["total"]
         if kwargs["type"] in (
-                "ps_resource",
-                "contractor_resource",
-                "total_resource",
-                "funded_resource",
+            "ps_resource",
+            "contractor_resource",
+            "total_resource",
+            "funded_resource",
         ):
             resource = ResourceData(master, **kwargs)
             return resource.totals[tp][kwargs["type"]]
     else:
         return cost.totals[tp]["total"]
 
 
@@ -202,18 +202,18 @@
             pf_colour = COLOUR_DICT["WHITE"]
             pf_colour_edge = COLOUR_DICT["GREY"]
         no_projects = len(get_group(self.master, self.quarter, **self.kwargs))
 
         pf_text = f"Total Portfolio,\n{no_projects} Projects,\n{dandelion_number_text(pf_wlc, **self.kwargs)}.\n(forecast costs.)"
         if "type" in self.kwargs:
             if self.kwargs["type"] in (
-                    "ps_resource",
-                    "contractor_resource",
-                    "total_resource",
-                    "funded_resource",
+                "ps_resource",
+                "contractor_resource",
+                "total_resource",
+                "funded_resource",
             ):
                 pf_text = f"Total Portfolio,\n{no_projects} Projects,\n{dandelion_number_text(pf_wlc, **self.kwargs)} FTEs."
 
         if pf_colour != COLOUR_DICT["WHITE"]:
             text_colour = "white"
         else:
             text_colour = "black"
@@ -249,15 +249,15 @@
                 try:
                     g_abb = BC_STAGE_DICT_FULL_TO_ABB[g]
                 except KeyError:
                     if g in BC_STAGE_DICT_ABB_TO_FULL.keys():
                         g_abb = g
 
             g_text = (
-                    g_abb + "\n" + dandelion_number_text(g_wlc, **self.kwargs)
+                g_abb + "\n" + dandelion_number_text(g_wlc, **self.kwargs)
             )  # group text
 
             if g_wlc < pf_wlc / 10:  # adjusts any very small figures
                 g_wlc_adjusted = pf_wlc / 10
             else:
                 g_wlc_adjusted = g_wlc
 
@@ -295,16 +295,16 @@
         g_radius_dist = g_d["portfolio"]["r"] * 2
         if len(self.group) > 3:
             g_radius_dist = g_d["portfolio"]["r"] * 2.5
 
         for i, g in enumerate(self.group):
             if len(self.group) > 1:  # this needs testing
                 y_axis = 0 + (
-                        (math.sqrt(pf_wlc) + g_radius_dist)
-                        * math.sin(math.radians(g_ang_l[i]))
+                    (math.sqrt(pf_wlc) + g_radius_dist)
+                    * math.sin(math.radians(g_ang_l[i]))
                 )
                 x_axis = 0 + (math.sqrt(pf_wlc) + g_radius_dist) * math.cos(
                     math.radians(g_ang_l[i])
                 )
 
                 g_d[g]["axis"] = (y_axis, x_axis)
                 g_d[g]["tp"] = (y_axis, x_axis)
@@ -353,15 +353,15 @@
                     p_data = get_correct_p_data(self.master, p, self.quarter)
 
                 if "same_size" in self.kwargs:
                     if self.kwargs["same_size"] == "Yes":
                         p_value = 6000
 
                 if (
-                        p_value < pf_wlc * 0.02
+                    p_value < pf_wlc * 0.02
                 ):  # achieve some consistency for zero / low values
                     p_value_adjusted = pf_wlc * 0.008
                 else:
                     p_value_adjusted = p_value
 
                 p_radius = math.sqrt(p_value_adjusted)
 
@@ -409,17 +409,17 @@
                     if self.kwargs["type"] in [
                         "ps resource",
                         "contract resource",
                         "total resource",
                         "funded resource",
                     ]:
                         project_text = (
-                                self.master.abbreviations[p]["abb"]
-                                + ", "
-                                + dandelion_number_text(p_value, **self.kwargs)
+                            self.master.abbreviations[p]["abb"]
+                            + ", "
+                            + dandelion_number_text(p_value, **self.kwargs)
                         )
                 if "values" in self.kwargs:
                     if self.kwargs["values"] == "No":
                         project_text = self.master.abbreviations[p]["abb"]
 
                 try:  # this is for pipeline projects
                     if "confidence" in self.kwargs:  # change confidence type here
@@ -507,15 +507,15 @@
                     ang_l = [
                         g_d[g]["angle"],
                         g_d[g]["angle"] + 70,
                         g_d[g]["angle"] + 140,
                     ]
 
             largest_p_radius = (
-                    max(p_radius_list) * 1.5
+                max(p_radius_list) * 1.5
             )  # value used for distance from inner circle.
             for i, p in enumerate(p_list):
                 angle = ang_l[i]
                 p_y_axis = g_y_axis + (g_radius + largest_p_radius) * math.sin(
                     math.radians(ang_l[i])
                 )
                 p_x_axis = g_x_axis + (g_radius + largest_p_radius) * math.cos(
@@ -586,15 +586,15 @@
             for fund in self.e_dict[g]:
                 for p in self.e_dict[g][fund]:
                     g_wlc += self.e_dict[p]["wlc"]
 
             g_abb = g
 
             g_text = (
-                    g_abb + "\n" + dandelion_number_text(g_wlc, **self.kwargs)
+                g_abb + "\n" + dandelion_number_text(g_wlc, **self.kwargs)
             )  # group text
 
             if g_wlc < pf_wlc / 10:  # adjusts any very small figures
                 g_wlc_adjusted = pf_wlc / 10
             else:
                 g_wlc_adjusted = g_wlc
 
@@ -622,16 +622,16 @@
                 )
 
         g_radius_dist = g_d["portfolio"]["r"] * 3
 
         for i, g in enumerate(self.e_groups):
             if len(self.e_groups) > 1:  # this needs testing
                 y_axis = 0 + (
-                        (math.sqrt(pf_wlc) + g_radius_dist)
-                        * math.sin(math.radians(g_ang_l[i]))
+                    (math.sqrt(pf_wlc) + g_radius_dist)
+                    * math.sin(math.radians(g_ang_l[i]))
                 )
                 x_axis = 0 + (math.sqrt(pf_wlc) + g_radius_dist) * math.cos(
                     math.radians(g_ang_l[i])
                 )
 
                 g_d[g]["axis"] = (y_axis, x_axis)
                 g_d[g]["tp"] = (y_axis, x_axis)
@@ -661,15 +661,15 @@
                 fund_value = 0
                 p_number = 0
                 for p in self.e_dict[g][fund]:
                     fund_value += self.e_dict[p]["wlc"]
                     p_number += 1
 
                 if (
-                        fund_value < pf_wlc * 0.02
+                    fund_value < pf_wlc * 0.02
                 ):  # achieve some consistency for zero / low values
                     fund_value_adjusted = pf_wlc * 0.008
                 else:
                     fund_value_adjusted = fund_value
 
                 p_radius = math.sqrt(fund_value_adjusted)
 
@@ -740,15 +740,15 @@
             else:
                 if len(fund_list) == 1:
                     ang_l = [g_d[g]["angle"]]
                 if len(fund_list) == 2:
                     ang_l = [g_d[g]["angle"], g_d[g]["angle"] + 70]
 
             largest_p_radius = (
-                    max(p_radius_list) * 1.5
+                max(p_radius_list) * 1.5
             )  # value used for distance from inner circle.
             for i, p in enumerate(fund_list):
                 angle = ang_l[i]
                 p_y_axis = g_y_axis + (g_radius + largest_p_radius) * math.sin(
                     math.radians(ang_l[i])
                 )
                 p_x_axis = g_x_axis + (g_radius + largest_p_radius) * math.cos(
```

### Comparing `analysis_engine-2.0.8/analysis_engine/dashboards.py` & `analysis_engine-2.0.9/analysis_engine/dashboards.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/data.py` & `analysis_engine-2.0.9/analysis_engine/data.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/data_review.py` & `analysis_engine-2.0.9/analysis_engine/data_review.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/dca.py` & `analysis_engine-2.0.9/analysis_engine/dca.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/dictionaries.py` & `analysis_engine-2.0.9/analysis_engine/dictionaries.py`

 * *Files 7% similar despite different names*

```diff
@@ -219,14 +219,29 @@
     "Portfolio Risk Impact Description",
     "Portfolio Risk Mitigation",
     "Portfolio Risk Likelihood",
     "Portfolio Risk Impact Assessment",
     "Severity Score Risk Category",
 ]
 
+PORTFOLIO_RISKS_WORD = [
+    "Portfolio Risk Likelihood",
+    "Portfolio Risk Impact Assessment",
+    "Portfolio Risk Impact Description",
+    "Portfolio Risk Mitigation",
+]
+
+RISK_NO_DICTIONARY = {
+    1: "Infrastructure Decarbonisation",
+    2: "Planning Policy",
+    3: "Supply Chain and Materials",
+    4: "Value for Money",
+    5: "Coordinated Stakeholder Management",
+}
+
 RISK_SCORES = {
     "Very Low": 0,
     "Low": 1,
     "Medium": 2,
     "High": 3,
     "Very High": 4,
     "N/A": None,
@@ -297,8 +312,7 @@
     "Benefits Narrative": "Benefits Narrative",
     "Benefits comparison with last quarter": "Ben comparison with last quarters cost - narrative",
     "Benefits comparison with baseline": "Ben comparison within this quarters cost - narrative",
     "Milestone narrative": "Milestone Commentary",
     "Resource commentary": "Resources commentary",
     "Project Scope": "Project Scope",
 }
-
```

### Comparing `analysis_engine-2.0.8/analysis_engine/error_msgs.py` & `analysis_engine-2.0.9/analysis_engine/error_msgs.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/gmpp_int.py` & `analysis_engine-2.0.9/analysis_engine/gmpp_int.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/main.py` & `analysis_engine-2.0.9/analysis_engine/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,21 @@
     cdg_dashboard,
     ipdc_dashboard,
 )
 from analysis_engine.gmpp_int import GmppOnlineCosts
 from analysis_engine.merge import Merge
 from analysis_engine.query import data_query_into_wb
 from analysis_engine.render_utils import get_input_doc, put_matplotlib_fig_into_word
-from analysis_engine.risks import RiskData, portfolio_risks_into_excel, risks_into_excel
+from analysis_engine.risks import (
+    RiskData,
+    portfolio_risks_into_excel,
+    risks_into_excel,
+    portfolio_risks_into_word_by_project,
+    portfolio_risks_into_word_by_risk,
+)
 from analysis_engine.settings import (
     report_config,
     set_default_args,
     return_koi_fn_keys,
     get_integration_data,
     get_masters_to_merge,
 )
@@ -35,15 +41,19 @@
 
 from analysis_engine.error_msgs import (
     logger,
     ProjectNameError,
     InputError,
 )
 
-from analysis_engine.costs import CostData, cost_profile_graph_new, cost_profile_into_wb_new
+from analysis_engine.costs import (
+    CostData,
+    cost_profile_graph_new,
+    cost_profile_into_wb_new,
+)
 from analysis_engine.summaries import run_p_reports
 
 
 class CliOpArgs:
     def __init__(self, args, settings):
         self.args = args
         self.settings = settings
@@ -55,15 +65,15 @@
 
     def cli_op_args(self):
         self.programme = self.args["subparser_name"]
         op_args = {k: v for k, v in self.args.items() if v is not None}
 
         # these programs have the latest two quarters as default.
         # other program defaults are setting very get_iter_list()
-        if self.programme in ["dcas", "speed_dials"]:
+        if self.programme in ["dcas", "speed_dials", "risks_printout"]:
             if "quarter" not in list(op_args.keys()):
                 op_args["quarter"] = "standard"
 
         if self.programme == "milestones":
             if "chart" not in (op_args.keys()):
                 op_args["chart"] = None
 
@@ -137,15 +147,16 @@
         if cli.programme == "costs":
             c = CostData(cli.md, **cli.combined_args)
             c.get_forecast_cost_profile()
             wb = cost_profile_into_wb_new(c)
             if cli.combined_args["chart"] == "save":
                 ms_graph = cost_profile_graph_new(c, **cli.combined_args)
                 doc = get_input_doc(
-                    str(cli.combined_args["root_path"]) + cli.combined_args["word_landscape"]
+                    str(cli.combined_args["root_path"])
+                    + cli.combined_args["word_landscape"]
                 )
                 put_matplotlib_fig_into_word(doc, ms_graph, width=Inches(8))
                 doc.save(
                     str(cli.combined_args["root_path"])
                     + cli.combined_args["word_save_path"].format("cost_chart")
                 )
             if cli.combined_args["chart"] == "show":
@@ -294,28 +305,41 @@
             md = GmppOnlineCosts(**cli.combined_args)
             md.place_into_dft_master_format()
 
         if cli.programme == "merge_masters":
             get_masters_to_merge(cli.combined_args)
             Merge(**cli.combined_args)
 
-        if cli.programme == "portfolio_risks":
+        if cli.programme == "risks_portfolio":
             rd = RiskData(cli.md, **cli.combined_args)
             wb = portfolio_risks_into_excel(rd)
             wb.save(
                 str(cli.settings["root_path"])
-                + cli.settings["excel_save_path"].format("portfolio_risks")
+                + cli.settings["excel_save_path"].format("risks_portfolio")
+            )
+
+        if cli.programme == "risks_printout":
+            rd = RiskData(cli.md, **cli.combined_args)
+            by_proj_doc = portfolio_risks_into_word_by_project(rd)
+            by_proj_doc.save(
+                str(cli.settings["root_path"])
+                + cli.settings["word_save_path"].format("risks_printout_by_project")
+            )
+            by_risk_doc = portfolio_risks_into_word_by_risk(rd)
+            by_risk_doc.save(
+                str(cli.settings["root_path"])
+                + cli.settings["word_save_path"].format("risks_printout_by_risk")
             )
 
-        if cli.programme == "project_risks":
+        if cli.programme == "risks_projects":
             rd = RiskData(cli.md, **cli.combined_args)
             wb = risks_into_excel(rd)
             wb.save(
                 str(cli.settings["root_path"])
-                + cli.settings["excel_save_path"].format("project_risks")
+                + cli.settings["excel_save_path"].format("risks_projects")
             )
 
         # ProjectNameError below captures any naming errors both this is hit.
         if "remove" in cli.combined_args.keys():
             for x in cli.combined_args["remove"]:
                 logger.info(f"{x} has been removed from analysis")
 
@@ -333,15 +357,14 @@
     subparsers = parser.add_subparsers(dest="subparser_name")
     subparsers.metavar = "                      "
 
     costs_description = (
         "Provides cost profile data and graphs. It provides the current quarters profile if not optional "
         "arguments are specified. All optional al arguments are as below including --baseline. "
         "This argument returns the baseline cost profile for any given quarter. "
-
     )
     parser_costs = subparsers.add_parser(
         "costs",
         help="cost trend profile graph and data.",
         description=costs_description,
     )
 
@@ -407,42 +430,48 @@
         "milestones",
         help="Compiles milestone schedule graphs and data.",
         description="Generates raw data outputs as well as visuals for milestone data. The default is simply "
         "the return of an excel file with milestone data. Use the --chart options to produce"
         "visual outputs ",
     )
 
+    parser_data_query = subparsers.add_parser(
+        "query", help="Returns data from master data set as specified by the user."
+    )
+
     parser_port_risks = subparsers.add_parser(
-        "portfolio_risks",
-        help="Compiles portfolio risk analysis.",
+        "risks_portfolio",
+        help="Compiles portfolio risk analysis into an excel document.",
         description="This program extracts all portfolio risk data used in the IPDC portfolio report.",
     )
     parser_risks = subparsers.add_parser(
-        "project_risks",
-        help="Compiles project risk analysis",
+        "risks_projects",
+        help="Compiles project risk analysis into an excel document.",
         description="This program extracts all project level risk data contained in the master data set.",
     )
-
-    parser_data_query = subparsers.add_parser(
-        "query", help="Returns data from master data set as specified by the user."
+    parser_risks_po = subparsers.add_parser(
+        "risks_printout",
+        help="Compiles into word documents a print out of all text related portfolio risk data.",
+        description="Compiles into word documents a print out of all text related portfolio risk data. Two word "
+        "documents are created. One with data ordered by project and one ordered by risk.",
     )
 
     parser_speed_dial = subparsers.add_parser(
         "speed_dials",
         help="Produces the speed dial analysis and visuals used in the portfolio management report.",
         description="Creates the speed dial visual outputs. All confidence speed dials are created "
         "at the same time and saved into the output folder. It has a maximum of two quarters "
         "for the --quarters argument.",
     )
 
     parser_summaries = subparsers.add_parser(
         "summaries",
         help="Produce summary reports for projects in a word document.",
         description="Produce summary reports for projects in a word document. You have use the --group argument "
-                    "to specify which projects you would like to produce summaries for."
+        "to specify which projects you would like to produce summaries for.",
     )
 
     parser_dandelion.add_argument(
         "--angles",
         type=int,
         metavar="",
         action="store",
@@ -455,15 +484,15 @@
         "--baseline",
         type=str,
         metavar="",
         action="store",
         nargs="*",
         # choices=[],
         help="Returns the baseline cost profile. --baseline is the default "
-             "and no other commands are necessary. "
+        "and no other commands are necessary. ",
     )
 
     parser_milestones.add_argument(
         "--blue_line",
         type=str,
         metavar="",
         action="store",
@@ -512,14 +541,15 @@
     # )
 
     # group
     for sub in [
         parser_dca,
         parser_risks,
         parser_port_risks,
+        parser_risks_po,
         parser_speed_dial,
         parser_dandelion,
         parser_milestones,
         parser_data_query,
         parser_costs,
         parser_summaries,
     ]:
@@ -568,26 +598,27 @@
     parser_dandelion.add_argument(
         "--pc",
         type=str,
         metavar="",
         action="store",
         choices=["G", "A/G", "A", "A/R", "R"],
         help="User can specify the colour of the central portfolio bubble, if desired. The options are "
-             "'G' 'A/G' 'A' 'A/R' 'R'.",
+        "'G' 'A/G' 'A' 'A/R' 'R'.",
     )
 
     # quarter
     for sub in [
         parser_speed_dial,
         parser_dandelion,
         parser_dca,
         parser_milestones,
         parser_data_query,
         parser_port_risks,
         parser_risks,
+        parser_risks_po,
         parser_costs,
     ]:
         sub.add_argument(
             "--quarter",
             type=str,
             metavar="",
             action="store",
@@ -597,14 +628,15 @@
         )
 
     # remove
     for sub in [
         parser_dca,
         parser_risks,
         parser_port_risks,
+        parser_risks_po,
         parser_speed_dial,
         parser_dandelion,
         parser_data_query,
         parser_milestones,
         parser_costs,
     ]:
         sub.add_argument(
@@ -619,14 +651,15 @@
 
     # stage
     for sub in [
         parser_dca,
         parser_speed_dial,
         parser_risks,
         parser_port_risks,
+        parser_risks_po,
         parser_dandelion,
         parser_data_query,
         parser_milestones,
         parser_costs,
     ]:
         sub.add_argument(
             "--stage",
```

### Comparing `analysis_engine-2.0.8/analysis_engine/merge.py` & `analysis_engine-2.0.9/analysis_engine/merge.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/milestones.py` & `analysis_engine-2.0.9/analysis_engine/milestones.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/query.py` & `analysis_engine-2.0.9/analysis_engine/query.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/render_utils.py` & `analysis_engine-2.0.9/analysis_engine/render_utils.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/resourcing.py` & `analysis_engine-2.0.9/analysis_engine/resourcing.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/risks.py` & `analysis_engine-2.0.9/analysis_engine/risks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from collections import Counter
 
 from openpyxl import workbook, Workbook
+from docx import Document
 
 from analysis_engine.dictionaries import (
     RISK_SCORES,
     PORTFOLIO_RISK_SCORES,
     RISK_LIST,
     PORTFOLIO_RISK_LIST,
+    PORTFOLIO_RISKS_WORD,
+    RISK_NO_DICTIONARY,
 )
 from analysis_engine.segmentation import get_group, get_correct_p_data
-from analysis_engine.render_utils import make_file_friendly
+from analysis_engine.render_utils import (
+    make_file_friendly,
+    get_input_doc,
+    compare_text_new_and_old,
+)
 from analysis_engine.error_msgs import logger
 
 
 def risk_score(risk_impact: str, risk_likelihood: str) -> str:
     impact_score = RISK_SCORES[risk_impact]
     try:
         likelihood_score = RISK_SCORES[risk_likelihood]
@@ -159,17 +166,15 @@
             portfolio_dict = {}
             group = get_group(self.master, tp, **self.kwargs)
             for p in group:
                 p_data = get_correct_p_data(self.master, p, tp)
                 if p_data is None:
                     continue
                 portfolio_number_dict = {}
-                for x in range(
-                    1, 7
-                ):  # currently 6 risks. Changed from 5 to 6 in Q4 2021
+                for x in range(1, 6):  # currently 5 risks.
                     portfolio_risk_list = []
                     group = (
                         "Group",
                         self.master["project_information"][p]["Group"],
                     )
                     stage = ("Stage", p_data["IPDC approval point"])
                     portfolio_risk_list.append(group)
@@ -518,7 +523,81 @@
             ws.cell(row=start_row + i + 1, column=8).value = sum(
                 risk_data.portfolio_type_impact_count[q][no].values()
             )
 
     wb.remove(wb["Sheet"])
 
     return wb
+
+
+def portfolio_risks_into_word_by_project(risk_data: RiskData) -> Document:
+    doc = get_input_doc(
+        risk_data.kwargs["root_path"] + risk_data.kwargs["word_portrait"]
+    )
+    latest_q = risk_data.quarters[0]
+    other_q = risk_data.quarters[1]
+    for p in risk_data.risk_dictionary[latest_q].keys():
+        heading = str(p)
+        intro = doc.add_heading(heading, 0)
+        intro.alignment = 1
+        intro.bold = True
+        for port_risk_no in range(1, 6):
+            doc.add_paragraph().add_run(RISK_NO_DICTIONARY[port_risk_no]).bold = True
+            for k in PORTFOLIO_RISKS_WORD:
+                try:
+                    doc.add_paragraph().add_run(k).italic = True
+                    text_one = str(
+                        risk_data.portfolio_risk_dictionary[latest_q][p][port_risk_no][
+                            k
+                        ]
+                    )
+                    try:
+                        text_two = str(
+                            risk_data.portfolio_risk_dictionary[other_q][p][
+                                port_risk_no
+                            ][k]
+                        )
+                    except (KeyError, IndexError):  # index error relates to data_bridge
+                        text_two = text_one
+                except KeyError:
+                    break
+
+                compare_text_new_and_old(text_one, text_two, doc)
+
+    return doc
+
+
+def portfolio_risks_into_word_by_risk(risk_data: RiskData) -> Document:
+    doc = get_input_doc(
+        risk_data.kwargs["root_path"] + risk_data.kwargs["word_portrait"]
+    )
+    latest_q = risk_data.quarters[0]
+    other_q = risk_data.quarters[1]
+    for port_risk_no in range(1, 6):
+        heading = str(RISK_NO_DICTIONARY[port_risk_no])
+        intro = doc.add_heading(heading, 0)
+        intro.alignment = 1
+        intro.bold = True
+        for p in risk_data.risk_dictionary[latest_q].keys():
+            doc.add_paragraph().add_run(p).bold = True
+            for k in PORTFOLIO_RISKS_WORD:
+                try:
+                    doc.add_paragraph().add_run(k).italic = True
+                    text_one = str(
+                        risk_data.portfolio_risk_dictionary[latest_q][p][port_risk_no][
+                            k
+                        ]
+                    )
+                    try:
+                        text_two = str(
+                            risk_data.portfolio_risk_dictionary[other_q][p][
+                                port_risk_no
+                            ][k]
+                        )
+                    except (KeyError, IndexError):  # index error relates to data_bridge
+                        text_two = text_one
+                except KeyError:
+                    break
+
+                compare_text_new_and_old(text_one, text_two, doc)
+
+    return doc
```

### Comparing `analysis_engine-2.0.8/analysis_engine/segmentation.py` & `analysis_engine-2.0.9/analysis_engine/segmentation.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine/settings.py` & `analysis_engine-2.0.9/analysis_engine/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         date_str = config["GLOBALS"]["date"]
         return parser.parse(date_str, dayfirst=True).date()
     except:
         config_issue()
 
 
 def get_remove_income(op_args):
-    if op_args['report'] == 'ipdc':
+    if op_args["report"] == "ipdc":
         try:
             config_path = op_args["root_path"] + op_args["config"]
             config = configparser.ConfigParser()
             config.read(config_path)
             return config["COSTS"]["remove_income"]
         except:
             config_issue()  # this could be improved to be more specific
```

### Comparing `analysis_engine-2.0.8/analysis_engine/speed_dials.py` & `analysis_engine-2.0.9/analysis_engine/speed_dials.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,31 +147,27 @@
     # if arrow_one != arrow_two:  # not sure what this did?
     plt.annotate(
         "",
         xy=(-0.2, 0.4),
         xycoords="data",
         xytext=(-0.4, 0.2),
         textcoords="data",
-        arrowprops=dict(
-            arrowstyle="->", connectionstyle="arc3, rad=-0.3", linewidth=4
-        ),
+        arrowprops=dict(arrowstyle="->", connectionstyle="arc3, rad=-0.3", linewidth=4),
     )
     ax.text(-0.35, 0.35, down, fontsize=30, fontname=FONT_TYPE)
 
     ax.text(0.35, 0.35, up, fontsize=30, fontname=FONT_TYPE)
 
     plt.annotate(
         "",
         xy=(0.4, 0.2),
         xycoords="data",
         xytext=(0.2, 0.4),
         textcoords="data",
-        arrowprops=dict(
-            arrowstyle="<-", connectionstyle="arc3, rad=-0.3", linewidth=4
-        ),
+        arrowprops=dict(arrowstyle="<-", connectionstyle="arc3, rad=-0.3", linewidth=4),
     )
 
     plt.axis("scaled")
     plt.axis("off")
 
     return fig
```

### Comparing `analysis_engine-2.0.8/analysis_engine/summaries.py` & `analysis_engine-2.0.9/analysis_engine/summaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
             milestones.milestone_dict,
             "Project - Start Date",
             str(master["current_quarter"]),
             abb,
         )
         hdr_cells[1].text = start_project.strftime("%d/%m/%Y")
     except (KeyError, AttributeError):
-        try:   # the team has two keys !!!!
+        try:  # the team has two keys !!!!
             start_project = get_milestone_date(
                 milestones.milestone_dict,
                 "Start of Project",
                 str(master["current_quarter"]),
                 abb,
             )
             hdr_cells[1].text = start_project.strftime("%d/%m/%Y")
```

### Comparing `analysis_engine-2.0.8/analysis_engine/top35_data.py` & `analysis_engine-2.0.9/analysis_engine/top35_data.py`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/analysis_engine.egg-info/PKG-INFO` & `analysis_engine-2.0.9/analysis_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-engine
-Version: 2.0.8
+Version: 2.0.9
 Summary: Analysis for the UK Department for Transport's major projects portfolio
 Home-page: https://github.com/banillie/analysis_engine
 Author: Will Grant
 Author-email: will.granty@yahoo.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `analysis_engine-2.0.8/analysis_engine.egg-info/SOURCES.txt` & `analysis_engine-2.0.9/analysis_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analysis_engine-2.0.8/setup.py` & `analysis_engine-2.0.9/setup.py`

 * *Files identical despite different names*


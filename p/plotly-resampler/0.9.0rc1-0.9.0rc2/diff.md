# Comparing `tmp/plotly_resampler-0.9.0rc1.tar.gz` & `tmp/plotly_resampler-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_resampler-0.9.0rc1.tar", max compression
+gzip compressed data, was "plotly_resampler-0.9.0rc2.tar", max compression
```

## Comparing `plotly_resampler-0.9.0rc1.tar` & `plotly_resampler-0.9.0rc2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1115 2023-05-03 12:32:58.928306 plotly_resampler-0.9.0rc1/LICENSE
--rw-r--r--   0        0        0     9540 2023-05-09 09:35:41.332034 plotly_resampler-0.9.0rc1/README.md
--rw-r--r--   0        0        0      853 2023-05-09 09:36:29.006385 plotly_resampler-0.9.0rc1/plotly_resampler/__init__.py
--rw-r--r--   0        0        0      796 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/__init__.py
--rw-r--r--   0        0        0     6934 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregation_interface.py
--rw-r--r--   0        0        0    11877 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregators.py
--rw-r--r--   0        0        0     3048 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handler_interface.py
--rw-r--r--   0        0        0     3179 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handlers.py
--rw-r--r--   0        0        0     7933 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/plotly_aggregator_parser.py
--rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/__init__.py
--rw-r--r--   0        0        0    23690 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler.py
--rw-r--r--   0        0        0    61202 2023-05-09 09:35:41.356033 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler_interface.py
--rw-r--r--   0        0        0    13669 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figurewidget_resampler.py
--rw-r--r--   0        0        0     5376 2023-05-07 09:13:04.096399 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/utils.py
--rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc1/plotly_resampler/registering.py
--rw-r--r--   0        0        0     2857 2023-05-09 09:36:04.819222 plotly_resampler-0.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0    11486 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-05-03 12:32:58.928306 plotly_resampler-0.9.0rc2/LICENSE
+-rw-r--r--   0        0        0     9540 2023-05-09 09:35:41.332034 plotly_resampler-0.9.0rc2/README.md
+-rw-r--r--   0        0        0      853 2023-05-11 09:37:41.902449 plotly_resampler-0.9.0rc2/plotly_resampler/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/__init__.py
+-rw-r--r--   0        0        0     6934 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregation_interface.py
+-rw-r--r--   0        0        0    11877 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregators.py
+-rw-r--r--   0        0        0     3048 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handler_interface.py
+-rw-r--r--   0        0        0     3179 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handlers.py
+-rw-r--r--   0        0        0     7933 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/plotly_aggregator_parser.py
+-rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/__init__.py
+-rw-r--r--   0        0        0    23690 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler.py
+-rw-r--r--   0        0        0    61317 2023-05-11 09:36:04.273826 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler_interface.py
+-rw-r--r--   0        0        0    13669 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figurewidget_resampler.py
+-rw-r--r--   0        0        0     5376 2023-05-07 09:13:04.096399 plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/utils.py
+-rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc2/plotly_resampler/registering.py
+-rw-r--r--   0        0        0     2857 2023-05-11 09:37:23.139098 plotly_resampler-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    11486 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc2/PKG-INFO
```

### Comparing `plotly_resampler-0.9.0rc1/LICENSE` & `plotly_resampler-0.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/README.md` & `plotly_resampler-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/__init__.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .aggregation import LTTB, EveryNthPoint, MinMaxLTTB
 from .figure_resampler import FigureResampler, FigureWidgetResampler
 from .registering import register_plotly_resampler, unregister_plotly_resampler
 
 __docformat__ = "numpy"
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
-__version__ = "0.9.0rc1"
+__version__ = "0.9.0rc2"
 
 __all__ = [
     "__version__",
     "FigureResampler",
     "FigureWidgetResampler",
     "MinMaxLTTB",
     "LTTB",
```

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/__init__.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregation_interface.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregation_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregators.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/aggregators.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handler_interface.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handler_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handlers.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/gap_handlers.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/plotly_aggregator_parser.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/aggregation/plotly_aggregator_parser.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler_interface.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figure_resampler_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,20 @@
         # The link above indicates that the trace index is derived from `data`
         if trace.name is None:
             trace.name = f"trace {len(self.data) + offset}"
 
         # Determine (1) the axis type and (2) the downsampler instance
         # & (3) store a hf_data entry for the corresponding trace,
         # identified by its UUID
-        axis_type = "date" if isinstance(dc.x, pd.DatetimeIndex) else "linear"
+        axis_type = (
+            "date"
+            if isinstance(dc.x, pd.DatetimeIndex)
+            or pd.core.dtypes.common.is_datetime64_any_dtype(dc.x)
+            else "linear"
+        )
 
         default_n_samples = False
         if max_n_samples is None:
             default_n_samples = True
             max_n_samples = self._global_n_shown_samples
 
         default_downsampler = False
```

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figurewidget_resampler.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/figurewidget_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/utils.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/figure_resampler/utils.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/plotly_resampler/registering.py` & `plotly_resampler-0.9.0rc2/plotly_resampler/registering.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc1/pyproject.toml` & `plotly_resampler-0.9.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plotly-resampler"  # Do not forget to update the __init__.py __version__ variable
-version = "0.9.0rc1"
+version = "0.9.0rc2"
 description = "Visualizing large time series with plotly"
 authors = ["Jonas Van Der Donckt", "Jeroen Van Der Donckt", "Emiel Deprost"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/predict-idlab/plotly-resampler"
 documentation = "https://predict-idlab.github.io/plotly-resampler"
 keywords = ["time-series", "visualization", "resampling", "plotly", "plotly-dash"]
```

### Comparing `plotly_resampler-0.9.0rc1/PKG-INFO` & `plotly_resampler-0.9.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotly-resampler
-Version: 0.9.0rc1
+Version: 0.9.0rc2
 Summary: Visualizing large time series with plotly
 Home-page: https://github.com/predict-idlab/plotly-resampler
 License: MIT
 Keywords: time-series,visualization,resampling,plotly,plotly-dash
 Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc1 Summary:
+Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc2 Summary:
 Visualizing large time series with plotly Home-page: https://github.com/
 predict-idlab/plotly-resampler License: MIT Keywords: time-
 series,visualization,resampling,plotly,plotly-dash Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
```


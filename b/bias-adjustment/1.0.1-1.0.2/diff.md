# Comparing `tmp/bias_adjustment-1.0.1.tar.gz` & `tmp/bias_adjustment-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bias_adjustment-1.0.1.tar", max compression
+gzip compressed data, was "bias_adjustment-1.0.2.tar", max compression
```

## Comparing `bias_adjustment-1.0.1.tar` & `bias_adjustment-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2022-12-22 04:55:07.013643 bias_adjustment-1.0.1/LICENSE
--rw-r--r--   0        0        0      274 2022-12-22 04:11:02.373255 bias_adjustment-1.0.1/README.md
--rw-r--r--   0        0        0      615 2022-12-22 05:00:27.493710 bias_adjustment-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      205 2022-12-22 04:11:02.374046 bias_adjustment-1.0.1/src/bias_adjustment/__init__.py
--rw-r--r--   0        0        0     1137 2022-12-22 04:11:02.374179 bias_adjustment-1.0.1/src/bias_adjustment/bias_adjustment.py
--rw-r--r--   0        0        0       97 2022-12-22 04:11:02.374333 bias_adjustment-1.0.1/src/bias_adjustment/distributions/__init__.py
--rw-r--r--   0        0        0     1788 2022-12-22 04:11:02.374450 bias_adjustment-1.0.1/src/bias_adjustment/distributions/distributions.py
--rw-r--r--   0        0        0      300 2022-12-22 04:11:02.374608 bias_adjustment-1.0.1/src/bias_adjustment/quantile_mapping/__init__.py
--rw-r--r--   0        0        0     1115 2022-12-22 04:11:02.374717 bias_adjustment-1.0.1/src/bias_adjustment/quantile_mapping/dqm.py
--rw-r--r--   0        0        0      854 2022-12-22 04:11:02.374824 bias_adjustment-1.0.1/src/bias_adjustment/quantile_mapping/qdm.py
--rw-r--r--   0        0        0      677 2022-12-22 04:11:02.374930 bias_adjustment-1.0.1/src/bias_adjustment/quantile_mapping/qm.py
--rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 bias_adjustment-1.0.1/setup.py
--rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 bias_adjustment-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-10 14:11:11.340594 bias_adjustment-1.0.2/LICENSE
+-rw-r--r--   0        0        0      274 2022-11-15 06:42:37.967412 bias_adjustment-1.0.2/README.md
+-rw-r--r--   0        0        0      705 2023-05-10 14:11:11.341594 bias_adjustment-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      205 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/__init__.py
+-rw-r--r--   0        0        0     2401 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/bias_adjustment.py
+-rw-r--r--   0        0        0       97 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/distributions/__init__.py
+-rw-r--r--   0        0        0     5089 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/distributions/distributions.py
+-rw-r--r--   0        0        0      300 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/__init__.py
+-rw-r--r--   0        0        0     1264 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/dqm.py
+-rw-r--r--   0        0        0     1018 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/qdm.py
+-rw-r--r--   0        0        0     1870 2023-05-10 14:11:11.361595 bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/qm.py
+-rw-r--r--   0        0        0      376 2023-05-10 14:11:11.362595 bias_adjustment-1.0.2/src/bias_adjustment/utils.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 bias_adjustment-1.0.2/PKG-INFO
```

### Comparing `bias_adjustment-1.0.1/LICENSE` & `bias_adjustment-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.1/src/bias_adjustment/quantile_mapping/dqm.py` & `bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/dqm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from dataclasses import dataclass
-from typing import Literal
+from typing import get_args
+
 import numpy as np
 
 from bias_adjustment.quantile_mapping.qm import QuantileMapping
+from bias_adjustment.utils import BAMode, FloatNDArray
 
 
 @dataclass
 class DetrendedQuantileMapping(QuantileMapping):
-    def delta(self, mode: Literal["rel", "abs"] = "rel"):
+    def delta(self, mode: BAMode = "rel"):
         mod_mean = np.nanmean(self.mod)
         dat_mean = np.nanmean(self.data)
         if mode == "rel":
             return dat_mean / mod_mean
         elif mode == "abs":
             return dat_mean - mod_mean
         return None
 
     def compute(
         self,
-        mode: Literal["rel", "abs"] = "rel",
+        mode: BAMode = "rel",
         dist_type="hist",
-    ) -> np.ndarray:
+    ) -> FloatNDArray:
+        if mode not in get_args(BAMode):
+            raise ValueError(f"Length of `mode` must be {get_args(BAMode)}.")
+
         o_dist = self.generate_distribution(self.obs, dist_type)
         m_dist = self.generate_distribution(self.mod, dist_type)
 
         delta = self.delta(mode)
         if mode == "rel":
             m_cdf = np.minimum(self.max_cdf, m_dist.cdf(self.data / delta))
             return o_dist.ppf(m_cdf) * delta
```

### Comparing `bias_adjustment-1.0.1/src/bias_adjustment/quantile_mapping/qm.py` & `bias_adjustment-1.0.2/src/bias_adjustment/quantile_mapping/qdm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from dataclasses import dataclass
+from typing import get_args
+
 import numpy as np
 
-from bias_adjustment.distributions import Distributions
+from bias_adjustment.quantile_mapping.qm import QuantileMapping
+from bias_adjustment.utils import BAMode, FloatNDArray
 
 
 @dataclass
-class QuantileMapping:
-    obs: np.ndarray
-    mod: np.ndarray
-    data: np.ndarray
-    max_cdf: float = 0.99999
-
-    @staticmethod
-    def generate_distribution(dat: np.ndarray, dist_type="hist"):
-        return Distributions(dat).fit(dist_type)
-
+class QuantileDeltaMapping(QuantileMapping):
     def compute(
         self,
+        mode: BAMode = "rel",
         dist_type="hist",
-    ) -> np.ndarray:
+    ) -> FloatNDArray:
+        if mode not in get_args(BAMode):
+            raise ValueError(f"Length of `mode` must be {get_args(BAMode)}.")
+
         o_dist = self.generate_distribution(self.obs, dist_type)
-        m_dist = self.generate_distribution(self.mod, dist_type)
+        mh_dist = self.generate_distribution(self.mod, dist_type)
+        mf_dist = self.generate_distribution(self.data, dist_type)
+
+        mf_cdf = np.minimum(self.max_cdf, mf_dist.cdf(self.data))
 
-        m_cdf = np.minimum(self.max_cdf, m_dist.cdf(self.data))
-        return o_dist.ppf(m_cdf)
+        if mode == "rel":  # Relative
+            return o_dist.ppf(mf_cdf) * (self.data / mh_dist.ppf(mf_cdf))
+        elif mode == "abs":  # Absolute
+            return o_dist.ppf(mf_cdf) + self.data - mh_dist.ppf(mf_cdf)
+        else:
+            return None
```

### Comparing `bias_adjustment-1.0.1/PKG-INFO` & `bias_adjustment-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: bias-adjustment
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bias Adjusment by Quantile Mapping
 Home-page: https://github.com/emiliogozo/bias_adjustment
 License: MIT
 Keywords: climatology,data analysis,quantile mapping,bias correction
 Author: Emilio Gozo
 Author-email: emiliogozo@proton.me
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: conda-lock (>=1.4.0,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Project-URL: Repository, https://github.com/emiliogozo/bias_adjustment
 Description-Content-Type: text/markdown
 
 # Bias Adjusment by Quantile Mapping
 
 Bias adjustment techniques:
```


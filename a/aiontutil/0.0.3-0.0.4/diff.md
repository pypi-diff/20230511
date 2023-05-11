# Comparing `tmp/aiontutil-0.0.3.tar.gz` & `tmp/aiontutil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiontutil-0.0.3.tar", max compression
+gzip compressed data, was "aiontutil-0.0.4.tar", max compression
```

## Comparing `aiontutil-0.0.3.tar` & `aiontutil-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.3/README.md
--rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.3/aiontutil/__init__.py
--rw-r--r--   0        0        0     3202 2023-05-08 08:12:48.272943 aiontutil-0.0.3/aiontutil/signal.py
--rw-r--r--   0        0        0      337 2023-05-08 08:20:32.190413 aiontutil-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 aiontutil-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.4/aiontutil/__init__.py
+-rw-r--r--   0        0        0     3600 2023-05-10 08:34:17.729001 aiontutil-0.0.4/aiontutil/signal.py
+-rw-r--r--   0        0        0      337 2023-05-10 08:43:07.826012 aiontutil-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 aiontutil-0.0.4/PKG-INFO
```

### Comparing `aiontutil-0.0.3/aiontutil/signal.py` & `aiontutil-0.0.4/aiontutil/signal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+from typing import List
+
 import numpy as np
 import scipy as sp
 from scipy import stats
 
 
+def list_all_feature_names() -> List[str]:
+    """
+    Returns a list of available feature names.
+    """
+    return list(name_dict.keys())
+
+
 def get_freq_amp(x: np.ndarray, fs: int):
     """
     Examples
     --------
     >>> n_secs = 5
     >>> fs = 256
     >>> true_freqs = np.array([11, 23, 31, 41])
@@ -21,48 +30,48 @@
     freq = sp.fft.fftfreq(n, d=1 / fs)
     fhat = sp.fft.fft(x)
     amp = 2 * np.abs(fhat) / n
     amp[..., 0] = 0
     return freq[: n // 2].copy(), amp[..., : n // 2].copy()
 
 
-def get_rmeds(x: np.ndarray, axis=-1):
+def get_rmeds(x: np.ndarray, axis=-1, keepdims=False):
     """
     Examples
     --------
     >>> rmeds = get_rmeds(np.random.randn(10, 1024))
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
-    return np.sqrt(np.median(x**2, axis=axis))
+    return np.sqrt(np.median(x**2, axis=axis, keepdims=keepdims))
 
 
-def get_rms(x: np.ndarray, axis=-1):
+def get_rms(x: np.ndarray, axis=-1, keepdims=False):
     """
     Examples
     --------
     >>> rms = get_rms(np.random.randn(10, 1024))
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
-    return np.sqrt(np.mean(x**2, axis=axis))
+    return np.sqrt(np.mean(x**2, axis=axis, keepdims=keepdims))
 
 
-def get_zcr(x: np.ndarray, axis=-1):
+def get_zcr(x: np.ndarray, axis=-1, keepdims=False):
     """
     Examples
     --------
     >>> zcr = get_zcr(np.random.randn(10, 1024))
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
-    zc = np.abs(np.diff(np.sign(x), axis=axis)).sum(axis) / 2
+    zc = np.abs(np.diff(np.sign(x), axis=axis)).sum(axis, keepdims=keepdims) / 2
     return zc / x.shape[1]
 
 
 name_dict = {
     "entropy": stats.entropy,
     "kurtosis": stats.kurtosis,
     "mad": stats.median_abs_deviation,
@@ -72,31 +81,37 @@
     "rms": get_rms,
     "skew": stats.skew,
     "std": np.std,
     "zcr": get_zcr,
 }
 
 
-def get_feature(x: np.ndarray, name: str):
+def get_feature(x: np.ndarray, name=None, keepdims=False):
     """
     Examples
     --------
     >>> n_samples = 4
     >>> n_size = 1024
     >>> x = np.random.randn(n_samples, n_size)
     >>> entropy = get_feature(x, name='entropy')
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
 
+    if name is None:
+        name = "mean"
+
     func = name_dict.get(name)
     if not func:
         raise TypeError("Unsupported provided name.")
-    return func(x, axis=1)
+    out = func(x, axis=1)
+    if keepdims:
+        out = out[..., np.newaxis]
+    return out
 
 
 def get_spectral_feature(
     x: np.ndarray,
     fs: int,
     freq_intervals: np.ndarray,
     name: str,
```

### Comparing `aiontutil-0.0.3/PKG-INFO` & `aiontutil-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiontutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: aiont utility package
 Author: jlan
 Author-email: jlan@aiont.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


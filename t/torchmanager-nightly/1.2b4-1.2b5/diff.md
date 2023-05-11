# Comparing `tmp/torchmanager_nightly-1.2b4.tar.gz` & `tmp/torchmanager_nightly-1.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2b4.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.2b5.tar", max compression
```

## Comparing `torchmanager_nightly-1.2b4.tar` & `torchmanager_nightly-1.2b5.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager_nightly-1.2b4/LICENSE
--rw-r--r--   0        0        0      630 2023-05-08 14:23:27.320345 torchmanager_nightly-1.2b4/pyproject.toml
--rw-r--r--   0        0        0      290 2023-05-08 13:43:46.325073 torchmanager_nightly-1.2b4/torchmanager/__init__.py
--rw-r--r--   0        0        0    10862 2023-05-08 13:43:46.325934 torchmanager_nightly-1.2b4/torchmanager/basic.py
--rw-r--r--   0        0        0      407 2023-05-08 14:17:30.950344 torchmanager_nightly-1.2b4/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4444 2023-05-08 13:43:46.326850 torchmanager_nightly-1.2b4/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4542 2023-05-05 19:12:14.634769 torchmanager_nightly-1.2b4/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-05-05 19:12:14.634924 torchmanager_nightly-1.2b4/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-05-05 19:12:14.635097 torchmanager_nightly-1.2b4/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     2224 2023-05-05 19:12:14.636103 torchmanager_nightly-1.2b4/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0      963 2023-05-05 19:12:14.636949 torchmanager_nightly-1.2b4/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-05-08 13:43:46.329009 torchmanager_nightly-1.2b4/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     2938 2023-05-08 13:43:46.329473 torchmanager_nightly-1.2b4/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-05-05 19:12:14.637989 torchmanager_nightly-1.2b4/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6872 2023-05-08 13:43:46.329939 torchmanager_nightly-1.2b4/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-05-08 13:43:46.330353 torchmanager_nightly-1.2b4/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      156 2023-05-08 13:43:46.330762 torchmanager_nightly-1.2b4/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-05-05 19:12:14.639321 torchmanager_nightly-1.2b4/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1047 2023-05-08 13:43:46.331239 torchmanager_nightly-1.2b4/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5757 2023-05-08 13:43:46.331846 torchmanager_nightly-1.2b4/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3117 2023-05-08 13:43:46.332319 torchmanager_nightly-1.2b4/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      333 2023-05-08 14:16:25.774412 torchmanager_nightly-1.2b4/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     4033 2023-05-08 13:43:46.333249 torchmanager_nightly-1.2b4/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     3678 2023-05-08 13:43:46.333784 torchmanager_nightly-1.2b4/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     2738 2023-05-08 14:16:10.459950 torchmanager_nightly-1.2b4/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2070 2023-05-08 13:43:46.334611 torchmanager_nightly-1.2b4/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4003 2023-05-08 13:43:46.335100 torchmanager_nightly-1.2b4/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     9661 2023-05-08 13:43:46.335569 torchmanager_nightly-1.2b4/torchmanager/testing.py
--rw-r--r--   0        0        0       96 2023-05-08 13:43:46.336135 torchmanager_nightly-1.2b4/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-05-05 19:12:14.643782 torchmanager_nightly-1.2b4/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      694 2023-05-08 13:43:46.336607 torchmanager_nightly-1.2b4/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    14606 2023-05-08 13:43:46.337152 torchmanager_nightly-1.2b4/torchmanager/training.py
--rw-r--r--   0        0        0      459 2023-05-08 13:43:46.337707 torchmanager_nightly-1.2b4/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      109 2023-05-08 13:43:46.338158 torchmanager_nightly-1.2b4/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4879 2023-05-08 13:43:46.339074 torchmanager_nightly-1.2b4/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-05-05 19:12:14.629968 torchmanager_nightly-1.2b4/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      212 2023-05-08 14:15:24.133141 torchmanager_nightly-1.2b4/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      435 2023-05-08 14:15:08.303138 torchmanager_nightly-1.2b4/torchmanager_core/errors/dependencies.py
--rw-r--r--   0        0        0      350 2023-05-05 19:12:14.630265 torchmanager_nightly-1.2b4/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-05-05 19:12:14.630479 torchmanager_nightly-1.2b4/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2772 2023-05-08 13:43:46.339627 torchmanager_nightly-1.2b4/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-05-08 13:43:46.340057 torchmanager_nightly-1.2b4/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-05-08 13:43:46.340502 torchmanager_nightly-1.2b4/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-05-05 19:12:14.631720 torchmanager_nightly-1.2b4/torchmanager_core/typing.py
--rw-r--r--   0        0        0     5137 2023-05-08 13:43:46.341063 torchmanager_nightly-1.2b4/torchmanager_core/version.py
--rw-r--r--   0        0        0      439 2023-05-08 13:43:46.341494 torchmanager_nightly-1.2b4/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-05-05 19:12:14.633240 torchmanager_nightly-1.2b4/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b4/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager_nightly-1.2b5/LICENSE
+-rw-r--r--   0        0        0      659 2023-05-11 14:10:04.977471 torchmanager_nightly-1.2b5/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-05-08 17:31:19.548937 torchmanager_nightly-1.2b5/torchmanager/__init__.py
+-rw-r--r--   0        0        0    10862 2023-05-08 17:31:19.549758 torchmanager_nightly-1.2b5/torchmanager/basic.py
+-rw-r--r--   0        0        0      638 2023-05-11 13:57:10.996802 torchmanager_nightly-1.2b5/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-05-08 17:31:19.551173 torchmanager_nightly-1.2b5/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4542 2023-05-08 15:41:32.410921 torchmanager_nightly-1.2b5/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-05-08 15:41:32.411287 torchmanager_nightly-1.2b5/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-05-08 15:41:32.411512 torchmanager_nightly-1.2b5/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4642 2023-05-11 13:57:10.998528 torchmanager_nightly-1.2b5/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-05-08 15:41:32.412048 torchmanager_nightly-1.2b5/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2599 2023-05-11 13:57:10.999017 torchmanager_nightly-1.2b5/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      963 2023-05-08 15:41:32.412409 torchmanager_nightly-1.2b5/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-05-08 17:31:19.551425 torchmanager_nightly-1.2b5/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     2938 2023-05-08 17:31:19.551828 torchmanager_nightly-1.2b5/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-05-08 15:41:32.412717 torchmanager_nightly-1.2b5/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6872 2023-05-08 17:31:19.552543 torchmanager_nightly-1.2b5/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-05-08 17:31:19.553192 torchmanager_nightly-1.2b5/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-05-08 17:31:19.553780 torchmanager_nightly-1.2b5/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-05-08 15:41:32.413797 torchmanager_nightly-1.2b5/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-05-08 17:31:19.554805 torchmanager_nightly-1.2b5/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5757 2023-05-08 17:31:19.555336 torchmanager_nightly-1.2b5/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3117 2023-05-08 17:31:19.555950 torchmanager_nightly-1.2b5/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      333 2023-05-08 17:31:19.556524 torchmanager_nightly-1.2b5/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4033 2023-05-08 17:31:19.557449 torchmanager_nightly-1.2b5/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3678 2023-05-08 17:31:19.558421 torchmanager_nightly-1.2b5/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-05-11 13:57:10.999702 torchmanager_nightly-1.2b5/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-05-08 17:31:19.561159 torchmanager_nightly-1.2b5/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4003 2023-05-08 17:31:19.561917 torchmanager_nightly-1.2b5/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     9661 2023-05-08 17:31:19.562736 torchmanager_nightly-1.2b5/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-05-08 17:31:19.563726 torchmanager_nightly-1.2b5/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-05-08 15:41:32.416190 torchmanager_nightly-1.2b5/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      694 2023-05-08 17:31:19.564048 torchmanager_nightly-1.2b5/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    14606 2023-05-08 17:31:19.564657 torchmanager_nightly-1.2b5/torchmanager/training.py
+-rw-r--r--   0        0        0      459 2023-05-08 17:31:19.565967 torchmanager_nightly-1.2b5/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-08 17:31:19.566369 torchmanager_nightly-1.2b5/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4879 2023-05-08 17:31:19.567159 torchmanager_nightly-1.2b5/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-05-08 15:41:32.417827 torchmanager_nightly-1.2b5/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-05-11 13:57:11.006538 torchmanager_nightly-1.2b5/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-05-08 15:41:32.418186 torchmanager_nightly-1.2b5/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-05-08 15:41:32.418350 torchmanager_nightly-1.2b5/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2772 2023-05-08 17:31:19.568914 torchmanager_nightly-1.2b5/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-05-08 17:31:19.569189 torchmanager_nightly-1.2b5/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-05-08 17:31:19.569753 torchmanager_nightly-1.2b5/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-05-08 15:41:32.418803 torchmanager_nightly-1.2b5/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     5137 2023-05-08 17:31:19.570362 torchmanager_nightly-1.2b5/torchmanager_core/version.py
+-rw-r--r--   0        0        0      439 2023-05-08 17:31:19.570634 torchmanager_nightly-1.2b5/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-08 15:41:32.420108 torchmanager_nightly-1.2b5/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b5/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2b4/LICENSE` & `torchmanager_nightly-1.2b5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/pyproject.toml` & `torchmanager_nightly-1.2b5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2b4"
-description = "PyTorch Training Manager v1.2 (Beta 4)"
+version = "1.2b5"
+description = "PyTorch Training Manager v1.2 (Beta 5)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = "*"
 tqdm = "*"
 
 [tool.poetry.optional-dependencies]
-scipy = { version = "*", extras = ["torchmanager_scipy"] }
-tensorboard = { version = "*", extras = ["torchmanager_tensorboard"] }
+scipy = { version = "*" }
+tensorboard = { version = "*" }
+
+[tool.poetry.extras]
+scipy = ["scipy"]
+tensorboard = ["tensorboard"]
+all = ["scipy", "tensorboard"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `torchmanager_nightly-1.2b4/torchmanager/basic.py` & `torchmanager_nightly-1.2b5/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.2b5/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.2b5/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.2b5/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.2b5/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.2b5/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/compatibility.py` & `torchmanager_nightly-1.2b5/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/configs/basic.py` & `torchmanager_nightly-1.2b5/torchmanager/configs/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/data/dataset.py` & `torchmanager_nightly-1.2b5/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/data/sliding.py` & `torchmanager_nightly-1.2b5/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.2b5/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/losses/dice.py` & `torchmanager_nightly-1.2b5/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/losses/loss.py` & `torchmanager_nightly-1.2b5/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/losses/mse.py` & `torchmanager_nightly-1.2b5/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.2b5/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.2b5/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.2b5/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/metrics/metric.py` & `torchmanager_nightly-1.2b5/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/testing.py` & `torchmanager_nightly-1.2b5/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/train/checkpoint.py` & `torchmanager_nightly-1.2b5/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.2b5/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager/training.py` & `torchmanager_nightly-1.2b5/torchmanager/training.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.2b5/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.2b5/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager_core/protocols.py` & `torchmanager_nightly-1.2b5/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.2b5/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b4/torchmanager_core/version.py` & `torchmanager_nightly-1.2b5/torchmanager_core/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2b4")
-DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 4)"
+CURRENT = Version("v1.2b5")
+DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 5)"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager_nightly-1.2b4/PKG-INFO` & `torchmanager_nightly-1.2b5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b4
-Summary: PyTorch Training Manager v1.2 (Beta 4)
+Version: 1.2b5
+Summary: PyTorch Training Manager v1.2 (Beta 5)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: scipy
+Provides-Extra: tensorboard
 Requires-Dist: torch
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/kisonho/torchmanager.git
```


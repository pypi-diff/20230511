# Comparing `tmp/gradient-accumulator-0.5.0.tar.gz` & `tmp/gradient-accumulator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gradient-accumulator-0.5.0.tar", last modified: Sun May  7 20:35:18 2023, max compression
+gzip compressed data, was "dist/gradient-accumulator-0.5.1.tar", last modified: Thu May 11 07:22:13 2023, max compression
```

## Comparing `gradient-accumulator-0.5.0.tar` & `gradient-accumulator-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6815 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/gradient_accumulator/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20181 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/accumulators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2609 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/agc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9030 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 07:22:13.000000 gradient-accumulator-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     8784 2023-05-11 07:22:13.000000 gradient-accumulator-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6836 2023-05-11 07:21:20.000000 gradient-accumulator-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 07:22:13.000000 gradient-accumulator-0.5.1/gradient_accumulator/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-11 07:21:20.000000 gradient-accumulator-0.5.1/gradient_accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20225 2023-05-11 07:21:20.000000 gradient-accumulator-0.5.1/gradient_accumulator/accumulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2609 2023-05-11 07:21:20.000000 gradient-accumulator-0.5.1/gradient_accumulator/agc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9030 2023-05-11 07:21:20.000000 gradient-accumulator-0.5.1/gradient_accumulator/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 07:22:13.000000 gradient-accumulator-0.5.1/gradient_accumulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8784 2023-05-11 07:22:12.000000 gradient-accumulator-0.5.1/gradient_accumulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-11 07:22:13.000000 gradient-accumulator-0.5.1/gradient_accumulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 07:22:12.000000 gradient-accumulator-0.5.1/gradient_accumulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-11 07:22:12.000000 gradient-accumulator-0.5.1/gradient_accumulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-11 07:22:12.000000 gradient-accumulator-0.5.1/gradient_accumulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-11 07:22:13.000000 gradient-accumulator-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-05-11 07:21:20.000000 gradient-accumulator-0.5.1/setup.py
```

### Comparing `gradient-accumulator-0.5.0/PKG-INFO` & `gradient-accumulator-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradient-accumulator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package for gradient accumulation in TensorFlow
 Home-page: https://github.com/andreped/GradientAccumulator
 Author: André Pedersen and David Bouget and Javier Pérez de Frutos and Tor-Arne Schmidt Nordmo
 Author-email: andrped94@gmail.com
 License: UNKNOWN
 Description: <div align="center">
         <img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
@@ -63,15 +63,15 @@
         ## [What?](https://github.com/andreped/GradientAccumulator#what)
         Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are then _accumulated_ to produce the full batch gradient.
         
         <p align="center">
         <img src="assets/grad_accum.png" width="70%">
         </p>
         
-        Note that the very natural how we perform gradient accumulation is slightly different to avoid us needing to have the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
+        Note that how we implemented gradient accumulation is slightly different from this illustration, as our design does not require having the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
         
         
         ## [Why?](https://github.com/andreped/GradientAccumulator#why)
         In TensorFlow 2, there did not exist a plug-and-play method to use gradient accumulation with any custom pipeline. Hence, we have implemented two generic TF2-compatible approaches:
         
         | Method | Usage |
         | - | - |
@@ -130,7 +130,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `gradient-accumulator-0.5.0/README.md` & `gradient-accumulator-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 ## [What?](https://github.com/andreped/GradientAccumulator#what)
 Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are then _accumulated_ to produce the full batch gradient.
 
 <p align="center">
 <img src="assets/grad_accum.png" width="70%">
 </p>
 
-Note that the very natural how we perform gradient accumulation is slightly different to avoid us needing to have the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
+Note that how we implemented gradient accumulation is slightly different from this illustration, as our design does not require having the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
 
 
 ## [Why?](https://github.com/andreped/GradientAccumulator#why)
 In TensorFlow 2, there did not exist a plug-and-play method to use gradient accumulation with any custom pipeline. Hence, we have implemented two generic TF2-compatible approaches:
 
 | Method | Usage |
 | - | - |
```

### Comparing `gradient-accumulator-0.5.0/gradient_accumulator/accumulators.py` & `gradient-accumulator-0.5.1/gradient_accumulator/accumulators.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 opt = tf.keras.optimizers.Optimizer
 if int(tf.version.VERSION.split(".")[1]) > 10:
     opt = tf.keras.optimizers.legacy.Optimizer
 
 
 # https://stackoverflow.com/a/66524901
 # https://keras.io/guides/customizing_what_happens_in_fit/
-@tf.keras.utils.register_keras_serializable()
+@tf.keras.utils.register_keras_serializable("gradient-accumulator")
 class GradientAccumulateModel(tf.keras.Model):
     """Model wrapper for gradient accumulation."""
 
     def __init__(
         self,
         accum_steps: int = 1,
         mixed_precision: bool = False,
@@ -191,15 +191,15 @@
             for i, v in enumerate(self.trainable_variables)
         ]
 
 
 # Implementation was derived from:
 # https://github.com/fsx950223/addons/blob/67c1e8ea19e82c3f2a5706674dd81f15ab5002a2/tensorflow_addons/optimizers/gradient_accumulator.py  # noqa
 # https://github.com/FreddeFrallan/Multilingual-CLIP/blob/5c82118452b3b59b41bb53714d61cd4990b1588d/multilingual_clip/TeacherLearning/Utils.py#L84  # noqa
-@tf.keras.utils.register_keras_serializable()
+@tf.keras.utils.register_keras_serializable("gradient-accumulator")
 class GradientAccumulateOptimizer(opt):
     """Optimizer wrapper for gradient accumulation."""
 
     def __init__(
         self,
         optimizer="SGD",
         accum_steps=1,
@@ -247,15 +247,15 @@
         self._optimizer._create_slots(var_list=var_list)
         for var in var_list:
             self.add_slot(var, "ga")
 
         self._gradients = [self.get_slot(var, "ga") for var in var_list]
 
     @property
-    def step(self):  # pragma: no cover
+    def step(self):
         """The number of training steps this Optimizer has run.
         Initializes step variable if None.
 
         Returns:
             Current number of optimizer steps.
         """
         if self._step is None:
@@ -268,15 +268,15 @@
                     trainable=False,
                     aggregation=tf.VariableAggregation.ONLY_FIRST_REPLICA,
                 )
             self._weights.append(self._step)
         return self._step
 
     @step.setter
-    def step(self, variable):
+    def step(self, variable):  # pragma: no cover
         """Sets the step value."""
         if self._step is not None:
             raise RuntimeError(
                 "Cannot set `step` to a new Variable after "
                 "the Optimizer weights have been created"
             )
         self._step = variable
```

### Comparing `gradient-accumulator-0.5.0/gradient_accumulator/agc.py` & `gradient-accumulator-0.5.1/gradient_accumulator/agc.py`

 * *Files identical despite different names*

### Comparing `gradient-accumulator-0.5.0/gradient_accumulator/layers.py` & `gradient-accumulator-0.5.1/gradient_accumulator/layers.py`

 * *Files identical despite different names*

### Comparing `gradient-accumulator-0.5.0/gradient_accumulator.egg-info/PKG-INFO` & `gradient-accumulator-0.5.1/gradient_accumulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradient-accumulator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package for gradient accumulation in TensorFlow
 Home-page: https://github.com/andreped/GradientAccumulator
 Author: André Pedersen and David Bouget and Javier Pérez de Frutos and Tor-Arne Schmidt Nordmo
 Author-email: andrped94@gmail.com
 License: UNKNOWN
 Description: <div align="center">
         <img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
@@ -63,15 +63,15 @@
         ## [What?](https://github.com/andreped/GradientAccumulator#what)
         Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are then _accumulated_ to produce the full batch gradient.
         
         <p align="center">
         <img src="assets/grad_accum.png" width="70%">
         </p>
         
-        Note that the very natural how we perform gradient accumulation is slightly different to avoid us needing to have the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
+        Note that how we implemented gradient accumulation is slightly different from this illustration, as our design does not require having the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
         
         
         ## [Why?](https://github.com/andreped/GradientAccumulator#why)
         In TensorFlow 2, there did not exist a plug-and-play method to use gradient accumulation with any custom pipeline. Hence, we have implemented two generic TF2-compatible approaches:
         
         | Method | Usage |
         | - | - |
@@ -130,7 +130,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```


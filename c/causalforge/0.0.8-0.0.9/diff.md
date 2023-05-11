# Comparing `tmp/causalforge-0.0.8.tar.gz` & `tmp/causalforge-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.8.tar", last modified: Fri May  5 23:30:22 2023, max compression
+gzip compressed data, was "causalforge-0.0.9.tar", last modified: Thu May 11 20:45:40 2023, max compression
```

## Comparing `causalforge-0.0.8.tar` & `causalforge-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.797928 causalforge-0.0.8/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.8/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-05 23:30:22.798164 causalforge-0.0.8/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     2580 2023-05-04 08:14:33.000000 causalforge-0.0.8/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.787429 causalforge-0.0.8/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)      146 2023-05-05 23:29:22.000000 causalforge-0.0.8/causalforge/__init__.py
--rw-r--r--   0 AG62216    (501) staff       (20)     3801 2023-05-03 23:40:50.000000 causalforge-0.0.8/causalforge/data_loader.py
--rw-r--r--   0 AG62216    (501) staff       (20)     3285 2023-05-05 22:52:33.000000 causalforge-0.0.8/causalforge/metrics.py
--rw-r--r--   0 AG62216    (501) staff       (20)     2870 2023-05-04 17:12:50.000000 causalforge-0.0.8/causalforge/model.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.796688 causalforge-0.0.8/causalforge/models/
--rw-r--r--   0 AG62216    (501) staff       (20)       85 2023-05-04 00:28:37.000000 causalforge-0.0.8/causalforge/models/__init__.py
--rw-r--r--   0 AG62216    (501) staff       (20)     7439 2023-05-05 22:30:35.000000 causalforge-0.0.8/causalforge/models/dragonnet.py
--rw-r--r--   0 AG62216    (501) staff       (20)     5911 2023-05-04 01:22:14.000000 causalforge-0.0.8/causalforge/models/utils.py
--rw-r--r--   0 AG62216    (501) staff       (20)      519 2023-05-05 04:55:01.000000 causalforge-0.0.8/causalforge/utils.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.793061 causalforge-0.0.8/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      417 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      137 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-05 23:30:22.799226 causalforge-0.0.8/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1660 2023-05-02 00:20:37.000000 causalforge-0.0.8/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.512554 causalforge-0.0.9/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.9/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-11 20:45:40.512770 causalforge-0.0.9/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     2580 2023-05-04 08:14:33.000000 causalforge-0.0.9/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.500987 causalforge-0.0.9/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)      146 2023-05-11 20:42:17.000000 causalforge-0.0.9/causalforge/__init__.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     3801 2023-05-03 23:40:50.000000 causalforge-0.0.9/causalforge/data_loader.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     3285 2023-05-05 22:52:33.000000 causalforge-0.0.9/causalforge/metrics.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     3381 2023-05-11 18:46:21.000000 causalforge-0.0.9/causalforge/model.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.511680 causalforge-0.0.9/causalforge/models/
+-rw-r--r--   0 AG62216    (501) staff       (20)      159 2023-05-11 18:46:32.000000 causalforge-0.0.9/causalforge/models/__init__.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     8906 2023-05-11 20:21:07.000000 causalforge-0.0.9/causalforge/models/bcauss.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     6699 2023-05-11 19:38:39.000000 causalforge-0.0.9/causalforge/models/dragonnet.py
+-rw-r--r--   0 AG62216    (501) staff       (20)    12960 2023-05-08 22:56:29.000000 causalforge-0.0.9/causalforge/models/ganite.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     6077 2023-05-11 19:12:08.000000 causalforge-0.0.9/causalforge/models/utils.py
+-rw-r--r--   0 AG62216    (501) staff       (20)      519 2023-05-05 04:55:01.000000 causalforge-0.0.9/causalforge/utils.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-11 20:45:40.505539 causalforge-0.0.9/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      475 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      137 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-11 20:45:40.000000 causalforge-0.0.9/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-11 20:45:40.514249 causalforge-0.0.9/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1660 2023-05-02 00:20:37.000000 causalforge-0.0.9/setup.py
```

### Comparing `causalforge-0.0.8/LICENSE` & `causalforge-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.8/PKG-INFO` & `causalforge-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalforge
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `causalforge-0.0.8/README.md` & `causalforge-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.8/causalforge/data_loader.py` & `causalforge-0.0.9/causalforge/data_loader.py`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.8/causalforge/metrics.py` & `causalforge-0.0.9/causalforge/metrics.py`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.8/causalforge/model.py` & `causalforge-0.0.9/causalforge/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     mod = __import__(components[0])
     for comp in components[1:]:
         mod = getattr(mod, comp)
     return mod
 
 
 class PROBLEM_TYPE(Enum):
-    CAUSAL_TREATMENT_EFFECT_ESTIMATION = 1
-    PROPENSITY_ESTIMATION = 2 
-    SYNTHETIC_DATA_GENERATION = 3
+    CAUSAL_TREATMENT_EFFECT_ESTIMATION = "causal_treatment_effect_estimation"
+    PROPENSITY_ESTIMATION = "propensity_estimation"
+    SYNTHETIC_DATA_GENERATION = "syntethic_data_generation"
 
 
 class Model(ABC):
     
     def __init__(self):
         pass
 
@@ -27,19 +27,29 @@
                      params,
                      problem_type=PROBLEM_TYPE.CAUSAL_TREATMENT_EFFECT_ESTIMATION, 
                      multiple_treatments=False):
         if  problem_type==PROBLEM_TYPE.CAUSAL_TREATMENT_EFFECT_ESTIMATION:
             if multiple_treatments:
                 raise Exception("Multiple treatments not supported yet")
             else:
-                if name == 'dragonnet':
+                if name == 'bcauss':
+                    klass = dynamic_import('causalforge.models.BCAUSS')
+                    net = klass()
+                    net.build(params)
+                    return net
+                elif name == 'dragonnet':
                     klass = dynamic_import('causalforge.models.DragonNet')
                     net = klass()
                     net.build(params)
                     return net
+                elif name == 'ganite':
+                    klass = dynamic_import('causalforge.models.Ganite')
+                    net = klass()
+                    net.build(params) 
+                    return net
                 elif name == 'bcauss':
                     pass 
                 else:
                     raise Exception("Model not supported yet::"+str(name))
         elif problem_type==PROBLEM_TYPE.PROPENSITY_ESTIMATION:
             raise Exception("problem_type not supported yet::"+str(problem_type))
         elif problem_type==PROBLEM_TYPE.SYNTHETIC_DATA_GENERATION:
```

### Comparing `causalforge-0.0.8/causalforge/models/dragonnet.py` & `causalforge-0.0.9/causalforge/models/dragonnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Code Skeleton from: https://github.com/uber/causalml/blob/master/causalml/inference/tf/dragonnet.py
 Original implementation: https://github.com/claudiashi57/dragonnet 
 """
 
 import numpy as np
-from tensorflow.keras import Input, Model
+from tensorflow.keras import Input
+from tensorflow.keras import Model as keras_Model
 from tensorflow.keras.callbacks import EarlyStopping, ReduceLROnPlateau, TerminateOnNaN
 from tensorflow.keras.layers import Dense, Concatenate
 from tensorflow.keras.optimizers import SGD, Adam
 from tensorflow.keras.regularizers import l2
 from tensorflow.keras.layers import Layer
 import tensorflow as tf
 import keras.backend as K
@@ -16,43 +17,19 @@
 from .utils import (
     dragonnet_loss_binarycross,
     EpsilonLayer,
     regression_loss,
     binary_classification_loss,
     treatment_accuracy,
     track_epsilon,
+    convert_pd_to_np,
     make_tarreg_loss,
 )
 
-def convert_pd_to_np(*args):
-    output = [obj.to_numpy() if hasattr(obj, "to_numpy") else obj for obj in args]
-    return output if len(output) > 1 else output[0]
-
-class EpsilonLayer(Layer):
-    """
-    Custom keras layer to allow epsilon to be learned during training process.
-    """
-
-    def __init__(self):
-        """
-        Inherits keras' Layer object.
-        """
-        super(EpsilonLayer, self).__init__()
-
-    def build(self, input_shape):
-        """
-        Creates a trainable weight variable for this layer.
-        """
-        self.epsilon = self.add_weight(
-            name="epsilon", shape=[1, 1], initializer="RandomNormal", trainable=True
-        )
-        super(EpsilonLayer, self).build(input_shape)
-
-    def call(self, inputs, **kwargs):
-        return self.epsilon * tf.ones_like(inputs)[:, 0:1]
+from causalforge.model import Model
 
 class DragonNet(Model):
     
     def build(self,user_params):
         
         if 'input_dim' not in user_params:
             raise Exception("input_dim must be specified!")
@@ -70,16 +47,15 @@
             'momentum': 0.9,
             'use_adam': True,
             'adam_epochs':30, 
             'adam_learning_rate': 1e-3
         }
         
         for k in params:
-            if k in user_params:
-                params[k] = user_params[k]
+            params[k] = user_params.get(k,params[k])
                 
         params['input_dim' ] = user_params['input_dim']
        
         # 
         K.clear_session()
         
         inputs = Input(shape=(params['input_dim'],), name="input")
@@ -143,15 +119,15 @@
 
         dl = EpsilonLayer()
         epsilons = dl(t_predictions, name="epsilon")
         concat_pred = Concatenate(1)(
             [y0_predictions, y1_predictions, t_predictions, epsilons]
         )
         
-        self.model = Model(inputs=inputs, outputs=concat_pred)
+        self.model = keras_Model(inputs=inputs, outputs=concat_pred)
         self.params = params
     
     def support_ite(self):
         return True 
     
     def predict_ite(self, X):
         preds = self.model.predict(X)
```

### Comparing `causalforge-0.0.8/causalforge/models/utils.py` & `causalforge-0.0.9/causalforge/models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import tensorflow as tf
 from tensorflow.keras import backend as K
 from tensorflow.keras.layers import Layer
 from tensorflow.keras.metrics import binary_accuracy
 
 
+def convert_pd_to_np(*args):
+    output = [obj.to_numpy() if hasattr(obj, "to_numpy") else obj for obj in args]
+    return output if len(output) > 1 else output[0]
+
+
 def binary_classification_loss(concat_true, concat_pred):
     """
     Implements a classification (binary cross-entropy) loss function for DragonNet architecture.
 
     Args:
         - concat_true (tf.tensor): tensor of true samples, with shape (n_samples, 2)
                                    Each row in concat_true is comprised of (y, treatment)
```

### Comparing `causalforge-0.0.8/causalforge/utils.py` & `causalforge-0.0.9/causalforge/utils.py`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.8/causalforge.egg-info/PKG-INFO` & `causalforge-0.0.9/causalforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalforge
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `causalforge-0.0.8/setup.py` & `causalforge-0.0.9/setup.py`

 * *Files identical despite different names*


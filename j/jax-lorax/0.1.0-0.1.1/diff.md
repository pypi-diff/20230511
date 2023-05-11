# Comparing `tmp/jax_lorax-0.1.0.tar.gz` & `tmp/jax_lorax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_lorax-0.1.0.tar", max compression
+gzip compressed data, was "jax_lorax-0.1.1.tar", max compression
```

## Comparing `jax_lorax-0.1.0.tar` & `jax_lorax-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-03 04:00:32.027251 jax_lorax-0.1.0/LICENSE
--rw-r--r--   0        0        0     4264 2023-05-03 21:13:33.920875 jax_lorax-0.1.0/README.md
--rw-r--r--   0        0        0      132 2023-05-03 18:07:36.010823 jax_lorax-0.1.0/lorax/__init__.py
--rw-r--r--   0        0        0       31 2023-05-03 17:53:42.180819 jax_lorax-0.1.0/lorax/constants.py
--rw-r--r--   0        0        0     3396 2023-05-05 21:12:10.615018 jax_lorax-0.1.0/lorax/helpers.py
--rw-r--r--   0        0        0    10227 2023-05-08 20:14:22.096215 jax_lorax-0.1.0/lorax/transform.py
--rw-r--r--   0        0        0      479 2023-05-08 20:46:10.859557 jax_lorax-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4908 1970-01-01 00:00:00.000000 jax_lorax-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 04:00:32.027251 jax_lorax-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4396 2023-05-11 00:46:40.640430 jax_lorax-0.1.1/README.md
+-rw-r--r--   0        0        0      132 2023-05-03 18:07:36.010823 jax_lorax-0.1.1/lorax/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-03 17:53:42.180819 jax_lorax-0.1.1/lorax/constants.py
+-rw-r--r--   0        0        0     3541 2023-05-11 00:45:32.753763 jax_lorax-0.1.1/lorax/helpers.py
+-rw-r--r--   0        0        0    10227 2023-05-08 20:14:22.096215 jax_lorax-0.1.1/lorax/transform.py
+-rw-r--r--   0        0        0      479 2023-05-11 00:58:46.167100 jax_lorax-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 jax_lorax-0.1.1/PKG-INFO
```

### Comparing `jax_lorax-0.1.0/LICENSE` & `jax_lorax-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_lorax-0.1.0/README.md` & `jax_lorax-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,29 @@
 This is a JAX transform which implements [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685). LoRA replaces operations like `Wx` with `(W + BA)x` where `A` and `B` are skinny rectangular matrices. You can then train only `A` and `B`, and leave `W` frozen, which dramatically reduces the amount of memory needed for things like optimizer states.
 
 Lorax should work on most JAX models. I did my testing with my models which use Haiku, and you can find an example of applying it to a HuggingFace Flax model in the [examples directory(examples/).
 
 ## Installation 
 
 ```bash
+pip install jax-lorax
+```
+
+### Running tests
+Install dev dependencies:
+```bash
 git clone https://github.com/davisyoshida/lorax.git
 cd lorax
-pip install -e .
+pip install poetry
+poetry install
+```
+
+Run tests:
+```
+pytest tests.py
 ```
 
 ## Minimal example
 Lorax makes it so you can take model code which wasn't written with LoRA in mind, and transform it so that it does! For example, consider the following MLP code:
 
 ```python
 import jax
```

### Comparing `jax_lorax-0.1.0/lorax/helpers.py` & `jax_lorax-0.1.1/lorax/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import jax
 import jax.numpy as jnp
 from jax.tree_util import tree_map_with_path, DictKey, SequenceKey
 
 from .constants import LORA_FREEZE, LORA_FULL
 from .transform import EmptyNode, LoraNode, custom_tree_map
 
-def init_lora(param_tree, spec, rng, stddev=0.01, dtype=jnp.float32, alpha=1.):
+def init_lora(param_tree, spec, rng, stddev=0.01, dtype=jnp.float32, alpha=1., is_leaf=None):
     def freeze_getter(param, spec_val):
         if spec_val == LORA_FULL:
             return EmptyNode
         return param
 
     def tune_getter(path, param, spec_val):
         if spec_val == LORA_FREEZE:
@@ -18,33 +18,36 @@
             return param
 
         if len(param.shape) == 1:
             raise ValueError(f'Vectors must either be frozen or fully tuned, but got spec value {spec} for param with path {path}')
         if len(param.shape) == 2:
             b_dim, a_dim = param.shape
 
+            print(f'b_dim: {b_dim}, a_dim: {a_dim}, spec_val: {spec_val}')
             b = jnp.zeros((b_dim, spec_val), dtype=param.dtype)
             a = jax.random.normal(rng, (spec_val, a_dim), dtype=param.dtype) * stddev
             return LoraNode(a, b, alpha=alpha)
 
         # conv case
-        print(path, param.shape)
         *window_shape, in_channels, out_channels = param.shape
 
         a = jnp.zeros((
             *(1 for _ in range(len(window_shape))),
             spec_val,
             out_channels
         ), dtype=param.dtype)
         b = jax.random.normal(rng, (*window_shape, in_channels, spec_val), dtype=param.dtype) * stddev
         return LoraNode(a, b, alpha=alpha)
 
-    return jax.tree_map(freeze_getter, param_tree, spec), jax.tree_util.tree_map_with_path(tune_getter, param_tree, spec)
+    return (
+        jax.tree_map(freeze_getter, param_tree, spec, is_leaf=is_leaf),
+        jax.tree_util.tree_map_with_path(tune_getter, param_tree, spec, is_leaf=is_leaf)
+    )
 
-def simple_spec(params, decision_fn=None, tune_vectors=False):
+def simple_spec(params, decision_fn=None, tune_vectors=False, is_leaf=None):
     """
     Create a simple lora spec for a pytree
     Args:
         params: pytree of parameters
         tune_vectors: If true, will flag all arrays with less than 2 dimensions for tuning
         decision_fn: A function that takes a string marking the position in the tree and the parameter,
             and returns the spec value for that parameter
@@ -67,15 +70,15 @@
                 else
                 str(node)
             ) for node in path
         )
         value = decision_fn(path_str, arr)
         return value
 
-    return tree_map_with_path(full_fn, params)
+    return tree_map_with_path(full_fn, params, is_leaf=is_leaf)
 
 def merge_params(frozen_params, tunable_params, destructive=True, use_scaling=True):
     """Re-merge LoRA parameters.
     Arguments:
         destructive: If True, the buffers in frozen_params may be freed to save memory.
         use_scaling: Whether to multiply LoRA params by alpha/r
     """
```

### Comparing `jax_lorax-0.1.0/lorax/transform.py` & `jax_lorax-0.1.1/lorax/transform.py`

 * *Files identical despite different names*

### Comparing `jax_lorax-0.1.0/PKG-INFO` & `jax_lorax-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-lorax
-Version: 0.1.0
+Version: 0.1.1
 Summary: A JAX transform which applies LoRA to arbitrary JAX functions/models
 License: MIT
 Author: Davis Yoshida
 Author-email: dyoshida@ttic.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,17 +20,29 @@
 This is a JAX transform which implements [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685). LoRA replaces operations like `Wx` with `(W + BA)x` where `A` and `B` are skinny rectangular matrices. You can then train only `A` and `B`, and leave `W` frozen, which dramatically reduces the amount of memory needed for things like optimizer states.
 
 Lorax should work on most JAX models. I did my testing with my models which use Haiku, and you can find an example of applying it to a HuggingFace Flax model in the [examples directory(examples/).
 
 ## Installation 
 
 ```bash
+pip install jax-lorax
+```
+
+### Running tests
+Install dev dependencies:
+```bash
 git clone https://github.com/davisyoshida/lorax.git
 cd lorax
-pip install -e .
+pip install poetry
+poetry install
+```
+
+Run tests:
+```
+pytest tests.py
 ```
 
 ## Minimal example
 Lorax makes it so you can take model code which wasn't written with LoRA in mind, and transform it so that it does! For example, consider the following MLP code:
 
 ```python
 import jax
```


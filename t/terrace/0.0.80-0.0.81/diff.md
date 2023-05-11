# Comparing `tmp/terrace-0.0.80.tar.gz` & `tmp/terrace-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrace-0.0.80.tar", last modified: Thu May 11 16:33:19 2023, max compression
+gzip compressed data, was "terrace-0.0.81.tar", last modified: Thu May 11 16:48:46 2023, max compression
```

## Comparing `terrace-0.0.80.tar` & `terrace-0.0.81.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:33:19.540887 terrace-0.0.80/
--rw-r--r--   0 boris     (1000) boris     (1001)     1077 2023-05-11 15:23:16.000000 terrace-0.0.80/LICENSE.txt
--rw-r--r--   0 boris     (1000) boris     (1001)     6101 2023-05-11 16:33:19.540887 terrace-0.0.80/PKG-INFO
--rw-r--r--   0 boris     (1000) boris     (1001)     5739 2023-05-11 16:33:18.000000 terrace-0.0.80/README.md
--rw-r--r--   0 boris     (1000) boris     (1001)       38 2023-05-11 16:33:19.540887 terrace-0.0.80/setup.cfg
--rw-r--r--   0 boris     (1000) boris     (1001)      693 2023-05-11 16:33:11.000000 terrace-0.0.80/setup.py
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:33:19.534221 terrace-0.0.80/src/
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:33:19.537554 terrace-0.0.80/src/terrace/
--rw-r--r--   0 boris     (1000) boris     (1001)      249 2023-05-11 15:23:16.000000 terrace-0.0.80/src/terrace/__init__.py
--rw-r--r--   0 boris     (1000) boris     (1001)    13436 2023-05-11 15:23:16.000000 terrace-0.0.80/src/terrace/batch.py
--rw-r--r--   0 boris     (1000) boris     (1001)     5817 2023-05-11 15:23:16.000000 terrace-0.0.80/src/terrace/categorical_tensor.py
--rw-r--r--   0 boris     (1000) boris     (1001)     1000 2023-05-11 15:23:16.000000 terrace-0.0.80/src/terrace/dataframe.py
--rw-r--r--   0 boris     (1000) boris     (1001)     9337 2023-05-11 15:23:16.000000 terrace-0.0.80/src/terrace/graph.py
--rw-r--r--   0 boris     (1000) boris     (1001)     2592 2023-05-11 15:23:16.000000 terrace-0.0.80/src/terrace/meta_utils.py
--rw-r--r--   0 boris     (1000) boris     (1001)     5051 2023-05-11 15:23:16.000000 terrace-0.0.80/src/terrace/module.py
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:33:19.537554 terrace-0.0.80/src/terrace.egg-info/
--rw-r--r--   0 boris     (1000) boris     (1001)     6101 2023-05-11 16:33:19.000000 terrace-0.0.80/src/terrace.egg-info/PKG-INFO
--rw-r--r--   0 boris     (1000) boris     (1001)      377 2023-05-11 16:33:19.000000 terrace-0.0.80/src/terrace.egg-info/SOURCES.txt
--rw-r--r--   0 boris     (1000) boris     (1001)        1 2023-05-11 16:33:19.000000 terrace-0.0.80/src/terrace.egg-info/dependency_links.txt
--rw-r--r--   0 boris     (1000) boris     (1001)       11 2023-05-11 16:33:19.000000 terrace-0.0.80/src/terrace.egg-info/requires.txt
--rw-r--r--   0 boris     (1000) boris     (1001)        8 2023-05-11 16:33:19.000000 terrace-0.0.80/src/terrace.egg-info/top_level.txt
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:48:46.818107 terrace-0.0.81/
+-rw-r--r--   0 boris     (1000) boris     (1001)     1077 2023-05-11 15:23:16.000000 terrace-0.0.81/LICENSE.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)     6147 2023-05-11 16:48:46.818107 terrace-0.0.81/PKG-INFO
+-rw-r--r--   0 boris     (1000) boris     (1001)     5785 2023-05-11 16:48:45.000000 terrace-0.0.81/README.md
+-rw-r--r--   0 boris     (1000) boris     (1001)       38 2023-05-11 16:48:46.818107 terrace-0.0.81/setup.cfg
+-rw-r--r--   0 boris     (1000) boris     (1001)      693 2023-05-11 16:48:39.000000 terrace-0.0.81/setup.py
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:48:46.818107 terrace-0.0.81/src/
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:48:46.818107 terrace-0.0.81/src/terrace/
+-rw-r--r--   0 boris     (1000) boris     (1001)      249 2023-05-11 15:23:16.000000 terrace-0.0.81/src/terrace/__init__.py
+-rw-r--r--   0 boris     (1000) boris     (1001)    13436 2023-05-11 15:23:16.000000 terrace-0.0.81/src/terrace/batch.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     5817 2023-05-11 15:23:16.000000 terrace-0.0.81/src/terrace/categorical_tensor.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     1000 2023-05-11 15:23:16.000000 terrace-0.0.81/src/terrace/dataframe.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     9337 2023-05-11 15:23:16.000000 terrace-0.0.81/src/terrace/graph.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     2592 2023-05-11 15:23:16.000000 terrace-0.0.81/src/terrace/meta_utils.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     5051 2023-05-11 15:23:16.000000 terrace-0.0.81/src/terrace/module.py
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:48:46.818107 terrace-0.0.81/src/terrace.egg-info/
+-rw-r--r--   0 boris     (1000) boris     (1001)     6147 2023-05-11 16:48:46.000000 terrace-0.0.81/src/terrace.egg-info/PKG-INFO
+-rw-r--r--   0 boris     (1000) boris     (1001)      377 2023-05-11 16:48:46.000000 terrace-0.0.81/src/terrace.egg-info/SOURCES.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)        1 2023-05-11 16:48:46.000000 terrace-0.0.81/src/terrace.egg-info/dependency_links.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)       11 2023-05-11 16:48:46.000000 terrace-0.0.81/src/terrace.egg-info/requires.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)        8 2023-05-11 16:48:46.000000 terrace-0.0.81/src/terrace.egg-info/top_level.txt
```

### Comparing `terrace-0.0.80/LICENSE.txt` & `terrace-0.0.81/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `terrace-0.0.80/PKG-INFO` & `terrace-0.0.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrace
-Version: 0.0.80
+Version: 0.0.81
 Summary: high level PyTorch utils
 Home-page: https://github.com/mixarcid/terrace
 Author: Michael Brocidiacono
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -17,15 +17,15 @@
 
 Welcome to Terrace, a collection of high-level utilities for writing concise and maintainable PyTorch code. I've been using PyTorch in my own work for a while now, and I developed these tools to boost my productivity. I'm now ready to share them with the world -- I hope you find Terrace to be as helpful as I have.
 
 Terrace provides two major features: Modules and Batches. Terrace Modules allow you to more concisely define your PyTorch models entirely in the `forward` method. Batches allow you to place all your data in nice classes rather than swinging around a bunch of raw tensors like a barbarian.
 
 ## Modules
 
-If you're writing a PyTorch model, you need to populate both the `__init__` and `forward` methods of your model. `__init__` specifies all the submodules of your model, including all the input and output tensor shapes. `forward` specifies how to use all these submodules in order to run your computation. A simple neural network with a single hidden layer might look something like this:
+If you're writing a vanilla PyTorch model, you need to populate both the `__init__` and `forward` methods of your model. `__init__` specifies all the submodules of your model, including all the input and output tensor shapes. `forward` specifies how to use all these submodules in order to run your computation. A simple neural network with a single hidden layer might look something like this:
 
 
 ```python
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
@@ -59,16 +59,15 @@
 ```python
 import terrace as ter
 
 class BetterSimpleNetwork(ter.Module):
 
     def forward(self, x):
         self.start_forward()
-        # with the LazyLinear layers, we only need to specify
-        # the output dimension
+        # with the LazyLinear layers, we only need to specify the output dimension
         hid = F.relu(self.make(ter.LazyLinear, 64)(x))
         out = self.make(ter.LazyLinear, 1)(hid)
         return out
     
 x = torch.randn(16, 128)
 model = BetterSimpleNetwork()
 out = model(x)
@@ -76,15 +75,15 @@
 ```
 
     torch.Size([16, 1])
 
 
 The first time this model is run, the `make` calls with create new linear layers, each of which lazily creates their weight matrices based on their inputs. Writing complex models is now easier, faster, and just more fun.
 
-There are some important caveats to this approach, so please make sure to check out the [documentation](https://terrace.readthedocs.io).
+There are some important caveats to this approach, so please make sure to check out the [documentation](https://terrace.readthedocs.io/en/latest/guides/module.html).
 
 ## Batches
 
 Out of the box, PyTorch can collate tensors (and tuples of tensors) into batches. But what about arbitrary classes? If your neural network is dealing with complex datatypes, structuring your data in classes is the solution. By inheriting from Terrace's `Batchable` class, you can create datasets of arbitrary objects.
 
 Let's say you're working with people who have faces and names
 
@@ -145,17 +144,19 @@
        face=Tensor(shape=torch.Size([8, 3, 256, 256]), dtype=torch.float32)
        name=Tensor(shape=torch.Size([8, 128]), dtype=torch.float32)
     )
 
 
 Terrace also has a higher-level interface for graph data, and several more features. Check out the [documentation](https://terrace.readthedocs.io)  for more info!
 
+## Getting started
+
 If you're interested in using Terrace for your own work, simply install via pip.
 
 ```bash
 pip install terrace
 ```
 
 If you find Terrace useful, or find a bug, or have an idea for further functionality, please reach out! [Email me](mailto:mixarcidiacono@gmail.com) or find me on [Twitter](https://twitter.com/mixarcid). 
 
-### Disclaimer
+## Disclaimer
 At the moment, Terrace is very much a work in progress. The API is subject to change and there are likely many bugs. In its current state, I would not recommend this package for production use.
```

### Comparing `terrace-0.0.80/README.md` & `terrace-0.0.81/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Welcome to Terrace, a collection of high-level utilities for writing concise and maintainable PyTorch code. I've been using PyTorch in my own work for a while now, and I developed these tools to boost my productivity. I'm now ready to share them with the world -- I hope you find Terrace to be as helpful as I have.
 
 Terrace provides two major features: Modules and Batches. Terrace Modules allow you to more concisely define your PyTorch models entirely in the `forward` method. Batches allow you to place all your data in nice classes rather than swinging around a bunch of raw tensors like a barbarian.
 
 ## Modules
 
-If you're writing a PyTorch model, you need to populate both the `__init__` and `forward` methods of your model. `__init__` specifies all the submodules of your model, including all the input and output tensor shapes. `forward` specifies how to use all these submodules in order to run your computation. A simple neural network with a single hidden layer might look something like this:
+If you're writing a vanilla PyTorch model, you need to populate both the `__init__` and `forward` methods of your model. `__init__` specifies all the submodules of your model, including all the input and output tensor shapes. `forward` specifies how to use all these submodules in order to run your computation. A simple neural network with a single hidden layer might look something like this:
 
 
 ```python
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
@@ -46,16 +46,15 @@
 ```python
 import terrace as ter
 
 class BetterSimpleNetwork(ter.Module):
 
     def forward(self, x):
         self.start_forward()
-        # with the LazyLinear layers, we only need to specify
-        # the output dimension
+        # with the LazyLinear layers, we only need to specify the output dimension
         hid = F.relu(self.make(ter.LazyLinear, 64)(x))
         out = self.make(ter.LazyLinear, 1)(hid)
         return out
     
 x = torch.randn(16, 128)
 model = BetterSimpleNetwork()
 out = model(x)
@@ -63,15 +62,15 @@
 ```
 
     torch.Size([16, 1])
 
 
 The first time this model is run, the `make` calls with create new linear layers, each of which lazily creates their weight matrices based on their inputs. Writing complex models is now easier, faster, and just more fun.
 
-There are some important caveats to this approach, so please make sure to check out the [documentation](https://terrace.readthedocs.io).
+There are some important caveats to this approach, so please make sure to check out the [documentation](https://terrace.readthedocs.io/en/latest/guides/module.html).
 
 ## Batches
 
 Out of the box, PyTorch can collate tensors (and tuples of tensors) into batches. But what about arbitrary classes? If your neural network is dealing with complex datatypes, structuring your data in classes is the solution. By inheriting from Terrace's `Batchable` class, you can create datasets of arbitrary objects.
 
 Let's say you're working with people who have faces and names
 
@@ -132,17 +131,19 @@
        face=Tensor(shape=torch.Size([8, 3, 256, 256]), dtype=torch.float32)
        name=Tensor(shape=torch.Size([8, 128]), dtype=torch.float32)
     )
 
 
 Terrace also has a higher-level interface for graph data, and several more features. Check out the [documentation](https://terrace.readthedocs.io)  for more info!
 
+## Getting started
+
 If you're interested in using Terrace for your own work, simply install via pip.
 
 ```bash
 pip install terrace
 ```
 
 If you find Terrace useful, or find a bug, or have an idea for further functionality, please reach out! [Email me](mailto:mixarcidiacono@gmail.com) or find me on [Twitter](https://twitter.com/mixarcid). 
 
-### Disclaimer
+## Disclaimer
 At the moment, Terrace is very much a work in progress. The API is subject to change and there are likely many bugs. In its current state, I would not recommend this package for production use.
```

### Comparing `terrace-0.0.80/setup.py` & `terrace-0.0.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="terrace",
-    version="0.0.80",
+    version="0.0.81",
     author="Michael Brocidiacono",
     author_email="",
     description="high level PyTorch utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mixarcid/terrace",
     packages=setuptools.find_packages(
```

### Comparing `terrace-0.0.80/src/terrace/batch.py` & `terrace-0.0.81/src/terrace/batch.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.80/src/terrace/categorical_tensor.py` & `terrace-0.0.81/src/terrace/categorical_tensor.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.80/src/terrace/dataframe.py` & `terrace-0.0.81/src/terrace/dataframe.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.80/src/terrace/graph.py` & `terrace-0.0.81/src/terrace/graph.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.80/src/terrace/meta_utils.py` & `terrace-0.0.81/src/terrace/meta_utils.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.80/src/terrace/module.py` & `terrace-0.0.81/src/terrace/module.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.80/src/terrace.egg-info/PKG-INFO` & `terrace-0.0.81/src/terrace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrace
-Version: 0.0.80
+Version: 0.0.81
 Summary: high level PyTorch utils
 Home-page: https://github.com/mixarcid/terrace
 Author: Michael Brocidiacono
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -17,15 +17,15 @@
 
 Welcome to Terrace, a collection of high-level utilities for writing concise and maintainable PyTorch code. I've been using PyTorch in my own work for a while now, and I developed these tools to boost my productivity. I'm now ready to share them with the world -- I hope you find Terrace to be as helpful as I have.
 
 Terrace provides two major features: Modules and Batches. Terrace Modules allow you to more concisely define your PyTorch models entirely in the `forward` method. Batches allow you to place all your data in nice classes rather than swinging around a bunch of raw tensors like a barbarian.
 
 ## Modules
 
-If you're writing a PyTorch model, you need to populate both the `__init__` and `forward` methods of your model. `__init__` specifies all the submodules of your model, including all the input and output tensor shapes. `forward` specifies how to use all these submodules in order to run your computation. A simple neural network with a single hidden layer might look something like this:
+If you're writing a vanilla PyTorch model, you need to populate both the `__init__` and `forward` methods of your model. `__init__` specifies all the submodules of your model, including all the input and output tensor shapes. `forward` specifies how to use all these submodules in order to run your computation. A simple neural network with a single hidden layer might look something like this:
 
 
 ```python
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
@@ -59,16 +59,15 @@
 ```python
 import terrace as ter
 
 class BetterSimpleNetwork(ter.Module):
 
     def forward(self, x):
         self.start_forward()
-        # with the LazyLinear layers, we only need to specify
-        # the output dimension
+        # with the LazyLinear layers, we only need to specify the output dimension
         hid = F.relu(self.make(ter.LazyLinear, 64)(x))
         out = self.make(ter.LazyLinear, 1)(hid)
         return out
     
 x = torch.randn(16, 128)
 model = BetterSimpleNetwork()
 out = model(x)
@@ -76,15 +75,15 @@
 ```
 
     torch.Size([16, 1])
 
 
 The first time this model is run, the `make` calls with create new linear layers, each of which lazily creates their weight matrices based on their inputs. Writing complex models is now easier, faster, and just more fun.
 
-There are some important caveats to this approach, so please make sure to check out the [documentation](https://terrace.readthedocs.io).
+There are some important caveats to this approach, so please make sure to check out the [documentation](https://terrace.readthedocs.io/en/latest/guides/module.html).
 
 ## Batches
 
 Out of the box, PyTorch can collate tensors (and tuples of tensors) into batches. But what about arbitrary classes? If your neural network is dealing with complex datatypes, structuring your data in classes is the solution. By inheriting from Terrace's `Batchable` class, you can create datasets of arbitrary objects.
 
 Let's say you're working with people who have faces and names
 
@@ -145,17 +144,19 @@
        face=Tensor(shape=torch.Size([8, 3, 256, 256]), dtype=torch.float32)
        name=Tensor(shape=torch.Size([8, 128]), dtype=torch.float32)
     )
 
 
 Terrace also has a higher-level interface for graph data, and several more features. Check out the [documentation](https://terrace.readthedocs.io)  for more info!
 
+## Getting started
+
 If you're interested in using Terrace for your own work, simply install via pip.
 
 ```bash
 pip install terrace
 ```
 
 If you find Terrace useful, or find a bug, or have an idea for further functionality, please reach out! [Email me](mailto:mixarcidiacono@gmail.com) or find me on [Twitter](https://twitter.com/mixarcid). 
 
-### Disclaimer
+## Disclaimer
 At the moment, Terrace is very much a work in progress. The API is subject to change and there are likely many bugs. In its current state, I would not recommend this package for production use.
```


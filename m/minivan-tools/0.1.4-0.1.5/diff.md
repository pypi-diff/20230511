# Comparing `tmp/minivan_tools-0.1.4.tar.gz` & `tmp/minivan_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minivan_tools-0.1.4.tar", max compression
+gzip compressed data, was "minivan_tools-0.1.5.tar", max compression
```

## Comparing `minivan_tools-0.1.4.tar` & `minivan_tools-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2308 2023-05-01 21:22:44.591656 minivan_tools-0.1.4/README.md
--rw-r--r--   0        0        0       46 2023-05-01 21:22:44.595656 minivan_tools-0.1.4/minivan/__init__.py
--rw-r--r--   0        0        0     5312 2023-05-01 21:22:44.595656 minivan_tools-0.1.4/minivan/index.py
--rw-r--r--   0        0        0     1014 2023-05-01 21:22:44.595656 minivan_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 minivan_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2205 2023-05-10 22:53:35.004670 minivan_tools-0.1.5/README.md
+-rw-r--r--   0        0        0       46 2023-05-10 22:53:35.008670 minivan_tools-0.1.5/minivan/__init__.py
+-rw-r--r--   0        0        0     6282 2023-05-10 22:53:35.008670 minivan_tools-0.1.5/minivan/index.py
+-rw-r--r--   0        0        0     1037 2023-05-10 22:53:35.008670 minivan_tools-0.1.5/minivan/metrics.py
+-rw-r--r--   0        0        0     1014 2023-05-10 22:53:35.008670 minivan_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 minivan_tools-0.1.5/PKG-INFO
```

### Comparing `minivan_tools-0.1.4/README.md` & `minivan_tools-0.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 # minivan
 
 ![Tests](https://github.com/aismlv/minivan/actions/workflows/test_and_lint.yml/badge.svg)
 [![codecov](https://codecov.io/gh/aismlv/minivan/branch/main/graph/badge.svg?token=5J503UR8O7)](https://codecov.io/gh/aismlv/minivan)
-[![PyPI version](https://badge.fury.io/py/minivan.svg?)](https://pypi.org/project/minivan/)
+[![PyPI version](https://badge.fury.io/py/minivan-tools.svg?)](https://pypi.org/project/minivan-tools/)
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 `minivan` is an exact nearest neighbor search Python library for those times when "approximate" just won't cut it (or is simply overkill).
 
 ## Installation
 
 Install `minivan` using `pip`:
 
 ```bash
 pip install minivan-tools
 ```
 
 ## Usage
-Here is an example of how to use `minivan`:
-
 Create new index:
 ```python
 from minivan import Index
 import numpy as np
 
-# Create an index with 128-dimensional embeddings and dot product metric. Cosine similarity is also supported
+# Create an index with 128-dimensional embeddings and dot product metric
 index = Index(dim=128, metric="dot_product")
 
 # Add embeddings to the index
-embedding1 = np.random.rand(128)
-embedding2 = np.random.rand(128)
-embedding3 = np.random.rand(128)
-
-index.add_items([1, 2, 3], [embedding1, embedding2, embedding3])
+embeddings = [np.random.rand(128) for _ in range(3)]
+index.add_items([1, 2, 3], embeddings)
 
 # Delete embeddings from the index
 index.delete_items([3])
 ```
 
-Search for the nearest neighbors:
+Query the index for the nearest neighbor:
 ```python
-# Query the index for the nearest neighbor of a given embedding
 query_embedding = np.random.rand(128)
 result = index.query(query_embedding, k=1)
 
 print(result)  # Returns [(index, similarity)] of the nearest neighbor
 ```
 
 Save the index for future use:
 ```python
-# Save
+# Save to disk
 index.save(filepath)
 
 # Load from a saved file
 new_index = Index.from_file(filepath)
 ```
 
-## Comparison with Approximate Nearest Neighbor Search
-Based on a [quick benchmark](https://github.com/aismlv/minivan/blob/main/experiments/benchmark/README.md), you might not require an ANN and go with a simpler approach if any of the below apply:
+## matmul vs ANN
 
-- Your document set isn't in the multiple millions and you don't have ultra-low latency requirements (to accommodate a heavy reranker, for example)
-- You're in the experimentation phase and want to iterate quickly on the index
+Due to numpy's use of BLAS and other optimisations, brute-force search is performant enough for a large set of real-world applications. There are a bunch of cases when you might not need an approximate nearest neighbour library and can go with a simpler approach:
+
+- Your document set is not in the multiple millions
+- You're in the experimentation phase and want to iterate on the index rapidly with fast build times
 - Your application requires the best accuracy
-- You don't want to fine-tune any hyperparameters (which can affect [latency/recall trade-off](https://github.com/erikbern/ann-benchmarks) quite a lot)
+- You want to avoid the need to finetune hyperparameters (which can affect [performance and latency](https://github.com/erikbern/ann-benchmarks) quite a lot)
+
+See a [quick benchmark](https://github.com/aismlv/minivan/blob/main/experiments/benchmark/README.md) for an illustration.
```

### Comparing `minivan_tools-0.1.4/minivan/index.py` & `minivan_tools-0.1.5/minivan/index.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 import logging
 from typing import List, Tuple, Union
 
 import numpy as np
 
-DOT_PRODUCT = "dot_product"
-COSINE = "cosine"
-
-
-def normalize(embedding: np.ndarray) -> np.ndarray:
-    return embedding / np.linalg.norm(embedding, axis=-1, keepdims=True)
+from .metrics import COSINE, DOT_PRODUCT, get_metric, normalize
 
 
 class Index:
     def __init__(self, dim: int, metric: str = DOT_PRODUCT, dtype: str = "float32") -> None:
         self.dim = dim
         self.metric = metric
         self.dtype = np.dtype(dtype)
         self.embeddings = np.empty((0, dim), dtype=dtype)
         self.index_map: List[int] = []
 
-        if self.metric == DOT_PRODUCT:
-            self.calc_similarities = lambda query_embedding: self.embeddings @ query_embedding
-        elif self.metric == COSINE:
-            self.calc_similarities = lambda query_embedding: self.embeddings @ normalize(query_embedding)
-        else:
-            raise ValueError(f"Invalid metric: {metric}. Supported metrics are '{DOT_PRODUCT}' and '{COSINE}'.")
+        self.calc_similarities = get_metric(metric)
+
+    def add_items(self, indices: Union[List[int], np.ndarray], embeddings: Union[List[np.ndarray], np.ndarray]) -> None:
+        if isinstance(indices, np.ndarray):
+            if indices.squeeze().ndim != 1:
+                raise ValueError(f"Indices must be a list or a 1D array. Got array with dimensions: {indices.ndim}")
+            indices = indices.squeeze().tolist()
+
+        if type(indices) != list:
+            raise TypeError(f"Indices must be a list or a 1D array. Got: {type(indices)}")
 
-    def add_items(self, indices: List[int], embeddings: Union[List[np.ndarray], np.ndarray]) -> None:
         for index in indices:
+            if type(index) != int:
+                raise TypeError(f"Index must be an integer. Got: {type(index)}")
             if index in self.index_map:
-                raise KeyError(f"Index {index} already exists.")
+                raise KeyError(f"Index {index} already exists")
 
         if isinstance(embeddings, list):
-            embeddings = [embedding.reshape(1, -1) for embedding in embeddings]
+            result = []
             for embedding in embeddings:
-                if embedding.shape[1] != self.dim:
+                if embedding.squeeze().ndim != 1:
                     raise ValueError(
-                        f"Embedding has invalid dimension: {embedding.shape[1]}. Expected dimension: {self.dim}."
+                        f"Embeddings must be a list of 1D arrays. Got array with dimensions: {embedding.ndim}"
                     )
-            embeddings = np.vstack(embeddings)
+                result.append(embedding.reshape(1, -1))
+            embeddings = np.vstack(result)
 
-        elif isinstance(embeddings, np.ndarray):
-            if embeddings.shape != (len(indices), self.dim):
-                raise ValueError(
-                    f"Embedding has invalid shape: {embeddings.shape}. Expected shape: {(len(indices), self.dim)}."
-                )
+        if not isinstance(embeddings, np.ndarray):
+            raise TypeError(f"Embeddings must be a list or a numpy array. Got: {type(embeddings)}")
+
+        expected_shape = (len(indices), self.dim)
+        if embeddings.shape != expected_shape:
+            raise ValueError(f"Embeddings have invalid shape: {embeddings.shape}. Expected shape: {expected_shape}")
+
+        embeddings = embeddings.astype(self.dtype)
 
         if self.metric == COSINE:
             embeddings = normalize(embeddings)
 
-        self.embeddings = np.append(self.embeddings, embeddings.astype(self.dtype), axis=0)
+        self.embeddings = np.append(self.embeddings, embeddings, axis=0)
         self.index_map.extend(indices)
 
     def delete_items(self, indices: List[int]) -> None:
-        for index in indices:
-            if index not in self.index_map:
-                raise KeyError(f"Index {index} not found.")
+        self._validate_indices_exist(indices)
 
         rows_to_delete = [self.index_map.index(index) for index in indices]
         self.embeddings = np.delete(self.embeddings, rows_to_delete, axis=0)
 
         for index in rows_to_delete:
             del self.index_map[index]
 
@@ -73,23 +75,23 @@
             dtype=str(self.dtype),
         )
 
     def load(self, filepath: str) -> None:
         with np.load(filepath) as data:
             if data["metric"].item() != self.metric:
                 raise ValueError(
-                    f"Metric mismatch. Index metric: {self.metric}. Loaded index metric: {data['metric'].item()}."
+                    f"Metric mismatch. Index metric: {self.metric}. Loaded index metric: {data['metric'].item()}"
                 )
             if data["dim"].item() != self.dim:
                 raise ValueError(
-                    f"Dimension mismatch. Index dimension: {self.dim}. Loaded index dimension: {data['dim'].item()}."
+                    f"Dimension mismatch. Index dimension: {self.dim}. Loaded index dimension: {data['dim'].item()}"
                 )
             if data["dtype"].item() != self.dtype:
                 raise ValueError(
-                    f"Dtype mismatch. Index dtype: {self.dtype}. Loaded index dtype: {data['dtype'].item()}."
+                    f"Dtype mismatch. Index dtype: {self.dtype}. Loaded index dtype: {data['dtype'].item()}"
                 )
             self.embeddings = data["embeddings"]
             self.index_map = data["index_map"].tolist()
 
     @classmethod
     def from_file(cls, filepath: str) -> "Index":
         with np.load(filepath) as data:
@@ -97,35 +99,54 @@
             dim = data["dim"].item()
             dtype = data["dtype"].item()
         index = cls(dim, metric, dtype)
         index.load(filepath)
         return index
 
     def query(self, query_embedding: np.ndarray, k: int = 1) -> List[Tuple[int, float]]:
+        if type(k) != int or k < 1:
+            raise ValueError(f"k must be a positive integer: {k}")
+        if k > len(self):
+            raise ValueError(f"k cannot be greater than the number of items in the index: {len(self)}")
+        if self.dim not in query_embedding.shape:
+            raise ValueError(
+                f"Query embedding has invalid dimension: {query_embedding.shape}"
+                f"Expected embedding dimension: {self.dim}"
+            )
+
         query_embedding = query_embedding.astype(self.dtype)
-        similarities = self.calc_similarities(query_embedding)
+        similarities = self.calc_similarities(query_embedding, self.embeddings)
         top_k_indices = np.argpartition(similarities, -k)[-k:]
         top_k_indices_sorted = top_k_indices[np.argsort(-similarities[top_k_indices])]
         top_k_values = similarities[top_k_indices_sorted]
 
         return [(self.index_map[i], similarity) for i, similarity in zip(top_k_indices_sorted, top_k_values)]
 
+    def query_item(self, index: int, k: int = 1) -> List[Tuple[int, float]]:
+        self._validate_indices_exist([index])
+        query_embedding = self.get_items([index])
+        result = self.query(query_embedding.squeeze(), k)
+        return [item for item in result if item[0] != index]
+
     def __len__(self) -> int:
         return len(self.index_map)
 
     def __repr__(self) -> str:
         return f"Index(num_items={len(self)}, dim={self.dim}, metric={self.metric}, dtype={self.dtype})"
 
     def get_items(self, indices: List[int]) -> np.ndarray:
-        for index in indices:
-            if index not in self.index_map:
-                raise KeyError(f"Index {index} not found.")
+        self._validate_indices_exist(indices)
 
         if self.metric == COSINE:
             logging.warning(
                 (
                     f"The vector retrieved from the index using the {COSINE} metric is not equivalent "
                     "to the initially added embeddings as it has been normalized to have a unit length"
                 )
             )
 
         return self.embeddings[[self.index_map.index(index) for index in indices]]
+
+    def _validate_indices_exist(self, indices: List[int]) -> None:
+        for index in indices:
+            if index not in self.index_map:
+                raise KeyError(f"Index {index} not found")
```

### Comparing `minivan_tools-0.1.4/pyproject.toml` & `minivan_tools-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "minivan-tools"
-version = "0.1.4"
+version = "0.1.5"
 description = "Exact nearest neighbor search library for those times when \"approximate\" just won't cut it (or is simply overkill)"
 authors = ["aismlv <adilzhan.ismailov@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/aismlv/minivan"
 keywords = ["nearest neighbor search"]
 packages = [
     { include = "minivan"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-numpy = "^1.24.2"
+numpy = "^1.24.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
-pre-commit = "^3.2.2"
+pre-commit = "^3.3.0"
 pytest-cov = "^4.0.0"
 isort = "^5.12.0"
 
 [tool.poetry.group.benchmark]
 optional = true
 
 [tool.poetry.group.benchmark.dependencies]
```

### Comparing `minivan_tools-0.1.4/PKG-INFO` & `minivan_tools-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 Metadata-Version: 2.1
 Name: minivan-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Exact nearest neighbor search library for those times when "approximate" just won't cut it (or is simply overkill)
 Home-page: https://github.com/aismlv/minivan
 License: Apache-2.0
 Keywords: nearest neighbor search
 Author: aismlv
 Author-email: adilzhan.ismailov@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Project-URL: Repository, https://github.com/aismlv/minivan
 Description-Content-Type: text/markdown
 
 # minivan
 
 ![Tests](https://github.com/aismlv/minivan/actions/workflows/test_and_lint.yml/badge.svg)
 [![codecov](https://codecov.io/gh/aismlv/minivan/branch/main/graph/badge.svg?token=5J503UR8O7)](https://codecov.io/gh/aismlv/minivan)
-[![PyPI version](https://badge.fury.io/py/minivan.svg?)](https://pypi.org/project/minivan/)
+[![PyPI version](https://badge.fury.io/py/minivan-tools.svg?)](https://pypi.org/project/minivan-tools/)
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 `minivan` is an exact nearest neighbor search Python library for those times when "approximate" just won't cut it (or is simply overkill).
 
 ## Installation
 
 Install `minivan` using `pip`:
 
 ```bash
 pip install minivan-tools
 ```
 
 ## Usage
-Here is an example of how to use `minivan`:
-
 Create new index:
 ```python
 from minivan import Index
 import numpy as np
 
-# Create an index with 128-dimensional embeddings and dot product metric. Cosine similarity is also supported
+# Create an index with 128-dimensional embeddings and dot product metric
 index = Index(dim=128, metric="dot_product")
 
 # Add embeddings to the index
-embedding1 = np.random.rand(128)
-embedding2 = np.random.rand(128)
-embedding3 = np.random.rand(128)
-
-index.add_items([1, 2, 3], [embedding1, embedding2, embedding3])
+embeddings = [np.random.rand(128) for _ in range(3)]
+index.add_items([1, 2, 3], embeddings)
 
 # Delete embeddings from the index
 index.delete_items([3])
 ```
 
-Search for the nearest neighbors:
+Query the index for the nearest neighbor:
 ```python
-# Query the index for the nearest neighbor of a given embedding
 query_embedding = np.random.rand(128)
 result = index.query(query_embedding, k=1)
 
 print(result)  # Returns [(index, similarity)] of the nearest neighbor
 ```
 
 Save the index for future use:
 ```python
-# Save
+# Save to disk
 index.save(filepath)
 
 # Load from a saved file
 new_index = Index.from_file(filepath)
 ```
 
-## Comparison with Approximate Nearest Neighbor Search
-Based on a [quick benchmark](https://github.com/aismlv/minivan/blob/main/experiments/benchmark/README.md), you might not require an ANN and go with a simpler approach if any of the below apply:
+## matmul vs ANN
 
-- Your document set isn't in the multiple millions and you don't have ultra-low latency requirements (to accommodate a heavy reranker, for example)
-- You're in the experimentation phase and want to iterate quickly on the index
+Due to numpy's use of BLAS and other optimisations, brute-force search is performant enough for a large set of real-world applications. There are a bunch of cases when you might not need an approximate nearest neighbour library and can go with a simpler approach:
+
+- Your document set is not in the multiple millions
+- You're in the experimentation phase and want to iterate on the index rapidly with fast build times
 - Your application requires the best accuracy
-- You don't want to fine-tune any hyperparameters (which can affect [latency/recall trade-off](https://github.com/erikbern/ann-benchmarks) quite a lot)
+- You want to avoid the need to finetune hyperparameters (which can affect [performance and latency](https://github.com/erikbern/ann-benchmarks) quite a lot)
+
+See a [quick benchmark](https://github.com/aismlv/minivan/blob/main/experiments/benchmark/README.md) for an illustration.
```


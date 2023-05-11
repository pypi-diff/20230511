# Comparing `tmp/pyqtorch-0.2.1.tar.gz` & `tmp/pyqtorch-0.2.2.tar.gz`

## Comparing `pyqtorch-0.2.1.tar` & `pyqtorch-0.2.2.tar`

### file list

```diff
@@ -1,76 +1,46 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/README.md
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/mkdocs.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/publish.sh
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/setup.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/21836652c37a637f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/2602555962d0fc4c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/30645ad5f1f1dcfe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/317d2f17a1075099
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/41d845d0f90a6417
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/617ac8c861e982f1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/68cc7f39a1692629
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/71de32d0dc4ef210
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/7ab8961a5fd3e34a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/7b50e93d7b401d37
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/7e9bc91eb0e4bec7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/8446b77184378e13
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/8c22cf14dc3075f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/8f831c3208d022cd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/963472f7f566f99d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/9b70b475da072d2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/a3b4cbbb65fe8420
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/aaa2c54c6449792b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/af9c8e117f709f43
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/c73abac16d830acc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/ce5cb2c96a07a572
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/ce5dade58b1ccd69
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/d49ef2d71d47c091
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/df86f5c8bc05afc4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/e69f22aa2552f985
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/f6f6f60064e20f97
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.ruff_cache/content/f78c2e380fc669b7
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/QAOA.ipynb
--rw-r--r--   0        0        0   154586 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/fit_function.ipynb
--rw-r--r--   0        0        0    74094 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/getting_started.ipynb
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/index.ipynb
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/embedding.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/tests/test_converters.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/tests/test_modules.py
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/tests/test_operations.py
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/LICENSE
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pyqtorch-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/README.md
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/mkdocs.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/setup.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/.github/workflows/run-tests-and-mypy.yml
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/QAOA.ipynb
+-rw-r--r--   0        0        0   154586 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/fit_function.ipynb
+-rw-r--r--   0        0        0    74094 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/getting_started.ipynb
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/index.ipynb
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/tests/test_converters.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/tests/test_modules.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pyqtorch-0.2.2/PKG-INFO
```

### Comparing `pyqtorch-0.2.1/.pre-commit-config.yaml` & `pyqtorch-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/mkdocs.yml` & `pyqtorch-0.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.2.2/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/QAOA.ipynb` & `pyqtorch-0.2.2/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/fit_function.ipynb` & `pyqtorch-0.2.2/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/getting_started.ipynb` & `pyqtorch-0.2.2/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/index.ipynb` & `pyqtorch-0.2.2/docs/index.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.2.2/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/deprecated/bench.py` & `pyqtorch-0.2.2/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.2.2/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.2.2/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.2.2/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/__init__.py` & `pyqtorch-0.2.2/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/ansatz.py` & `pyqtorch-0.2.2/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/embedding.py` & `pyqtorch-0.2.2/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/matrices.py` & `pyqtorch-0.2.2/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/matrices_sparse.py` & `pyqtorch-0.2.2/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/converters/store_ops.py` & `pyqtorch-0.2.2/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.2.2/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/core/__init__.py` & `pyqtorch-0.2.2/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/core/batched_operation.py` & `pyqtorch-0.2.2/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/core/circuit.py` & `pyqtorch-0.2.2/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/core/measurement.py` & `pyqtorch-0.2.2/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/core/operation.py` & `pyqtorch-0.2.2/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/core/utils.py` & `pyqtorch-0.2.2/pyqtorch/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/modules/circuit.py` & `pyqtorch-0.2.2/tests/test_module_hamevo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,74 @@
 from __future__ import annotations
 
-from typing import Any
+import random
+from math import isclose
 
+import numpy as np
+import pytest
 import torch
-from torch.nn import Module, ModuleList, Parameter, init
 
-from pyqtorch.modules.primitive import CNOT
+import pyqtorch.modules as pyq
 
-PI = 2.0 * torch.asin(torch.Tensor([1.0]).double()).item()
+random.seed(0)
+np.random.seed(0)
+torch.manual_seed(0)
+torch.use_deterministic_algorithms(not torch.cuda.is_available())
+
+
+pi = torch.tensor(torch.pi, dtype=torch.cdouble)
+
+
+def overlap(state1: torch.Tensor, state2: torch.Tensor) -> float | list[float]:
+    N = len(state1.shape) - 1
+    state1_T = torch.transpose(state1, N, 0)
+    overlap = torch.tensordot(state1_T, state2, dims=N)
+    res: list[float] = list(map(float, torch.abs(overlap**2).flatten()))
+    if len(res) == 1:
+        return res[0]
+    else:
+        return res
+
+
+def Hamiltonian(batch_size: int = 1) -> torch.Tensor:
+    sigmaz = torch.diag(torch.tensor([1.0, -1.0], dtype=torch.cdouble))
+    Hbase = torch.kron(sigmaz, sigmaz)
+    H = torch.kron(Hbase, Hbase)
+    if batch_size == 1:
+        return H
+    else:
+        return torch.stack((H, H.conj()), dim=2)
+
+
+@pytest.mark.parametrize(
+    "ham_evo",
+    [pyq.HamEvo, pyq.HamEvoEig],
+)
+def test_hamevo_modules_single(ham_evo: torch.nn.Module) -> None:
+    n_qubits = 4
+    H = Hamiltonian(1)
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+    hamevo = ham_evo(H, t_evo, range(n_qubits), n_qubits)
+    psi = pyq.uniform_state(n_qubits)
+    psi_star = hamevo.forward(psi)
+    result = overlap(psi_star, psi)
+    result = result if isinstance(result, float) else result[0]
+    assert isclose(result, 0.5)
+
+
+@pytest.mark.parametrize(
+    "ham_evo",
+    [pyq.HamEvo, pyq.HamEvoEig],
+)
+def test_hamevo_modules_batch(ham_evo: torch.nn.Module) -> None:
+    n_qubits = 4
+    batch_size = 2
+    H = Hamiltonian(batch_size)
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+
+    hamevo = ham_evo(H, t_evo, range(n_qubits), n_qubits)
+    psi = pyq.uniform_state(n_qubits, batch_size)
+    psi_star = hamevo.forward(psi)
+    result = overlap(psi_star, psi)
+    print(result)
 
-
-def zero_state(
-    n_qubits: int,
-    batch_size: int = 1,
-    device: str | torch.device = "cpu",
-    dtype: torch.dtype = torch.cdouble,
-) -> torch.Tensor:
-    state = torch.zeros((2**n_qubits, batch_size), dtype=dtype, device=device)
-    state[0] = 1
-    state = state.reshape([2] * n_qubits + [batch_size])
-    return state
-
-
-def uniform_state(
-    n_qubits: int,
-    batch_size: int = 1,
-    device: str | torch.device = "cpu",
-    dtype: torch.dtype = torch.cdouble,
-) -> torch.Tensor:
-    state = torch.ones((2**n_qubits, batch_size), dtype=dtype, device=device)
-    state = state / torch.sqrt(torch.tensor(2**n_qubits))
-    state = state.reshape([2] * n_qubits + [batch_size])
-    return state
-
-
-class QuantumCircuit(Module):
-    def __init__(self, n_qubits: int, operations: list):
-        super().__init__()
-        self.n_qubits = n_qubits
-        self.operations = torch.nn.ModuleList(operations)
-
-    def forward(self, state: torch.Tensor, thetas: torch.Tensor = None) -> torch.Tensor:
-        for op in self.operations:
-            state = op(state, thetas)
-        return state
-
-    @property
-    def _device(self) -> torch.device:
-        devices = set(p.device for p in self.parameters())
-        if len(devices) == 0:
-            return torch.device("cpu")
-        elif len(devices) == 1:
-            return devices.pop()
-        else:
-            raise ValueError("only one device supported.")
-
-    def init_state(self, batch_size: int) -> torch.Tensor:
-        return zero_state(self.n_qubits, batch_size, device=self._device)
-
-
-def FeaturemapLayer(n_qubits: int, Op: Any) -> QuantumCircuit:
-    operations = [Op([i], n_qubits) for i in range(n_qubits)]
-    return QuantumCircuit(n_qubits, operations)
-
-
-class VariationalLayer(QuantumCircuit):
-    def __init__(self, n_qubits: int, Op: Any):
-        operations = ModuleList([Op([i], n_qubits) for i in range(n_qubits)])
-        super().__init__(n_qubits, operations)
-
-        self.thetas = Parameter(torch.empty(n_qubits, Op.n_params))
-        self.reset_parameters()
-
-    def reset_parameters(self) -> None:
-        init.uniform_(self.thetas, -2 * PI, 2 * PI)
-
-    def forward(self, state: torch.Tensor, _: torch.Tensor = None) -> torch.Tensor:
-        for (op, t) in zip(self.operations, self.thetas):
-            state = op(state, t)
-        return state
-
-
-class EntanglingLayer(QuantumCircuit):
-    def __init__(self, n_qubits: int):
-        operations = ModuleList(
-            [CNOT([i % n_qubits, (i + 1) % n_qubits], n_qubits) for i in range(n_qubits)]
-        )
-        super().__init__(n_qubits, operations)
+    assert map(isclose, zip(result, [0.5, 0.5]))  # type: ignore [arg-type]
```

### Comparing `pyqtorch-0.2.1/pyqtorch/modules/hamevo.py` & `pyqtorch-0.2.2/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/modules/parametric.py` & `pyqtorch-0.2.2/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyqtorch/modules/primitive.py` & `pyqtorch-0.2.2/pyqtorch/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/tests/conftest.py` & `pyqtorch-0.2.2/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pyqtorch import QuantumCircuit, batchedRY, measurement
 from pyqtorch.core.measurement import total_magnetization
 from pyqtorch.core.operation import CNOT, RX, RY, RZ, H, X, Y, Z
 
 random.seed(42)
 np.random.seed(42)
 torch.manual_seed(42)
-torch.use_deterministic_algorithms(True)
+torch.use_deterministic_algorithms(not torch.cuda.is_available())
 
 
 class TestFM(QuantumCircuit):
     def __init__(self, n_qubits: int = 4):
         super().__init__(n_qubits)
         self.qubits = range(n_qubits)
```

### Comparing `pyqtorch-0.2.1/tests/test_batched_operations.py` & `pyqtorch-0.2.2/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/tests/test_converters.py` & `pyqtorch-0.2.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/tests/test_modules.py` & `pyqtorch-0.2.2/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/tests/test_operations.py` & `pyqtorch-0.2.2/tests/test_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import torch
 from torch.autograd import grad
 
 random.seed(0)
 np.random.seed(0)
 torch.manual_seed(0)
-torch.use_deterministic_algorithms(True)
+torch.use_deterministic_algorithms(not torch.cuda.is_available())
 
 from conftest import TestBatchedFM, TestFM, TestNetwork  # noqa: E402
 
 from pyqtorch.ansatz import AlternateLayerAnsatz  # noqa: E402
 from pyqtorch.core import operation  # noqa: E402
 
 state_0 = torch.tensor([[1, 0]], dtype=torch.cdouble)
```

### Comparing `pyqtorch-0.2.1/tests/test_operations_hamevo.py` & `pyqtorch-0.2.2/tests/test_operations_hamevo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pyqtorch.core.circuit import QuantumCircuit
 from pyqtorch.core.operation import hamiltonian_evolution, hamiltonian_evolution_eig
 from pyqtorch.matrices import generate_ising_from_graph
 
 random.seed(0)
 np.random.seed(0)
 torch.manual_seed(0)
-torch.use_deterministic_algorithms(True)
+torch.use_deterministic_algorithms(not torch.cuda.is_available())
 
 state_00 = torch.tensor([[1, 0], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
 state_10 = torch.tensor([[0, 1], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
 state_01 = torch.tensor([[0, 0], [1, 0]], dtype=torch.cdouble).unsqueeze(2)
 state_11 = torch.tensor([[0, 0], [0, 1]], dtype=torch.cdouble).unsqueeze(2)
 
 pi = torch.tensor(torch.pi, dtype=torch.cdouble)
```

### Comparing `pyqtorch-0.2.1/LICENSE` & `pyqtorch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.1/pyproject.toml` & `pyqtorch-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8.1,<3.11"
 license = {text = "Proprietary"}
-version = "0.2.1"
+version = "0.2.2"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.2.1/PKG-INFO` & `pyqtorch-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```


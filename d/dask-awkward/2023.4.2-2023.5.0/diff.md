# Comparing `tmp/dask_awkward-2023.4.2.tar.gz` & `tmp/dask_awkward-2023.5.0.tar.gz`

## Comparing `dask_awkward-2023.4.2.tar` & `dask_awkward-2023.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0    61405 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    28896 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.4.2/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0    61467 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/LICENSE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/PKG-INFO
```

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.5.0/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/typing.py` & `dask_awkward-2023.5.0/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/utils.py` & `dask_awkward-2023.5.0/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.5.0/src/dask_awkward/layers/layers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/core.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1733,15 +1733,18 @@
 
     """
     return tuple(map(meta_or_identity, objects))
 
 
 def length_zero_array_or_identity(obj: Any) -> Any:
     if is_awkward_collection(obj):
-        return obj._meta.layout.form.length_zero_array(behavior=obj.behavior)
+        return ak.Array(
+            obj._meta.layout.form.length_zero_array(highlevel=False),
+            behavior=obj.behavior,
+        )
     return obj
 
 
 def to_length_zero_arrays(objects: Sequence[Any]) -> tuple[Any, ...]:
     return tuple(map(length_zero_array_or_identity, objects))
```

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from dask_awkward.lib.core import (
     Array,
     compatible_partitions,
     map_partitions,
     new_known_scalar,
     total_reduction_to_scalar,
-    typetracer_from_form,
 )
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
     IncompatiblePartitions,
     borrow_docstring,
 )
 
@@ -679,26 +678,14 @@
 
 class _SingletonsFn:
     def __init__(self, axis, **kwargs):
         self.axis = axis
         self.kwargs = kwargs
 
     def __call__(self, array):
-        # TODO: remove this length-zero calculation once https://github.com/scikit-hep/awkward/issues/2123 is addressed
-        if ak.backend(array) == "typetracer":
-            array.layout._touch_data(recursive=False)
-            zl_out = ak.singletons(
-                array.layout.form.length_zero_array(behavior=array.behavior),
-                axis=self.axis,
-                **self.kwargs,
-            )
-            return ak.Array(
-                zl_out.layout.to_typetracer(forget_length=True),
-                behavior=zl_out.behavior,
-            )
         return ak.singletons(array, axis=self.axis, **self.kwargs)
 
 
 @borrow_docstring(ak.singletons)
 def singletons(array, axis=0, highlevel=True, behavior=None):
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
@@ -765,33 +752,21 @@
     warnings.warn(
         f"""Please ensure that {counts}
         is partitionwise-compatible with {array}
         (e.g. counts comes from a dak.num(array, axis=1)),
         otherwise this unflatten operation will fail when computed!"""
     )
 
-    #  TODO: remove after fixing issue in awkward
-    meta = typetracer_from_form(
-        ak.unflatten(
-            array._meta.layout.form.length_zero_array(behavior=array.behavior),
-            counts._meta.layout.form.length_zero_array(behavior=counts.behavior),
-            axis=axis,
-            highlevel=highlevel,
-            behavior=behavior,
-        ).layout.form
-    )
-
     return map_partitions(
         ak.unflatten,
         array,
         counts,
         axis=axis,
         highlevel=highlevel,
         behavior=behavior,
-        meta=meta,
         label="unflatten",
     )
 
 
 @borrow_docstring(ak.unzip)
 def unzip(
     array: Array, highlevel: bool = True, behavior: dict | None = None
@@ -935,33 +910,19 @@
     name: str,
     highlevel: bool = True,
     behavior: dict | None = None,
 ) -> Array:
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
 
-    #  TODO: remove once fixed in awkward
-    meta = ak.Array(
-        typetracer_from_form(
-            ak.with_name(
-                array._meta.layout.form.length_zero_array(),
-                name,
-                highlevel=highlevel,
-                behavior=behavior,
-            ).layout.form
-        ),
-        behavior=behavior if behavior is not None else array._meta.behavior,
-    )
-
     return map_partitions(
         _WithNameFn(name=name, behavior=behavior),
         array,
         label="with-name",
         output_divisions=1,
-        meta=meta,
     )
 
 
 class _WithParameterFn:
     def __init__(self, parameter, value, behavior):
         self.parameter = parameter
         self.value = value
```

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.5.0/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/.gitignore` & `dask_awkward-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/LICENSE` & `dask_awkward-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/README.md` & `dask_awkward-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.4.2/pyproject.toml` & `dask_awkward-2023.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-  "awkward >=2.1.3",
+  "awkward >=2.2.0",
   "dask >=2023.04.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
```

### Comparing `dask_awkward-2023.4.2/PKG-INFO` & `dask_awkward-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.4.2
+Version: 2023.5.0
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: awkward>=2.1.3
+Requires-Dist: awkward>=2.2.0
 Requires-Dist: dask>=2023.04.0
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: pyarrow; extra == 'complete'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
 Requires-Dist: pytest>=6.0; extra == 'complete'
 Requires-Dist: requests>=2.27.1; extra == 'complete'
```


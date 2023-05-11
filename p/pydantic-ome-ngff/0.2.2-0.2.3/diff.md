# Comparing `tmp/pydantic_ome_ngff-0.2.2.tar.gz` & `tmp/pydantic_ome_ngff-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_ome_ngff-0.2.2.tar", max compression
+gzip compressed data, was "pydantic_ome_ngff-0.2.3.tar", max compression
```

## Comparing `pydantic_ome_ngff-0.2.2.tar` & `pydantic_ome_ngff-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1466 2023-02-14 18:55:46.264580 pydantic_ome_ngff-0.2.2/LICENSE
--rw-r--r--   0        0        0     1928 2023-02-27 17:33:34.485461 pydantic_ome_ngff-0.2.2/README.md
--rw-r--r--   0        0        0     1008 2023-03-22 18:48:23.762905 pydantic_ome_ngff-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       85 2023-03-22 18:16:41.323863 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/__init__.py
--rw-r--r--   0        0        0      446 2023-03-22 18:16:41.327918 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/base.py
--rw-r--r--   0        0        0      360 2023-03-08 00:10:20.528092 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/__init__.py
--rw-r--r--   0        0        0     2402 2023-03-20 21:12:06.229789 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/axes.py
--rw-r--r--   0        0        0       20 2023-03-08 00:10:20.167824 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/base.py
--rw-r--r--   0        0        0     1661 2023-03-20 21:12:06.229864 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/coordinateTransformations.py
--rw-r--r--   0        0        0      470 2023-03-07 21:33:31.538364 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/imageLabel.py
--rw-r--r--   0        0        0     8690 2023-03-20 21:12:39.558265 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/multiscales.py
--rw-r--r--   0        0        0      441 2023-03-07 21:17:42.823412 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/plate.py
--rw-r--r--   0        0        0      432 2023-03-07 21:34:04.945766 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/well.py
--rw-r--r--   0        0        0        0 2023-03-22 18:28:17.442462 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/py.typed
--rw-r--r--   0        0        0     1690 2023-03-20 21:12:06.229959 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/tree.py
--rw-r--r--   0        0        0      441 2023-03-20 21:12:39.874223 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/utils.py
--rw-r--r--   0        0        0      430 2023-03-08 00:10:20.188881 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/__init__.py
--rw-r--r--   0        0        0     3851 2023-03-20 21:12:06.230046 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/axes.py
--rw-r--r--   0        0        0       16 2023-03-08 00:10:20.185875 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/base.py
--rw-r--r--   0        0        0     2307 2023-03-20 21:12:06.230085 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/coordinateTransformations.py
--rw-r--r--   0        0        0     2136 2023-03-20 21:12:39.490060 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/imageLabel.py
--rw-r--r--   0        0        0     8694 2023-03-20 21:12:39.573818 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/multiscales.py
--rw-r--r--   0        0        0      920 2023-03-07 23:14:47.975021 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/plate.py
--rw-r--r--   0        0        0      560 2023-03-07 21:34:45.608891 pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/well.py
--rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 pydantic_ome_ngff-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1466 2023-02-14 18:55:46.264580 pydantic_ome_ngff-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1928 2023-02-27 17:33:34.485461 pydantic_ome_ngff-0.2.3/README.md
+-rw-r--r--   0        0        0     1008 2023-05-11 13:42:31.501598 pydantic_ome_ngff-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-03-22 18:16:41.323863 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/__init__.py
+-rw-r--r--   0        0        0      446 2023-03-22 18:16:41.327918 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/base.py
+-rw-r--r--   0        0        0      360 2023-03-08 00:10:20.528092 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/__init__.py
+-rw-r--r--   0        0        0     2402 2023-05-11 13:42:02.972582 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/axes.py
+-rw-r--r--   0        0        0       20 2023-03-08 00:10:20.167824 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/base.py
+-rw-r--r--   0        0        0     1661 2023-05-11 13:42:02.972870 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/coordinateTransformations.py
+-rw-r--r--   0        0        0      470 2023-05-11 13:42:02.973348 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/imageLabel.py
+-rw-r--r--   0        0        0     8749 2023-05-11 13:42:05.518320 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/multiscales.py
+-rw-r--r--   0        0        0      441 2023-05-11 13:42:02.974346 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/plate.py
+-rw-r--r--   0        0        0      432 2023-05-11 13:42:02.974828 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/well.py
+-rw-r--r--   0        0        0        0 2023-03-22 18:28:17.442462 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/py.typed
+-rw-r--r--   0        0        0     1690 2023-05-11 13:42:02.975172 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/tree.py
+-rw-r--r--   0        0        0      441 2023-03-20 21:12:39.874223 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/utils.py
+-rw-r--r--   0        0        0      430 2023-03-08 00:10:20.188881 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/__init__.py
+-rw-r--r--   0        0        0     3851 2023-05-11 13:42:02.975993 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/axes.py
+-rw-r--r--   0        0        0       16 2023-03-08 00:10:20.185875 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/base.py
+-rw-r--r--   0        0        0     2307 2023-05-11 13:42:02.976547 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/coordinateTransformations.py
+-rw-r--r--   0        0        0     2136 2023-05-11 13:42:02.977224 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/imageLabel.py
+-rw-r--r--   0        0        0     8753 2023-05-11 13:42:05.519709 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/multiscales.py
+-rw-r--r--   0        0        0      920 2023-05-11 13:42:02.978134 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/plate.py
+-rw-r--r--   0        0        0      560 2023-05-11 13:42:02.978576 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/well.py
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 pydantic_ome_ngff-0.2.3/PKG-INFO
```

### Comparing `pydantic_ome_ngff-0.2.2/LICENSE` & `pydantic_ome_ngff-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/README.md` & `pydantic_ome_ngff-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/pyproject.toml` & `pydantic_ome_ngff-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-ome-ngff"
-version = "0.2.2"
+version = "0.2.3"
 description = "Pydantic models for the OME-NGFF"
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_ome_ngff", from="src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/axes.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/axes.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/coordinateTransformations.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/coordinateTransformations.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/latest/multiscales.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/multiscales.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from collections import Counter
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 import warnings
 
-from pydantic import root_validator, validator, Field
+from pydantic import conlist, root_validator, validator, Field
 from pydantic_ome_ngff.base import StrictBase, StrictVersionedBase
 from pydantic_ome_ngff.latest.base import version
 from pydantic_ome_ngff.latest import coordinateTransformations as ctx
 from pydantic_ome_ngff.tree import Array, Attrs, Group
 from pydantic_ome_ngff.utils import duplicates
 from pydantic_ome_ngff.v04.axes import AxisType
 from pydantic_ome_ngff.latest.axes import Axis
 
 
 class MultiscaleDataset(StrictBase):
     path: str
-    coordinateTransformations: List[
-        Union[ctx.ScaleTransform, ctx.TranslationTransform]
-    ] = Field(..., min_items=1, max_items=2)
+    coordinateTransformations: conlist(
+        Union[ctx.ScaleTransform, ctx.TranslationTransform], min_items=1, max_items=2
+    )
 
     @validator("coordinateTransformations")
     def check_transforms_dimensionality(
         cls,
         transforms: List[
             Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]
         ],
@@ -46,22 +46,22 @@
         if (tform := transforms[0].type) != "scale":
             raise ValueError(
                 f"""
             The first element of coordinateTransformations must be a scale transform.
             Got {tform} instead.
             """
             )
-
-        if (tform := transforms[1].type) != "translation":
-            raise ValueError(
-                f"""
-            The second element of coordinateTransformations must be a translation 
-            transform. got {tform} instead.
-            """
-            )
+        if len(transforms) == 2:
+            if (tform := transforms[1].type) != "translation":
+                raise ValueError(
+                    f"""
+                The second element of coordinateTransformations must be a translation 
+                transform. got {tform} instead.
+                """
+                )
         return transforms
 
 
 class Multiscale(StrictVersionedBase):
     """
     Multiscale image metadata.
     See https://ngff.openmicroscopy.org/latest/#multiscale-md
```

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/tree.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/tree.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/axes.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/axes.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/coordinateTransformations.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/coordinateTransformations.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/imageLabel.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/imageLabel.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/multiscales.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/multiscales.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from collections import Counter
 import warnings
 from typing import Any, Dict, List, Optional, Union, Tuple, cast
 
-from pydantic import Field, root_validator, validator
+from pydantic import Field, conlist, root_validator, validator
 
 from pydantic_ome_ngff.utils import duplicates
 from pydantic_ome_ngff.base import StrictBase, StrictVersionedBase
 from pydantic_ome_ngff.tree import Group, Attrs, Array
 from pydantic_ome_ngff.v04.base import version
 from pydantic_ome_ngff.v04.axes import Axis, AxisType
 import pydantic_ome_ngff.v04.coordinateTransformations as ctx
 
 
 class MultiscaleDataset(StrictBase):
     path: str
-    coordinateTransformations: List[
-        Union[ctx.ScaleTransform, ctx.TranslationTransform]
-    ] = Field(..., min_items=1, max_items=2)
+    coordinateTransformations: conlist(
+        Union[ctx.ScaleTransform, ctx.TranslationTransform], min_items=1, max_items=2
+    )
 
     @validator("coordinateTransformations")
     def check_transforms_dimensionality(
         cls,
         transforms: List[
             Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]
         ],
@@ -49,22 +49,22 @@
         if (tform := transforms[0].type) != "scale":
             raise ValueError(
                 f"""
             The first element of coordinateTransformations must be a scale transform.
             Got {tform} instead.
             """
             )
-
-        if (tform := transforms[1].type) != "translation":
-            raise ValueError(
-                f"""
-            The second element of coordinateTransformations must be a translation 
-            transform. got {tform} instead.
-            """
-            )
+        if len(transforms) == 2:
+            if (tform := transforms[1].type) != "translation":
+                raise ValueError(
+                    f"""
+                The second element of coordinateTransformations must be a translation 
+                transform. got {tform} instead.
+                """
+                )
         return transforms
 
 
 class Multiscale(StrictVersionedBase):
     """
     Multiscale image metadata.
     See https://ngff.openmicroscopy.org/0.4/#multiscale-md
```

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/plate.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/plate.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/src/pydantic_ome_ngff/v04/well.py` & `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/well.py`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.2/PKG-INFO` & `pydantic_ome_ngff-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-ome-ngff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Pydantic models for the OME-NGFF
 License: MIT
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


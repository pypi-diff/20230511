# Comparing `tmp/sakkara-0.6.0.tar.gz` & `tmp/sakkara-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakkara-0.6.0.tar", max compression
+gzip compressed data, was "sakkara-0.6.1.tar", max compression
```

## Comparing `sakkara-0.6.0.tar` & `sakkara-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,54 @@
--rw-r--r--   0        0        0     1082 2023-03-07 10:34:12.072457 sakkara-0.6.0/LICENSE
--rw-r--r--   0        0        0      586 2023-05-09 13:13:23.637756 sakkara-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.334926 sakkara-0.6.0/sakkara/__init__.py
--rw-r--r--   0        0        0      601 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/__init__.py
--rw-r--r--   0        0        0     3226 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/base.py
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.382440 sakkara-0.6.0/sakkara/model/composable/__init__.py
--rw-r--r--   0        0        0     2647 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/composable/base.py
--rw-r--r--   0        0        0     5101 2023-04-26 14:01:04.108397 sakkara-0.6.0/sakkara/model/composable/group.py
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.481572 sakkara-0.6.0/sakkara/model/composable/hierarchical/__init__.py
--rw-r--r--   0        0        0     2402 2023-03-17 09:47:10.624449 sakkara-0.6.0/sakkara/model/composable/hierarchical/base.py
--rw-r--r--   0        0        0     1002 2023-03-16 08:43:10.158383 sakkara-0.6.0/sakkara/model/composable/hierarchical/deterministic.py
--rw-r--r--   0        0        0     2009 2023-03-14 13:24:52.998285 sakkara-0.6.0/sakkara/model/composable/hierarchical/distribution.py
--rw-r--r--   0        0        0     4337 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/composable/hierarchical/likelihood.py
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.569428 sakkara-0.6.0/sakkara/model/fixed/__init__.py
--rw-r--r--   0        0        0     1871 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/fixed/base.py
--rw-r--r--   0        0        0     2123 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/fixed/data.py
--rw-r--r--   0        0        0        0 2023-03-17 09:47:10.624449 sakkara-0.6.0/sakkara/model/function/__init__.py
--rw-r--r--   0        0        0     6629 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/function/base.py
--rw-r--r--   0        0        0     1559 2023-03-17 09:47:10.624449 sakkara-0.6.0/sakkara/model/function/wrapper.py
--rw-r--r--   0        0        0     2043 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/math_op.py
--rw-r--r--   0        0        0     1940 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/minibatch.py
--rw-r--r--   0        0        0     1156 2023-03-14 08:13:04.119000 sakkara-0.6.0/sakkara/model/utils.py
--rw-r--r--   0        0        0        8 2023-03-07 10:34:12.642766 sakkara-0.6.0/sakkara/relation/__init__.py
--rw-r--r--   0        0        0     2389 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/relation/group.py
--rw-r--r--   0        0        0     3522 2023-05-04 08:07:35.496801 sakkara-0.6.0/sakkara/relation/groupset.py
--rw-r--r--   0        0        0    11252 2023-05-04 06:57:24.906801 sakkara-0.6.0/sakkara/relation/representation.py
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 sakkara-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-03-07 10:34:12.072457 sakkara-0.6.1/LICENSE
+-rw-r--r--   0        0        0      572 2023-05-11 08:25:14.550606 sakkara-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.334926 sakkara-0.6.1/sakkara/__init__.py
+-rw-r--r--   0        0        0      646 2023-05-10 14:09:39.980962 sakkara-0.6.1/sakkara/model/__init__.py
+-rw-r--r--   0        0        0      907 2023-05-10 14:12:25.070962 sakkara-0.6.1/sakkara/model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4043 2023-05-09 13:22:28.307756 sakkara-0.6.1/sakkara/model/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2050 2023-05-11 08:16:40.870606 sakkara-0.6.1/sakkara/model/__pycache__/deterministic.cpython-310.pyc
+-rw-r--r--   0        0        0     2712 2023-05-09 13:22:28.307756 sakkara-0.6.1/sakkara/model/__pycache__/math_op.cpython-310.pyc
+-rw-r--r--   0        0        0     1875 2023-05-10 14:19:49.940962 sakkara-0.6.1/sakkara/model/__pycache__/minibatch.cpython-310.pyc
+-rw-r--r--   0        0        0     1418 2023-03-14 09:56:13.451273 sakkara-0.6.1/sakkara/model/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1820 2023-05-10 15:06:24.867301 sakkara-0.6.1/sakkara/model/__pycache__/wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     3226 2023-05-09 13:13:23.637756 sakkara-0.6.1/sakkara/model/base.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.382440 sakkara-0.6.1/sakkara/model/composable/__init__.py
+-rw-r--r--   0        0        0      181 2023-03-08 15:06:52.432053 sakkara-0.6.1/sakkara/model/composable/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3346 2023-05-10 14:12:25.090962 sakkara-0.6.1/sakkara/model/composable/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     4374 2023-05-10 14:12:25.080962 sakkara-0.6.1/sakkara/model/composable/__pycache__/group.cpython-310.pyc
+-rw-r--r--   0        0        0     2647 2023-05-10 14:10:52.980962 sakkara-0.6.1/sakkara/model/composable/base.py
+-rw-r--r--   0        0        0     5101 2023-05-10 14:10:52.980962 sakkara-0.6.1/sakkara/model/composable/group.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.481572 sakkara-0.6.1/sakkara/model/composable/hierarchical/__init__.py
+-rw-r--r--   0        0        0      194 2023-03-08 15:12:14.538964 sakkara-0.6.1/sakkara/model/composable/hierarchical/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2830 2023-05-10 14:12:25.090962 sakkara-0.6.1/sakkara/model/composable/hierarchical/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2637 2023-03-14 13:46:49.561172 sakkara-0.6.1/sakkara/model/composable/hierarchical/__pycache__/distribution.cpython-310.pyc
+-rw-r--r--   0        0        0     4266 2023-05-10 15:49:05.417301 sakkara-0.6.1/sakkara/model/composable/hierarchical/__pycache__/likelihood.cpython-310.pyc
+-rw-r--r--   0        0        0     1267 2023-05-11 08:21:57.530606 sakkara-0.6.1/sakkara/model/composable/hierarchical/__pycache__/reshaper.cpython-310.pyc
+-rw-r--r--   0        0        0     2402 2023-05-10 14:10:52.980962 sakkara-0.6.1/sakkara/model/composable/hierarchical/base.py
+-rw-r--r--   0        0        0     2009 2023-03-14 13:24:52.998285 sakkara-0.6.1/sakkara/model/composable/hierarchical/distribution.py
+-rw-r--r--   0        0        0     4339 2023-05-10 15:49:01.817300 sakkara-0.6.1/sakkara/model/composable/hierarchical/likelihood.py
+-rw-r--r--   0        0        0      712 2023-05-10 14:09:40.020962 sakkara-0.6.1/sakkara/model/composable/hierarchical/reshaper.py
+-rw-r--r--   0        0        0     1275 2023-05-11 08:16:37.450606 sakkara-0.6.1/sakkara/model/deterministic.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.569428 sakkara-0.6.1/sakkara/model/fixed/__init__.py
+-rw-r--r--   0        0        0      176 2023-03-08 15:06:53.685750 sakkara-0.6.1/sakkara/model/fixed/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3204 2023-05-10 14:12:25.080962 sakkara-0.6.1/sakkara/model/fixed/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     3036 2023-05-09 13:43:46.067756 sakkara-0.6.1/sakkara/model/fixed/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     1871 2023-05-10 11:52:32.244689 sakkara-0.6.1/sakkara/model/fixed/base.py
+-rw-r--r--   0        0        0     2131 2023-05-09 13:43:42.797756 sakkara-0.6.1/sakkara/model/fixed/data.py
+-rw-r--r--   0        0        0        0 2023-03-17 09:47:10.624449 sakkara-0.6.1/sakkara/model/function/__init__.py
+-rw-r--r--   0        0        0      152 2023-03-17 12:50:49.980171 sakkara-0.6.1/sakkara/model/function/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8043 2023-05-10 15:10:51.337301 sakkara-0.6.1/sakkara/model/function/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2183 2023-03-17 12:50:50.010171 sakkara-0.6.1/sakkara/model/function/__pycache__/wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     6734 2023-05-10 15:10:45.077300 sakkara-0.6.1/sakkara/model/function/base.py
+-rw-r--r--   0        0        0     1559 2023-03-17 09:47:10.624449 sakkara-0.6.1/sakkara/model/function/wrapper.py
+-rw-r--r--   0        0        0     2043 2023-05-09 13:13:23.637756 sakkara-0.6.1/sakkara/model/math_op.py
+-rw-r--r--   0        0        0     1369 2023-05-10 14:19:45.010962 sakkara-0.6.1/sakkara/model/minibatch.py
+-rw-r--r--   0        0        0     1156 2023-03-14 08:13:04.119000 sakkara-0.6.1/sakkara/model/utils.py
+-rw-r--r--   0        0        0     1008 2023-05-10 15:06:16.127301 sakkara-0.6.1/sakkara/model/wrapper.py
+-rw-r--r--   0        0        0        8 2023-03-07 10:34:12.642766 sakkara-0.6.1/sakkara/relation/__init__.py
+-rw-r--r--   0        0        0      187 2023-03-08 15:06:52.860747 sakkara-0.6.1/sakkara/relation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3153 2023-05-09 13:22:28.307756 sakkara-0.6.1/sakkara/relation/__pycache__/group.cpython-310.pyc
+-rw-r--r--   0        0        0     3383 2023-05-04 08:07:43.196801 sakkara-0.6.1/sakkara/relation/__pycache__/groupset.cpython-310.pyc
+-rw-r--r--   0        0        0    11275 2023-05-04 07:58:34.096801 sakkara-0.6.1/sakkara/relation/__pycache__/representation.cpython-310.pyc
+-rw-r--r--   0        0        0     2389 2023-05-09 13:13:23.637756 sakkara-0.6.1/sakkara/relation/group.py
+-rw-r--r--   0        0        0     3522 2023-05-04 08:07:35.496801 sakkara-0.6.1/sakkara/relation/groupset.py
+-rw-r--r--   0        0        0    11252 2023-05-04 06:57:24.906801 sakkara-0.6.1/sakkara/relation/representation.py
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 sakkara-0.6.1/PKG-INFO
```

### Comparing `sakkara-0.6.0/LICENSE` & `sakkara-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/pyproject.toml` & `sakkara-0.6.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sakkara"
-version = "0.6.0"
-description = "Tools for simplified creation of PyMC models"
+version = "0.6.1"
+description = "Tools for creating PyMC models"
 authors = ["Henrik Håkansson <henrik.hakansson@fcc.chalmers.se>", "Anders Sjöberg <anders.sjoberg@fcc.chalmers.se>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pymc = "^5"
 numpy = "^1.23"
 pandas = "^1.4"
```

### Comparing `sakkara-0.6.0/sakkara/model/__init__.py` & `sakkara-0.6.1/sakkara/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from sakkara.model.composable.group import GroupComponent
 from sakkara.model.composable.hierarchical.likelihood import Likelihood, MinibatchLikelihood
 from sakkara.model.composable.hierarchical.distribution import DistributionComponent
-from sakkara.model.composable.hierarchical.deterministic import DeterministicComponent
+from sakkara.model.composable.hierarchical.reshaper import Reshaper
+from sakkara.model.deterministic import DeterministicComponent
 from sakkara.model.fixed.base import UnrepeatableComponent
 from sakkara.model.fixed.data import DataComponent, data_components
 from sakkara.model.function.base import FunctionComponent
 from sakkara.model.function.wrapper import f_
 from sakkara.model.utils import build
```

### Comparing `sakkara-0.6.0/sakkara/model/base.py` & `sakkara-0.6.1/sakkara/model/base.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/composable/base.py` & `sakkara-0.6.1/sakkara/model/composable/base.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/composable/group.py` & `sakkara-0.6.1/sakkara/model/composable/group.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/composable/hierarchical/base.py` & `sakkara-0.6.1/sakkara/model/composable/hierarchical/base.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/composable/hierarchical/distribution.py` & `sakkara-0.6.1/sakkara/model/composable/hierarchical/distribution.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/composable/hierarchical/likelihood.py` & `sakkara-0.6.1/sakkara/model/composable/hierarchical/likelihood.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         :param observed: Data to input as observed keyword in PyMC.
         :param batch_size: Size of mini-batch (# of observations per evaluation)
         :param name: Name of the corresponding variable to register in PyMC.
         :param group: Group of which the component is defined for.
         :param nan_param_mask: Masked distribution parameters to use for rows with `Nan`, must be defined for each keyword argument entered. Required if there are `Nan` in observed.
         :param nan_data_mask: Masked observed value to use for rows with `Nan`. Required if there are `Nan` in observed.
         """
+
     def __init__(self, generator: Callable,
                  observed: DataComponent,
                  batch_size: int,
                  name: str = 'likelihood',
                  group: str = 'obs',
                  nan_param_mask: Dict[str, Any] = None,
                  nan_data_mask: Any = None,
```

### Comparing `sakkara-0.6.0/sakkara/model/fixed/base.py` & `sakkara-0.6.1/sakkara/model/fixed/base.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/fixed/data.py` & `sakkara-0.6.1/sakkara/model/fixed/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def build_representation(self, groupset: GroupSet) -> None:
         self.representation = MinimalTensorRepresentation()
         for g in self.group:
             self.representation.add_group(groupset[g])
 
     def build_variable(self) -> None:
-        self.variable = pm.Data(self.name, self.values)
+        self.variable = pm.ConstantData(self.name, self.values)
 
     def to_minibatch(self, batch_size: int, group: str) -> 'ModelComponent':
         return MinibatchComponent(self, batch_size, group)
 
 
 def data_components(df: pd.DataFrame, group: Union[str, Tuple[str, ...]] = 'obs') -> Dict[str, DataComponent]:
     """
```

### Comparing `sakkara-0.6.0/sakkara/model/function/base.py` & `sakkara-0.6.1/sakkara/model/function/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,18 @@
     def retrieve_groups(self) -> Set[str]:
         group = set()
         for component in chain(self.args, self.kwargs.values()):
             group = group.union(component.retrieve_groups())
         return group
 
     def to_minibatch(self, batch_size: int, group: str) -> 'ModelComponent':
-        self.args = [m.to_minibatch(batch_size, group) for m in self.args]
-        self.kwargs = {k: v.to_minibatch(batch_size, group) for k, v in self.kwargs.items()}
-        return self
+        return FunctionComponent(self.fct,
+                                 self.output_group,
+                                 *[m.to_minibatch(batch_size, group) for m in self.args],
+                                 **{k: v.to_minibatch(batch_size, group) for k, v in self.kwargs.items()})
 
     @staticmethod
     def math_op(fct: Callable, left: Any, right: Any) -> ModelComponent:
         if isinstance(left, ModelComponent) and isinstance(right, ModelComponent):
             return FunctionComponent(fct, None, left, right)
         if isinstance(left, ModelComponent):
             return FunctionComponent(lambda x: fct(x, right), None, left)
```

### Comparing `sakkara-0.6.0/sakkara/model/function/wrapper.py` & `sakkara-0.6.1/sakkara/model/function/wrapper.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/math_op.py` & `sakkara-0.6.1/sakkara/model/math_op.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/model/utils.py` & `sakkara-0.6.1/sakkara/model/utils.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/relation/group.py` & `sakkara-0.6.1/sakkara/relation/group.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/relation/groupset.py` & `sakkara-0.6.1/sakkara/relation/groupset.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.6.0/sakkara/relation/representation.py` & `sakkara-0.6.1/sakkara/relation/representation.py`

 * *Files identical despite different names*


# Comparing `tmp/jaxtyping-0.2.8.tar.gz` & `tmp/jaxtyping-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxtyping-0.2.8.tar", last modified: Mon Nov 14 06:26:13 2022, max compression
+gzip compressed data, was "jaxtyping-0.2.9.tar", last modified: Thu Dec  8 01:22:27 2022, max compression
```

## Comparing `jaxtyping-0.2.8.tar` & `jaxtyping-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:26:13.781760 jaxtyping-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-11-14 06:26:13.781760 jaxtyping-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:26:13.781760 jaxtyping-0.2.8/jaxtyping/
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/jaxtyping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19474 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/jaxtyping/array_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/jaxtyping/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11293 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/jaxtyping/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/jaxtyping/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2220 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/jaxtyping/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/jaxtyping/pytree_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:26:13.781760 jaxtyping-0.2.8/jaxtyping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-11-14 06:26:13.000000 jaxtyping-0.2.8/jaxtyping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-14 06:26:13.000000 jaxtyping-0.2.8/jaxtyping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 06:26:13.000000 jaxtyping-0.2.8/jaxtyping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-14 06:26:13.000000 jaxtyping-0.2.8/jaxtyping.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 06:26:13.000000 jaxtyping-0.2.8/jaxtyping.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-14 06:26:13.000000 jaxtyping-0.2.8/jaxtyping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-14 06:26:13.000000 jaxtyping-0.2.8/jaxtyping.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 06:26:13.781760 jaxtyping-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-11-14 06:26:06.000000 jaxtyping-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 01:22:27.581109 jaxtyping-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2022-12-08 01:22:27.577109 jaxtyping-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 01:22:27.577109 jaxtyping-0.2.9/jaxtyping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/jaxtyping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18941 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/jaxtyping/array_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/jaxtyping/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/jaxtyping/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/jaxtyping/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/jaxtyping/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/jaxtyping/pytree_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 01:22:27.577109 jaxtyping-0.2.9/jaxtyping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2022-12-08 01:22:27.000000 jaxtyping-0.2.9/jaxtyping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2022-12-08 01:22:27.000000 jaxtyping-0.2.9/jaxtyping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 01:22:27.000000 jaxtyping-0.2.9/jaxtyping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-08 01:22:27.000000 jaxtyping-0.2.9/jaxtyping.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 01:22:27.000000 jaxtyping-0.2.9/jaxtyping.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-08 01:22:27.000000 jaxtyping-0.2.9/jaxtyping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-08 01:22:27.000000 jaxtyping-0.2.9/jaxtyping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 01:22:27.581109 jaxtyping-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2022-12-08 01:22:22.000000 jaxtyping-0.2.9/setup.py
```

### Comparing `jaxtyping-0.2.8/LICENSE` & `jaxtyping-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxtyping-0.2.8/PKG-INFO` & `jaxtyping-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxtyping
-Version: 0.2.8
+Version: 0.2.9
 Summary: Type annotations and runtime checking for shape and dtype of JAX arrays, and PyTrees.
 Home-page: https://github.com/google/jaxtyping
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: MIT
@@ -52,14 +52,16 @@
         
         ### See also: other tools in the JAX ecosystem
         
         Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
         
         Numerical differential equation solvers: [Diffrax](https://github.com/patrick-kidger/diffrax).
         
+        Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+        
         SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
         
         ### Acknowledgements
         
         Shape annotations + runtime type checking is inspired by [TorchTyping](https://github.com/patrick-kidger/torchtyping).
         
         The concise syntax is partially inspired by [etils.array_types](https://github.com/google/etils/tree/main/etils/array_types).
```

### Comparing `jaxtyping-0.2.8/README.md` & `jaxtyping-0.2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
 ### See also: other tools in the JAX ecosystem
 
 Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
 
 Numerical differential equation solvers: [Diffrax](https://github.com/patrick-kidger/diffrax).
 
+Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+
 SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
 
 ### Acknowledgements
 
 Shape annotations + runtime type checking is inspired by [TorchTyping](https://github.com/patrick-kidger/torchtyping).
 
 The concise syntax is partially inspired by [etils.array_types](https://github.com/google/etils/tree/main/etils/array_types).
```

### Comparing `jaxtyping-0.2.8/jaxtyping/__init__.py` & `jaxtyping-0.2.9/jaxtyping/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,57 +14,79 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import typing
+import typing_extensions
 
 
-if typing.TYPE_CHECKING:
-    # type checkers don't know which branch below will be executed
-    from jax.numpy import ndarray as Array
+try:
+    import jax
+except ImportError:
+    has_jax = False
 else:
+    has_jax = True
+    del jax
+
+
+# Type checkers don't know which branch below will be executed.
+if typing.TYPE_CHECKING:
+    # For imports, we need to explicitly `import X as X` in order for Pyright to see
+    # them as public. See discussion at https://github.com/microsoft/pyright/issues/2277
+    from jax import Array as Array
+elif has_jax:
     if getattr(typing, "GENERATING_DOCUMENTATION", False):
 
         class Array:
             pass
 
         Array.__module__ = "builtins"
     else:
-        from jax.numpy import ndarray as Array
+        from jax import Array as Array
 
 from .array_types import (
-    AbstractArray,
-    AbstractDtype,
-    BFloat16,
-    Bool,
-    Complex,
-    Complex64,
-    Complex128,
-    Float,
-    Float16,
-    Float32,
-    Float64,
-    get_array_name_format,
-    Inexact,
-    Int,
-    Int8,
-    Int16,
-    Int32,
-    Int64,
-    Integer,
-    Num,
-    set_array_name_format,
-    Shaped,
-    UInt,
-    UInt8,
-    UInt16,
-    UInt32,
-    UInt64,
+    AbstractArray as AbstractArray,
+    AbstractDtype as AbstractDtype,
+    BFloat16 as BFloat16,
+    Bool as Bool,
+    Complex as Complex,
+    Complex64 as Complex64,
+    Complex128 as Complex128,
+    Float as Float,
+    Float16 as Float16,
+    Float32 as Float32,
+    Float64 as Float64,
+    get_array_name_format as get_array_name_format,
+    Inexact as Inexact,
+    Int as Int,
+    Int8 as Int8,
+    Int16 as Int16,
+    Int32 as Int32,
+    Int64 as Int64,
+    Integer as Integer,
+    Num as Num,
+    set_array_name_format as set_array_name_format,
+    Shaped as Shaped,
+    UInt as UInt,
+    UInt8 as UInt8,
+    UInt16 as UInt16,
+    UInt32 as UInt32,
+    UInt64 as UInt64,
 )
-from .decorator import jaxtyped
-from .import_hook import install_import_hook
-from .pytree_type import PyTree
+from .decorator import jaxtyped as jaxtyped
+from .import_hook import install_import_hook as install_import_hook
+
+
+if typing.TYPE_CHECKING:
+    _T = typing.TypeVar("_T")
+
+    class PyTree(typing_extensions.Protocol[_T]):
+        pass
+
+elif has_jax:
+    from .pytree_type import PyTree
 
+del has_jax
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
```

### Comparing `jaxtyping-0.2.8/jaxtyping/array_types.py` & `jaxtyping-0.2.9/jaxtyping/array_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -429,37 +429,39 @@
         cls.dtypes = dtypes
 
 
 if TYPE_CHECKING:
     # Note that `from typing_extensions import Annotated; ... = Annotated`
     # does not work with static type checkers. `Annotated` is a typeform rather
     # than a type, meaning it cannot be assigned.
-    from typing_extensions import Annotated as BFloat16
-    from typing_extensions import Annotated as Bool
-    from typing_extensions import Annotated as Complex
-    from typing_extensions import Annotated as Complex64
-    from typing_extensions import Annotated as Complex128
-    from typing_extensions import Annotated as Float
-    from typing_extensions import Annotated as Float16
-    from typing_extensions import Annotated as Float32
-    from typing_extensions import Annotated as Float64
-    from typing_extensions import Annotated as Inexact
-    from typing_extensions import Annotated as Int
-    from typing_extensions import Annotated as Int8
-    from typing_extensions import Annotated as Int16
-    from typing_extensions import Annotated as Int32
-    from typing_extensions import Annotated as Int64
-    from typing_extensions import Annotated as Integer
-    from typing_extensions import Annotated as Num
-    from typing_extensions import Annotated as Shaped
-    from typing_extensions import Annotated as UInt
-    from typing_extensions import Annotated as UInt8
-    from typing_extensions import Annotated as UInt16
-    from typing_extensions import Annotated as UInt32
-    from typing_extensions import Annotated as UInt64
+    from typing_extensions import (
+        Annotated as BFloat16,
+        Annotated as Bool,
+        Annotated as Complex,
+        Annotated as Complex64,
+        Annotated as Complex128,
+        Annotated as Float,
+        Annotated as Float16,
+        Annotated as Float32,
+        Annotated as Float64,
+        Annotated as Inexact,
+        Annotated as Int,
+        Annotated as Int8,
+        Annotated as Int16,
+        Annotated as Int32,
+        Annotated as Int64,
+        Annotated as Integer,
+        Annotated as Num,
+        Annotated as Shaped,
+        Annotated as UInt,
+        Annotated as UInt8,
+        Annotated as UInt16,
+        Annotated as UInt32,
+        Annotated as UInt64,
+    )
 else:
     _bool = "bool_"
     _uint8 = "uint8"
     _uint16 = "uint16"
     _uint32 = "uint32"
     _uint64 = "uint64"
     _int8 = "int8"
```

### Comparing `jaxtyping-0.2.8/jaxtyping/decorator.py` & `jaxtyping-0.2.9/jaxtyping/decorator.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+import dataclasses
 import functools as ft
 import inspect
 import threading
 
 
 storage = threading.local()
 
@@ -42,12 +43,34 @@
             return self.fn(*args, **kwargs)
         finally:
             memo_stack.pop()
 
 
 def jaxtyped(fn):
     if inspect.isclass(fn):  # allow decorators on class definitions
-        init = jaxtyped(fn.__init__)
-        fn.__init__ = init
-        return fn
+        if dataclasses.is_dataclass(fn):
+            init = jaxtyped(fn.__init__)
+            fn.__init__ = init
+            return fn
+        else:
+            raise ValueError(
+                "jaxtyped may only be added as a class decorator to dataclasses"
+            )
     else:
         return ft.wraps(fn)(_Jaxtyped(fn))
+
+
+def _jaxtyped_typechecker(typechecker):
+    # typechecker is expected to probably be either `typeguard.typechecked`, or
+    # `beartype.beartype`, or `None`.
+
+    if typechecker is None:
+        typechecker = lambda x: x
+
+    def _wrapper(kls):
+        assert inspect.isclass(kls)
+        if dataclasses.is_dataclass(kls):
+            init = jaxtyped(typechecker(kls.__init__))
+            kls.__init__ = init
+        return kls
+
+    return _wrapper
```

### Comparing `jaxtyping-0.2.8/jaxtyping/import_hook.py` & `jaxtyping-0.2.9/jaxtyping/import_hook.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,23 @@
 def _call_with_frames_removed(f, *args, **kwargs):
     return f(*args, **kwargs)
 
 
 def _optimized_cache_from_source(path, debug_override=None):
     # Version 2: change the position of the `@jaxtyped` decorator, so need a
     # different name to avoid hitting old __pycache__
-    return cache_from_source(path, debug_override, optimization="jaxtyping2")
+    # Version 3: now also annotating classes.
+    return cache_from_source(path, debug_override, optimization="jaxtyping3")
+
+
+def _dot_lookup(*elements):
+    out = ast.Name(id=elements[0], ctx=ast.Load())
+    for element in elements[1:]:
+        out = ast.Attribute(out, element, ctx=ast.Load())
+    return out
 
 
 class _JaxtypingTransformer(ast.NodeVisitor):
     def __init__(self, *, typechecker) -> None:
         self._parents: List[ast.AST] = []
         self._typechecker = typechecker
 
@@ -93,45 +101,45 @@
                 break
 
         self._parents.append(node)
         self.generic_visit(node)
         self._parents.pop()
         return node
 
+    def visit_ClassDef(self, node: ast.ClassDef):
+        func = _dot_lookup("jaxtyping", "decorator", "_jaxtyped_typechecker")
+        if self._typechecker is None:
+            args = [ast.Constant(None)]
+        else:
+            args = [_dot_lookup(*self._typechecker)]
+        node.decorator_list.append(ast.Call(func, args, keywords=[]))
+        self._parents.append(node)
+        self.generic_visit(node)
+        self._parents.pop()
+        return node
+
     def visit_FunctionDef(self, node: ast.FunctionDef):
         has_annotated_args = any(arg for arg in node.args.args if arg.annotation)
         has_annotated_return = bool(node.returns)
         if has_annotated_args or has_annotated_return:
             # Place at the end of the decorator list, as otherwise we wrap e.g.
             # `jax.custom_{jvp,vjp}` and lose the ability to `defjvp` etc.
             #
             # Note that the counter-argument here is that we'd like to place this
             # at the start of the decorator list, in case a typechecking annotation
             # has been manually applied, and we'd need to be above that. In this
             # case we're just going to have to need to ask the user to remove their
             # typechecking annotation (and let this decorator do it instead).
             # It's more important we be compatible with normal JAX code.
-            node.decorator_list.append(
-                ast.Attribute(
-                    ast.Name(id="jaxtyping", ctx=ast.Load()), "jaxtyped", ast.Load()
-                ),
-            )
+            node.decorator_list.append(_dot_lookup("jaxtyping", "jaxtyped"))
             if self._typechecker is not None:
                 # Place at the end of the decorator list, as decorators
                 # frequently remove annotations from functions and we'd like to
                 # use those annotations.
-                typechecker_module, typechecker_function = self._typechecker
-                node.decorator_list.append(
-                    ast.Attribute(
-                        ast.Name(id=typechecker_module, ctx=ast.Load()),
-                        typechecker_function,
-                        ast.Load(),
-                    )
-                )
-
+                node.decorator_list.append(_dot_lookup(*self._typechecker))
         self._parents.append(node)
         self.generic_visit(node)
         self._parents.pop()
         return node
 
 
 class _JaxtypingLoader(SourceFileLoader):
```

### Comparing `jaxtyping-0.2.8/jaxtyping/pytest_plugin.py` & `jaxtyping-0.2.9/jaxtyping/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `jaxtyping-0.2.8/jaxtyping/pytree_type.py` & `jaxtyping-0.2.9/jaxtyping/pytree_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import functools as ft
 import typing
-from typing import Generic, TYPE_CHECKING, TypeVar
-from typing_extensions import Protocol
+from typing import Generic, TypeVar
 
 import jax.tree_util as jtu
 import typeguard
 
 
 _T = TypeVar("_T")
 
@@ -83,22 +82,15 @@
             else:
                 return True
 
         leaves = jtu.tree_leaves(obj, is_leaf=is_leaftype)
         return all(map(is_leaftype, leaves))
 
 
-if TYPE_CHECKING:
-    # Work around pytype bug #1288
-    # pytype: skip-file
-    class PyTree(Protocol[_T]):
-        pass
-
-else:
-    PyTree = _MetaPyTree("PyTree", (), {})
-    if getattr(typing, "GENERATING_DOCUMENTATION", False):
-        PyTree.__module__ = "builtins"
-    else:
-        PyTree.__module__ = "jaxtyping"
 # Can't do `class PyTree(Generic[_T]): ...` because we need to override the
 # instancecheck for PyTree[foo], but subclassing
 # `type(Generic[int])`, i.e. `typing._GenericAlias` is disallowed.
+PyTree = _MetaPyTree("PyTree", (), {})
+if getattr(typing, "GENERATING_DOCUMENTATION", False):
+    PyTree.__module__ = "builtins"
+else:
+    PyTree.__module__ = "jaxtyping"
```

### Comparing `jaxtyping-0.2.8/jaxtyping.egg-info/PKG-INFO` & `jaxtyping-0.2.9/jaxtyping.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxtyping
-Version: 0.2.8
+Version: 0.2.9
 Summary: Type annotations and runtime checking for shape and dtype of JAX arrays, and PyTrees.
 Home-page: https://github.com/google/jaxtyping
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: MIT
@@ -52,14 +52,16 @@
         
         ### See also: other tools in the JAX ecosystem
         
         Neural networks: [Equinox](https://github.com/patrick-kidger/equinox).
         
         Numerical differential equation solvers: [Diffrax](https://github.com/patrick-kidger/diffrax).
         
+        Computer vision models: [Eqxvision](https://github.com/paganpasta/eqxvision).
+        
         SymPy<->JAX conversion; train symbolic expressions via gradient descent: [sympy2jax](https://github.com/google/sympy2jax).
         
         ### Acknowledgements
         
         Shape annotations + runtime type checking is inspired by [TorchTyping](https://github.com/patrick-kidger/torchtyping).
         
         The concise syntax is partially inspired by [etils.array_types](https://github.com/google/etils/tree/main/etils/array_types).
```

### Comparing `jaxtyping-0.2.8/setup.py` & `jaxtyping-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
 # We use typeguard internally (in a fairly minimal way), but it's not required that
 # end users make the same choice.
 # For typing_extensions, we choose versions that match
 # https://github.com/explosion/confection/blob/main/setup.cfg#L33 used in colab
 
 install_requires = [
-    "jax>=0.3.4",
     "numpy>=1.20.0",
     "typeguard>=2.13.3",
     "typing_extensions>=3.7.4.1",
 ]
 
 entry_points = dict(pytest11=["jaxtyping = jaxtyping.pytest_plugin"])
```


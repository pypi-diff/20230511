# Comparing `tmp/lazi-1.0.3.tar.gz` & `tmp/lazi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.0.3.tar", max compression
+gzip compressed data, was "lazi-1.0.4.tar", max compression
```

## Comparing `lazi-1.0.3.tar` & `lazi-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      980 2023-05-10 07:53:22.639513 lazi-1.0.3/README.md
--rw-r--r--   0        0        0      212 2023-05-10 07:27:31.387501 lazi-1.0.3/lazi/auto.py
--rw-r--r--   0        0        0      933 2023-05-10 07:01:49.042718 lazi-1.0.3/lazi/conf/conf.py
--rw-r--r--   0        0        0        0 2023-05-10 06:52:02.602781 lazi-1.0.3/lazi/core/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-10 06:59:28.888814 lazi-1.0.3/lazi/core/finder.py
--rw-r--r--   0        0        0     1875 2023-05-10 06:52:02.606781 lazi-1.0.3/lazi/core/loader.py
--rw-r--r--   0        0        0     2765 2023-05-10 07:11:26.686038 lazi-1.0.3/lazi/core/record.py
--rw-r--r--   0        0        0      854 2023-05-10 06:52:02.602781 lazi-1.0.3/lazi/core/util.py
--rw-r--r--   0        0        0     1084 2023-05-10 07:58:22.167238 lazi-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 lazi-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.0.4/LICENSE
+-rw-r--r--   0        0        0      980 2023-05-10 07:53:22.639513 lazi-1.0.4/README.md
+-rw-r--r--   0        0        0      212 2023-05-10 07:27:31.387501 lazi-1.0.4/lazi/auto.py
+-rw-r--r--   0        0        0     1067 2023-05-11 03:25:56.231912 lazi-1.0.4/lazi/conf/conf.py
+-rw-r--r--   0        0        0        0 2023-05-10 06:52:02.602781 lazi-1.0.4/lazi/core/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-11 03:22:35.445233 lazi-1.0.4/lazi/core/finder.py
+-rw-r--r--   0        0        0     2662 2023-05-11 03:24:26.238697 lazi-1.0.4/lazi/core/loader.py
+-rw-r--r--   0        0        0     3309 2023-05-11 03:11:35.124620 lazi-1.0.4/lazi/core/record.py
+-rw-r--r--   0        0        0      815 2023-05-11 02:16:42.153612 lazi-1.0.4/lazi/core/util.py
+-rw-r--r--   0        0        0     1123 2023-05-11 03:27:25.321116 lazi-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 lazi-1.0.4/PKG-INFO
```

### Comparing `lazi-1.0.3/README.md` & `lazi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lazi-1.0.3/lazi/conf/conf.py` & `lazi-1.0.4/lazi/conf/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """Default configuration for Lazi.
 """
 
+DEBUG_TRACING: bool = False          # Enable debug traces.
+
 SPECR_KEEP_EMPTY: bool = False      # Keep records without a spec.
 SPECR_KEEP_0HOOK: bool = False      # Keep records without a hook.
-SPECR_KEEP_STACK: bool = True       # Keep import stacks in records.
 SPECR_HOOK_STDLI: bool = False      # Hook stdlib modules.
 
+LOADER_AUTO_DEPS: bool = True       # Also load dependent imports when loading a module.
+
+
 def __load():
     import sys
     from pkgutil import iter_modules
     from importlib import import_module
     import lazi.conf as namespace
 
     dic = sys.modules[__name__].__dict__
     keys = set(key for key in dic.keys() if not key.startswith("_") and key.isupper())
 
     for module_info in (mi for mi in iter_modules(namespace.__path__, namespace.__name__ + ".") if mi.name != __name__):
         module = import_module(module_info.name)
 
         for key in (key for key in keys if hasattr(module, key)):
-            dic[key] = getattr(module, key)
+            dic[key] = getattr(module, key)  # TODO (As Needed): Check type and merge accordingly.
 
-    # for key in keys:
-    #     setattr(namespace, key, dic[key])
+    for key in keys:
+        setattr(namespace, key, dic[key])
 
 
 __load()
```

### Comparing `lazi-1.0.3/lazi/core/finder.py` & `lazi-1.0.4/lazi/core/finder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from __future__ import annotations
 
 import sys
+from types import ModuleType
 from importlib.util import find_spec
 from importlib.machinery import ModuleSpec
 from importlib.abc import MetaPathFinder
 
 from .record import SpecRecord
 from .loader import Loader
-from .util import nofail
+from .util import trace
 
 __all__ = "Finder",
 
 
+# noinspection PyMethodMayBeStatic
 class Finder(MetaPathFinder):
     LoaderType: type[Loader] = Loader
     SpecRecordType: type[SpecRecord] = SpecRecord
 
-    def on_import(self, spec_record: SpecRecord):
-        pass
+    def pre_import(self, spec_record: SpecRecord) -> None:
+        return  # trace("pre_import", spec_record.name, spec_record.spec)
 
-    def on_preload(self, spec_record: SpecRecord):
-        pass
+    def on_import(self, spec_record: SpecRecord) -> None:
+        return trace("on_import", spec_record.name, spec_record.spec)
 
-    def on_load(self, spec_record: SpecRecord, stack: tuple[SpecRecord, ...] | None = None):
-        pass
+    def pre_load(self, spec_record: SpecRecord) -> None:
+        return trace("pre_load", spec_record.name, spec_record.spec)
+
+    def on_load(self, spec_record: SpecRecord) -> None:
+        return trace("on_load", spec_record.name, spec_record.spec)
+
+    def on_create(self, spec_record: SpecRecord, module: ModuleType) -> None:
+        return trace("on_create", spec_record.name, spec_record.spec, module)
 
     @classmethod
     def install(cls, *, force: bool = False) -> Finder | None:
         if not force and any(isinstance(finder, cls) for finder in sys.meta_path):
             return None
         sys.meta_path.insert(0, self := cls())
         return self
@@ -45,18 +53,18 @@
             return find_spec(fullname)
 
         finally:
             if meta_path:
                 sys.meta_path.insert(0, self)
 
     def find_spec(self, fullname, path=None, target=None) -> ModuleSpec | None:
+        # trace("find_spec", fullname, path, target)
         record = self.SpecRecordType.register(
             finder=self,
             name=fullname,
             path=path,
             target=target,
         )
-        nofail(self.on_import, record)
         return record.spec
 
     def invalidate_caches(self) -> None:
         self.SpecRecordType.RECORD.clear()
```

### Comparing `lazi-1.0.3/lazi/core/loader.py` & `lazi-1.0.4/lazi/core/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,88 @@
 from types import ModuleType
-from contextlib import contextmanager
-import importlib.util
+from importlib.util import LazyLoader, module_from_spec
 
+# noinspection PyUnresolvedReferences,PyProtectedMember
+from importlib.util import _LazyModule  # type: type[ModuleType]
+
+from lazi.conf import conf
 from .record import SpecRecord
-from .util import nofail
+from .util import trace
 
 __all__ = "Loader",
 
-# noinspection PyUnresolvedReferences,PyProtectedMember
-_LazyModule: type[ModuleType] = importlib.util._LazyModule
 
-
-class Loader(importlib.util.LazyLoader):
+class Loader(LazyLoader):
+    __module: ModuleType | None = None
     spec_record: SpecRecord
-    __stack__: list[SpecRecord] = []
 
     def __init__(self, spec_record: SpecRecord):
         self.spec_record = spec_record
         super().__init__(spec_record.spec.loader)
 
     @property
     def loaded(self) -> bool:
         return self.spec_record.used
 
-    @property
-    def stack(self) -> tuple[SpecRecord, ...]:
-        return tuple(self.__stack__)
-
     def hook(self):
-        assert self.spec_record.hook
+        assert self.spec_record.hook is True
         self.spec_record.spec.loader = self
 
-    def on_preload(self):
-        nofail(self.spec_record.on_preload)
-        self.__stack__.append(self.spec_record)
-
-    def on_load(self, stack: tuple[SpecRecord, ...]):
-        assert not self.loaded
-        assert self.__stack__.pop() is self.spec_record
-        nofail(self.spec_record.on_load, stack)
+    def pre_load(self):
+        return self.spec_record.pre_load()
+
+    def on_load(self):
+        assert self.loaded is False
+
+        if conf.LOADER_AUTO_DEPS:
+            for dep in (dep for dep in self.spec_record.deps if dep.spec is not None):
+                # New discovery from this: dep.spec.loader gets changed between its on_create() and here.
+
+                trace("dep_load", self.spec_record.name, "->", dep.spec, dep.loader, dep.spec.loader)
+
+                if not dep.hook:
+                    module = module_from_spec(dep.spec)
+                else:
+                    assert dep.loader is not None
+                    module = dep.loader.__module
+
+                getattr(module, "__path__", None)  # Force the module to load.
+
+        return self.spec_record.on_load()
+
+    def on_create(self, module: ModuleType):
+        assert self.__module is None
+        self.__module = module
+        return self.spec_record.on_create(module)
+
+    def exec_module(self, module: ModuleType):
+        self.on_create(module)
 
-    def exec_module(self, module):
         super().exec_module(module)
 
         # noinspection PyMethodParameters
         class LazyModule(_LazyModule):
             def __getattribute__(self_, attr):
-                assert not self.loaded
+                trace("getattribute", self.spec_record.name, attr)
+
+                assert self.loaded is False
 
                 if attr == "__spec__":
                     return self.spec_record.spec
 
-                with self.__load_context__():
-                    return _LazyModule.__getattribute__(self_, attr)
+                self.pre_load()
+
+                try:
+                    trace("getattribute", self.spec_record.name, attr, "load")
+                    return _LazyModule.__getattribute__(self_, attr)  # Errors here come from the import two lines above.
+
+                except Exception:
+                    raise
+
+                finally:
+                    self.on_load()
 
             def __delattr__(self_, attr):
                 return _LazyModule.__delattr__(self_,  attr)
 
         module.__class__ = LazyModule
 
-    @contextmanager
-    def __load_context__(self):
-        self.on_preload()
-
-        try:
-            yield
-        finally:
-            self.on_load(self.stack)
```

### Comparing `lazi-1.0.3/lazi/core/util.py` & `lazi-1.0.4/lazi/core/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import sys
-from typing import Callable
 from types import ModuleType
 from importlib.machinery import ModuleSpec
 import sysconfig
 from pathlib import Path
 
-STD_LIB_PATH = sysconfig.get_path("stdlib")
+from lazi.conf import conf
 
 
 def is_stdlib_or_builtin(module: ModuleType | ModuleSpec) -> bool:
+
     if isinstance(module, ModuleType):
         spec = getattr(module, "__spec__", None)
         return (spec is None) or is_stdlib_or_builtin(spec)
+
     elif isinstance(module, ModuleSpec):
         origin = module.origin
-        return (origin in (None, "built-in")) or Path(origin).is_relative_to(STD_LIB_PATH)
+        return (origin in (None, "built-in")) or Path(origin).is_relative_to(sysconfig.get_path("stdlib"))
 
     raise TypeError(f"Expected ModuleType or ModuleSpec, got {type(module)}")
 
 
-def nofail(func: Callable, /, *args, **kwds):
-    try:
-        func(*args, **kwds)
-    except Exception as exc:
-        print(f"Exception when calling {func.__name__}(): {exc}", file=sys.stderr)
+if conf.DEBUG_TRACING:
+    def trace(*args, **kwds):
+        kwds.setdefault("file", sys.stderr)
+        return print(*args, **kwds)
+
+else:
+    def trace(*args, **kwds):
+        pass
```

### Comparing `lazi-1.0.3/pyproject.toml` & `lazi-1.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.0.3"
+version = "1.0.4"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
@@ -26,14 +26,16 @@
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 django = "^4.2.1"
+requests = "^2.30.0"
+toolz = "^0.12.0"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 
 
 [build-system]
```

### Comparing `lazi-1.0.3/PKG-INFO` & `lazi-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.0.3
+Version: 1.0.4
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: Environment :: Web Environment
```


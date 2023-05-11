# Comparing `tmp/lazi-1.0.4.tar.gz` & `tmp/lazi-1.1.0.post13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.0.4.tar", max compression
+gzip compressed data, was "lazi-1.1.0.post13.tar", max compression
```

## Comparing `lazi-1.0.4.tar` & `lazi-1.1.0.post13.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.0.4/LICENSE
--rw-r--r--   0        0        0      980 2023-05-10 07:53:22.639513 lazi-1.0.4/README.md
--rw-r--r--   0        0        0      212 2023-05-10 07:27:31.387501 lazi-1.0.4/lazi/auto.py
--rw-r--r--   0        0        0     1067 2023-05-11 03:25:56.231912 lazi-1.0.4/lazi/conf/conf.py
--rw-r--r--   0        0        0        0 2023-05-10 06:52:02.602781 lazi-1.0.4/lazi/core/__init__.py
--rw-r--r--   0        0        0     2163 2023-05-11 03:22:35.445233 lazi-1.0.4/lazi/core/finder.py
--rw-r--r--   0        0        0     2662 2023-05-11 03:24:26.238697 lazi-1.0.4/lazi/core/loader.py
--rw-r--r--   0        0        0     3309 2023-05-11 03:11:35.124620 lazi-1.0.4/lazi/core/record.py
--rw-r--r--   0        0        0      815 2023-05-11 02:16:42.153612 lazi-1.0.4/lazi/core/util.py
--rw-r--r--   0        0        0     1123 2023-05-11 03:27:25.321116 lazi-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 lazi-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.1.0.post13/LICENSE
+-rw-r--r--   0        0        0      980 2023-05-10 07:53:22.639513 lazi-1.1.0.post13/README.md
+-rw-r--r--   0        0        0      104 2023-05-11 08:57:20.841058 lazi-1.1.0.post13/lazi/auto.py
+-rw-r--r--   0        0        0       37 2023-05-11 10:10:32.878224 lazi-1.1.0.post13/lazi/conf/all.py
+-rw-r--r--   0        0        0      863 2023-05-11 10:10:32.874224 lazi-1.1.0.post13/lazi/conf/base.py
+-rw-r--r--   0        0        0      720 2023-05-11 10:24:25.485088 lazi-1.1.0.post13/lazi/conf/conf.py
+-rw-r--r--   0        0        0      453 2023-05-11 09:12:13.132626 lazi-1.1.0.post13/lazi/core/__init__.py
+-rw-r--r--   0        0        0     3173 2023-05-11 10:24:25.477088 lazi-1.1.0.post13/lazi/core/finder.py
+-rw-r--r--   0        0        0     2609 2023-05-11 09:48:59.517349 lazi-1.1.0.post13/lazi/core/loader.py
+-rw-r--r--   0        0        0     4953 2023-05-11 10:24:25.461088 lazi-1.1.0.post13/lazi/core/record.py
+-rw-r--r--   0        0        0      815 2023-05-11 10:00:09.202100 lazi-1.1.0.post13/lazi/core/util.py
+-rw-r--r--   0        0        0       32 2023-05-11 08:56:50.716672 lazi-1.1.0.post13/lazi/lazi.py
+-rw-r--r--   0        0        0     1166 2023-05-11 10:39:13.272620 lazi-1.1.0.post13/pyproject.toml
+-rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 lazi-1.1.0.post13/PKG-INFO
```

### Comparing `lazi-1.0.4/LICENSE` & `lazi-1.1.0.post13/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.0.4/README.md` & `lazi-1.1.0.post13/README.md`

 * *Files identical despite different names*

### Comparing `lazi-1.0.4/lazi/core/loader.py` & `lazi-1.1.0.post13/lazi/core/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from types import ModuleType
-from importlib.util import LazyLoader, module_from_spec
-
+from importlib.util import LazyLoader
 # noinspection PyUnresolvedReferences,PyProtectedMember
 from importlib.util import _LazyModule  # type: type[ModuleType]
 
 from lazi.conf import conf
 from .record import SpecRecord
 from .util import trace
 
 __all__ = "Loader",
 
 
 class Loader(LazyLoader):
-    __module: ModuleType | None = None
     spec_record: SpecRecord
 
     def __init__(self, spec_record: SpecRecord):
         self.spec_record = spec_record
         super().__init__(spec_record.spec.loader)
 
     @property
@@ -35,54 +33,50 @@
 
         if conf.LOADER_AUTO_DEPS:
             for dep in (dep for dep in self.spec_record.deps if dep.spec is not None):
                 # New discovery from this: dep.spec.loader gets changed between its on_create() and here.
 
                 trace("dep_load", self.spec_record.name, "->", dep.spec, dep.loader, dep.spec.loader)
 
-                if not dep.hook:
-                    module = module_from_spec(dep.spec)
-                else:
-                    assert dep.loader is not None
-                    module = dep.loader.__module
-
-                getattr(module, "__path__", None)  # Force the module to load.
+                getattr(dep.module, "__path__", None)  # Force the module to load.
 
         return self.spec_record.on_load()
 
     def on_create(self, module: ModuleType):
-        assert self.__module is None
-        self.__module = module
         return self.spec_record.on_create(module)
 
     def exec_module(self, module: ModuleType):
         self.on_create(module)
-
         super().exec_module(module)
 
         # noinspection PyMethodParameters
         class LazyModule(_LazyModule):
             def __getattribute__(self_, attr):
                 trace("getattribute", self.spec_record.name, attr)
 
                 assert self.loaded is False
 
-                if attr == "__spec__":
-                    return self.spec_record.spec
+                if attr in conf.LOADER_FAKE_ATTR:
+                    match attr:
+                        case "__spec__":
+                            return self.spec_record.spec
+                        case "__loader__":
+                            return self
+                        case "__name__":
+                            return self.spec_record.name
 
                 self.pre_load()
 
                 try:
                     trace("getattribute", self.spec_record.name, attr, "load")
-                    return _LazyModule.__getattribute__(self_, attr)  # Errors here come from the import two lines above.
+                    return _LazyModule.__getattribute__(self_, attr)  # Errors here are from the import two lines above (in trace)
 
                 except Exception:
                     raise
 
                 finally:
                     self.on_load()
 
             def __delattr__(self_, attr):
                 return _LazyModule.__delattr__(self_,  attr)
 
         module.__class__ = LazyModule
-
```

### Comparing `lazi-1.0.4/lazi/core/util.py` & `lazi-1.1.0.post13/lazi/core/util.py`

 * *Files identical despite different names*

### Comparing `lazi-1.0.4/pyproject.toml` & `lazi-1.1.0.post13/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.0.4"
+version = "1.1.0-13"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
@@ -28,14 +28,16 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 django = "^4.2.1"
 requests = "^2.30.0"
 toolz = "^0.12.0"
+rich = "^13.3.5"
+setuptools = "^67.7.2"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 
 
 [build-system]
```

### Comparing `lazi-1.0.4/PKG-INFO` & `lazi-1.1.0.post13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.0.4
+Version: 1.1.0.post13
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: Environment :: Web Environment
```


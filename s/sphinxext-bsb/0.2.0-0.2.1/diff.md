# Comparing `tmp/sphinxext-bsb-0.2.0.tar.gz` & `tmp/sphinxext-bsb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxext-bsb-0.2.0.tar", last modified: Fri Mar  3 16:43:29 2023, max compression
+gzip compressed data, was "sphinxext-bsb-0.2.1.tar", last modified: Thu May 11 11:23:06 2023, max compression
```

## Comparing `sphinxext-bsb-0.2.0.tar` & `sphinxext-bsb-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 16:43:29.374038 sphinxext-bsb-0.2.0/
--rw-rw-rw-   0        0        0     1095 2022-09-01 10:32:49.000000 sphinxext-bsb-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      128 2023-03-03 16:43:29.374038 sphinxext-bsb-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       61 2022-09-01 10:32:49.000000 sphinxext-bsb-0.2.0/README.md
--rw-rw-rw-   0        0        0    12511 2023-03-03 16:42:32.000000 sphinxext-bsb-0.2.0/bsbdocs.py
--rw-rw-rw-   0        0        0      223 2023-03-03 16:42:19.000000 sphinxext-bsb-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-03 16:43:29.374038 sphinxext-bsb-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-03 16:43:29.373040 sphinxext-bsb-0.2.0/sphinxext_bsb.egg-info/
--rw-rw-rw-   0        0        0      128 2023-03-03 16:43:29.000000 sphinxext-bsb-0.2.0/sphinxext_bsb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-03-03 16:43:29.000000 sphinxext-bsb-0.2.0/sphinxext_bsb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 16:43:29.000000 sphinxext-bsb-0.2.0/sphinxext_bsb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-03 16:43:29.000000 sphinxext-bsb-0.2.0/sphinxext_bsb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-03 16:43:29.000000 sphinxext-bsb-0.2.0/sphinxext_bsb.egg-info/top_level.txt
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-05-11 11:23:05.950919 sphinxext-bsb-0.2.1/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     1074 2022-08-31 13:26:49.000000 sphinxext-bsb-0.2.1/LICENSE
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      123 2023-05-11 11:23:05.939931 sphinxext-bsb-0.2.1/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       59 2022-08-31 13:26:49.000000 sphinxext-bsb-0.2.1/README.md
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    12453 2023-05-11 11:21:26.000000 sphinxext-bsb-0.2.1/bsbdocs.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      223 2023-05-11 11:22:55.000000 sphinxext-bsb-0.2.1/pyproject.toml
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-05-11 11:23:05.951917 sphinxext-bsb-0.2.1/setup.cfg
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-05-11 11:23:05.927928 sphinxext-bsb-0.2.1/sphinxext_bsb.egg-info/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      123 2023-05-11 11:23:05.000000 sphinxext-bsb-0.2.1/sphinxext_bsb.egg-info/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      227 2023-05-11 11:23:05.000000 sphinxext-bsb-0.2.1/sphinxext_bsb.egg-info/SOURCES.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        1 2023-05-11 11:23:05.000000 sphinxext-bsb-0.2.1/sphinxext_bsb.egg-info/dependency_links.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       14 2023-05-11 11:23:05.000000 sphinxext-bsb-0.2.1/sphinxext_bsb.egg-info/requires.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        8 2023-05-11 11:23:05.000000 sphinxext-bsb-0.2.1/sphinxext_bsb.egg-info/top_level.txt
```

### Comparing `sphinxext-bsb-0.2.0/LICENSE` & `sphinxext-bsb-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Robin De Schepper
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Robin De Schepper
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sphinxext-bsb-0.2.0/bsbdocs.py` & `sphinxext-bsb-0.2.1/bsbdocs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,31 +12,28 @@
 from bsb.config.parsers import get_parser_classes
 from bsb.config.types import class_
 from docutils import nodes
 from docutils.parsers.rst import Directive
 from docutils.statemachine import StringList
 from sphinx.util.docutils import SphinxDirective
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 def example_function():
     pass
 
 
-example_function.__module__ = "my_module"
-example_function.__name__ = "my_function"
-
 _example_values = {
     bool: True,
     list: [],
     str: "example",
     int: 42,
     float: 3.14,
-    FunctionType: example_function,
+    FunctionType: "my_module.my_function",
     dict: {},
 }
 
 
 class ComponentIntro(Directive):
     has_content = False
 
@@ -161,22 +158,25 @@
             # has the "no-imports" option set, which disables the prepended import stmnt
             if "no-imports" in self.options or any(
                 m.startswith("_") for m in type_.__module__.split(".")
             ):
                 untree = self.private_untree(type_)
             else:
                 untree = self.public_untree(type_)
-            # Configuration lists and dicts should be packed into a list/dict
-            if isinstance(attr, ConfigurationListAttribute):
-                untree = self.list_untree(untree)
-            elif isinstance(attr, ConfigurationDictAttribute):
-                untree = self.dict_untree(untree)
-            return (untree, self.guess_example(type_, deeper - 1))
+            value = self.guess_example(type_, deeper - 1)
         else:
-            return (self.argument_untree, self.guess_example_value(attr))
+            untree = self.argument_untree
+            value = self.guess_example_value(attr)
+        # Configuration lists and dicts should be packed into a list/dict
+        if isinstance(attr, ConfigurationListAttribute):
+            untree = self.list_untree(untree)
+        elif isinstance(attr, ConfigurationDictAttribute):
+            untree = self.dict_untree(untree)
+        return untree, value
+
 
     def guess_example_value(self, attr):
         type_ = self.get_attr_type(attr)
         # The attribute may have a hinted example from the declaration `hint` kwarg,
         # or from the `__hint__` method of its type handler
         hint = attr.get_hint()
         if hint is not MISSING:
```


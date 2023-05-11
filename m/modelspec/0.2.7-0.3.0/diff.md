# Comparing `tmp/modelspec-0.2.7.tar.gz` & `tmp/modelspec-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelspec-0.2.7.tar", last modified: Wed Jan 18 12:04:50 2023, max compression
+gzip compressed data, was "modelspec-0.3.0.tar", last modified: Thu May 11 16:03:07 2023, max compression
```

## Comparing `modelspec-0.2.7.tar` & `modelspec-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,45 @@
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2023-01-18 12:04:50.390624 modelspec-0.2.7/
--rw-r--r--   0 padraig    (501) staff       (20)    11357 2022-03-15 15:04:33.000000 modelspec-0.2.7/LICENSE
--rw-r--r--   0 padraig    (501) staff       (20)     2005 2023-01-18 12:04:50.390869 modelspec-0.2.7/PKG-INFO
--rw-r--r--   0 padraig    (501) staff       (20)      589 2022-04-05 09:52:45.000000 modelspec-0.2.7/README.md
--rw-r--r--   0 padraig    (501) staff       (20)      146 2022-03-28 16:41:55.000000 modelspec-0.2.7/pyproject.toml
--rw-r--r--   0 padraig    (501) staff       (20)     2676 2023-01-18 12:04:50.391959 modelspec-0.2.7/setup.cfg
--rw-r--r--   0 padraig    (501) staff       (20)      817 2022-12-05 12:05:04.000000 modelspec-0.2.7/setup.py
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2023-01-18 12:04:50.383662 modelspec-0.2.7/src/
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2023-01-18 12:04:50.388600 modelspec-0.2.7/src/modelspec/
--rw-r--r--   0 padraig    (501) staff       (20)      198 2022-08-08 11:04:35.000000 modelspec-0.2.7/src/modelspec/__init__.py
--rw-r--r--   0 padraig    (501) staff       (20)    34436 2022-08-12 11:46:01.000000 modelspec-0.2.7/src/modelspec/base_types.py
--rw-r--r--   0 padraig    (501) staff       (20)    10647 2022-07-29 11:53:13.000000 modelspec-0.2.7/src/modelspec/utils.py
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2023-01-18 12:04:50.390360 modelspec-0.2.7/src/modelspec.egg-info/
--rw-r--r--   0 padraig    (501) staff       (20)     2005 2023-01-18 12:04:50.000000 modelspec-0.2.7/src/modelspec.egg-info/PKG-INFO
--rw-r--r--   0 padraig    (501) staff       (20)      312 2023-01-18 12:04:50.000000 modelspec-0.2.7/src/modelspec.egg-info/SOURCES.txt
--rw-r--r--   0 padraig    (501) staff       (20)        1 2023-01-18 12:04:50.000000 modelspec-0.2.7/src/modelspec.egg-info/dependency_links.txt
--rw-r--r--   0 padraig    (501) staff       (20)      848 2023-01-18 12:04:50.000000 modelspec-0.2.7/src/modelspec.egg-info/requires.txt
--rw-r--r--   0 padraig    (501) staff       (20)       10 2023-01-18 12:04:50.000000 modelspec-0.2.7/src/modelspec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.418286 modelspec-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.414286 modelspec-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.414286 modelspec-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-11 16:02:55.000000 modelspec-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 16:02:55.000000 modelspec-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-11 16:02:55.000000 modelspec-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-11 16:02:55.000000 modelspec-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 16:02:55.000000 modelspec-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-11 16:03:07.418286 modelspec-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-11 16:02:55.000000 modelspec-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.418286 modelspec-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.bson
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.specification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/document.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.418286 modelspec-0.3.0/examples/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/test/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/test/test.specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 16:02:55.000000 modelspec-0.3.0/examples/test/test_instance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-11 16:02:55.000000 modelspec-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-11 16:03:07.418286 modelspec-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-11 16:02:55.000000 modelspec-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.414286 modelspec-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.418286 modelspec-0.3.0/src/modelspec/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-11 16:02:55.000000 modelspec-0.3.0/src/modelspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-11 16:02:55.000000 modelspec-0.3.0/src/modelspec/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-05-11 16:02:55.000000 modelspec-0.3.0/src/modelspec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.418286 modelspec-0.3.0/src/modelspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-11 16:03:07.000000 modelspec-0.3.0/src/modelspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-11 16:03:07.000000 modelspec-0.3.0/src/modelspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:03:07.000000 modelspec-0.3.0/src/modelspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-11 16:03:07.000000 modelspec-0.3.0/src/modelspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 16:03:07.000000 modelspec-0.3.0/src/modelspec.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      146 2023-05-11 16:02:55.000000 modelspec-0.3.0/test_all.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.418286 modelspec-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:03:07.418286 modelspec-0.3.0/tests/temp/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 16:02:55.000000 modelspec-0.3.0/tests/temp/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-05-11 16:02:55.000000 modelspec-0.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-11 16:02:55.000000 modelspec-0.3.0/tests/test_utils.py
```

### Comparing `modelspec-0.2.7/LICENSE` & `modelspec-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelspec-0.2.7/PKG-INFO` & `modelspec-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 Metadata-Version: 2.1
 Name: modelspec
-Version: 0.2.7
+Version: 0.3.0
 Summary: A common JSON/YAML based format for compact model specification
 Home-page: https://github.com/ModECI/modelspec
 Author: Padraig Gleeson; ...
 Author-email: p.gleeson@gmail.com
 Maintainer: Padraig Gleeson; ...
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
-Description: # Modelspec
-        
-        
-        [![Continuous builds](https://github.com/ModECI/modelspec/actions/workflows/ci.yml/badge.svg)](https://github.com/ModECI/modelspec/actions/workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/modelspec)](https://pypi.org/project/modelspec/)
-        
-        
-        Functionality for specifying the structure of models & enabling automatic serialization to them (e.g. in JSON and YAML format).
-        
-        This package is being used by [NeuroMLlite](https://github.com/NeuroML/NeuroMLlite) & [MDF](https://github.com/ModECI/MDF).
-        
-        For an example of the use of this package see [here](examples/README.md).
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
@@ -40,7 +27,20 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
+License-File: LICENSE
+
+# Modelspec
+
+
+[![Continuous builds](https://github.com/ModECI/modelspec/actions/workflows/ci.yml/badge.svg)](https://github.com/ModECI/modelspec/actions/workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/modelspec)](https://pypi.org/project/modelspec/)
+
+
+Functionality for specifying the structure of models & enabling automatic serialization to them (e.g. in JSON and YAML format).
+
+This package is being used by [NeuroMLlite](https://github.com/NeuroML/NeuroMLlite) & [MDF](https://github.com/ModECI/MDF).
+
+For an example of the use of this package see [here](examples/README.md).
```

### Comparing `modelspec-0.2.7/README.md` & `modelspec-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.2.7/setup.cfg` & `modelspec-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelspec-0.2.7/setup.py` & `modelspec-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `modelspec-0.2.7/src/modelspec/base_types.py` & `modelspec-0.3.0/src/modelspec/base_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,19 +201,21 @@
         Returns:
             A YAML string representation of the object.
         """
         return yaml.dump(
             yaml_converter.unstructure(self.to_dict()), sort_keys=False, indent=4
         )
 
-    def to_yaml_file(self, filename: str, include_metadata: bool = True) -> str:
+    def to_yaml_file(
+        self, filename: Optional[str] = None, include_metadata: Optional[bool] = True
+    ) -> str:
         """Convert modelspec format to yaml format
 
         Args:
-            filename: File in modelspec format (Filename extension: .yaml )
+            filename: File in modelspec format (Filename extension: .yaml). If None, use :code:`f"{self.id}.yaml"`
             include_metadata: Contains contact information, citations, acknowledgements, pointers to sample data,
                               benchmark results, and environments in which the specified model was originally implemented
         Returns:
             The name of the generated yaml file
         """
 
         if filename is None:
@@ -580,15 +582,15 @@
                 f"Unknown format: '{format}', recognised formats: '{ALL_FORMATS}''"
             )
 
         definition = cls._parse_definition()
         allowed_fields = cls._parse_allowed_fields()
         allowed_children = cls._parse_allowed_children()
 
-        print(f" - {cls.__name__} ({definition})")
+        # print(f" - {cls.__name__} ({definition})")
 
         rst_url_format = "`%s <%s>`__"
 
         def insert_links(text, format=MARKDOWN_FORMAT):
 
             code_ref = ":code:`"
             # print("    > Converting: %s" % text)
@@ -689,15 +691,15 @@
         referenced = []
 
         for f, (description, type_) in allowed_fields.items():
             referencable = not Base._is_base_type(
                 type_, can_be_eval_expr=True, can_be_dict=True
             )
             type_str = Base._type_to_str(type_)
-            print("    Allowed parameter: {} {}".format(f, (description, type_str)))
+            # print("    Allowed parameter: {} {}".format(f, (description, type_str)))
 
             if format == DICT_FORMAT:
                 doc_dict[name]["allowed_parameters"][f] = {}
                 doc_dict[name]["allowed_parameters"][f]["type"] = type_str
                 doc_dict[name]["allowed_parameters"][f]["description"] = description
 
             elif format == MARKDOWN_FORMAT:
@@ -746,15 +748,15 @@
                 doc_string += "%s\n\n" % (ap)
                 table_info = []
             elif format == DICT_FORMAT:
                 doc_dict[name]["allowed_children"] = {}
 
         for c, (description, type_) in allowed_children.items():
             type_str = Base._type_to_str(type_)
-            print("    Allowed child: {} {}".format(c, (description, type_str)))
+            # print("    Allowed child: {} {}".format(c, (description, type_str)))
 
             referencable = not Base._is_base_type(type_, can_be_dict=True)
 
             if format == DICT_FORMAT:
                 doc_dict[name]["allowed_children"][c] = {}
                 doc_dict[name]["allowed_children"][c]["type"] = type_str
                 doc_dict[name]["allowed_children"][c]["description"] = allowed_children[
```

### Comparing `modelspec-0.2.7/src/modelspec/utils.py` & `modelspec-0.3.0/src/modelspec/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,53 @@
 import os
 import math
 import numpy as np
 
 from modelspec.base_types import print_
 from modelspec.base_types import EvaluableExpression
 
+from random import Random
+from typing import Union
+
 verbose = False
 
 
-def load_json(filename):
+def load_json(filename: str):
     """
     Load a generic JSON file
+
+    Args:
+        filename: The name of the JSON file to load
     """
 
     with open(filename) as f:
         data = json.load(f, object_hook=ascii_encode_dict)
 
     return data
 
 
-def load_yaml(filename):
+def load_yaml(filename: str):
     """
     Load a generic YAML file
+
+    Args:
+        filename: The name of the YAML file to load
     """
     with open(filename) as f:
         data = yaml.load(f, Loader=yaml.SafeLoader)
 
     return data
 
 
-def load_bson(filename):
+def load_bson(filename: str):
     """
     Load a generic BSON file
+
+    Args:
+        filename: The name of the BSON file to load
     """
     with open(filename, "rb") as infile:
         data_encoded = infile.read()
         data = bson.decode(data_encoded)
 
     return data
 
@@ -207,19 +219,34 @@
 
 
 # Ideas in development...
 FORMAT_NUMPY = "numpy"
 FORMAT_TENSORFLOW = "tensorflow"
 
 
-def evaluate(expr, parameters={}, rng=None, array_format=FORMAT_NUMPY, verbose=False):
+def evaluate(
+    expr: Union[int, float, str, list, dict],
+    parameters: dict = {},
+    rng: Random = None,
+    array_format: str = FORMAT_NUMPY,
+    verbose: bool = False,
+    cast_to_int: bool = False,
+):
     """
     Evaluate a general string like expression (e.g. "2 * weight") using a dict
     of parameters (e.g. {'weight':10}). Returns floats, ints, etc. if that's what's
     given in expr
+
+    Args:
+        expr: The expression to convert
+        parameters: A dict of the parameters which can be substituted in to the expression
+        rng: The random number generator to use
+        array_format: numpy or tensorflow
+        verbose: Print the calculations
+        cast_to_int: return an int for float/string values if castable
     """
 
     if array_format == FORMAT_TENSORFLOW:
         import tensorflow as tf
 
     if verbose:
         print_(
@@ -229,105 +256,108 @@
         )
     try:
         if type(expr) == str and expr in parameters:
             expr = parameters[
                 expr
             ]  # replace with the value in parameters & check whether it's float/int...
             if verbose:
-                print_("Using for that param: %s" % _val_info(expr), verbose)
+                print_("   Using for that param: %s" % _val_info(expr), verbose)
 
         if type(expr) == str:
             try:
                 if array_format == FORMAT_TENSORFLOW:
                     expr = tf.constant(int(expr))
                 else:
                     expr = int(expr)
             except:
-                pass
-            try:
-                if array_format == FORMAT_TENSORFLOW:
-                    expr = tf.constant(float(expr))
-                else:
-                    expr = float(expr)
-            except:
-                pass
+
+                try:
+                    if array_format == FORMAT_TENSORFLOW:
+                        expr = tf.constant(float(expr))
+                    else:
+                        expr = float(expr)
+                except:
+                    pass
 
         if type(expr) == list:
             if verbose:
-                print_("Returning a list in format: %s" % array_format, verbose)
+                print_("   Returning a list in format: %s" % array_format, verbose)
             if array_format == FORMAT_TENSORFLOW:
                 return tf.constant(expr, dtype=tf.float64)
             else:
                 return np.array(expr)
 
         if type(expr) == np.ndarray:
             if verbose:
-                print_("Returning a numpy array in format: %s" % array_format, verbose)
+                print_(
+                    "   Returning a numpy array in format: %s" % array_format, verbose
+                )
             if array_format == FORMAT_TENSORFLOW:
                 return tf.convert_to_tensor(expr, dtype=tf.float64)
             else:
                 return np.array(expr)
 
         if "Tensor" in type(expr).__name__:
             if verbose:
                 print_(
-                    "Returning a tensorflow Tensor in format: %s" % array_format,
+                    "   Returning a tensorflow Tensor in format: %s" % array_format,
                     verbose,
                 )
             if array_format == FORMAT_NUMPY:
                 return expr.numpy()
             else:
                 return expr
 
-        if int(expr) == expr:
+        if int(expr) == expr and cast_to_int:
             if verbose:
-                print_("Returning int: %s" % int(expr), verbose)
+                print_("   Returning int: %s" % int(expr), verbose)
             return int(expr)
         else:  # will have failed if not number
             if verbose:
-                print_("Returning float: %s" % expr, verbose)
-            return float(expr)
+                print_("   Returning {}: {}".format(type(expr), expr), verbose)
+            return expr
     except:
         try:
             if rng:
                 expr = expr.replace("random()", "rng.random()")
                 parameters["rng"] = rng
 
             if type(expr) == str and "math." in expr:
                 parameters["math"] = math
             if type(expr) == str and "numpy." in expr:
                 parameters["numpy"] = np
 
             if verbose:
                 print_(
-                    "Trying to eval [%s] with Python using %s..."
+                    "   Trying to eval [%s] with Python using %s..."
                     % (expr, parameters.keys()),
                     verbose,
                 )
 
             v = eval(expr, parameters)
 
             if verbose:
                 print_(
-                    "Evaluated with Python: {} = {}".format(expr, _val_info(v)), verbose
+                    "   Evaluated with Python: {} = {}".format(expr, _val_info(v)),
+                    verbose,
                 )
 
             if (type(v) == float or type(v) == str) and int(v) == v:
 
                 if verbose:
-                    print_("Returning int: %s" % int(v), verbose)
+                    print_("   Returning int: %s" % int(v), verbose)
 
                 if array_format == FORMAT_TENSORFLOW:
                     return tf.constant(int(v))
                 else:
                     return int(v)
             return v
         except Exception as e:
             if verbose:
-                print_(f"Returning without altering: {expr} (error: {e})", verbose)
+                print_(f"   Returning without altering: {expr} (error: {e})", verbose)
             return expr
 
 
 """
     Translates a string like '3', '[0,2]' to a list
 """
```

### Comparing `modelspec-0.2.7/src/modelspec.egg-info/PKG-INFO` & `modelspec-0.3.0/src/modelspec.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 Metadata-Version: 2.1
 Name: modelspec
-Version: 0.2.7
+Version: 0.3.0
 Summary: A common JSON/YAML based format for compact model specification
 Home-page: https://github.com/ModECI/modelspec
 Author: Padraig Gleeson; ...
 Author-email: p.gleeson@gmail.com
 Maintainer: Padraig Gleeson; ...
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
-Description: # Modelspec
-        
-        
-        [![Continuous builds](https://github.com/ModECI/modelspec/actions/workflows/ci.yml/badge.svg)](https://github.com/ModECI/modelspec/actions/workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/modelspec)](https://pypi.org/project/modelspec/)
-        
-        
-        Functionality for specifying the structure of models & enabling automatic serialization to them (e.g. in JSON and YAML format).
-        
-        This package is being used by [NeuroMLlite](https://github.com/NeuroML/NeuroMLlite) & [MDF](https://github.com/ModECI/MDF).
-        
-        For an example of the use of this package see [here](examples/README.md).
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
@@ -40,7 +27,20 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
+License-File: LICENSE
+
+# Modelspec
+
+
+[![Continuous builds](https://github.com/ModECI/modelspec/actions/workflows/ci.yml/badge.svg)](https://github.com/ModECI/modelspec/actions/workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/modelspec)](https://pypi.org/project/modelspec/)
+
+
+Functionality for specifying the structure of models & enabling automatic serialization to them (e.g. in JSON and YAML format).
+
+This package is being used by [NeuroMLlite](https://github.com/NeuroML/NeuroMLlite) & [MDF](https://github.com/ModECI/MDF).
+
+For an example of the use of this package see [here](examples/README.md).
```

### Comparing `modelspec-0.2.7/src/modelspec.egg-info/requires.txt` & `modelspec-0.3.0/src/modelspec.egg-info/requires.txt`

 * *Files identical despite different names*


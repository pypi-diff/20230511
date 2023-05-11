# Comparing `tmp/kgcl_rdflib-0.4.0rc1.tar.gz` & `tmp/kgcl_rdflib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcl_rdflib-0.4.0rc1.tar", max compression
+gzip compressed data, was "kgcl_rdflib-0.5.0.tar", max compression
```

## Comparing `kgcl_rdflib-0.4.0rc1.tar` & `kgcl_rdflib-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-05-08 22:55:06.123477 kgcl_rdflib-0.4.0rc1/LICENSE
--rw-r--r--   0        0        0      380 2023-05-08 22:55:06.123477 kgcl_rdflib-0.4.0rc1/README.md
--rw-r--r--   0        0        0     7695 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/README.md
--rw-r--r--   0        0        0        0 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/__init__.py
--rw-r--r--   0        0        0      540 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/graph_transformer.py
--rw-r--r--   0        0        0    65986 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/kgcl_2_sparql.py
--rw-r--r--   0        0        0        0 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/__init__.py
--rw-r--r--   0        0        0    13033 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/change_detection.py
--rw-r--r--   0        0        0     5831 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_existential.py
--rw-r--r--   0        0        0    21085 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_single.py
--rw-r--r--   0        0        0     7591 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py
--rw-r--r--   0        0        0     3538 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/graph_diff.py
--rw-r--r--   0        0        0    11823 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/owlstar_sublanguage.py
--rw-r--r--   0        0        0    12052 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/pretty_print_kgcl.py
--rw-r--r--   0        0        0     8080 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/render_operations.py
--rw-r--r--   0        0        0     5531 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/summary_generation.py
--rw-r--r--   0        0        0     1560 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl.py
--rw-r--r--   0        0        0     7952 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl_diff.py
--rw-r--r--   0        0        0     6145 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/render_kgcl.py
--rw-r--r--   0        0        0      798 2023-05-08 22:55:46.003692 kgcl_rdflib-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 kgcl_rdflib-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-11 21:29:53.029876 kgcl_rdflib-0.5.0/LICENSE
+-rw-r--r--   0        0        0      380 2023-05-11 21:29:53.029876 kgcl_rdflib-0.5.0/README.md
+-rw-r--r--   0        0        0     7695 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/apply/__init__.py
+-rw-r--r--   0        0        0      540 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/apply/graph_transformer.py
+-rw-r--r--   0        0        0    65986 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/apply/kgcl_2_sparql.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/__init__.py
+-rw-r--r--   0        0        0    13033 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/change_detection.py
+-rw-r--r--   0        0        0     5831 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/diff_2_kgcl_existential.py
+-rw-r--r--   0        0        0    21085 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/diff_2_kgcl_single.py
+-rw-r--r--   0        0        0     7591 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py
+-rw-r--r--   0        0        0     3538 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/graph_diff.py
+-rw-r--r--   0        0        0    11823 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/owlstar_sublanguage.py
+-rw-r--r--   0        0        0    12052 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/pretty_print_kgcl.py
+-rw-r--r--   0        0        0     8080 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/render_operations.py
+-rw-r--r--   0        0        0     5531 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/diff/summary_generation.py
+-rw-r--r--   0        0        0     1560 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/kgcl.py
+-rw-r--r--   0        0        0     7952 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/kgcl_diff.py
+-rw-r--r--   0        0        0     6145 2023-05-11 21:29:53.033876 kgcl_rdflib-0.5.0/kgcl_rdflib/render_kgcl.py
+-rw-r--r--   0        0        0      796 2023-05-11 21:30:35.789765 kgcl_rdflib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1046 1970-01-01 00:00:00.000000 kgcl_rdflib-0.5.0/PKG-INFO
```

### Comparing `kgcl_rdflib-0.4.0rc1/LICENSE` & `kgcl_rdflib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/README.md` & `kgcl_rdflib-0.5.0/kgcl_rdflib/README.md`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/graph_transformer.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/apply/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/kgcl_2_sparql.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/apply/kgcl_2_sparql.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/change_detection.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/change_detection.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_existential.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/diff_2_kgcl_existential.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_single.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/diff_2_kgcl_single.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/graph_diff.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/graph_diff.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/owlstar_sublanguage.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/owlstar_sublanguage.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/pretty_print_kgcl.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/pretty_print_kgcl.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/render_operations.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/render_operations.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/summary_generation.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/diff/summary_generation.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/kgcl.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl_diff.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/kgcl_diff.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/render_kgcl.py` & `kgcl_rdflib-0.5.0/kgcl_rdflib/render_kgcl.py`

 * *Files identical despite different names*

### Comparing `kgcl_rdflib-0.4.0rc1/pyproject.toml` & `kgcl_rdflib-0.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 [tool.poetry]
 name = "kgcl-rdflib"
-version = "v0.4.0-rc1"
+version = "v0.5.0"
 description = "Schema for the KGCL project."
 authors = [
     "Christian Kindermann <christian.kindermann@postgrad.manchester.ac.uk>",
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>"
     ]
 license = "MIT"
 readme = "README.md"
-
+packages = [{include = "kgcl_rdflib"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-linkml-runtime = "^1.1.24"
-lark = "^1.1.2"
-kgcl-schema = "0.4.0-rc1"
-
-[tool.poetry.dev-dependencies]
-linkml = "^1.2.15"
-mkdocs-material = "^8.2.8"
-pytest = "^7.1.2"
+linkml-runtime = ">=1.1.24"
+kgcl-schema = ">=0.5.0"
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry.group.dev.dependencies]
+mkdocs-material = "^9.1.11"
+pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 kgcl-diff = "kgcl.kgcl_diff:cli"
 kgcl-apply = "kgcl.kgcl:cli"
 kgcl-parse = "kgcl.grammar.parser:cli"
 
 [tool.poetry.extras]
 docs = ["linkml", "mkdocs-material"]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `kgcl_rdflib-0.4.0rc1/PKG-INFO` & `kgcl_rdflib-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: kgcl-rdflib
-Version: 0.4.0rc1
+Version: 0.5.0
 Summary: Schema for the KGCL project.
 License: MIT
 Author: Christian Kindermann
 Author-email: christian.kindermann@postgrad.manchester.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: kgcl-schema (==0.4.0-rc1)
-Requires-Dist: lark (>=1.1.2,<2.0.0)
-Requires-Dist: linkml-runtime (>=1.1.24,<2.0.0)
+Requires-Dist: kgcl-schema (>=0.5.0)
+Requires-Dist: linkml-runtime (>=1.1.24)
 Description-Content-Type: text/markdown
 
 # kgcl-rdflib
 
 An engine that applies changes or diffs specified in KGCL to an RDF graph stored using rdflib
 
 ## KGCL
```


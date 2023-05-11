# Comparing `tmp/rdflib_ocdm-0.1.1.tar.gz` & `tmp/rdflib_ocdm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdflib_ocdm-0.1.1.tar", max compression
+gzip compressed data, was "rdflib_ocdm-0.2.0.tar", max compression
```

## Comparing `rdflib_ocdm-0.1.1.tar` & `rdflib_ocdm-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      497 2023-05-11 10:57:10.371486 rdflib_ocdm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      840 2023-04-20 10:05:30.759897 rdflib_ocdm-0.1.1/rdflib_ocdm/__init__.py
--rw-r--r--   0        0        0     6176 2023-04-19 10:29:03.161700 rdflib_ocdm-0.1.1/rdflib_ocdm/abstract_entity.py
--rw-r--r--   0        0        0      839 2023-04-14 08:27:27.373276 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     2444 2023-04-14 08:14:45.294985 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0     5349 2023-04-14 08:28:09.422946 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0     3119 2023-04-14 08:28:16.301132 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     3589 2023-05-11 10:55:37.891219 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     4600 2023-04-18 15:55:19.068117 rdflib_ocdm-0.1.1/rdflib_ocdm/ocdm_graph.py
--rw-r--r--   0        0        0      839 2023-04-14 08:14:45.296986 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-19 11:46:36.923513 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0     7604 2023-04-19 10:32:08.234267 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/provenance.py
--rw-r--r--   0        0        0    13514 2023-04-19 09:56:14.655005 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/snapshot_entity.py
--rw-r--r--   0        0        0     4447 2023-04-19 11:43:30.274044 rdflib_ocdm-0.1.1/rdflib_ocdm/query_utils.py
--rw-r--r--   0        0        0     2077 2023-04-18 13:52:43.532866 rdflib_ocdm-0.1.1/rdflib_ocdm/reader.py
--rw-r--r--   0        0        0     4905 2023-04-19 10:53:30.709617 rdflib_ocdm-0.1.1/rdflib_ocdm/storer.py
--rw-r--r--   0        0        0     2570 2023-04-19 10:34:23.494049 rdflib_ocdm-0.1.1/rdflib_ocdm/support.py
--rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.1.1/README.md
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 rdflib_ocdm-0.1.1/setup.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 rdflib_ocdm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      497 2023-05-11 11:41:27.372364 rdflib_ocdm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      840 2023-04-20 10:05:30.759897 rdflib_ocdm-0.2.0/rdflib_ocdm/__init__.py
+-rw-r--r--   0        0        0     6176 2023-04-19 10:29:03.161700 rdflib_ocdm-0.2.0/rdflib_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0      839 2023-04-14 08:27:27.373276 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     2444 2023-04-14 08:14:45.294985 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0     5349 2023-04-14 08:28:09.422946 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0     3119 2023-04-14 08:28:16.301132 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     3589 2023-05-11 10:55:37.891219 rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     4600 2023-04-18 15:55:19.068117 rdflib_ocdm-0.2.0/rdflib_ocdm/ocdm_graph.py
+-rw-r--r--   0        0        0      839 2023-04-14 08:14:45.296986 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0     2906 2023-04-19 11:46:36.923513 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0     7604 2023-04-19 10:32:08.234267 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/provenance.py
+-rw-r--r--   0        0        0    13514 2023-04-19 09:56:14.655005 rdflib_ocdm-0.2.0/rdflib_ocdm/prov/snapshot_entity.py
+-rw-r--r--   0        0        0     4447 2023-04-19 11:43:30.274044 rdflib_ocdm-0.2.0/rdflib_ocdm/query_utils.py
+-rw-r--r--   0        0        0     2259 2023-05-11 11:36:15.565333 rdflib_ocdm-0.2.0/rdflib_ocdm/reader.py
+-rw-r--r--   0        0        0     4905 2023-04-19 10:53:30.709617 rdflib_ocdm-0.2.0/rdflib_ocdm/storer.py
+-rw-r--r--   0        0        0     2570 2023-04-19 10:34:23.494049 rdflib_ocdm-0.2.0/rdflib_ocdm/support.py
+-rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.2.0/README.md
+-rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.0/setup.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 rdflib_ocdm-0.2.0/PKG-INFO
```

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/__init__.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/abstract_entity.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/__init__.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/counter_handler.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/ocdm_graph.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/ocdm_graph.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/__init__.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/prov_entity.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/provenance.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/provenance.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/snapshot_entity.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/prov/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/query_utils.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/query_utils.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/reader.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
 # OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
 # DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
 # ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
 # SOFTWARE.
 from __future__ import annotations
 
+from typing import List
+
 from oc_ocdm.support.reporter import Reporter
 from rdflib import ConjunctiveGraph, URIRef
-from SPARQLWrapper import JSON, SPARQLWrapper
+from SPARQLWrapper import POST, XML, SPARQLWrapper
 
 from rdflib_ocdm.ocdm_graph import OCDMGraph
 
 
 class Reader(object):
     def __init__(self, repok: Reporter = None, reperr: Reporter = None):
         if repok is None:
@@ -31,18 +33,24 @@
 
         if reperr is None:
             self.reperr: Reporter = Reporter(prefix="[Reader: ERROR] ")
         else:
             self.reperr: Reporter = reperr
 
     @staticmethod
-    def import_entity_from_triplestore(ocdm_graph: OCDMGraph, ts_url: str, res: URIRef) -> URIRef:
+    def import_entities_from_triplestore(ocdm_graph: OCDMGraph, ts_url: str, res_list: List[URIRef]) -> URIRef:
         sparql: SPARQLWrapper = SPARQLWrapper(ts_url)
-        query: str = f"CONSTRUCT {{<{res}> ?p ?o}} WHERE {{<{res}> ?p ?o}}"
+        query: str = f'''
+            CONSTRUCT {{?s ?p ?o}} 
+            WHERE {{
+                ?s ?p ?o. 
+                VALUES ?s {{<{'> <'.join(res_list)}>}}
+        }}'''
         sparql.setQuery(query)
-        sparql.setMethod('GET')
-        result: ConjunctiveGraph = sparql.query().convert()
+        sparql.setMethod(POST)
+        sparql.setReturnFormat(XML)
+        result: ConjunctiveGraph = sparql.queryAndConvert()
         if result is not None:
             for triple in result.triples((None, None, None)):
                 ocdm_graph.add(triple)
         else:
-            raise ValueError(f"The entity {res} was not found.")
+            raise ValueError(f"An entity was not found.")
```

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/storer.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/storer.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/rdflib_ocdm/support.py` & `rdflib_ocdm-0.2.0/rdflib_ocdm/support.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/README.md` & `rdflib_ocdm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.1/setup.py` & `rdflib_ocdm-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['oc-ocdm>=7.1.7,<8.0.0', 'rdflib>=6.2.0,<7.0.0', 'sparqlwrapper>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'rdflib-ocdm',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': '',
     'long_description': '[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/rdflib-ocdm/main/test/coverage/coverage.svg)\n![PyPI](https://img.shields.io/pypi/pyversions/rdflib-ocdm)\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/rdflib-ocdm)\n\n# rdflib-ocdm\n',
     'author': 'arcangelo7',
     'author_email': 'arcangelomas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rdflib_ocdm-0.1.1/PKG-INFO` & `rdflib_ocdm-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdflib-ocdm
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/rdflib_ocdm-0.1.0.tar.gz` & `tmp/rdflib_ocdm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdflib_ocdm-0.1.0.tar", max compression
+gzip compressed data, was "rdflib_ocdm-0.1.1.tar", max compression
```

## Comparing `rdflib_ocdm-0.1.0.tar` & `rdflib_ocdm-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      497 2023-04-20 10:01:07.654957 rdflib_ocdm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      840 2023-04-20 10:05:30.759897 rdflib_ocdm-0.1.0/rdflib_ocdm/__init__.py
--rw-r--r--   0        0        0     6176 2023-04-19 10:29:03.161700 rdflib_ocdm-0.1.0/rdflib_ocdm/abstract_entity.py
--rw-r--r--   0        0        0      839 2023-04-14 08:27:27.373276 rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     2444 2023-04-14 08:14:45.294985 rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0     5349 2023-04-14 08:28:09.422946 rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0     3119 2023-04-14 08:28:16.301132 rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     3506 2023-04-14 08:28:21.508383 rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     4600 2023-04-18 15:55:19.068117 rdflib_ocdm-0.1.0/rdflib_ocdm/ocdm_graph.py
--rw-r--r--   0        0        0      839 2023-04-14 08:14:45.296986 rdflib_ocdm-0.1.0/rdflib_ocdm/prov/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-19 11:46:36.923513 rdflib_ocdm-0.1.0/rdflib_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0     7604 2023-04-19 10:32:08.234267 rdflib_ocdm-0.1.0/rdflib_ocdm/prov/provenance.py
--rw-r--r--   0        0        0    13514 2023-04-19 09:56:14.655005 rdflib_ocdm-0.1.0/rdflib_ocdm/prov/snapshot_entity.py
--rw-r--r--   0        0        0     4447 2023-04-19 11:43:30.274044 rdflib_ocdm-0.1.0/rdflib_ocdm/query_utils.py
--rw-r--r--   0        0        0     2077 2023-04-18 13:52:43.532866 rdflib_ocdm-0.1.0/rdflib_ocdm/reader.py
--rw-r--r--   0        0        0     4905 2023-04-19 10:53:30.709617 rdflib_ocdm-0.1.0/rdflib_ocdm/storer.py
--rw-r--r--   0        0        0     2570 2023-04-19 10:34:23.494049 rdflib_ocdm-0.1.0/rdflib_ocdm/support.py
--rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.1.0/README.md
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 rdflib_ocdm-0.1.0/setup.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 rdflib_ocdm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      497 2023-05-11 10:57:10.371486 rdflib_ocdm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      840 2023-04-20 10:05:30.759897 rdflib_ocdm-0.1.1/rdflib_ocdm/__init__.py
+-rw-r--r--   0        0        0     6176 2023-04-19 10:29:03.161700 rdflib_ocdm-0.1.1/rdflib_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0      839 2023-04-14 08:27:27.373276 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     2444 2023-04-14 08:14:45.294985 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0     5349 2023-04-14 08:28:09.422946 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0     3119 2023-04-14 08:28:16.301132 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     3589 2023-05-11 10:55:37.891219 rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     4600 2023-04-18 15:55:19.068117 rdflib_ocdm-0.1.1/rdflib_ocdm/ocdm_graph.py
+-rw-r--r--   0        0        0      839 2023-04-14 08:14:45.296986 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0     2906 2023-04-19 11:46:36.923513 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0     7604 2023-04-19 10:32:08.234267 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/provenance.py
+-rw-r--r--   0        0        0    13514 2023-04-19 09:56:14.655005 rdflib_ocdm-0.1.1/rdflib_ocdm/prov/snapshot_entity.py
+-rw-r--r--   0        0        0     4447 2023-04-19 11:43:30.274044 rdflib_ocdm-0.1.1/rdflib_ocdm/query_utils.py
+-rw-r--r--   0        0        0     2077 2023-04-18 13:52:43.532866 rdflib_ocdm-0.1.1/rdflib_ocdm/reader.py
+-rw-r--r--   0        0        0     4905 2023-04-19 10:53:30.709617 rdflib_ocdm-0.1.1/rdflib_ocdm/storer.py
+-rw-r--r--   0        0        0     2570 2023-04-19 10:34:23.494049 rdflib_ocdm-0.1.1/rdflib_ocdm/support.py
+-rw-r--r--   0        0        0      600 2023-04-20 10:52:06.623319 rdflib_ocdm-0.1.1/README.md
+-rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 rdflib_ocdm-0.1.1/setup.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 rdflib_ocdm-0.1.1/PKG-INFO
```

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/__init__.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/abstract_entity.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/__init__.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/counter_handler.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/filesystem_counter_handler.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/in_memory_counter_handler.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/counter_handler/sqlite_counter_handler.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
 # OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
 # DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
 # ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
 # SOFTWARE.
 
 import sqlite3
+import urllib.parse
 
 from rdflib_ocdm.counter_handler.counter_handler import CounterHandler
 
 
 class SqliteCounterHandler(CounterHandler):
     """A concrete implementation of the ``CounterHandler`` interface that persistently stores
     the counter values within a SQLite database."""
@@ -44,29 +45,29 @@
         :param new_value: The new counter value to be set
         :type new_value: int
         :param entity_name: The entity name
         :type entity_name: str
         :raises ValueError: if ``new_value`` is a negative integer.
         :return: None
         """
-        entity_name = str(entity_name)
+        entity_name = urllib.parse.quote((str(entity_name)))
         if new_value < 0:
             raise ValueError("new_value must be a non negative integer!")
         self.cur.execute(f"INSERT OR REPLACE INTO info (entity, count) VALUES ('{entity_name}', {new_value})")
         self.con.commit()
 
     def read_counter(self, entity_name: str) -> int:
         """
         It allows to read the counter value of provenance entities.
 
         :param entity_name: The entity name
         :type entity_name: str
         :return: The requested counter value.
         """
-        entity_name = str(entity_name)
+        entity_name = urllib.parse.quote(str(entity_name))
         result = self.cur.execute(f"SELECT count FROM info WHERE entity='{entity_name}'")
         rows = result.fetchall()
         if len(rows) == 1:
             return rows[0][0]
         elif len(rows) == 0:
             return 0
         else:
@@ -76,12 +77,12 @@
         """
         It allows to increment the counter value of graph and provenance entities by one unit.
 
         :param entity_name: The entity name
         :type entity_name: str
         :return: The newly-updated (already incremented) counter value.
         """
-        entity_name = str(entity_name)
+        entity_name = urllib.parse.quote(str(entity_name))
         cur_count = self.read_counter(entity_name)
         count = cur_count + 1
         self.set_counter(count, entity_name)
         return count
```

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/ocdm_graph.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/ocdm_graph.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/prov/__init__.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/prov/prov_entity.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/prov/provenance.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/provenance.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/prov/snapshot_entity.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/prov/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/query_utils.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/query_utils.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/reader.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/reader.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/storer.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/storer.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/rdflib_ocdm/support.py` & `rdflib_ocdm-0.1.1/rdflib_ocdm/support.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/README.md` & `rdflib_ocdm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.1.0/setup.py` & `rdflib_ocdm-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['oc-ocdm>=7.1.7,<8.0.0', 'rdflib>=6.2.0,<7.0.0', 'sparqlwrapper>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'rdflib-ocdm',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/rdflib-ocdm/main/test/coverage/coverage.svg)\n![PyPI](https://img.shields.io/pypi/pyversions/rdflib-ocdm)\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/rdflib-ocdm)\n\n# rdflib-ocdm\n',
     'author': 'arcangelo7',
     'author_email': 'arcangelomas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rdflib_ocdm-0.1.0/PKG-INFO` & `rdflib_ocdm-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdflib-ocdm
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```


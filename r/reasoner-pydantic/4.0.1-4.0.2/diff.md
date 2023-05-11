# Comparing `tmp/reasoner-pydantic-4.0.1.tar.gz` & `tmp/reasoner-pydantic-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.1.tar", last modified: Tue May  9 19:52:45 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.2.tar", last modified: Thu May 11 17:40:46 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.1.tar` & `reasoner-pydantic-4.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:45.884259 reasoner-pydantic-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-09 19:52:45.884259 reasoner-pydantic-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:45.880259 reasoner-pydantic-4.0.1/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:45.880259 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:52:45.884259 reasoner-pydantic-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:40:46.253917 reasoner-pydantic-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-11 17:40:46.253917 reasoner-pydantic-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:40:46.253917 reasoner-pydantic-4.0.2/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:40:46.253917 reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-11 17:40:46.000000 reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-11 17:40:46.000000 reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:40:46.000000 reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:40:46.000000 reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 17:40:46.000000 reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 17:40:46.000000 reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 17:40:46.253917 reasoner-pydantic-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-11 17:40:42.000000 reasoner-pydantic-4.0.2/setup.py
```

### Comparing `reasoner-pydantic-4.0.1/PKG-INFO` & `reasoner-pydantic-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.1
+Version: 4.0.2
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.1/README.md` & `reasoner-pydantic-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .kgraph import KnowledgeGraph, Node, Edge
 from .qgraph import (
     QueryGraph,
     QNode,
     QEdge,
     AttributeConstraint,
 )
-from .results import Result, NodeBinding, EdgeBinding, Results
+from .results import Result, NodeBinding, EdgeBinding, Results, Analysis
 from .auxgraphs import AuxiliaryGraphs, AuxiliaryGraph
 from .message import (
     Message,
     Query,
     Response,
     AsyncQuery,
 )
@@ -60,8 +60,11 @@
     MetaEdge,
     MetaNode,
     MetaKnowledgeGraph,
     MetaAttribute,
     Results,
     AuxiliaryGraph,
     AuxiliaryGraphs,
+    Operation,
+    Workflow,
+    Analysis,
 ]
```

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/message.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/message.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/results.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/results.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.2/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.1
+Version: 4.0.2
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.2/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.1/setup.py` & `reasoner-pydantic-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.1",
+    version="4.0.2",
     author="Kenneth Morton",
     author_email="kenny@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```


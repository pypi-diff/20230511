# Comparing `tmp/paperscraper-0.2.6.tar.gz` & `tmp/paperscraper-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperscraper-0.2.6.tar", last modified: Sun May  7 22:40:04 2023, max compression
+gzip compressed data, was "paperscraper-0.2.7.tar", last modified: Wed May 10 22:10:05 2023, max compression
```

## Comparing `paperscraper-0.2.6.tar` & `paperscraper-0.2.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-05-07 22:39:50.000000 paperscraper-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-05-07 22:40:04.292587 paperscraper-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10554 2023-05-07 22:39:50.000000 paperscraper-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.284587 paperscraper-0.2.6/paperscraper/
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/arxiv/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/arxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/arxiv/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/arxiv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/get_dumps/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1484 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/biorxiv.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/chemrxiv.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1508 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/medrxiv.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/get_dumps/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/journal_if.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/load_dumps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/pubmed/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pubmed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pubmed/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pubmed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/scholar/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/scholar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3140 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/scholar/scholar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/server_dumps/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/server_dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/xrxiv/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/xrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-07 22:40:04.292587 paperscraper-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-05-07 22:39:50.000000 paperscraper-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.358510 paperscraper-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-05-10 22:09:54.000000 paperscraper-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-05-10 22:10:05.358510 paperscraper-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10554 2023-05-10 22:09:54.000000 paperscraper-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.350510 paperscraper-0.2.7/paperscraper/
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/arxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/arxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/arxiv/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/arxiv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/get_dumps/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1484 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/biorxiv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/chemrxiv.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1508 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/medrxiv.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/get_dumps/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/get_dumps/utils/chemrxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/utils/chemrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4166 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/get_dumps/utils/chemrxiv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/journal_if.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/load_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/pubmed/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/pubmed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/pubmed/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/pubmed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/scholar/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/scholar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3140 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/scholar/scholar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/server_dumps/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/server_dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper/xrxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/xrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/xrxiv/xrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-05-10 22:09:54.000000 paperscraper-0.2.7/paperscraper/xrxiv/xrxiv_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 22:10:05.354510 paperscraper-0.2.7/paperscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-05-10 22:10:05.000000 paperscraper-0.2.7/paperscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-10 22:10:05.000000 paperscraper-0.2.7/paperscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 22:10:05.000000 paperscraper-0.2.7/paperscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 22:10:05.000000 paperscraper-0.2.7/paperscraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-10 22:10:05.000000 paperscraper-0.2.7/paperscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-10 22:10:05.000000 paperscraper-0.2.7/paperscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 22:10:05.358510 paperscraper-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-05-10 22:09:54.000000 paperscraper-0.2.7/setup.py
```

### Comparing `paperscraper-0.2.6/LICENSE` & `paperscraper-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/PKG-INFO` & `paperscraper-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.6
+Version: 0.2.7
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paperscraper-0.2.6/README.md` & `paperscraper-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/__init__.py` & `paperscraper-0.2.7/paperscraper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Initialize the module."""
 __name__ = "paperscraper"
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 import logging
 import os
 import sys
 from typing import List, Union
 
 from .load_dumps import QUERY_FN_DICT
```

### Comparing `paperscraper-0.2.6/paperscraper/arxiv/arxiv.py` & `paperscraper-0.2.7/paperscraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/arxiv/utils.py` & `paperscraper-0.2.7/paperscraper/arxiv/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/get_dumps/biorxiv.py` & `paperscraper-0.2.7/paperscraper/get_dumps/biorxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/get_dumps/chemrxiv.py` & `paperscraper-0.2.7/paperscraper/get_dumps/chemrxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/get_dumps/medrxiv.py` & `paperscraper-0.2.7/paperscraper/get_dumps/medrxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py` & `paperscraper-0.2.7/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import os
 import sys
 from datetime import datetime
 from typing import Dict, Optional
+from urllib.parse import urljoin
 
 import requests
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 logger = logging.getLogger(__name__)
 
 now_datetime = datetime.now()
@@ -14,15 +15,15 @@
 
 
 class ChemrxivAPI:
     """Handle OpenEngage API requests, using access.
     Adapted from https://github.com/fxcoudert/tools/blob/master/chemRxiv/chemRxiv.py.
     """
 
-    base = "https://chemrxiv.org/engage/chemrxiv/public-api/v1"
+    base = "https://chemrxiv.org/engage/chemrxiv/public-api/v1/"
 
     def __init__(
         self,
         begin_date: Optional[str] = None,
         end_date: Optional[str] = None,
         page_size: Optional[int] = None,
     ):
@@ -74,17 +75,16 @@
         elif method.casefold() == "post":
             return requests.post(url, json=params)
         else:
             raise ConnectionError(f"Unknown method for query: {method}")
 
     def query(self, query, method="get", params=None):
         """Perform a direct query."""
-        r = self.request(
-            os.path.join(f"{self.base}", f"{query}"), method, params=params
-        )
+
+        r = self.request(urljoin(self.base, query), method, params=params)
         r.raise_for_status()
         return r.json()
 
     def query_generator(self, query, method: str = "get", params: Dict = {}):
         """Query for a list of items, with paging. Returns a generator."""
 
         page = 0
@@ -93,15 +93,15 @@
                 {
                     "limit": self.page_size,
                     "skip": page * self.page_size,
                     "searchDateFrom": self.begin_date,
                     "searchDateTo": self.end_date,
                 }
             )
-            r = self.request(os.path.join(self.base, query), method, params=params)
+            r = self.request(urljoin(self.base, query), method, params=params)
             if r.status_code == 400:
                 raise ValueError(r.json()["message"])
             r.raise_for_status()
             r = r.json()
             r = r["itemHits"]
 
             # If we have no more results, bail out
```

### Comparing `paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/utils.py` & `paperscraper-0.2.7/paperscraper/get_dumps/utils/chemrxiv/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/journal_if.py` & `paperscraper-0.2.7/paperscraper/journal_if.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/load_dumps.py` & `paperscraper-0.2.7/paperscraper/load_dumps.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/pdf.py` & `paperscraper-0.2.7/paperscraper/pdf.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/plotting.py` & `paperscraper-0.2.7/paperscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/postprocessing.py` & `paperscraper-0.2.7/paperscraper/postprocessing.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/pubmed/pubmed.py` & `paperscraper-0.2.7/paperscraper/pubmed/pubmed.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/pubmed/utils.py` & `paperscraper-0.2.7/paperscraper/pubmed/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/scholar/scholar.py` & `paperscraper-0.2.7/paperscraper/scholar/scholar.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/utils.py` & `paperscraper-0.2.7/paperscraper/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_api.py` & `paperscraper-0.2.7/paperscraper/xrxiv/xrxiv_api.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_query.py` & `paperscraper-0.2.7/paperscraper/xrxiv/xrxiv_query.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/paperscraper.egg-info/PKG-INFO` & `paperscraper-0.2.7/paperscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.6
+Version: 0.2.7
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paperscraper-0.2.6/paperscraper.egg-info/SOURCES.txt` & `paperscraper-0.2.7/paperscraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.6/setup.py` & `paperscraper-0.2.7/setup.py`

 * *Files identical despite different names*


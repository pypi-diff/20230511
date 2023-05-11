# Comparing `tmp/tgclients-0.8.0.tar.gz` & `tmp/tgclients-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgclients-0.8.0.tar", last modified: Wed Jan 11 11:12:54 2023, max compression
+gzip compressed data, was "tgclients-0.9.0.tar", last modified: Fri Jan 13 15:17:15 2023, max compression
```

## Comparing `tgclients-0.8.0.tar` & `tgclients-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 11:12:54.621536 tgclients-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-01-11 11:12:42.000000 tgclients-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2799 2023-01-11 11:12:54.621536 tgclients-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-01-11 11:12:42.000000 tgclients-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-01-11 11:12:42.000000 tgclients-0.8.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1874 2023-01-11 11:12:54.621536 tgclients-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-01-11 11:12:42.000000 tgclients-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 11:12:54.613536 tgclients-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 11:12:54.617536 tgclients-0.8.0/src/tgclients/
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-01-11 11:12:51.000000 tgclients-0.8.0/src/tgclients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/aggregator.py
--rw-rw-rw-   0 root         (0) root         (0)     9075 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     3768 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/config.py
--rw-rw-rw-   0 root         (0) root         (0)    11063 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/crud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 11:12:54.617536 tgclients-0.8.0/src/tgclients/databinding/
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/databinding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/databinding/rdf.py
--rw-rw-rw-   0 root         (0) root         (0)    36404 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/databinding/textgrid_metadata_2010.py
--rw-rw-rw-   0 root         (0) root         (0)    25581 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/databinding/textgrid_metadata_agent_2010.py
--rw-rw-rw-   0 root         (0) root         (0)     7273 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/databinding/textgrid_metadata_script_2010.py
--rw-rw-rw-   0 root         (0) root         (0)    10256 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/databinding/tgsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     9089 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    24799 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/mime.types
--rw-rw-rw-   0 root         (0) root         (0)    17660 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 11:12:54.621536 tgclients-0.8.0/src/tgclients/templates/
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/templates/aggregation.xml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/templates/aggregation.xml.jinja2.license
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/templates/metadata.xml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/templates/metadata.xml.jinja2.license
--rw-rw-rw-   0 root         (0) root         (0)     5502 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/tgfilenames.rules
--rw-rw-rw-   0 root         (0) root         (0)     1766 2023-01-11 11:12:42.000000 tgclients-0.8.0/src/tgclients/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 11:12:54.617536 tgclients-0.8.0/src/tgclients.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2799 2023-01-11 11:12:54.000000 tgclients-0.8.0/src/tgclients.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      963 2023-01-11 11:12:54.000000 tgclients-0.8.0/src/tgclients.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 11:12:54.000000 tgclients-0.8.0/src/tgclients.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      289 2023-01-11 11:12:54.000000 tgclients-0.8.0/src/tgclients.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-11 11:12:54.000000 tgclients-0.8.0/src/tgclients.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:17:15.905694 tgclients-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-01-13 15:17:03.000000 tgclients-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-01-13 15:17:15.905694 tgclients-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-01-13 15:17:03.000000 tgclients-0.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-01-13 15:17:03.000000 tgclients-0.9.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-01-13 15:17:15.905694 tgclients-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-01-13 15:17:03.000000 tgclients-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:17:15.901694 tgclients-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:17:15.905694 tgclients-0.9.0/src/tgclients/
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-01-13 15:17:12.000000 tgclients-0.9.0/src/tgclients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/aggregator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9075 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     3768 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11063 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/crud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:17:15.905694 tgclients-0.9.0/src/tgclients/databinding/
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/databinding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/databinding/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    36404 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/databinding/textgrid_metadata_2010.py
+-rw-rw-rw-   0 root         (0) root         (0)    25581 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/databinding/textgrid_metadata_agent_2010.py
+-rw-rw-rw-   0 root         (0) root         (0)     7273 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/databinding/textgrid_metadata_script_2010.py
+-rw-rw-rw-   0 root         (0) root         (0)    10256 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/databinding/tgsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     7270 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    24799 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/mime.types
+-rw-rw-rw-   0 root         (0) root         (0)    17660 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:17:15.905694 tgclients-0.9.0/src/tgclients/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/templates/aggregation.xml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/templates/aggregation.xml.jinja2.license
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/templates/metadata.xml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/templates/metadata.xml.jinja2.license
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/tgfilenames.rules
+-rw-rw-rw-   0 root         (0) root         (0)     1766 2023-01-13 15:17:03.000000 tgclients-0.9.0/src/tgclients/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:17:15.905694 tgclients-0.9.0/src/tgclients.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-01-13 15:17:15.000000 tgclients-0.9.0/src/tgclients.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      963 2023-01-13 15:17:15.000000 tgclients-0.9.0/src/tgclients.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 15:17:15.000000 tgclients-0.9.0/src/tgclients.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2023-01-13 15:17:15.000000 tgclients-0.9.0/src/tgclients.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-01-13 15:17:15.000000 tgclients-0.9.0/src/tgclients.egg-info/top_level.txt
```

### Comparing `tgclients-0.8.0/LICENSE` & `tgclients-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/PKG-INFO` & `tgclients-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: tgclients
-Version: 0.8.0
+Version: 0.9.0
 Summary: TextGrid Python client library for textgrid.de repository access.
 Home-page: https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients
 Author: Stefan Hynek, Ubbo Veentjer
 License: LGPL
 Project-URL: Documentation, https://dariah-de.pages.gwdg.de/textgridrep/textgrid-python-clients/docs/index.html
 Project-URL: Source, https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients
 Project-URL: Tracker, https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients/-/issues
 Project-URL: Changelog, https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients/-/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: icu
 Provides-Extra: docs
 License-File: LICENSE
 
 <!--
```

### Comparing `tgclients-0.8.0/README.md` & `tgclients-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/setup.cfg` & `tgclients-0.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 project_urls = 
 	Documentation = https://dariah-de.pages.gwdg.de/textgridrep/textgrid-python-clients/docs/index.html
 	Source = https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients
 	Tracker = https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients/-/issues
 	Changelog = https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients/-/blob/main/CHANGELOG.md
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.7
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	requests
 	requests-toolbelt
 	jinja2
```

### Comparing `tgclients-0.8.0/src/tgclients/__init__.py` & `tgclients-0.9.0/src/tgclients/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Georg-August-Universität Göttingen
 #
 # SPDX-License-Identifier: CC0-1.0
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 from tgclients.aggregator import (
     Aggregator,
 )
 from tgclients.auth import (
     TextgridAuth,
     TextgridAuthException,
```

### Comparing `tgclients-0.8.0/src/tgclients/aggregator.py` & `tgclients-0.9.0/src/tgclients/aggregator.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/auth.py` & `tgclients-0.9.0/src/tgclients/auth.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/config.py` & `tgclients-0.9.0/src/tgclients/config.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/crud.py` & `tgclients-0.9.0/src/tgclients/crud.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/databinding/__init__.py` & `tgclients-0.9.0/src/tgclients/databinding/__init__.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/databinding/rdf.py` & `tgclients-0.9.0/src/tgclients/databinding/rdf.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/databinding/textgrid_metadata_2010.py` & `tgclients-0.9.0/src/tgclients/databinding/textgrid_metadata_2010.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/databinding/textgrid_metadata_agent_2010.py` & `tgclients-0.9.0/src/tgclients/databinding/textgrid_metadata_agent_2010.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/databinding/textgrid_metadata_script_2010.py` & `tgclients-0.9.0/src/tgclients/databinding/textgrid_metadata_script_2010.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/databinding/tgsearch.py` & `tgclients-0.9.0/src/tgclients/databinding/tgsearch.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/mime.types` & `tgclients-0.9.0/src/tgclients/mime.types`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/search.py` & `tgclients-0.9.0/src/tgclients/search.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/tgfilenames.rules` & `tgclients-0.9.0/src/tgclients/tgfilenames.rules`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients/utils.py` & `tgclients-0.9.0/src/tgclients/utils.py`

 * *Files identical despite different names*

### Comparing `tgclients-0.8.0/src/tgclients.egg-info/PKG-INFO` & `tgclients-0.9.0/src/tgclients.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: tgclients
-Version: 0.8.0
+Version: 0.9.0
 Summary: TextGrid Python client library for textgrid.de repository access.
 Home-page: https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients
 Author: Stefan Hynek, Ubbo Veentjer
 License: LGPL
 Project-URL: Documentation, https://dariah-de.pages.gwdg.de/textgridrep/textgrid-python-clients/docs/index.html
 Project-URL: Source, https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients
 Project-URL: Tracker, https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients/-/issues
 Project-URL: Changelog, https://gitlab.gwdg.de/dariah-de/textgridrep/textgrid-python-clients/-/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: icu
 Provides-Extra: docs
 License-File: LICENSE
 
 <!--
```

### Comparing `tgclients-0.8.0/src/tgclients.egg-info/SOURCES.txt` & `tgclients-0.9.0/src/tgclients.egg-info/SOURCES.txt`

 * *Files identical despite different names*


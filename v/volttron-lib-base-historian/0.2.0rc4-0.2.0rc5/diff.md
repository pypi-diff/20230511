# Comparing `tmp/volttron_lib_base_historian-0.2.0rc4.tar.gz` & `tmp/volttron_lib_base_historian-0.2.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_base_historian-0.2.0rc4.tar", max compression
+gzip compressed data, was "volttron_lib_base_historian-0.2.0rc5.tar", max compression
```

## Comparing `volttron_lib_base_historian-0.2.0rc4.tar` & `volttron_lib_base_historian-0.2.0rc5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11928 2023-05-09 22:27:38.306139 volttron_lib_base_historian-0.2.0rc4/LICENSE
--rw-r--r--   0        0        0     2871 2023-05-09 22:27:38.306139 volttron_lib_base_historian-0.2.0rc4/README.md
--rw-r--r--   0        0        0     1278 2023-05-09 22:28:57.419412 volttron_lib_base_historian-0.2.0rc4/pyproject.toml
--rw-r--r--   0        0        0     1250 2023-05-09 22:27:38.306139 volttron_lib_base_historian-0.2.0rc4/src/historian/base/__init__.py
--rw-r--r--   0        0        0    96502 2023-05-09 22:27:38.306139 volttron_lib_base_historian-0.2.0rc4/src/historian/base/base_historian.py
--rw-r--r--   0        0        0        0 2023-05-09 22:27:38.310139 volttron_lib_base_historian-0.2.0rc4/tests/historian/testing/__init__.py
--rw-r--r--   0        0        0    20260 2023-05-09 22:27:38.310139 volttron_lib_base_historian-0.2.0rc4/tests/historian/testing/integration_test_interface.py
--rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc4/setup.py
--rw-r--r--   0        0        0     3627 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-11 21:16:38.148425 volttron_lib_base_historian-0.2.0rc5/LICENSE
+-rw-r--r--   0        0        0     2871 2023-05-11 21:16:38.148425 volttron_lib_base_historian-0.2.0rc5/README.md
+-rw-r--r--   0        0        0     1278 2023-05-11 21:18:18.561777 volttron_lib_base_historian-0.2.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     1250 2023-05-11 21:16:38.152425 volttron_lib_base_historian-0.2.0rc5/src/historian/base/__init__.py
+-rw-r--r--   0        0        0    96502 2023-05-11 21:16:38.152425 volttron_lib_base_historian-0.2.0rc5/src/historian/base/base_historian.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:16:38.152425 volttron_lib_base_historian-0.2.0rc5/tests/historian/testing/__init__.py
+-rw-r--r--   0        0        0    20260 2023-05-11 21:16:38.152425 volttron_lib_base_historian-0.2.0rc5/tests/historian/testing/integration_test_interface.py
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc5/setup.py
+-rw-r--r--   0        0        0     3627 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.0rc5/PKG-INFO
```

### Comparing `volttron_lib_base_historian-0.2.0rc4/LICENSE` & `volttron_lib_base_historian-0.2.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc4/README.md` & `volttron_lib_base_historian-0.2.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc4/pyproject.toml` & `volttron_lib_base_historian-0.2.0rc5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-lib-base-historian"
-version = "0.2.0rc4"
+version = "0.2.0rc5"
 description = "A base library with extension points for using with the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-base-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-base-historian"
 keywords = []
```

### Comparing `volttron_lib_base_historian-0.2.0rc4/src/historian/base/__init__.py` & `volttron_lib_base_historian-0.2.0rc5/src/historian/base/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc4/src/historian/base/base_historian.py` & `volttron_lib_base_historian-0.2.0rc5/src/historian/base/base_historian.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc4/tests/historian/testing/integration_test_interface.py` & `volttron_lib_base_historian-0.2.0rc5/tests/historian/testing/integration_test_interface.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.0rc4/setup.py` & `volttron_lib_base_historian-0.2.0rc5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['ply>=3.11,<4.0', 'volttron>=10.0.3a9,<11.0']
 
 setup_kwargs = {
     'name': 'volttron-lib-base-historian',
-    'version': '0.2.0rc4',
+    'version': '0.2.0rc5',
     'description': 'A base library with extension points for using with the VOLTTRON platform.',
     'long_description': '[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Run Pytests](https://github.com/eclipse-volttron/volttron-lib-base-historian/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-lib-base-historian/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-lib-base-historian.svg)](https://pypi.org/project/volttron-lib-base-historian/)\n\nVOLTTRON base historian framework that provide common functions such as caching, error handling, input validation etc. This historian cannot be used as agent as is. VOLTTRON historian agents can be created by subclassing the [BaseHistorian class](https://github.com/eclipse-volttron/volttron-lib-base-historian/blob/develop/src/historian/base/base_historian.py) in this library.\n\n## Requirements\n\n - Python >= 3.10\n\n## Installation\n\nThis library can be installed using ```pip install volttron-lib-base-historian```. However, this is not necessary. Any \nhistorian agent that uses this library will automatically install it as part of its installation. For example, \ninstalling [SQLiteHistorian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) will automatically install \nvolttron-lib-base-historian into the same python environment\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
     'author': 'VOLTTRON Team',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/eclipse-volttron/volttron-lib-base-historian',
```

### Comparing `volttron_lib_base_historian-0.2.0rc4/PKG-INFO` & `volttron_lib_base_historian-0.2.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-base-historian
-Version: 0.2.0rc4
+Version: 0.2.0rc5
 Summary: A base library with extension points for using with the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-base-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


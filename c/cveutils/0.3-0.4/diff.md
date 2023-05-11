# Comparing `tmp/cveutils-0.3.tar.gz` & `tmp/cveutils-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cveutils-0.3.tar", last modified: Thu May 11 04:33:52 2023, max compression
+gzip compressed data, was "cveutils-0.4.tar", last modified: Thu May 11 05:21:30 2023, max compression
```

## Comparing `cveutils-0.3.tar` & `cveutils-0.4.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:33:52.313009 cveutils-0.3/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2020 2023-05-11 04:33:52.312350 cveutils-0.3/PKG-INFO
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1670 2023-05-11 04:22:48.000000 cveutils-0.3/README.md
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:33:52.309350 cveutils-0.3/cveutils.egg-info/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2020 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/PKG-INFO
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      206 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/SOURCES.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/dependency_links.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/requires.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/top_level.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:19:26.000000 cveutils-0.3/pyproject.toml
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 04:33:52.313009 cveutils-0.3/setup.cfg
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      673 2023-05-11 04:33:38.000000 cveutils-0.3/setup.py
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:33:52.311349 cveutils-0.3/tests/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 04:01:48.000000 cveutils-0.3/tests/test.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:21:30.090154 cveutils-0.4/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1065 2023-05-11 05:12:53.000000 cveutils-0.4/LICENSE
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2325 2023-05-11 05:21:30.089134 cveutils-0.4/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1953 2023-05-11 05:12:53.000000 cveutils-0.4/README.md
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:12:53.000000 cveutils-0.4/pyproject.toml
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 05:21:30.091148 cveutils-0.4/setup.cfg
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      654 2023-05-11 05:19:03.000000 cveutils-0.4/setup.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:21:30.069677 cveutils-0.4/src/
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:21:30.079751 cveutils-0.4/src/cveutils/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:15:45.000000 cveutils-0.4/src/cveutils/__init__.py
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     3231 2023-05-11 05:15:38.000000 cveutils-0.4/src/cveutils/cveutils.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:21:30.086749 cveutils-0.4/src/cveutils.egg-info/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2325 2023-05-11 05:21:29.000000 cveutils-0.4/src/cveutils.egg-info/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      284 2023-05-11 05:21:30.000000 cveutils-0.4/src/cveutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 05:21:29.000000 cveutils-0.4/src/cveutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 05:21:29.000000 cveutils-0.4/src/cveutils.egg-info/requires.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 05:21:29.000000 cveutils-0.4/src/cveutils.egg-info/top_level.txt
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:21:30.087751 cveutils-0.4/tests/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 05:12:53.000000 cveutils-0.4/tests/test.py
```

### Comparing `cveutils-0.3/PKG-INFO` & `cveutils-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: cveutils
-Version: 0.3
+Version: 0.4
 Summary: This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
 Author: Vinicius Pereira (big0us)
 Author-email: vini@cius.xyz
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # cveutils
+![logo](https://raw.githubusercontent.com/viniciuspereiras/cveutils/main/static/logo.png)
+
+[![PyPI](https://img.shields.io/pypi/v/cveutils?style=flat)](https://pypi.python.org/pypi/cveutils/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
 This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
-## Requirements
-This library requires the requests module and the datetime module.
+## Instalation
+```bash
+pip install cveutils
+```
 ## Usage
 To use this library, simply import the CVE class and initialize an instance with a CVE ID as a string.
 
 ```python
 
-from cve import CVE
+from cveutils import CVE
 
 cve = CVE('CVE-2021-12345')
 ```
 ### CVE Object
 
 The `CVE` object has the following attributes:
 - `ID`: The CVE ID
```

### Comparing `cveutils-0.3/README.md` & `cveutils-0.4/src/cveutils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,33 @@
+Metadata-Version: 2.1
+Name: cveutils
+Version: 0.4
+Summary: This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
+Author: Vinicius Pereira (big0us)
+Author-email: vini@cius.xyz
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cveutils
+![logo](https://raw.githubusercontent.com/viniciuspereiras/cveutils/main/static/logo.png)
+
+[![PyPI](https://img.shields.io/pypi/v/cveutils?style=flat)](https://pypi.python.org/pypi/cveutils/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
 This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
-## Requirements
-This library requires the requests module and the datetime module.
+## Instalation
+```bash
+pip install cveutils
+```
 ## Usage
 To use this library, simply import the CVE class and initialize an instance with a CVE ID as a string.
 
 ```python
 
-from cve import CVE
+from cveutils import CVE
 
 cve = CVE('CVE-2021-12345')
 ```
 ### CVE Object
 
 The `CVE` object has the following attributes:
 - `ID`: The CVE ID
```

### Comparing `cveutils-0.3/cveutils.egg-info/PKG-INFO` & `cveutils-0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1
-Name: cveutils
-Version: 0.3
-Summary: This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
-Author: Vinicius Pereira (big0us)
-Author-email: vini@cius.xyz
-Description-Content-Type: text/markdown
-
 # cveutils
+![logo](https://raw.githubusercontent.com/viniciuspereiras/cveutils/main/static/logo.png)
+
+[![PyPI](https://img.shields.io/pypi/v/cveutils?style=flat)](https://pypi.python.org/pypi/cveutils/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
 This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
-## Requirements
-This library requires the requests module and the datetime module.
+## Instalation
+```bash
+pip install cveutils
+```
 ## Usage
 To use this library, simply import the CVE class and initialize an instance with a CVE ID as a string.
 
 ```python
 
-from cve import CVE
+from cveutils import CVE
 
 cve = CVE('CVE-2021-12345')
 ```
 ### CVE Object
 
 The `CVE` object has the following attributes:
 - `ID`: The CVE ID
```

### Comparing `cveutils-0.3/setup.py` & `cveutils-0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 import os
 
-# ... other setup code ...
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='cveutils',
-    version='0.3',
+    version='0.4',
     description='This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.',
     author='Vinicius Pereira (big0us)',
     author_email='vini@cius.xyz',
-    packages=find_packages(exclude=['tests']),
+    package_dir={'': 'src'},
+    packages=['cveutils'],
     install_requires=[
         'requests',
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```


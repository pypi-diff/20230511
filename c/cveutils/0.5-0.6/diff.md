# Comparing `tmp/cveutils-0.5.tar.gz` & `tmp/cveutils-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cveutils-0.5.tar", last modified: Thu May 11 05:25:06 2023, max compression
+gzip compressed data, was "cveutils-0.6.tar", last modified: Thu May 11 06:03:45 2023, max compression
```

## Comparing `cveutils-0.5.tar` & `cveutils-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:25:06.621732 cveutils-0.5/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1065 2023-05-11 05:12:53.000000 cveutils-0.5/LICENSE
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2325 2023-05-11 05:25:06.620732 cveutils-0.5/PKG-INFO
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1953 2023-05-11 05:12:53.000000 cveutils-0.5/README.md
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:12:53.000000 cveutils-0.5/pyproject.toml
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 05:25:06.621732 cveutils-0.5/setup.cfg
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      654 2023-05-11 05:24:48.000000 cveutils-0.5/setup.py
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:25:06.603326 cveutils-0.5/src/
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:25:06.609825 cveutils-0.5/src/cveutils/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     3231 2023-05-11 05:24:41.000000 cveutils-0.5/src/cveutils/__init__.py
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:25:06.617839 cveutils-0.5/src/cveutils.egg-info/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2325 2023-05-11 05:25:06.000000 cveutils-0.5/src/cveutils.egg-info/PKG-INFO
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      259 2023-05-11 05:25:06.000000 cveutils-0.5/src/cveutils.egg-info/SOURCES.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 05:25:06.000000 cveutils-0.5/src/cveutils.egg-info/dependency_links.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 05:25:06.000000 cveutils-0.5/src/cveutils.egg-info/requires.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 05:25:06.000000 cveutils-0.5/src/cveutils.egg-info/top_level.txt
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:25:06.619703 cveutils-0.5/tests/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 05:12:53.000000 cveutils-0.5/tests/test.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 06:03:45.410979 cveutils-0.6/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1065 2023-05-11 05:12:53.000000 cveutils-0.6/LICENSE
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2325 2023-05-11 06:03:45.409981 cveutils-0.6/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1953 2023-05-11 05:12:53.000000 cveutils-0.6/README.md
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 05:12:53.000000 cveutils-0.6/pyproject.toml
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 06:03:45.410979 cveutils-0.6/setup.cfg
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      654 2023-05-11 06:03:14.000000 cveutils-0.6/setup.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 06:03:45.389676 cveutils-0.6/src/
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 06:03:45.399836 cveutils-0.6/src/cveutils/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     3453 2023-05-11 05:51:27.000000 cveutils-0.6/src/cveutils/__init__.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 06:03:45.407984 cveutils-0.6/src/cveutils.egg-info/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2325 2023-05-11 06:03:45.000000 cveutils-0.6/src/cveutils.egg-info/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      259 2023-05-11 06:03:45.000000 cveutils-0.6/src/cveutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 06:03:45.000000 cveutils-0.6/src/cveutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 06:03:45.000000 cveutils-0.6/src/cveutils.egg-info/requires.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 06:03:45.000000 cveutils-0.6/src/cveutils.egg-info/top_level.txt
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 06:03:45.408980 cveutils-0.6/tests/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 05:28:07.000000 cveutils-0.6/tests/test.py
```

### Comparing `cveutils-0.5/LICENSE` & `cveutils-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cveutils-0.5/PKG-INFO` & `cveutils-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cveutils
-Version: 0.5
+Version: 0.6
 Summary: This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
 Author: Vinicius Pereira (big0us)
 Author-email: vini@cius.xyz
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cveutils
```

### Comparing `cveutils-0.5/README.md` & `cveutils-0.6/README.md`

 * *Files identical despite different names*

### Comparing `cveutils-0.5/setup.py` & `cveutils-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='cveutils',
-    version='0.5',
+    version='0.6',
     description='This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.',
     author='Vinicius Pereira (big0us)',
     author_email='vini@cius.xyz',
     package_dir={'': 'src'},
     packages=['cveutils'],
     install_requires=[
         'requests',
```

### Comparing `cveutils-0.5/src/cveutils/__init__.py` & `cveutils-0.6/src/cveutils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     """
     def __getattr__(self, key):
         return self[key]
     
     def __str__(self) -> str:
         return self.baseScore
 
+class CVENotFound(Exception):
+    pass
+
 class CVE:
     """
     A class that represents a CVE
 
     :param CVEID: The CVE ID
     :type CVEID: str
 
@@ -48,14 +51,16 @@
     :vartype references: list
 
     :returns: A CVE object
     """
     def __init__(self, CVEID) -> None:
         self.ID = CVEID
         self.info = self.getCVEInfo()
+        if 'message' in self.info.keys() and 'Unable to find vuln' in self.info['message']:
+            raise CVENotFound('CVE not found')
         self.description = self.info["result"]["CVE_Items"][0]["cve"]["description"]["description_data"][0]["value"]
         self.getCVSS()
         self.published_date = self.publishedDate()
         self.last_modified_date = self.lastModifiedDate()
         self.assigner = self.info["result"]["CVE_Items"][0]["cve"]["CVE_data_meta"]["ASSIGNER"]
         self.references = self.info["result"]["CVE_Items"][0]["cve"]["references"]["reference_data"]
 
@@ -102,8 +107,10 @@
         p = self.info["result"]["CVE_Items"][0]["lastModifiedDate"]
         datetime_obj = datetime.fromisoformat(p[:-1])
         date_str = datetime_obj.date().isoformat()
         return date_str
     
 
 if '__main__' == __name__:
-    pass
+    cve = CVE("CVE-2022-35405")
+
+    print(cve.ID)
```

### Comparing `cveutils-0.5/src/cveutils.egg-info/PKG-INFO` & `cveutils-0.6/src/cveutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cveutils
-Version: 0.5
+Version: 0.6
 Summary: This library provides functionality for fetching and parsing information about Common Vulnerabilities and Exposures (CVE) using the NIST National Vulnerability Database (NVD) RESTful API.
 Author: Vinicius Pereira (big0us)
 Author-email: vini@cius.xyz
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cveutils
```


# Comparing `tmp/pytmv1-0.4.1.tar.gz` & `tmp/pytmv1-0.4.2.tar.gz`

## Comparing `pytmv1-0.4.1.tar` & `pytmv1-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.4.1/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.4.1/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26132 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10922 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/logger.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.4.1/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.4.1/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.4.1/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.4.1/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.4.2/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.4.2/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26132 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10922 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/logger.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.4.2/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.4.2/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.4.2/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.4.2/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.4.2/PKG-INFO
```

### Comparing `pytmv1-0.4.1/src/pytmv1/__init__.py` & `pytmv1-0.4.2/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/caller.py` & `pytmv1-0.4.2/src/pytmv1/caller.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/core.py` & `pytmv1-0.4.2/src/pytmv1/core.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/exceptions.py` & `pytmv1-0.4.2/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/logger.py` & `pytmv1-0.4.2/src/pytmv1/logger.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/mapper.py` & `pytmv1-0.4.2/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/results.py` & `pytmv1-0.4.2/src/pytmv1/results.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/utils.py` & `pytmv1-0.4.2/src/pytmv1/utils.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/model/commons.py` & `pytmv1-0.4.2/src/pytmv1/model/commons.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/model/enums.py` & `pytmv1-0.4.2/src/pytmv1/model/enums.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/model/requests.py` & `pytmv1-0.4.2/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/src/pytmv1/model/responses.py` & `pytmv1-0.4.2/src/pytmv1/model/responses.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/LICENSE.txt` & `pytmv1-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/README.md` & `pytmv1-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.1/pyproject.toml` & `pytmv1-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
     "beautifulsoup4 ~= 4.11.1",
-    "requests ~= 2.28.1",
+    "requests ~= 2.27.1",
     "pydantic ~= 1.10.4",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch ~= 1.6.3",
     "psutil ~= 5.9.4",
```

### Comparing `pytmv1-0.4.1/PKG-INFO` & `pytmv1-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4~=4.11.1
 Requires-Dist: pydantic~=1.10.4
-Requires-Dist: requests~=2.28.1
+Requires-Dist: requests~=2.27.1
 Provides-Extra: dev
 Requires-Dist: hatch~=1.6.3; extra == 'dev'
 Requires-Dist: psutil~=5.9.4; extra == 'dev'
 Requires-Dist: pytest-cov~=4.0.0; extra == 'dev'
 Requires-Dist: pytest-mock~=3.10.0; extra == 'dev'
 Requires-Dist: pytest~=7.2.0; extra == 'dev'
 Description-Content-Type: text/markdown
```


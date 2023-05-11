# Comparing `tmp/pycanha_core-0.0.1.tar.gz` & `tmp/pycanha_core-0.0.2.tar.gz`

## Comparing `pycanha_core-0.0.1.tar` & `pycanha_core-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycanha_core-0.0.1/src/pycanha-core/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pycanha_core-0.0.1/src/pycanha-core/example.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pycanha_core-0.0.1/LICENSE
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pycanha_core-0.0.1/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pycanha_core-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pycanha_core-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycanha_core-0.0.2/src/pycanha-core/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pycanha_core-0.0.2/src/pycanha-core/example.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pycanha_core-0.0.2/LICENSE
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pycanha_core-0.0.2/README.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pycanha_core-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pycanha_core-0.0.2/PKG-INFO
```

### Comparing `pycanha_core-0.0.1/LICENSE` & `pycanha_core-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.1/PKG-INFO` & `pycanha_core-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pycanha-core
-Version: 0.0.1
-Summary: Placeholder for the future PyCanha-core package
-Project-URL: Homepage, https://github.com/pycanha-project/pycanha-core
-Project-URL: Bug Tracker, https://github.com/pycanha-project/pycanha-core/issues
+Version: 0.0.2
+Summary: Python bindings for pycanha-coree
+Project-URL: Homepage, https://github.com/pycanha-project/pycanha-core-python
+Project-URL: Bug Tracker, https://github.com/pycanha-project/pycanha-core-python/issues
 Author-email: Javier Piqueras Carreño <javier.piqueras@upm.es>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
-# pycanha-core
-Future placeholder for the PyCanha-core package
+# pycanha-core-python
+Python bindings for pycanha-core
```


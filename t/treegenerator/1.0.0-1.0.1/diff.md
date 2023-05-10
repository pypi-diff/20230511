# Comparing `tmp/treegenerator-1.0.0.tar.gz` & `tmp/treegenerator-1.0.1.tar.gz`

## Comparing `treegenerator-1.0.0.tar` & `treegenerator-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 treegenerator-1.0.0/docs/index.html
--rw-r--r--   0        0        0    19007 2020-02-02 00:00:00.000000 treegenerator-1.0.0/docs/treegenerator.html
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 treegenerator-1.0.0/src/treegenerator/__init__.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 treegenerator-1.0.0/src/treegenerator/treegenerator.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 treegenerator-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 treegenerator-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 treegenerator-1.0.0/README.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 treegenerator-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 treegenerator-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 treegenerator-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 treegenerator-1.0.1/docs/index.html
+-rw-r--r--   0        0        0    21950 2020-02-02 00:00:00.000000 treegenerator-1.0.1/docs/search.js
+-rw-r--r--   0        0        0    34169 2020-02-02 00:00:00.000000 treegenerator-1.0.1/docs/treegenerator.html
+-rw-r--r--   0        0        0   113383 2020-02-02 00:00:00.000000 treegenerator-1.0.1/docs/treegenerator/treegenerator.html
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 treegenerator-1.0.1/src/treegenerator/__init__.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 treegenerator-1.0.1/src/treegenerator/treegenerator.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 treegenerator-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 treegenerator-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 treegenerator-1.0.1/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 treegenerator-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 treegenerator-1.0.1/PKG-INFO
```

### Comparing `treegenerator-1.0.0/src/treegenerator/treegenerator.py` & `treegenerator-1.0.1/src/treegenerator/treegenerator.py`

 * *Files identical despite different names*

### Comparing `treegenerator-1.0.0/LICENSE.txt` & `treegenerator-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `treegenerator-1.0.0/README.md` & `treegenerator-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `treegenerator-1.0.0/pyproject.toml` & `treegenerator-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "treegenerator"
 authors = [{name="Matt Manes"}]
 description = "Generate a recursive tree diagram given a starting directory or a list of URIs."
-version = "1.0.0"
+version = "1.0.1"
 requires-python = ">=3.10"
 dependencies = [
 
-	"printbuddies~=1.0.0"
+	"printbuddies",
+
+	"pytest"
 ]
 readme = "README.md"
 keywords = [
     "tree",
     "visualization",
     "directory"
 ]
```

### Comparing `treegenerator-1.0.0/PKG-INFO` & `treegenerator-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: treegenerator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate a recursive tree diagram given a starting directory or a list of URIs.
 Project-URL: Homepage, https://github.com/matt-manes/treegenerator
 Project-URL: Documentation, https://github.com/matt-manes/treegenerator/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/treegenerator/tree/main/src/treegenerator
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: directory,tree,visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: printbuddies~=1.0.0
+Requires-Dist: printbuddies
+Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # treegenerator
 Generate a recursive tree diagram given a starting directory or a list of URIs.<br>
 Install with:
 <pre>pip install treegenerator</pre>
 Contains two classes: TreeGenerator and UrlTreeGenerator.<br>
```


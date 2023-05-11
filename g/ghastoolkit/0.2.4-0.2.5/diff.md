# Comparing `tmp/ghastoolkit-0.2.4.tar.gz` & `tmp/ghastoolkit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.2.4.tar", last modified: Fri May  5 21:07:04 2023, max compression
+gzip compressed data, was "ghastoolkit-0.2.5.tar", last modified: Thu May 11 20:38:41 2023, max compression
```

## Comparing `ghastoolkit-0.2.4.tar` & `ghastoolkit-0.2.5.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.420273 ghastoolkit-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-11 20:38:41.420273 ghastoolkit-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:38:41.420273 ghastoolkit-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.412273 ghastoolkit-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.416273 ghastoolkit-0.2.5/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.416273 ghastoolkit-0.2.5/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/codeql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.416273 ghastoolkit-0.2.5/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.416273 ghastoolkit-0.2.5/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.416273 ghastoolkit-0.2.5/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.416273 ghastoolkit-0.2.5/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-11 20:38:41.000000 ghastoolkit-0.2.5/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-11 20:38:41.000000 ghastoolkit-0.2.5/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:38:41.000000 ghastoolkit-0.2.5/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 20:38:41.000000 ghastoolkit-0.2.5/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 20:38:41.000000 ghastoolkit-0.2.5/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:41.420273 ghastoolkit-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-11 20:38:13.000000 ghastoolkit-0.2.5/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.2.4/LICENSE` & `ghastoolkit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/PKG-INFO` & `ghastoolkit-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.4
+Version: 0.2.5
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.4/README.md` & `ghastoolkit-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/pyproject.toml` & `ghastoolkit-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/__init__.py` & `ghastoolkit-0.2.5/src/ghastoolkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -36,7 +36,9 @@
 from ghastoolkit.supplychain.advisories import Advisory
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependency, Dependencies
 from ghastoolkit.supplychain.licensing import Licenses
 
 # CodeQL
 from ghastoolkit.codeql.databases import CodeQLDatabases, CodeQLDatabase
+from ghastoolkit.codeql.cli import CodeQL
+from ghastoolkit.codeql.results import CodeQLResults
```

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/__main__.py` & `ghastoolkit-0.2.5/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.2.5/src/ghastoolkit/codeql/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,21 @@
             codeql_db_file = os.path.join(self.path, "codeql-database.yml")
             return os.path.exists(codeql_db_file)
         return False
 
     def exists(self) -> bool:
         return False if not self.path else os.path.exists(self.path)
 
+    @property
+    def default_pack(self) -> str:
+        return f"codeql/{self.language}-queries"
+
+    def getSuite(self, name: str) -> str:
+        return f"{self.default_pack}:codeql-suites/{self.language}-{name}.qls"
+
     def display_name(self, owner: Optional[str] = None) -> str:
         """Display Name"""
         if self.repository:
             own = self.repository.owner
             repo = self.repository.repo
 
             if own and own == owner:
@@ -105,20 +112,21 @@
     @staticmethod
     def loadDatabaseYml(path: str) -> "CodeQLDatabase":
         if not os.path.exists(path):
             raise Exception("CodeQL Database YML does not exist")
         if not path.endswith(".yml"):
             raise Exception("File is not a YML file")
 
-        name = os.path.basename(os.path.dirname(path))
+        dbdir = os.path.dirname(path)
+        name = os.path.basename(dbdir)
 
         with open(path, "r") as handle:
             data = safe_load(handle)
 
-        db = CodeQLDatabase(name, data.get("primaryLanguage"), path=path)
+        db = CodeQLDatabase(name, data.get("primaryLanguage"), path=dbdir)
         return db
 
     def downloadDatabase(self, output: Optional[str], use_cache: bool = True) -> str:
         """Download CodeQL database"""
         output = output or self.path or self.path_download
         if not output:
             raise Exception(f"CodeQL Database path not set")
@@ -229,10 +237,16 @@
 
         for root, _, files in os.walk(path):
             for file in files:
                 if file == "codeql-database.yml":
                     path = os.path.join(root, file)
                     self.append(CodeQLDatabase.loadDatabaseYml(path))
 
+    def get(self, name: str) -> Optional[CodeQLDatabase]:
+        for db in self:
+            if db.name == name:
+                return db
+        return
+
     def downloadDatabases(self):
         for db in self:
             db.downloadDatabase(None)
```

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.2.5/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.2.5/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.2.5/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.2.5/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.2.5/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.2.5/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.2.5/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.2.5/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.2.5/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.2.5/src/ghastoolkit/supplychain/licensing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime
 import os
 import json
 import logging
 from types import coroutine
 from typing import Optional
 
+from requests import request
+
 from ghastoolkit.octokit.github import Repository
 
-# from ghastoolkit.supplychain.dependencies import Dependency
 
 logger = logging.getLogger("ghastoolkit.supplychain.licenses")
 
 NO_LICENSES = ["None", "NA", "NOASSERTION"]
 
 
 class Licenses:
```

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.2.5/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.4
+Version: 0.2.5
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.4/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.2.5/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 src/ghastoolkit/__main__.py
 src/ghastoolkit.egg-info/PKG-INFO
 src/ghastoolkit.egg-info/SOURCES.txt
 src/ghastoolkit.egg-info/dependency_links.txt
 src/ghastoolkit.egg-info/requires.txt
 src/ghastoolkit.egg-info/top_level.txt
 src/ghastoolkit/codeql/__init__.py
+src/ghastoolkit/codeql/cli.py
 src/ghastoolkit/codeql/consts.py
 src/ghastoolkit/codeql/databases.py
+src/ghastoolkit/codeql/results.py
 src/ghastoolkit/codeql/utils.py
 src/ghastoolkit/octokit/__init__.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependabot.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
```

### Comparing `ghastoolkit-0.2.4/tests/test_codeqldb.py` & `ghastoolkit-0.2.5/tests/test_codeqldb.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,7 +15,17 @@
             os.path.join("/tmp", "java", "GeekMasher", "ghastoolkit"),
         )
 
         codeql = CodeQLDatabase("db", "java")
         self.assertEqual(
             codeql.createDownloadPath("/tmp"), os.path.join("/tmp", "java", "db")
         )
+    
+    def test_pack(self):
+        codeql = CodeQLDatabase("db", "java", self.repo)
+        self.assertEqual(codeql.default_pack, "codeql/java-queries")
+
+    def test_suite(self):
+        codeql = CodeQLDatabase("db", "java", self.repo)
+        self.assertEqual(codeql.getSuite("code-scanning"), "codeql/java-queries:codeql-suites/java-code-scanning.qls")
+
+
```

### Comparing `ghastoolkit-0.2.4/tests/test_codescanning.py` & `ghastoolkit-0.2.5/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/tests/test_default.py` & `ghastoolkit-0.2.5/tests/test_default.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
         alert = DependencyAlert("high", Advisory("0000", "high"), "pypi/ghastoolkit")
 
     def test_codescanning(self):
         cs = CodeScanning()
         alert = CodeAlert(0, "open", "", {}, {})
 
+    def test_codeql(self):
+        codeql = CodeQL("codeql")
+        alerts = CodeQLResults()
+
     def test_secretscanning(self):
         ss = SecretScanning()
         alert = SecretAlert(
             0, "open", "", "geekmasher_token", "GeekMasher Token", "ABCD"
         )
 
     def test_licenses(self):
```

### Comparing `ghastoolkit-0.2.4/tests/test_dependencies.py` & `ghastoolkit-0.2.5/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/tests/test_depgraph.py` & `ghastoolkit-0.2.5/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/tests/test_github.py` & `ghastoolkit-0.2.5/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/tests/test_licenses.py` & `ghastoolkit-0.2.5/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/tests/test_octokit.py` & `ghastoolkit-0.2.5/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.4/tests/test_secretscanning.py` & `ghastoolkit-0.2.5/tests/test_secretscanning.py`

 * *Files identical despite different names*


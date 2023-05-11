# Comparing `tmp/mrfix-1.0.1.tar.gz` & `tmp/mrfix-1.0.2.tar.gz`

## Comparing `mrfix-1.0.1.tar` & `mrfix-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.1/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.1/src/mrfix/__init__.py
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 mrfix-1.0.1/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.1/.gitignore
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.1/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.2/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.2/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 mrfix-1.0.2/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.2/.gitignore
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.2/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.2/PKG-INFO
```

### Comparing `mrfix-1.0.1/LICENZE` & `mrfix-1.0.2/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.1/src/mrfix/mrfix.py` & `mrfix-1.0.2/src/mrfix/mrfix.py`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.1/.gitignore` & `mrfix-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.1/README.md` & `mrfix-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.1/pyproject.toml` & `mrfix-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "1.0.1"
+version = "1.0.2"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-1.0.1/PKG-INFO` & `mrfix-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfix
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```


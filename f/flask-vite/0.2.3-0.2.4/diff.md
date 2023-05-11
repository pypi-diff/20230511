# Comparing `tmp/flask_vite-0.2.3.tar.gz` & `tmp/flask_vite-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_vite-0.2.3.tar", max compression
+gzip compressed data, was "flask_vite-0.2.4.tar", max compression
```

## Comparing `flask_vite-0.2.3.tar` & `flask_vite-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2022-04-08 07:03:12.325318 flask_vite-0.2.3/LICENSE
--rw-r--r--   0        0        0     1395 2022-11-02 07:44:40.948526 flask_vite-0.2.3/README.md
--rw-r--r--   0        0        0     1384 2023-03-29 08:12:00.431756 flask_vite-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       48 2022-09-02 18:03:03.970225 flask_vite-0.2.3/src/flask_vite/__init__.py
--rw-r--r--   0        0        0     1528 2022-12-22 10:32:22.015899 flask_vite-0.2.3/src/flask_vite/cli.py
--rw-r--r--   0        0        0     1512 2023-01-04 10:16:29.839673 flask_vite-0.2.3/src/flask_vite/extension.py
--rw-r--r--   0        0        0      737 2022-11-27 18:02:52.022408 flask_vite-0.2.3/src/flask_vite/npm.py
--rw-r--r--   0        0        0       12 2022-04-08 07:03:12.420495 flask_vite-0.2.3/src/flask_vite/starter/.gitignore
--rw-r--r--   0        0        0      650 2022-04-08 07:03:12.420123 flask_vite-0.2.3/src/flask_vite/starter/bs.config.js
--rw-r--r--   0        0        0     1421 2022-04-08 07:03:12.420695 flask_vite-0.2.3/src/flask_vite/starter/package.json
--rw-r--r--   0        0        0      123 2022-04-08 07:03:12.420844 flask_vite-0.2.3/src/flask_vite/starter/postcss.config.js
--rw-r--r--   0        0        0       59 2022-04-08 07:03:12.421128 flask_vite-0.2.3/src/flask_vite/starter/src/styles.css
--rw-r--r--   0        0        0     1346 2022-04-08 07:03:12.420281 flask_vite-0.2.3/src/flask_vite/starter/tailwind.config.js
--rw-r--r--   0        0        0      902 2023-01-04 10:16:52.879813 flask_vite-0.2.3/src/flask_vite/tags.py
--rw-r--r--   0        0        0       40 2022-04-08 07:28:14.665349 flask_vite-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      677 2022-04-08 07:28:14.668027 flask_vite-0.2.3/tests/test_flask_vite.py
--rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 flask_vite-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-04-08 07:03:12.325318 flask_vite-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1395 2022-11-02 07:44:40.948526 flask_vite-0.2.4/README.md
+-rw-r--r--   0        0        0     1367 2023-03-29 13:15:37.907340 flask_vite-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       48 2022-09-02 18:03:03.970225 flask_vite-0.2.4/src/flask_vite/__init__.py
+-rw-r--r--   0        0        0     1499 2023-03-29 13:14:22.348889 flask_vite-0.2.4/src/flask_vite/cli.py
+-rw-r--r--   0        0        0     1512 2023-01-04 10:16:29.839673 flask_vite-0.2.4/src/flask_vite/extension.py
+-rw-r--r--   0        0        0      737 2022-11-27 18:02:52.022408 flask_vite-0.2.4/src/flask_vite/npm.py
+-rw-r--r--   0        0        0       12 2022-04-08 07:03:12.420495 flask_vite-0.2.4/src/flask_vite/starter/.gitignore
+-rw-r--r--   0        0        0      650 2022-04-08 07:03:12.420123 flask_vite-0.2.4/src/flask_vite/starter/bs.config.js
+-rw-r--r--   0        0        0     1421 2022-04-08 07:03:12.420695 flask_vite-0.2.4/src/flask_vite/starter/package.json
+-rw-r--r--   0        0        0      123 2022-04-08 07:03:12.420844 flask_vite-0.2.4/src/flask_vite/starter/postcss.config.js
+-rw-r--r--   0        0        0       59 2022-04-08 07:03:12.421128 flask_vite-0.2.4/src/flask_vite/starter/src/styles.css
+-rw-r--r--   0        0        0     1346 2022-04-08 07:03:12.420281 flask_vite-0.2.4/src/flask_vite/starter/tailwind.config.js
+-rw-r--r--   0        0        0      902 2023-01-04 10:16:52.879813 flask_vite-0.2.4/src/flask_vite/tags.py
+-rw-r--r--   0        0        0       40 2022-04-08 07:28:14.665349 flask_vite-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      677 2022-04-08 07:28:14.668027 flask_vite-0.2.4/tests/test_flask_vite.py
+-rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 flask_vite-0.2.4/PKG-INFO
```

### Comparing `flask_vite-0.2.3/LICENSE` & `flask_vite-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/README.md` & `flask_vite-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/pyproject.toml` & `flask_vite-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-vite"
-version = "0.2.3"
+version = "0.2.4"
 homepage = "https://github.com/abilian/flask-vite"
 description = "Flask+Vite integration."
 authors = ["Abilian SAS <contact@abilian.com>"]
 readme = "README.md"
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
@@ -21,19 +21,18 @@
 
 [tool.poetry.plugins."flask.commands"]
 vite = "flask_vite.cli:vite"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 flask = "^2"
-rich = "^12"
 
 [tool.poetry.dev-dependencies]
 abilian-devtools = "*"
-devtools = "^0.10"
+devtools = "*"
 pyanalyze = "*"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `flask_vite-0.2.3/src/flask_vite/cli.py` & `flask_vite-0.2.4/src/flask_vite/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Console script for flask_vite."""
 
 import shutil
 import sys
 from pathlib import Path
 
 import click
-import rich
+from click import secho
 from flask.cli import with_appcontext
 
 from .npm import NPM
 
 
 @click.group()
 def vite():
@@ -23,22 +23,19 @@
 @command()
 @with_appcontext
 def init():
     """Init the vite/ directory (if it doesn't exist)"""
     source_dir = Path(__file__).parent / "starter"
     dest_dir = Path("vite")
     if dest_dir.exists():
-        rich.print(f"[red]Target directory '{dest_dir}' exists, aborting.[/red]")
+        secho(f"Target directory '{dest_dir}' exists, aborting.", fg="red")
         sys.exit(1)
 
     shutil.copytree(source_dir, dest_dir)
-    rich.print(
-        f"[green]Vite source directory and starter content installed in "
-        f"'{dest_dir}'.[/green]",
-    )
+    secho(f"Vite source directory and starter content installed in '{dest_dir}'.", fg="green")
 
 
 @command()
 @with_appcontext
 def install():
     """Install the dependencies using npm."""
     npm_run("install")
```

### Comparing `flask_vite-0.2.3/src/flask_vite/extension.py` & `flask_vite-0.2.4/src/flask_vite/extension.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/src/flask_vite/npm.py` & `flask_vite-0.2.4/src/flask_vite/npm.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/src/flask_vite/starter/bs.config.js` & `flask_vite-0.2.4/src/flask_vite/starter/bs.config.js`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/src/flask_vite/starter/package.json` & `flask_vite-0.2.4/src/flask_vite/starter/package.json`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/src/flask_vite/starter/tailwind.config.js` & `flask_vite-0.2.4/src/flask_vite/starter/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/src/flask_vite/tags.py` & `flask_vite-0.2.4/src/flask_vite/tags.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/tests/test_flask_vite.py` & `flask_vite-0.2.4/tests/test_flask_vite.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.2.3/PKG-INFO` & `flask_vite-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-vite
-Version: 0.2.3
+Version: 0.2.4
 Summary: Flask+Vite integration.
 Home-page: https://github.com/abilian/flask-vite
 Author: Abilian SAS
 Author-email: contact@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: flask (>=2,<3)
-Requires-Dist: rich (>=12,<13)
 Description-Content-Type: text/markdown
 
 # Flask-Vite
 
 [![image](https://img.shields.io/pypi/v/flask-tailwind.svg)](https://pypi.python.org/pypi/flask-tailwind)
 
 Plugin to simplify use of Vite from Flask.
```


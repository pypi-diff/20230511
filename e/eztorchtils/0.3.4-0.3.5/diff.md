# Comparing `tmp/eztorchtils-0.3.4.tar.gz` & `tmp/eztorchtils-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztorchtils-0.3.4.tar", max compression
+gzip compressed data, was "eztorchtils-0.3.5.tar", max compression
```

## Comparing `eztorchtils-0.3.4.tar` & `eztorchtils-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-03-22 06:46:25.139675 eztorchtils-0.3.4/LICENSE
--rw-r--r--   0        0        0    12888 2023-03-30 17:08:04.711241 eztorchtils-0.3.4/README.md
--rw-r--r--   0        0        0      625 2023-03-22 08:09:15.706132 eztorchtils-0.3.4/eztorchtils/__init__.py
--rw-r--r--   0        0        0     1420 2023-03-30 17:05:48.314479 eztorchtils-0.3.4/eztorchtils/utils/__init__.py
--rw-r--r--   0        0        0     5798 2023-03-30 17:05:48.314479 eztorchtils-0.3.4/eztorchtils/utils/arrays.py
--rw-r--r--   0        0        0     2288 2023-03-30 17:38:35.082471 eztorchtils-0.3.4/eztorchtils/utils/logging.py
--rw-r--r--   0        0        0      962 2023-03-22 07:00:11.121189 eztorchtils-0.3.4/eztorchtils/utils/model_wrappers.py
--rw-r--r--   0        0        0     3549 2023-03-30 17:39:23.461737 eztorchtils-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    14047 1970-01-01 00:00:00.000000 eztorchtils-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-11 17:48:58.015545 eztorchtils-0.3.5/LICENSE
+-rw-r--r--   0        0        0    12888 2023-05-11 17:48:58.015545 eztorchtils-0.3.5/README.md
+-rw-r--r--   0        0        0      625 2023-05-11 17:48:58.015545 eztorchtils-0.3.5/eztorchtils/__init__.py
+-rw-r--r--   0        0        0     1445 2023-05-11 17:50:29.090603 eztorchtils-0.3.5/eztorchtils/utils/__init__.py
+-rw-r--r--   0        0        0     5798 2023-05-11 17:48:58.015545 eztorchtils-0.3.5/eztorchtils/utils/arrays.py
+-rw-r--r--   0        0        0     2288 2023-05-11 17:48:58.015545 eztorchtils-0.3.5/eztorchtils/utils/logging.py
+-rw-r--r--   0        0        0      962 2023-05-11 17:48:58.015545 eztorchtils-0.3.5/eztorchtils/utils/model_wrappers.py
+-rw-r--r--   0        0        0     1029 2023-05-11 17:50:54.074345 eztorchtils-0.3.5/eztorchtils/utils/structures.py
+-rw-r--r--   0        0        0     3546 2023-05-11 17:51:17.742100 eztorchtils-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    14057 1970-01-01 00:00:00.000000 eztorchtils-0.3.5/setup.py
+-rw-r--r--   0        0        0    14047 1970-01-01 00:00:00.000000 eztorchtils-0.3.5/PKG-INFO
```

### Comparing `eztorchtils-0.3.4/LICENSE` & `eztorchtils-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eztorchtils-0.3.4/README.md` & `eztorchtils-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `eztorchtils-0.3.4/eztorchtils/__init__.py` & `eztorchtils-0.3.5/eztorchtils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztorchtils-0.3.4/eztorchtils/utils/__init__.py` & `eztorchtils-0.3.5/eztorchtils/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,7 +55,8 @@
     # return os.path.dirname(getsourcefile(lambda:0)) # type: ignore
     return os.path.dirname(getsourcefile(inspect_.stack()[1][0]))  # type: ignore
 
 
 from .arrays import *
 from .logging import *
 from .model_wrappers import *
+from .structures import *
```

### Comparing `eztorchtils-0.3.4/eztorchtils/utils/arrays.py` & `eztorchtils-0.3.5/eztorchtils/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `eztorchtils-0.3.4/eztorchtils/utils/logging.py` & `eztorchtils-0.3.5/eztorchtils/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eztorchtils-0.3.4/eztorchtils/utils/model_wrappers.py` & `eztorchtils-0.3.5/eztorchtils/utils/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `eztorchtils-0.3.4/pyproject.toml` & `eztorchtils-0.3.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
-requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry_core>=1.0.0"]
 
 [tool.poetry]
-name = "eztorchtils"
-version = "0.3.4"
-description = "eds torch stuff"
-readme = "README.md"
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
+description = "eds torch stuff"
+homepage = "https://github.com/ezhang7423/eztorchtils"
 license = "MIT"
+name = "eztorchtils"
+readme = "README.md"
 repository = "https://github.com/ezhang7423/eztorchtils"
-homepage = "https://github.com/ezhang7423/eztorchtils"
+version = "0.3.5"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
-classifiers = [ #! Update me
+classifiers = [
+  #! Update me
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
+einops = "^0.6.0"
+loguru = "^0.6.0"
 python = "^3.8"
 rich = "^13.3.3"
-einops = "^0.6.0"
 tqdm = "^4.65.0"
-loguru = "^0.6.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.5"
-black = { version = "^23.3.0", allow-prereleases = true }
+black = {version = "^23.3.0", allow-prereleases = true}
+coverage = "^7.2.2"
+coverage-badge = "^1.1.0"
 darglint = "^1.8.1"
-isort = { extras = ["colors"], version = "^5.12.0" }
+isort = {extras = ["colors"], version = "^5.12.0"}
 mypy = "^1.1.1"
 mypy-extensions = "^1.0.0"
 pre-commit = "^3.2.1"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.1"
 pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+pytest-html = "^3.2.0"
 pyupgrade = "^3.3.1"
 safety = "^2.3.5"
-coverage = "^7.2.2"
-coverage-badge = "^1.1.0"
-pytest-html = "^3.2.0"
-pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.11.0"
 
 [tool.black]
 # https://github.com/psf/black
-target-version = ["py38"]
-line-length = 88
 color = true
+line-length = 88
+target-version = ["py38"]
 
 exclude = '''
 /(
     \.git
     | \.hg
     | \.mypy_cache
     | \.tox
@@ -76,44 +77,44 @@
     | env
     | venv
 )/
 '''
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
-py_version = 38
 line_length = 88
+py_version = 38
 
+color_output = true
+include_trailing_comma = true
+indent = 4
 known_typing = [
   "typing",
   "types",
   "typing_extensions",
   "mypy",
   "mypy_extensions",
 ]
+multi_line_output = 3
+profile = "black"
 sections = [
   "FUTURE",
   "TYPING",
   "STDLIB",
   "THIRDPARTY",
   "FIRSTPARTY",
   "LOCALFOLDER",
 ]
-include_trailing_comma = true
-profile = "black"
-multi_line_output = 3
-indent = 4
-color_output = true
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
-python_version = 3.8
+color_output = true
 pretty = true
+python_version = 3.8
 show_traceback = true
-color_output = true
 
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 ignore_missing_imports = true
 implicit_reexport = false
@@ -126,34 +127,33 @@
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
+doctest_optionflags = [
+  "NUMBER",
+  "NORMALIZE_WHITESPACE",
+  "IGNORE_EXCEPTION_DETAIL",
+]
 norecursedirs = [
   "hooks",
   "*.egg",
   ".eggs",
   "dist",
   "build",
   "docs",
   ".tox",
   ".git",
   "__pycache__",
 ]
-doctest_optionflags = [
-  "NUMBER",
-  "NORMALIZE_WHITESPACE",
-  "IGNORE_EXCEPTION_DETAIL",
-]
 
 # Extra options:
 addopts = [
   "--strict-markers",
   "--tb=short",
   "--doctest-modules",
   "--doctest-continue-on-failure",
```

### Comparing `eztorchtils-0.3.4/PKG-INFO` & `eztorchtils-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztorchtils
-Version: 0.3.4
+Version: 0.3.5
 Summary: eds torch stuff
 Home-page: https://github.com/ezhang7423/eztorchtils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```


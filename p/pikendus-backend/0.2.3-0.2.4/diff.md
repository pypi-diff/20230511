# Comparing `tmp/pikendus_backend-0.2.3.tar.gz` & `tmp/pikendus_backend-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikendus_backend-0.2.3.tar", last modified: Thu May 11 11:20:21 2023, max compression
+gzip compressed data, was "pikendus_backend-0.2.4.tar", last modified: Thu May 11 14:33:38 2023, max compression
```

## Comparing `pikendus_backend-0.2.3.tar` & `pikendus_backend-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/LICENSE
--rw-r--r--   0        0        0     3105 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/pikendus_backend/PikendusWheelBuilder.py
--rw-r--r--   0        0        0     1702 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/pikendus_backend/__init__.py
--rw-r--r--   0        0        0      823 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/pikendus_backend/main.py
--rwxr-xr-x   0        0        0     3459 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/calc_dep_f90.py
--rw-r--r--   0        0        0     4213 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/compile.py
--rwxr-xr-x   0        0        0     1728 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/gene_py_src.py
--rwxr-xr-x   0        0        0     2117 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/ligne_debug.py
--rw-r--r--   0        0        0    13199 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/structure.py
--rw-r--r--   0        0        0     2780 2023-05-11 11:20:21.922962 pikendus_backend-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 pikendus_backend-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/LICENSE
+-rw-r--r--   0        0        0      728 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/README.md
+-rw-r--r--   0        0        0     3105 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/pikendus_backend/PikendusWheelBuilder.py
+-rw-r--r--   0        0        0     1702 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/pikendus_backend/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/pikendus_backend/main.py
+-rwxr-xr-x   0        0        0     3459 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/calc_dep_f90.py
+-rw-r--r--   0        0        0     4229 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/compile.py
+-rwxr-xr-x   0        0        0     1728 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/gene_py_src.py
+-rwxr-xr-x   0        0        0     2117 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/ligne_debug.py
+-rw-r--r--   0        0        0    13199 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/structure.py
+-rw-r--r--   0        0        0     2879 2023-05-11 14:33:38.565645 pikendus_backend-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 pikendus_backend-0.2.4/PKG-INFO
```

### Comparing `pikendus_backend-0.2.3/LICENSE` & `pikendus_backend-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pikendus_backend/PikendusWheelBuilder.py` & `pikendus_backend-0.2.4/pikendus_backend/PikendusWheelBuilder.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pikendus_backend/__init__.py` & `pikendus_backend-0.2.4/pikendus_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pikendus_backend/main.py` & `pikendus_backend-0.2.4/pikendus_backend/main.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pikendus_backend/scripts/calc_dep_f90.py` & `pikendus_backend-0.2.4/pikendus_backend/scripts/calc_dep_f90.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pikendus_backend/scripts/compile.py` & `pikendus_backend-0.2.4/pikendus_backend/scripts/compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     linker = pikendus_cfg.get("linker", "gcc")
     fflags: str = pikendus_cfg.get(
         "fflags",
         "-g -Wpadded -Wpacked -Waliasing -Wampersand -Wsurprising "
         "-Wintrinsics-std -Wintrinsic-shadow -Wline-truncation -Wreal-q-constant "
         "-Wunused -Wunderflow -Warray-temporaries -ffixed-line-length-132 "
         "-fcray-pointer -Os -fd-lines-as-comments -mavx -funroll-loops "
-        "-fexpensive-optimizations -fno-range-check -fbackslash",
+        "-fexpensive-optimizations -fno-range-check -fbackslash -fimplicit-none",
     )
     cflags: str = pikendus_cfg.get("cflags", "-g -std=gnu99 -Wall")
     lflags: str = pikendus_cfg.get("lflags", "")
 
     fflags += f" -I{pdm_build_dir} {py_inc_dir} -I{numpy_inc_dir} -I{f2py_inc_dir}"
     cflags += f" -I{pdm_build_dir} {py_inc_dir} -I{numpy_inc_dir} -I{f2py_inc_dir}"
```

### Comparing `pikendus_backend-0.2.3/pikendus_backend/scripts/gene_py_src.py` & `pikendus_backend-0.2.4/pikendus_backend/scripts/gene_py_src.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pikendus_backend/scripts/ligne_debug.py` & `pikendus_backend-0.2.4/pikendus_backend/scripts/ligne_debug.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pikendus_backend/structure.py` & `pikendus_backend-0.2.4/pikendus_backend/structure.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.3/pyproject.toml` & `pikendus_backend-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,32 +7,36 @@
 [project]
 name = "pikendus-backend"
 dynamic = []
 description = "A PEP517 compliant build backend, able to compile C and fortran source files"
 authors = [
     { name = "Yann de Thé", email = "yann@johncloud.fr" },
 ]
+readme = "README.md"
 dependencies = [
     "rich>=13.3",
     "setuptools-scm>=7.1",
     "pdm-backend>=2.0.6",
     "wheel>=0.40.0",
     "numpy>=1.24.3",
     "toml>=0.10.2",
     "networkx>=3.1",
     "PyYAML>=6.0",
 ]
 requires-python = ">3.8"
-version = "0.2.3"
+version = "0.2.4"
+
+[project.license]
+file = "LICENSE"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/ydethe/pikendus-backend/issues"
 Homepage = "https://gitlab.com/ydethe/pikendus-backend"
 Source = "https://gitlab.com/ydethe/pikendus-backend"
-Documentation = "https://ydethe.gitlab.io/-/pikendus-backend/-/jobs/4267041254/artifacts/htmldoc/index.html"
+Documentation = "https://ydethe.gitlab.io/pikendus-backend"
 
 [tool.pylint.main]
 ignore-patterns = [
     "kt_*.py",
 ]
 
 [tool.pylint.format]
@@ -99,25 +103,28 @@
     "coverage-badge>=1.1.0",
     "docstr-coverage>=2.2.0",
     "ipython~=7.23.1",
     "pre-commit",
     "snakeviz>=2.1.2",
     "types-PyYAML>=6.0.12.9",
     "networkx-stubs>=0.0.1",
+    "doc>=0.1.0",
+    "mkdocs-include-markdown-plugin>=3.9.1",
 ]
 maintain = [
     "black==22.3.0",
     "blacken-docs==1.12.1",
     "git-changelog>=1.0",
 ]
 quality = [
     "mypy>=1.2.0",
     "ruff>=0.0.246",
 ]
 doc = [
+    "jinja2>=3.0.0,<3.1.0",
     "mkdocs-material>=9.1.11",
 ]
 test = [
     "pytest~=7.1.3",
     "pytest-cov~=3.0.0",
     "pytest-mock~=3.8.2",
     "pytest-instafail~=0.4.2",
```


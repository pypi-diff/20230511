# Comparing `tmp/dev_dependencies-0.0.3.tar.gz` & `tmp/dev-dependencies-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev_dependencies-0.0.3.tar", max compression
+gzip compressed data, was "dev-dependencies-0.1.1.tar", last modified: Thu Apr 27 15:06:26 2023, max compression
```

## Comparing `dev_dependencies-0.0.3.tar` & `dev-dependencies-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,26 @@
--rw-r--r--   0        0        0     1069 2023-05-11 15:10:14.471512 dev_dependencies-0.0.3/LICENSE
--rw-r--r--   0        0        0      839 2023-05-11 15:10:14.471512 dev_dependencies-0.0.3/README.md
--rw-r--r--   0        0        0      376 2023-05-11 15:10:14.471512 dev_dependencies-0.0.3/dev_dependencies/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 15:10:14.471512 dev_dependencies-0.0.3/dev_dependencies/py.typed
--rw-r--r--   0        0        0     1447 2023-05-11 15:10:43.927875 dev_dependencies-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 dev_dependencies-0.0.3/PKG-INFO
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.370403 dev-dependencies-0.1.1/
+-rw-r--r--   0 justinmills   (501) staff       (20)       14 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.envrc
+-rw-r--r--   0 justinmills   (501) staff       (20)      255 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.flake8
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.365117 dev-dependencies-0.1.1/.github/
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.368474 dev-dependencies-0.1.1/.github/workflows/
+-rw-r--r--   0 justinmills   (501) staff       (20)     1223 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 justinmills   (501) staff       (20)      192 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.gitignore
+-rw-r--r--   0 justinmills   (501) staff       (20)        7 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.python-version
+-rw-r--r--   0 justinmills   (501) staff       (20)     1069 2023-04-26 12:26:45.000000 dev-dependencies-0.1.1/LICENSE
+-rw-r--r--   0 justinmills   (501) staff       (20)      955 2023-04-27 15:06:26.370220 dev-dependencies-0.1.1/PKG-INFO
+-rw-r--r--   0 justinmills   (501) staff       (20)      281 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/Pipfile
+-rw-r--r--   0 justinmills   (501) staff       (20)    38840 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/Pipfile.lock
+-rw-r--r--   0 justinmills   (501) staff       (20)      686 2023-04-27 15:04:07.000000 dev-dependencies-0.1.1/README.md
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369303 dev-dependencies-0.1.1/dev_dependencies.egg-info/
+-rw-r--r--   0 justinmills   (501) staff       (20)      955 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/PKG-INFO
+-rw-r--r--   0 justinmills   (501) staff       (20)      381 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/SOURCES.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)        1 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/dependency_links.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)      120 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/requires.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)        8 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/top_level.txt
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369710 dev-dependencies-0.1.1/devdeps/
+-rw-r--r--   0 justinmills   (501) staff       (20)      225 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/devdeps/__init__.py
+-rw-r--r--   0 justinmills   (501) staff       (20)      160 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/devdeps/_version.py
+-rw-r--r--   0 justinmills   (501) staff       (20)     1501 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/pyproject.toml
+-rw-r--r--   0 justinmills   (501) staff       (20)       38 2023-04-27 15:06:26.370456 dev-dependencies-0.1.1/setup.cfg
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369903 dev-dependencies-0.1.1/tests/
+-rw-r--r--   0 justinmills   (501) staff       (20)      273 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/tests/test_version.py
```

### Comparing `dev_dependencies-0.0.3/LICENSE` & `dev-dependencies-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dev_dependencies-0.0.3/README.md` & `dev-dependencies-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,17 +24,12 @@
 
 * Tests
 
       pytest
 
 ## Building a package to release
 
-    # Build a distribution (for releases, do this on main with a fresh tag)
     python -m build
 
     # To release that package
     twine upload dist/dev-dependencies-*.tar.gz dist/dev_dependencies-*-py3-none-any.whl
 
-    # To see what the current version will be
-    python -m setuptools_scm
-
-
```

### Comparing `dev_dependencies-0.0.3/PKG-INFO` & `dev-dependencies-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: dev-dependencies
-Version: 0.0.3
+Version: 0.1.1
 Summary: An opinionated library of dev-time dependencies
-License: MIT
 Author: Justin Mills
-Author-email: vortexjj@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic
-Requires-Dist: toml
-Requires-Dist: types-toml
+License: MIT
+Keywords: library,dependencies
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Dev Dependencies
 
 Opinionated development dependencies for python projects.
 
 Install this as your only dev dependency to pick up a bunch of common dev-time libraries you may need for things like linting, type checking and tests.
 
@@ -40,18 +35,12 @@
 
 * Tests
 
       pytest
 
 ## Building a package to release
 
-    # Build a distribution (for releases, do this on main with a fresh tag)
     python -m build
 
     # To release that package
     twine upload dist/dev-dependencies-*.tar.gz dist/dev_dependencies-*-py3-none-any.whl
 
-    # To see what the current version will be
-    python -m setuptools_scm
-
-
-
```


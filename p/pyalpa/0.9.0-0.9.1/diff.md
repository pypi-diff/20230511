# Comparing `tmp/pyalpa-0.9.0.tar.gz` & `tmp/pyalpa-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.9.0.tar", max compression
+gzip compressed data, was "pyalpa-0.9.1.tar", max compression
```

## Comparing `pyalpa-0.9.0.tar` & `pyalpa-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-05-11 20:59:18.638701 pyalpa-0.9.0/LICENSE
--rw-r--r--   0        0        0      683 2023-05-11 20:59:18.638701 pyalpa-0.9.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/cli/__init__.py
--rw-r--r--   0        0        0      732 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1203 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/cli/base.py
--rw-r--r--   0        0        0     6810 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      160 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/__init__.py
--rw-r--r--   0        0        0     1264 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2649 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/base.py
--rw-r--r--   0        0        0     3344 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/metadata.py
--rw-r--r--   0        0        0     1233 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/exceptions.py
--rw-r--r--   0        0        0     4055 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/gh.py
--rw-r--r--   0        0        0     2735 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/git.py
--rw-r--r--   0        0        0     1553 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/messages.py
--rw-r--r--   0        0        0     2956 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/packit.py
--rw-r--r--   0        0        0      298 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/__init__.py
--rw-r--r--   0        0        0    12145 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/base.py
--rw-r--r--   0        0        0     5810 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/branch.py
--rw-r--r--   0        0        0     1666 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/upstream_integration.py
--rw-r--r--   0        0        0      846 2023-05-11 20:59:18.646701 pyalpa-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 pyalpa-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-11 21:45:17.076266 pyalpa-0.9.1/LICENSE
+-rw-r--r--   0        0        0      683 2023-05-11 21:45:17.076266 pyalpa-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1203 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/base.py
+-rw-r--r--   0        0        0     6810 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      160 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1264 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2599 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/base.py
+-rw-r--r--   0        0        0     3344 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/metadata.py
+-rw-r--r--   0        0        0     1233 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/exceptions.py
+-rw-r--r--   0        0        0     4055 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/gh.py
+-rw-r--r--   0        0        0     2735 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/git.py
+-rw-r--r--   0        0        0     1553 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/messages.py
+-rw-r--r--   0        0        0     2956 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/packit.py
+-rw-r--r--   0        0        0      298 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    12145 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/base.py
+-rw-r--r--   0        0        0     5810 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1666 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      846 2023-05-11 21:45:17.080266 pyalpa-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 pyalpa-0.9.1/PKG-INFO
```

### Comparing `pyalpa-0.9.0/LICENSE` & `pyalpa-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/README.md` & `pyalpa-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/cli/alpa_repo.py` & `pyalpa-0.9.1/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/cli/base.py` & `pyalpa-0.9.1/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/cli/local_repo.py` & `pyalpa-0.9.1/alpa/cli/local_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/config/alpa_local.py` & `pyalpa-0.9.1/alpa/config/alpa_local.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/config/alpa_repo.py` & `pyalpa-0.9.1/alpa/config/alpa_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,14 +76,12 @@
             ["git", "rev-parse", "--show-toplevel"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         if process.returncode != 0:
             raise AlpaConfException(process.stderr)
 
-        alpa_config = cls._load_alpa_config(
-            Path("/home/jkyjovsk/Documents/git/github/alpa/test-branch-repo")
-        )
+        alpa_config = cls._load_alpa_config(Path(process.stdout.decode().strip()))
         if alpa_config is None:
             raise FileNotFoundError("No alpa config file in git root found")
 
         return alpa_config
```

### Comparing `pyalpa-0.9.0/alpa/config/base.py` & `pyalpa-0.9.1/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/config/metadata.py` & `pyalpa-0.9.1/alpa/config/metadata.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/constants.py` & `pyalpa-0.9.1/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/gh.py` & `pyalpa-0.9.1/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/git.py` & `pyalpa-0.9.1/alpa/git.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/messages.py` & `pyalpa-0.9.1/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/packit.py` & `pyalpa-0.9.1/alpa/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/repository/base.py` & `pyalpa-0.9.1/alpa/repository/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/repository/branch.py` & `pyalpa-0.9.1/alpa/repository/branch.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/repository/subdirectory.py` & `pyalpa-0.9.1/alpa/repository/subdirectory.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/alpa/upstream_integration.py` & `pyalpa-0.9.1/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.0/pyproject.toml` & `pyalpa-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.9.0"
+version = "0.9.1"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
```

### Comparing `pyalpa-0.9.0/PKG-INFO` & `pyalpa-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.9.0
+Version: 0.9.1
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
```


# Comparing `tmp/facefinder-0.1.7.tar.gz` & `tmp/facefinder-0.1.8.tar.gz`

## Comparing `facefinder-0.1.7.tar` & `facefinder-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.7/Cargo.toml
--rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.7/.github/workflows/CI.yml
--rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.7/.gitignore
--rw-r--r--   0        0        0      547 2023-05-10 14:39:00.000000 facefinder-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.7/src/python/facefinder/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-10 14:38:00.000000 facefinder-0.1.7/src/python/facefinder/interact.py
--rw-r--r--   0        0        0     4565 2023-05-10 04:29:33.000000 facefinder-0.1.7/src/python/facefinder/metadata.py
--rw-r--r--   0        0        0    28631 2023-05-10 10:42:06.000000 facefinder-0.1.7/src/python/facefinder/metrics.py
--rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.7/src/python/facefinder/prompting.py
--rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.7/src/rust/lib.rs
--rw-r--r--   0        0        0     7654 2023-05-10 14:40:07.000000 facefinder-0.1.7/Cargo.lock
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 facefinder-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.8/Cargo.toml
+-rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.8/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.8/.gitignore
+-rw-r--r--   0        0        0      571 2023-05-10 14:49:46.000000 facefinder-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.8/src/python/facefinder/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-10 14:38:00.000000 facefinder-0.1.8/src/python/facefinder/interact.py
+-rw-r--r--   0        0        0     4565 2023-05-10 04:29:33.000000 facefinder-0.1.8/src/python/facefinder/metadata.py
+-rw-r--r--   0        0        0    28631 2023-05-10 10:42:06.000000 facefinder-0.1.8/src/python/facefinder/metrics.py
+-rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.8/src/python/facefinder/prompting.py
+-rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.8/src/rust/lib.rs
+-rw-r--r--   0        0        0     7654 2023-05-10 14:50:13.000000 facefinder-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 facefinder-0.1.8/PKG-INFO
```

### Comparing `facefinder-0.1.7/.github/workflows/CI.yml` & `facefinder-0.1.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.7/.gitignore` & `facefinder-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.7/pyproject.toml` & `facefinder-0.1.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "facefinder"
-requires-python = ">=3.7,<3.11"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
     "deepface",
     "pandas",
     "numpy",
     "opencv-python",
     "tqdm",
     "regex",
+    "mediapipe",
+    "pillow"
 ]
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "src/python"
 module-name = "facefinder.rust"
```

### Comparing `facefinder-0.1.7/src/python/facefinder/interact.py` & `facefinder-0.1.8/src/python/facefinder/interact.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.7/src/python/facefinder/metadata.py` & `facefinder-0.1.8/src/python/facefinder/metadata.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.7/src/python/facefinder/metrics.py` & `facefinder-0.1.8/src/python/facefinder/metrics.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.7/src/python/facefinder/prompting.py` & `facefinder-0.1.8/src/python/facefinder/prompting.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.7/Cargo.lock` & `facefinder-0.1.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "facefinder"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```


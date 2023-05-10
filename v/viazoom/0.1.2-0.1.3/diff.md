# Comparing `tmp/viazoom-0.1.2.tar.gz` & `tmp/viazoom-0.1.3.tar.gz`

## Comparing `viazoom-0.1.2.tar` & `viazoom-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 viazoom-0.1.2/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-05-04 15:14:47.000000 viazoom-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      685 2023-05-04 15:14:47.000000 viazoom-0.1.2/.gitignore
--rwxrwxrwx   0     1000     1000      386 2023-05-09 20:32:18.000000 viazoom-0.1.2/README.md
--rw-r--r--   0     1000     1000      369 2023-05-04 15:14:47.000000 viazoom-0.1.2/pyproject.toml
--rwxrwxrwx   0     1000     1000     3305 2023-05-09 20:18:23.000000 viazoom-0.1.2/src/client.rs
--rw-r--r--   0     1000     1000      164 2023-05-04 17:13:15.000000 viazoom-0.1.2/src/lib.rs
--rwxrwxrwx   0     1000     1000     1097 2023-05-10 15:05:42.000000 viazoom-0.1.2/viazoom.pyi
--rwxrwxrwx   0     1000     1000    38982 2023-05-09 20:56:03.000000 viazoom-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 viazoom-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 viazoom-0.1.3/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-05-04 15:14:47.000000 viazoom-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      685 2023-05-04 15:14:47.000000 viazoom-0.1.3/.gitignore
+-rwxrwxrwx   0     1000     1000      486 2023-05-10 22:10:20.000000 viazoom-0.1.3/Dockerfile
+-rwxrwxrwx   0     1000     1000      386 2023-05-09 20:32:18.000000 viazoom-0.1.3/README.md
+-rwxrwxrwx   0     1000     1000      101 2023-05-10 22:11:41.000000 viazoom-0.1.3/build.sh
+-rw-r--r--   0     1000     1000      369 2023-05-04 15:14:47.000000 viazoom-0.1.3/pyproject.toml
+-rwxrwxrwx   0     1000     1000     3305 2023-05-09 20:18:23.000000 viazoom-0.1.3/src/client.rs
+-rw-r--r--   0     1000     1000      164 2023-05-04 17:13:15.000000 viazoom-0.1.3/src/lib.rs
+-rwxrwxrwx   0     1000     1000     1097 2023-05-10 15:05:42.000000 viazoom-0.1.3/viazoom.pyi
+-rwxrwxrwx   0     1000     1000    38982 2023-05-10 21:55:25.000000 viazoom-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 viazoom-0.1.3/PKG-INFO
```

### Comparing `viazoom-0.1.2/Cargo.toml` & `viazoom-0.1.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "viazoom"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 authors = ["Spencer Neveux <spencer.neveux@viasat.com>"]
 
 [lib]
 name = "viazoom"
 crate-type = ["cdylib"]
```

### Comparing `viazoom-0.1.2/.github/workflows/CI.yml` & `viazoom-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `viazoom-0.1.2/.gitignore` & `viazoom-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `viazoom-0.1.2/src/client.rs` & `viazoom-0.1.3/src/client.rs`

 * *Files identical despite different names*

### Comparing `viazoom-0.1.2/viazoom.pyi` & `viazoom-0.1.3/viazoom.pyi`

 * *Files identical despite different names*

### Comparing `viazoom-0.1.2/Cargo.lock` & `viazoom-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1194,15 +1194,15 @@
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "viazoom"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "base64 0.13.1",
  "chrono",
  "pyo3",
  "rand",
  "reqwest",
  "serde",
```

### Comparing `viazoom-0.1.2/PKG-INFO` & `viazoom-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viazoom
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Author: Spencer Neveux <spencer.neveux@viasat.com>
 Author-email: Spencer Neveux <spencer.neveux@viasat.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```


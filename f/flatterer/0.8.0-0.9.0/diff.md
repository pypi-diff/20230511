# Comparing `tmp/flatterer-0.8.0.tar.gz` & `tmp/flatterer-0.9.0.tar.gz`

## Comparing `flatterer-0.8.0.tar` & `flatterer-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 flatterer-0.8.0/Cargo.toml
--rw-r--r--   0     1001      121     6334 2021-12-07 20:17:03.000000 flatterer-0.8.0/.github/workflows/dist.yml
--rw-r--r--   0     1001      121      716 2021-12-07 20:17:03.000000 flatterer-0.8.0/.github/workflows/docs.yml
--rw-r--r--   0     1001      121       62 2021-12-07 20:17:03.000000 flatterer-0.8.0/.gitignore
--rw-r--r--   0     1001      121    29189 2021-12-07 20:20:00.000000 flatterer-0.8.0/Cargo.lock
--rw-r--r--   0     1001      121      738 2021-12-07 20:17:03.000000 flatterer-0.8.0/Dockerfile
--rw-r--r--   0     1001      121     1080 2021-12-07 20:17:03.000000 flatterer-0.8.0/LICENSE
--rw-r--r--   0     1001      121     4087 2021-12-07 20:17:03.000000 flatterer-0.8.0/README.md
--rw-r--r--   0     1001      121       81 2021-12-07 20:17:03.000000 flatterer-0.8.0/docker-entrypoint.sh
--rw-r--r--   0     1001      121      634 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/Makefile
--rw-r--r--   0     1001      121     1919 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/changelog.md
--rw-r--r--   0     1001      121     1988 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/conf.py
--rw-r--r--   0     1001      121      650 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/development.md
--rw-r--r--   0     1001      121     4260 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/index.md
--rw-r--r--   0     1001      121      795 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/make.bat
--rw-r--r--   0     1001      121     9993 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/options.md
--rw-r--r--   0     1001      121     5759 2021-12-07 20:17:03.000000 flatterer-0.8.0/docs/outputs.md
--rw-r--r--   0     1001      121      513 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/basic.json
--rw-r--r--   0     1001      121       64 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic/csv/developer.csv
--rw-r--r--   0     1001      121      132 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic/csv/main.csv
--rw-r--r--   0     1001      121       90 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic/csv/platforms.csv
--rw-r--r--   0     1001      121     2054 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic/data_package.json
--rw-r--r--   0     1001      121      451 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic/fields.csv
--rw-r--r--   0     1001      121     6237 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic/output.xlsx
--rw-r--r--   0     1001      121      157 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic_inline/csv/main.csv
--rw-r--r--   0     1001      121       90 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic_inline/csv/platforms.csv
--rw-r--r--   0     1001      121     1646 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic_inline/data_package.json
--rw-r--r--   0     1001      121      398 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic_inline/fields.csv
--rw-r--r--   0     1001      121     5713 2021-12-07 20:17:03.000000 flatterer-0.8.0/fixtures/expected_basic_inline/output.xlsx
--rw-r--r--   0     1001      121     4156 2021-12-07 20:17:03.000000 flatterer-0.8.0/flatterer/__init__.py
--rw-r--r--   0     1001      121      426 2021-12-07 20:17:03.000000 flatterer-0.8.0/pyproject.toml
--rw-r--r--   0     1001      121       52 2021-12-07 20:17:03.000000 flatterer-0.8.0/requirements_docs.txt
--rw-r--r--   0     1001      121     6416 2021-12-07 20:17:03.000000 flatterer-0.8.0/src/lib.rs
--rw-r--r--   0     1001      121     4281 2021-12-07 20:17:03.000000 flatterer-0.8.0/src/main.rs
--rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 flatterer-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 flatterer-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      121     6334 2021-12-12 21:41:34.000000 flatterer-0.9.0/.github/workflows/dist.yml
+-rw-r--r--   0     1001      121      716 2021-12-12 21:41:34.000000 flatterer-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0     1001      121       62 2021-12-12 21:41:34.000000 flatterer-0.9.0/.gitignore
+-rw-r--r--   0     1001      121    29212 2021-12-12 21:41:34.000000 flatterer-0.9.0/Cargo.lock
+-rw-r--r--   0     1001      121      738 2021-12-12 21:41:34.000000 flatterer-0.9.0/Dockerfile
+-rw-r--r--   0     1001      121     1080 2021-12-12 21:41:34.000000 flatterer-0.9.0/LICENSE
+-rw-r--r--   0     1001      121     4087 2021-12-12 21:41:34.000000 flatterer-0.9.0/README.md
+-rw-r--r--   0     1001      121       81 2021-12-12 21:41:34.000000 flatterer-0.9.0/docker-entrypoint.sh
+-rw-r--r--   0     1001      121      634 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/Makefile
+-rw-r--r--   0     1001      121     2368 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/changelog.md
+-rw-r--r--   0     1001      121     1988 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/conf.py
+-rw-r--r--   0     1001      121      650 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/development.md
+-rw-r--r--   0     1001      121     4260 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/index.md
+-rw-r--r--   0     1001      121      795 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/make.bat
+-rw-r--r--   0     1001      121     9993 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/options.md
+-rw-r--r--   0     1001      121     5759 2021-12-12 21:41:34.000000 flatterer-0.9.0/docs/outputs.md
+-rw-r--r--   0     1001      121      513 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/basic.json
+-rw-r--r--   0     1001      121       64 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic/csv/developer.csv
+-rw-r--r--   0     1001      121      132 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic/csv/main.csv
+-rw-r--r--   0     1001      121       90 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic/csv/platforms.csv
+-rw-r--r--   0     1001      121     2054 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic/data_package.json
+-rw-r--r--   0     1001      121      451 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic/fields.csv
+-rw-r--r--   0     1001      121     6237 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic/output.xlsx
+-rw-r--r--   0     1001      121      157 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic_inline/csv/main.csv
+-rw-r--r--   0     1001      121       90 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic_inline/csv/platforms.csv
+-rw-r--r--   0     1001      121     1646 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic_inline/data_package.json
+-rw-r--r--   0     1001      121      398 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic_inline/fields.csv
+-rw-r--r--   0     1001      121     5713 2021-12-12 21:41:34.000000 flatterer-0.9.0/fixtures/expected_basic_inline/output.xlsx
+-rw-r--r--   0     1001      121     4156 2021-12-12 21:41:34.000000 flatterer-0.9.0/flatterer/__init__.py
+-rw-r--r--   0     1001      121      426 2021-12-12 21:41:34.000000 flatterer-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      121       52 2021-12-12 21:41:34.000000 flatterer-0.9.0/requirements_docs.txt
+-rw-r--r--   0     1001      121     6416 2021-12-12 21:41:34.000000 flatterer-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      121     4281 2021-12-12 21:41:34.000000 flatterer-0.9.0/src/main.rs
+-rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 flatterer-0.9.0/PKG-INFO
```

### Comparing `flatterer-0.8.0/Cargo.toml` & `flatterer-0.9.0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "flatterer"
-version = "0.8.0"
+version = "0.9.0"
 authors = ["David Raznick <kindly@gmail.com>"]
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 clap = "2"
 crossbeam-channel="0.5"
 serde_json = { version = "1", features = ["preserve_order"] }
 pyo3 = {version = "0.14", features = ["extension-module"] }
 anyhow={version = "1.0"}
-libflatterer={version = "0.8"}
+libflatterer={version = "0.9"}
 
 [profile.release]
 debug = true
 
 [lib]
 name = "flatterer"
 path = "src/lib.rs"
```

### Comparing `flatterer-0.8.0/.github/workflows/dist.yml` & `flatterer-0.9.0/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/.github/workflows/docs.yml` & `flatterer-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/Cargo.lock` & `flatterer-0.9.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "flatterer"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "anyhow",
  "clap",
  "crossbeam-channel",
  "libflatterer",
  "pyo3",
  "serde_json",
@@ -306,14 +306,15 @@
 name = "indexmap"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc633605454125dec4b66843673f01c7df2b89479b32e0ed634e43a91cff62a5"
 dependencies = [
  "autocfg",
  "hashbrown",
+ "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "47741a8bc60fb26eb8d6e0238bbb26d8575ff623fdc97b1a2c00c050b9684ed8"
@@ -403,20 +404,21 @@
 name = "libc"
 version = "0.2.107"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbe5e23404da5b4f555ef85ebed98fb4083e55a00c317800bc2a50ede9f3d219"
 
 [[package]]
 name = "libflatterer"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "638474e0e6a1a59c5fe24433abfa4ef715da1686a85732b0f28aa163c5729d9d"
+checksum = "6fa07dee5a3e98acddece11f48113e6768883ce600a3fd3f087ad23169611616"
 dependencies = [
  "crossbeam-channel",
  "csv",
+ "indexmap",
  "itertools",
  "jsonref",
  "regex",
  "serde",
  "serde_json",
  "slug",
  "smallvec",
```

### Comparing `flatterer-0.8.0/Dockerfile` & `flatterer-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/LICENSE` & `flatterer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/README.md` & `flatterer-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/docs/Makefile` & `flatterer-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/docs/changelog.md` & `flatterer-0.9.0/docs/changelog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 # Change Log
 All notable changes to this project will be documented in this file.
  
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [0.9] - 2021-12-12
+ 
+### Fixed
+
+- Removed unwrap on channel send, to remove possible panic.
+
+### Changed
+
+- Table ordering of output in JSON input order.  Making `xlsx` and `fields.csv` table order reflect the input data.
+- Lib has new `FlatFiles::new_with_dafualts()` to make using the library less verbose.
+- Use insta for more tests.
+
+### New
+
+- Lib has preview option, meaning CSV output will optionally only show specified number of lines.
+
 ## [0.8] - 2021-12-01
  
 ### Changed
 
 - Paths to data in sqlite and postgres start at root of output.
 - Clippy for linting and insta for tests.
```

### Comparing `flatterer-0.8.0/docs/conf.py` & `flatterer-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'flatterer'
 copyright = '2021, David Raznick'
 author = 'David Raznick'
 
 # The full version, including alpha/beta/rc tags
-release = '0.7'
+release = '0.9'
 
 myst_heading_anchors = 3
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `flatterer-0.8.0/docs/development.md` & `flatterer-0.9.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/docs/index.md` & `flatterer-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/docs/make.bat` & `flatterer-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/docs/options.md` & `flatterer-0.9.0/docs/options.md`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/docs/outputs.md` & `flatterer-0.9.0/docs/outputs.md`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/fixtures/basic.json` & `flatterer-0.9.0/fixtures/basic.json`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/fixtures/expected_basic/data_package.json` & `flatterer-0.9.0/fixtures/expected_basic/data_package.json`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/fixtures/expected_basic/output.xlsx` & `flatterer-0.9.0/fixtures/expected_basic/output.xlsx`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/fixtures/expected_basic_inline/data_package.json` & `flatterer-0.9.0/fixtures/expected_basic_inline/data_package.json`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/fixtures/expected_basic_inline/output.xlsx` & `flatterer-0.9.0/fixtures/expected_basic_inline/output.xlsx`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/flatterer/__init__.py` & `flatterer-0.9.0/flatterer/__init__.py`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/src/lib.rs` & `flatterer-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/src/main.rs` & `flatterer-0.9.0/src/main.rs`

 * *Files identical despite different names*

### Comparing `flatterer-0.8.0/PKG-INFO` & `flatterer-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatterer
-Version: 0.8.0
+Version: 0.9.0
 Requires-Dist: orjson
 Requires-Dist: ijson
 Requires-Dist: click
 Summary: Opinionated JSON to CSV converter
 Author: David Raznick <kindly@gmail.com>
 Author-email: David Raznick <kindly@gmail.com>
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```


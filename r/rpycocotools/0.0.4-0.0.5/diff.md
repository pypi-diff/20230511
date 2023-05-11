# Comparing `tmp/rpycocotools-0.0.4.tar.gz` & `tmp/rpycocotools-0.0.5.tar.gz`

## Comparing `rpycocotools-0.0.4.tar` & `rpycocotools-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.toml
--rw-r--r--   0     1001      123       30 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/.gitignore
--rw-r--r--   0     1001      123    55307 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.lock
--rw-r--r--   0     1001      123      980 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/README.md
--rw-r--r--   0     1001      123     1186 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/argparse.rs
--rw-r--r--   0     1001      123    18281 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/object_detection.rs
--rw-r--r--   0     1001      123     6758 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/pyo3.rs
--rw-r--r--   0     1001      123      181 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/coco.rs
--rw-r--r--   0     1001      123     3024 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/errors.rs
--rw-r--r--   0     1001      123     1901 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/lib.rs
--rw-r--r--   0     1001      123     1510 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/main.rs
--rw-r--r--   0     1001      123    22560 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/mask/conversions.rs
--rw-r--r--   0     1001      123      215 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/mask.rs
--rw-r--r--   0     1001      123      724 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/utils.rs
--rw-r--r--   0     1001      123     2296 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/display.rs
--rw-r--r--   0     1001      123     6037 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/draw.rs
--rw-r--r--   0     1001      123      141 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize.rs
--rw-r--r--   0     1001      123      610 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/tests/load_coco.rs
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 rpycocotools-0.0.4/Cargo.toml
--rw-r--r--   0     1001      123      173 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/.gitignore
--rw-r--r--   0     1001      123       58 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/.rustfmt.toml
--rw-r--r--   0     1001      123    45992 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/Cargo.lock
--rw-r--r--   0     1001      123     2033 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/README.md
--rw-r--r--   0     1001      123       10 2023-05-08 07:08:04.000000 rpycocotools-0.0.4/dist/rpycocotools-0.0.4.tar.gz
--rw-r--r--   0     1001      123      634 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/Makefile
--rw-r--r--   0     1001      123        0 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/_static/.gitkeep
--rw-r--r--   0     1001      123     1572 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/conf.py
--rw-r--r--   0     1001      123     8574 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/dataset.rst
--rw-r--r--   0     1001      123      631 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/examples.rst
--rw-r--r--   0     1001      123      731 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/index.rst
--rw-r--r--   0     1001      123      800 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/make.bat
--rw-r--r--   0     1001      123      101 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/quickstart.rst
--rw-r--r--   0     1001      123     2805 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/segmentation_masks.rst
--rw-r--r--   0     1001      123     4077 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/pyproject.toml
--rw-r--r--   0     1001      123      157 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/python/rpycocotools/__init__.py
--rw-r--r--   0     1001      123     2147 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/python/rpycocotools/mask.py
--rw-r--r--   0     1001      123      872 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/README.md
--rw-r--r--   0     1001      123     4323 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-build.txt
--rw-r--r--   0     1001      123     6529 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-dev.txt
--rw-r--r--   0     1001      123    19383 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-doc.txt
--rw-r--r--   0     1001      123     7535 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-flake8.txt
--rw-r--r--   0     1001      123     4641 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-test.txt
--rw-r--r--   0     1001      123     3142 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements.txt
--rw-r--r--   0     1001      123     5136 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/coco.rs
--rw-r--r--   0     1001      123     1179 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/errors.rs
--rw-r--r--   0     1001      123     1434 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/lib.rs
--rw-r--r--   0     1001      123       31 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/main.rs
--rw-r--r--   0     1001      123     5032 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/mask.rs
--rw-r--r--   0     1001      123      204 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/tests/conftest.py
--rw-r--r--   0     1001      123     3061 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/tests/test_coco.py
--rw-r--r--   0     1001      123     2289 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/tests/test_mask.py
--rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 rpycocotools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.toml
+-rw-r--r--   0     1001      123       30 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/.gitignore
+-rw-r--r--   0     1001      123    55307 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.lock
+-rw-r--r--   0     1001      123      980 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/README.md
+-rw-r--r--   0     1001      123     1186 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/argparse.rs
+-rw-r--r--   0     1001      123    18281 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/object_detection.rs
+-rw-r--r--   0     1001      123     7039 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/pyo3.rs
+-rw-r--r--   0     1001      123      181 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/coco.rs
+-rw-r--r--   0     1001      123     3024 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/errors.rs
+-rw-r--r--   0     1001      123     1901 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/lib.rs
+-rw-r--r--   0     1001      123     1510 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/main.rs
+-rw-r--r--   0     1001      123    23262 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/mask/conversions.rs
+-rw-r--r--   0     1001      123     6222 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/mask/utils.rs
+-rw-r--r--   0     1001      123      230 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/mask.rs
+-rw-r--r--   0     1001      123      724 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/utils.rs
+-rw-r--r--   0     1001      123     2296 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/display.rs
+-rw-r--r--   0     1001      123     6037 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/draw.rs
+-rw-r--r--   0     1001      123      141 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize.rs
+-rw-r--r--   0     1001      123      610 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/tests/load_coco.rs
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 rpycocotools-0.0.5/Cargo.toml
+-rw-r--r--   0     1001      123      173 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/.gitignore
+-rw-r--r--   0     1001      123       58 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/.rustfmt.toml
+-rw-r--r--   0     1001      123    45992 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/Cargo.lock
+-rw-r--r--   0     1001      123     2127 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/README.md
+-rw-r--r--   0     1001      123       10 2023-05-11 14:57:42.000000 rpycocotools-0.0.5/dist/rpycocotools-0.0.5.tar.gz
+-rw-r--r--   0     1001      123      634 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/Makefile
+-rw-r--r--   0     1001      123        0 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/_static/.gitkeep
+-rw-r--r--   0     1001      123     1572 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/conf.py
+-rw-r--r--   0     1001      123     9080 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/dataset.rst
+-rw-r--r--   0     1001      123      623 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/examples.rst
+-rw-r--r--   0     1001      123      731 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/index.rst
+-rw-r--r--   0     1001      123      800 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/make.bat
+-rw-r--r--   0     1001      123      101 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/quickstart.rst
+-rw-r--r--   0     1001      123     2368 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/segmentation_masks.rst
+-rw-r--r--   0     1001      123     4114 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/pyproject.toml
+-rw-r--r--   0     1001      123      157 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/python/rpycocotools/__init__.py
+-rw-r--r--   0     1001      123     3402 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/python/rpycocotools/mask.py
+-rw-r--r--   0     1001      123      872 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/README.md
+-rw-r--r--   0     1001      123     4323 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-build.txt
+-rw-r--r--   0     1001      123     6529 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-dev.txt
+-rw-r--r--   0     1001      123    19383 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-doc.txt
+-rw-r--r--   0     1001      123     7535 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-flake8.txt
+-rw-r--r--   0     1001      123     4641 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-test.txt
+-rw-r--r--   0     1001      123     3142 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements.txt
+-rw-r--r--   0     1001      123     5136 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/coco.rs
+-rw-r--r--   0     1001      123     1179 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/errors.rs
+-rw-r--r--   0     1001      123     1433 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/lib.rs
+-rw-r--r--   0     1001      123       31 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/main.rs
+-rw-r--r--   0     1001      123     6476 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/mask.rs
+-rw-r--r--   0     1001      123      205 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/tests/conftest.py
+-rw-r--r--   0     1001      123     3062 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/tests/test_coco.py
+-rw-r--r--   0     1001      123     5096 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/tests/test_mask.py
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 rpycocotools-0.0.5/PKG-INFO
```

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.toml` & `rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "cocotools"
-version = "0.0.3"
+version = "0.0.5"
 edition = "2021"
 rust-version = "1.64.0"
 description = "Package providing functionalities to work with COCO format datasets."
 readme = "README.md"
 categories = ["command-line-utilities"]
 authors = ["Hoel Bagard"]
 license = "MIT OR Apache-2.0"
```

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.lock` & `rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "cocotools"
-version = "0.0.3"
+version = "0.0.5"
 dependencies = [
  "anyhow",
  "clap 4.1.8",
  "criterion",
  "image",
  "imageproc",
  "minifb",
```

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/README.md` & `rpycocotools-0.0.5/local_dependencies/cocotools/README.md`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/argparse.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/argparse.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/object_detection.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/object_detection.rs`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 /// Internal type used to represent polygons.
 ///
 /// It contains the width and height of the image for easier handling, notably when using traits.
 #[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
 #[derive(Clone, Debug, Deserialize, Serialize)]
 pub struct PolygonsRS {
-    /// Vector with two elements, the width and height of the image corresponding to the segmentation mask.
+    /// Vector with two elements, the height and width of the image corresponding to the segmentation mask.
     pub size: Vec<u32>,
     /// See [`Polygons`].
     pub counts: Vec<Vec<f64>>,
 }
 
 /// Segmentation mask compressed as a [Run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding).
 #[cfg_attr(
```

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/pyo3.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/pyo3.rs`

 * *Files 8% similar despite different names*

```diff
@@ -132,23 +132,24 @@
             inner: vec![slf.left, slf.top, slf.width, slf.height].into_iter(),
         };
         Py::new(slf.py(), iter)
     }
 
     fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
         match op {
-            CompareOp::Eq => (self.left == other.left
-                && self.top == other.top
-                && self.width == other.width
-                && self.height == other.height)
+            // For some reason, the COCO dataset uses floats instead of ints, hence the < 0.01.
+            CompareOp::Eq => ((self.left - other.left).abs() < 0.01
+                && (self.top - other.top).abs() < 0.01
+                && (self.width - other.width).abs() < 0.01
+                && (self.height - other.height).abs() < 0.01)
                 .into_py(py),
-            CompareOp::Ne => (self.left != other.left
-                || self.top != other.top
-                || self.width != other.width
-                || self.height != other.height)
+            CompareOp::Ne => ((self.left - other.left).abs() > 0.01
+                || (self.top - other.top).abs() > 0.01
+                || (self.width - other.width).abs() > 0.01
+                || (self.height - other.height).abs() > 0.01)
                 .into_py(py),
             _ => py.NotImplemented(),
         }
     }
 }
 
 #[pymethods]
@@ -200,14 +201,15 @@
 
     fn __repr__(&self) -> String {
         format!("PolygonsRS(size={:?}, counts={:?})", self.size, self.counts)
     }
 
     fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
         match op {
+            // FIXME: `counts` are floats, don't compare them with "==".
             CompareOp::Eq => (self.size == other.size && self.counts == other.counts).into_py(py),
             CompareOp::Ne => (self.size != other.size || self.counts != other.counts).into_py(py),
             _ => py.NotImplemented(),
         }
     }
 }
```

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/errors.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/errors.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/lib.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/main.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/main.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/mask/conversions.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/mask/conversions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -382,14 +382,15 @@
 /// - The decompressed mask.
 #[allow(clippy::cast_possible_truncation, clippy::module_name_repetitions)]
 pub fn mask_from_poly(
     poly: &object_detection::Polygons,
     width: u32,
     height: u32,
 ) -> Result<Mask, MaskError> {
+    // FIXME TODO: handle more than one poly.
     let mut points_poly: Vec<imageproc::point::Point<i32>> = Vec::new();
     for i in (0..poly[0].len()).step_by(2) {
         points_poly.push(imageproc::point::Point::new(
             poly[0][i] as i32,
             poly[0][i + 1] as i32,
         ));
     }
@@ -466,14 +467,31 @@
         let poly = Polygons::from(rle);
         let mask = mask_from_poly(&poly, rle.size[1], rle.size[0]).unwrap();
         let result_rle = Rle::try_from(&mask).unwrap();
         assert_eq!(&result_rle, rle);
     }
 
     #[rstest]
+    #[case::horizontal_thick_line(
+        &PolygonsRS {size: vec![7, 7], counts: vec![vec![1.0, 2.0, 1.0, 4.0, 5.0, 4.0, 5.0, 2.0]]},
+        &array![[0, 0, 0, 0, 0, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 0, 0, 0, 0, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0]],
+    )]
+    // FIXME: Non-square tests seem to fail.
+    fn poly_rs_to_mask(#[case] poly: &PolygonsRS, #[case] expected_mask: &Mask) {
+        let mask = Mask::try_from(poly).unwrap();
+        assert_eq!(&mask, expected_mask);
+    }
+
+    #[rstest]
     #[case::square(
         &Rle {size: vec![4, 4], counts: vec![5, 2, 2, 2, 5]},
         &PolygonsRS {size: vec![4, 4], counts: vec![vec![1.0, 1.0, 1.0, 2.0, 2.0, 2.0, 2.0, 1.0]] }
     )]
     #[case::horizontal_thick_line(
         &Rle {size: vec![7, 7], counts: vec![9, 3, 4, 3, 4, 3, 4, 3, 4, 3, 9]},
         &PolygonsRS {size: vec![7, 7], counts: vec![vec![1.0, 2.0, 1.0, 4.0, 5.0, 4.0, 5.0, 2.0]]}
```

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/utils.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/display.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/display.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/draw.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/draw.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/local_dependencies/cocotools/tests/load_coco.rs` & `rpycocotools-0.0.5/local_dependencies/cocotools/tests/load_coco.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/Cargo.lock` & `rpycocotools-0.0.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "cocotools"
-version = "0.0.3"
+version = "0.0.5"
 dependencies = [
  "anyhow",
  "clap",
  "image",
  "imageproc",
  "minifb",
  "ndarray",
```

### Comparing `rpycocotools-0.0.4/README.md` & `rpycocotools-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,29 @@
 
 [![PyPI](https://img.shields.io/pypi/v/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rpycocotools?style=flat-square)](https://pypistats.org/packages/rpycocotools)
 [![PyPI - License](https://img.shields.io/pypi/l/rpycocotools?style=flat)](https://opensource.org/licenses/MIT)
 
-The `rpycocotools` package provides tools to load, manipulate, convert and visualize COCO format datasets.
+The `rpycocotools` package provides tools to load, manipulate, convert and visualize COCO format datasets. The documentation is available [here](https://cocotools-rs.readthedocs.io/en/latest/index.html).
 
 ### Installation
 
 You can install the package through pip:
 ```
 pip install rpycocotools
 ```
 
-You can also build and install it into a virtualenv with `pip install .` (do not use `maturin develop`, the imports will not work).
+You can also git clone this repo and build it yourself with:
+```
+pip install -r requirements/requirements-build.txt
+pip install .
+```
+(do not use `maturin develop`, the imports will not work).
 
 ### Usage example
 
 Visualize image with a given `id`:
 ```python
 import rpycocotools
 coco_dataset = rpycocotools.COCO("../data_samples/coco_25k/annotations.json", "../data_samples/coco_25k/images")
@@ -40,9 +45,8 @@
 
 <p align="center">
   <img alt="bike_segmentation" src="https://user-images.githubusercontent.com/34478245/226691842-8a11cde1-905d-434e-b287-0c3c685e01d1.png">
 </p>
 
 
 ## TODO list:
-- Make it possible to get the dataset as a json (in order to be able to save/print it).
-- Make it possible to get the visualization image as a numpy array.
+- [ ] Make it possible to get the dataset as a json (in order to be able to save/print it).
```

### Comparing `rpycocotools-0.0.4/docs/Makefile` & `rpycocotools-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/docs/conf.py` & `rpycocotools-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/docs/dataset.rst` & `rpycocotools-0.0.5/docs/dataset.rst`

 * *Files 2% similar despite different names*

```diff
@@ -67,33 +67,40 @@
     :rtype: list[Annotation]
     :raises KeyError: If there is no entry in the dataset corresponding to `img_id`.
 
     .. method:: visualize_img(img_id: int) -> None
 
     Visualize an image and its annotations.
 
-    :param int img_id: The `id` of the `Image` to whose annotations should be visualized.
+    :param int img_id: The `id` of the `Image` whose annotations should be visualized.
     :raises ValueError: If the image cannot be drawn (potentially due to it not being in the dataset) or cannot be displayed.
 
+    .. method:: draw_anns(self: Self, img_id: int, draw_bboxes: bool) -> npt.NDArray[np.uint8]: ...
 
-.. class:: rpycocotools.anns.Annotation(id: int, image_id: int, category_id: int, segmentation: Polygons | PolygonsRS | Rle | CocoRle, area: float, bbox: Bbox, iscrowd: int) -> None
+    Draw the annotations on the image and returns it as a (RGB) numpy array.
+
+    :param int img_id: The `id` of the `Image` whose annotations should be visualized.
+    :param bool draw_bboxes: Whether to display bounding boxes or not (if `False`, only the masks will be drawn).
+    :raises ValueError: If the image cannot be drawn (potentially due to it not being in the dataset) or cannot be displayed.
+
+.. class:: rpycocotools.anns.Annotation(id: int, image_id: int, category_id: int, segmentation: Polygons | PolygonsRS | RLE | COCO_RLE, area: float, bbox: BBox, iscrowd: int) -> None
 
     Create an annotation used for object detection tasks.
 
     Each object instance annotation contains a series of fields, including the category id and segmentation mask of the object.\
     In [the original COCO dataset](https://cocodataset.org/#home), the segmentation format depends on whether the instance represents a single object (`iscrowd=0` in which case polygons are used) or a collection of objects (`iscrowd=1` in which case RLE is used). Note that a single object (iscrowd=0) may require multiple polygons, for example if occluded.\
     Crowd annotations (`iscrowd=1`) are used to label large groups of objects (e.g. a crowd of people). In addition, an enclosing bounding box is provided for each object (box coordinates are measured from the top left image corner and are 0-indexed).\
     Finally, the categories field of the annotation structure stores the mapping of category id to category and supercategory names.
 
     :param int id: The id of the annotation.
     :param int image_id: The id of the image corresponding to this annotation.
     :param int category_id: The id of the category corresponding to this annotation.
-    :param Polygons | PolygonsRS | Rle | CocoRle segmentation: The segmentation data for the annotation, which can be of type Polygons, PolygonsRS, Rle or CocoRle.
+    :param Polygons | PolygonsRS | RLE | COCO_RLE segmentation: The segmentation data for the annotation, which can be of type Polygons, PolygonsRS, RLE or COCO_RLE.
     :param float area: The area of the annotation bounding box.
-    :param Bbox bbox: The bounding box of the annotation.
+    :param BBox bbox: The bounding box of the annotation.
     :param int iscrowd: The iscrowd flag for the annotation, which indicates if the annotation represents a group of objects or not.
 
 .. class:: rpycocotools.anns.Category(id: int, name: str, supercategory: str) -> None
 
     Creates a category used for COCO object detection tasks.
 
     :param int id: The id of the category.
@@ -114,15 +121,15 @@
 
     .. attribute:: supercategory
 
         The supercategory of the category.
 
         :type: str
 
-.. class:: rpycocotools.anns.Bbox(left: float, top: float, width: float, height: float) -> None
+.. class:: rpycocotools.anns.BBox(left: float, top: float, width: float, height: float) -> None
 
     A bounding box used for object detection tasks.
 
     :param float left: The top-left x coordinate of the bounding box.
     :param float top: The top-left y coordinate of the bounding box.
     :param float width: The width of the bounding box.
     :param float height: The height of the bounding box.
```

### Comparing `rpycocotools-0.0.4/docs/examples.rst` & `rpycocotools-0.0.5/docs/examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 .. code-block:: python
     :caption: Load a mask and decode it
 
     import rpycocotools
     coco_dataset = rpycocotools.COCO("../data_samples/coco_25k/annotations.json", "../data_samples/coco_25k/images")
     anns = coco_dataset.get_img_anns(174482)
     encoded_mask = anns[0].segmentation
-    mask = rpycocotools.mask.decode_poly_rs(encoded_mask)
+    mask = rpycocotools.mask.decode(encoded_mask)
```

### Comparing `rpycocotools-0.0.4/docs/index.rst` & `rpycocotools-0.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/docs/make.bat` & `rpycocotools-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/docs/segmentation_masks.rst` & `rpycocotools-0.0.5/docs/segmentation_masks.rst`

 * *Files 17% similar despite different names*

```diff
@@ -40,137 +40,109 @@
 00000270: 7472 6f64 7563 6573 2061 2066 6f75 7274  troduces a fourt
 00000280: 6820 6f6e 6520 6361 6c6c 6564 203a 7079  h one called :py
 00000290: 3a63 6c61 7373 3a60 506f 6c79 676f 6e73  :class:`Polygons
 000002a0: 5253 602e 0a49 7420 666f 6c6c 6f77 7320  RS`..It follows 
 000002b0: 7468 6520 7361 6d65 2066 6f72 6d61 7420  the same format 
 000002c0: 6173 2074 6865 203a 7079 3a63 6c61 7373  as the :py:class
 000002d0: 3a60 524c 4560 2061 6e64 203a 7079 3a63  :`RLE` and :py:c
-000002e0: 6c61 7373 3a60 436f 636f 526c 6560 2074  lass:`CocoRle` t
-000002f0: 7970 6573 2c20 6275 7420 7573 6573 2074  ypes, but uses t
-00000300: 6865 2070 6f6c 7967 6f6e 7320 666f 7220  he polygons for 
-00000310: 7468 6520 6063 6f75 6e74 7360 2066 6965  the `counts` fie
-00000320: 6c64 3a0a 0a2a 203a 7079 3a63 6c61 7373  ld:..* :py:class
-00000330: 3a60 506f 6c79 676f 6e73 5253 603a 2060  :`PolygonsRS`: `
-00000340: 2273 6567 6d65 6e74 6174 696f 6e22 3a20  "segmentation": 
-00000350: 7b22 7369 7a65 223a 205b 3438 302c 2036  {"size": [480, 6
-00000360: 3430 5d2c 2022 636f 756e 7473 223a 205b  40], "counts": [
-00000370: 5b35 3130 2e36 362c 2034 3233 2e30 312c  [510.66, 423.01,
-00000380: 2035 3131 2e37 322c 2034 3230 2e30 332c   511.72, 420.03,
-00000390: 202e 2e2e 2c20 3531 302e 3435 2c20 3432   ..., 510.45, 42
-000003a0: 332e 3031 5d5d 7d60 0a0a 5468 6520 6164  3.01]]}`..The ad
-000003b0: 7661 6e74 6167 6520 6f66 2074 6869 7320  vantage of this 
-000003c0: 666f 726d 6174 2069 6620 7468 6174 2068  format if that h
-000003d0: 6520 706f 6c79 676f 6e73 2063 616e 2062  e polygons can b
-000003e0: 6520 6465 636f 6465 6420 696e 746f 2061  e decoded into a
-000003f0: 206d 6173 6b20 6f66 2074 6865 2073 616d   mask of the sam
-00000400: 6520 6173 2074 6865 2069 6e70 7574 2069  e as the input i
-00000410: 6d61 6765 2077 6974 686f 7574 2068 6176  mage without hav
-00000420: 696e 6720 746f 206c 6f6f 6b20 7570 2069  ing to look up i
-00000430: 7473 2073 697a 652e 2048 6f77 6576 6572  ts size. However
-00000440: 2069 7420 7368 6f75 6c64 206e 6f74 2062   it should not b
-00000450: 6520 7772 6974 7465 6e20 746f 2061 206a  e written to a j
-00000460: 736f 6e20 6669 6c65 2028 6173 2069 7420  son file (as it 
-00000470: 6973 206e 6f6e 2d73 7461 6e64 6172 6429  is non-standard)
-00000480: 2e0a 0a4d 6173 6b20 636f 6e76 6572 7369  ...Mask conversi
-00000490: 6f6e 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ons.------------
-000004a0: 2d2d 2d2d 0a0a 2e2e 2066 756e 6374 696f  ----.... functio
-000004b0: 6e3a 3a20 7270 7963 6f63 6f74 6f6f 6c73  n:: rpycocotools
-000004c0: 2e6d 6173 6b2e 6465 636f 6465 5f72 6c65  .mask.decode_rle
-000004d0: 2865 6e63 6f64 6564 5f6d 6173 6b3a 2052  (encoded_mask: R
-000004e0: 6c65 2920 2d3e 206e 7074 2e4e 4441 7272  le) -> npt.NDArr
-000004f0: 6179 5b6e 702e 7569 6e74 385d 0a0a 2020  ay[np.uint8]..  
-00000500: 4465 636f 6465 2061 6e20 524c 4520 6d61  Decode an RLE ma
-00000510: 736b 2074 6f20 6120 3a63 6c61 7373 3a60  sk to a :class:`
-00000520: 6e75 6d70 792e 6e64 6172 7261 7960 2e0a  numpy.ndarray`..
-00000530: 0a20 203a 7061 7261 6d20 526c 6520 656e  .  :param Rle en
-00000540: 636f 6465 645f 6d61 736b 3a20 5468 6520  coded_mask: The 
-00000550: 7275 6e2d 6c65 6e67 7468 2065 6e63 6f64  run-length encod
-00000560: 6564 206d 6173 6b2e 0a20 203a 7261 6973  ed mask..  :rais
-00000570: 6520 5661 6c75 6545 7272 6f72 3a20 4966  e ValueError: If
-00000580: 2074 6865 206d 6173 6b20 636f 6e76 6572   the mask conver
-00000590: 7369 6f6e 2066 6169 6c65 642e 0a20 203a  sion failed..  :
-000005a0: 7265 7475 726e 3a20 5468 6520 6465 636f  return: The deco
-000005b0: 6465 6420 6d61 736b 2061 7320 6120 4e75  ded mask as a Nu
-000005c0: 6d50 7920 6172 7261 792e 0a20 203a 7274  mPy array..  :rt
-000005d0: 7970 653a 2060 606e 7074 2e4e 4441 7272  ype: ``npt.NDArr
-000005e0: 6179 5b6e 702e 7569 6e74 385d 6060 0a0a  ay[np.uint8]``..
-000005f0: 2e2e 2066 756e 6374 696f 6e3a 3a20 7270  .. function:: rp
-00000600: 7963 6f63 6f74 6f6f 6c73 2e6d 6173 6b2e  ycocotools.mask.
-00000610: 6465 636f 6465 5f63 6f63 6f5f 726c 6528  decode_coco_rle(
-00000620: 656e 636f 6465 645f 6d61 736b 3a20 434f  encoded_mask: CO
-00000630: 434f 5f52 4c45 2920 2d3e 206e 7074 2e4e  CO_RLE) -> npt.N
-00000640: 4441 7272 6179 5b6e 702e 7569 6e74 385d  DArray[np.uint8]
-00000650: 0a0a 2020 4465 636f 6465 2061 6e20 434f  ..  Decode an CO
-00000660: 434f 2052 4c45 206d 6173 6b20 746f 2061  CO RLE mask to a
-00000670: 203a 636c 6173 733a 606e 756d 7079 2e6e   :class:`numpy.n
-00000680: 6461 7272 6179 602e 0a0a 2020 3a70 6172  darray`...  :par
-00000690: 616d 2043 4f43 4f5f 524c 4520 656e 636f  am COCO_RLE enco
-000006a0: 6465 645f 6d61 736b 3a20 5468 6520 434f  ded_mask: The CO
-000006b0: 434f 2072 756e 2d6c 656e 6774 6820 656e  CO run-length en
-000006c0: 636f 6465 6420 6d61 736b 2e0a 2020 3a72  coded mask..  :r
-000006d0: 6169 7365 2056 616c 7565 4572 726f 723a  aise ValueError:
-000006e0: 2049 6620 7468 6520 6d61 736b 2063 6f6e   If the mask con
-000006f0: 7665 7273 696f 6e20 6661 696c 6564 2e0a  version failed..
-00000700: 2020 3a72 6574 7572 6e3a 2054 6865 2064    :return: The d
-00000710: 6563 6f64 6564 206d 6173 6b20 6173 2061  ecoded mask as a
-00000720: 204e 756d 5079 2061 7272 6179 2e0a 2020   NumPy array..  
-00000730: 3a72 7479 7065 3a20 6060 6e70 742e 4e44  :rtype: ``npt.ND
-00000740: 4172 7261 795b 6e70 2e75 696e 7438 5d60  Array[np.uint8]`
-00000750: 600a 0a2e 2e20 6675 6e63 7469 6f6e 3a3a  `.... function::
-00000760: 2072 7079 636f 636f 746f 6f6c 732e 6d61   rpycocotools.ma
-00000770: 736b 2e64 6563 6f64 655f 706f 6c79 5f72  sk.decode_poly_r
-00000780: 7328 656e 636f 6465 645f 6d61 736b 3a20  s(encoded_mask: 
-00000790: 506f 6c79 676f 6e73 5253 2920 2d3e 206e  PolygonsRS) -> n
-000007a0: 7074 2e4e 4441 7272 6179 5b6e 702e 7569  pt.NDArray[np.ui
-000007b0: 6e74 385d 0a0a 2020 4465 636f 6465 2061  nt8]..  Decode a
-000007c0: 2070 6f6c 7967 6f6e 7320 6d61 736b 2028   polygons mask (
-000007d0: 696e 636c 7564 696e 6720 696d 6167 6520  including image 
-000007e0: 7369 7a65 2920 7265 7072 6573 656e 7461  size) representa
-000007f0: 7469 6f6e 2074 6f20 6120 3a63 6c61 7373  tion to a :class
-00000800: 3a60 6e75 6d70 792e 6e64 6172 7261 7960  :`numpy.ndarray`
-00000810: 2e0a 0a20 203a 7061 7261 6d20 506f 6c79  ...  :param Poly
-00000820: 676f 6e73 5253 2065 6e63 6f64 6564 5f6d  gonsRS encoded_m
-00000830: 6173 6b3a 2054 6865 2070 6f6c 7967 6f6e  ask: The polygon
-00000840: 2069 6e20 3a63 6c61 7373 3a60 524c 4560   in :class:`RLE`
-00000850: 2066 6f72 6d61 742e 0a20 203a 7261 6973   format..  :rais
-00000860: 6520 5661 6c75 6545 7272 6f72 3a20 4966  e ValueError: If
-00000870: 2074 6865 206d 6173 6b20 636f 6e76 6572   the mask conver
-00000880: 7369 6f6e 2066 6169 6c65 642e 0a20 203a  sion failed..  :
-00000890: 7265 7475 726e 3a20 5468 6520 6465 636f  return: The deco
-000008a0: 6465 6420 6d61 736b 2061 7320 6120 4e75  ded mask as a Nu
-000008b0: 6d50 7920 6172 7261 792e 0a20 203a 7274  mPy array..  :rt
-000008c0: 7970 653a 2060 606e 7074 2e4e 4441 7272  ype: ``npt.NDArr
-000008d0: 6179 5b6e 702e 7569 6e74 385d 6060 0a0a  ay[np.uint8]``..
-000008e0: 2e2e 2066 756e 6374 696f 6e3a 3a20 7270  .. function:: rp
-000008f0: 7963 6f63 6f74 6f6f 6c73 2e6d 6173 6b2e  ycocotools.mask.
-00000900: 6465 636f 6465 5f70 6f6c 7928 706f 6c79  decode_poly(poly
-00000910: 3a20 506f 6c79 676f 6e73 2c20 7769 6474  : Polygons, widt
-00000920: 683a 2069 6e74 2c20 6865 6967 6874 3a20  h: int, height: 
-00000930: 696e 7429 202d 3e20 6e70 742e 4e44 4172  int) -> npt.NDAr
-00000940: 7261 795b 6e70 2e75 696e 7438 5d0a 0a20  ray[np.uint8].. 
-00000950: 2044 6563 6f64 6520 6120 706f 6c79 676f   Decode a polygo
-00000960: 6e73 206d 6173 6b20 7265 7072 6573 656e  ns mask represen
-00000970: 7461 7469 6f6e 2074 6f20 6120 3a63 6c61  tation to a :cla
-00000980: 7373 3a60 6e75 6d70 792e 6e64 6172 7261  ss:`numpy.ndarra
-00000990: 7960 2e0a 0a20 203a 7061 7261 6d20 506f  y`...  :param Po
-000009a0: 6c79 676f 6e73 2070 6f6c 793a 2054 6865  lygons poly: The
-000009b0: 2060 506f 6c79 676f 6e73 6020 746f 2063   `Polygons` to c
-000009c0: 6f6d 706f 7369 6e67 2074 6865 206d 6173  omposing the mas
-000009d0: 6b2e 0a20 203a 7061 7261 6d20 696e 7420  k..  :param int 
-000009e0: 7769 6474 683a 2054 6865 2077 6964 7468  width: The width
-000009f0: 206f 6620 7468 6520 696d 6167 6520 636f   of the image co
-00000a00: 7272 6573 706f 6e64 696e 6720 746f 2074  rresponding to t
-00000a10: 6865 2070 6f6c 7967 6f6e 730a 2020 3a70  he polygons.  :p
-00000a20: 6172 616d 2069 6e74 2068 6569 6768 743a  aram int height:
-00000a30: 2054 6865 2068 6569 6768 7420 6f66 2074   The height of t
-00000a40: 6865 2069 6d61 6765 2063 6f72 7265 7370  he image corresp
-00000a50: 6f6e 6469 6e67 2074 6f20 7468 6520 706f  onding to the po
-00000a60: 6c79 676f 6e73 0a20 203a 7261 6973 6520  lygons.  :raise 
-00000a70: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
-00000a80: 6865 206d 6173 6b20 636f 6e76 6572 7369  he mask conversi
-00000a90: 6f6e 2066 6169 6c65 642e 0a20 203a 7265  on failed..  :re
-00000aa0: 7475 726e 3a20 5468 6520 6269 6e61 7279  turn: The binary
-00000ab0: 206d 6173 6b20 6f66 2074 6865 2064 6563   mask of the dec
-00000ac0: 6f64 6564 2060 506f 6c79 676f 6e73 602e  oded `Polygons`.
-00000ad0: 0a20 203a 7274 7970 653a 2060 606e 7074  .  :rtype: ``npt
-00000ae0: 2e4e 4441 7272 6179 5b6e 702e 7569 6e74  .NDArray[np.uint
-00000af0: 385d 6060 0a                             8]``.
+000002e0: 6c61 7373 3a60 434f 434f 5f52 4c45 6020  lass:`COCO_RLE` 
+000002f0: 7479 7065 732c 2062 7574 2075 7365 7320  types, but uses 
+00000300: 7468 6520 706f 6c79 676f 6e73 2066 6f72  the polygons for
+00000310: 2074 6865 2060 636f 756e 7473 6020 6669   the `counts` fi
+00000320: 656c 643a 0a0a 2a20 3a70 793a 636c 6173  eld:..* :py:clas
+00000330: 733a 6050 6f6c 7967 6f6e 7352 5360 3a20  s:`PolygonsRS`: 
+00000340: 6022 7365 676d 656e 7461 7469 6f6e 223a  `"segmentation":
+00000350: 207b 2273 697a 6522 3a20 5b34 3830 2c20   {"size": [480, 
+00000360: 3634 305d 2c20 2263 6f75 6e74 7322 3a20  640], "counts": 
+00000370: 5b5b 3531 302e 3636 2c20 3432 332e 3031  [[510.66, 423.01
+00000380: 2c20 3531 312e 3732 2c20 3432 302e 3033  , 511.72, 420.03
+00000390: 2c20 2e2e 2e2c 2035 3130 2e34 352c 2034  , ..., 510.45, 4
+000003a0: 3233 2e30 315d 5d7d 600a 0a54 6865 2061  23.01]]}`..The a
+000003b0: 6476 616e 7461 6765 206f 6620 7468 6973  dvantage of this
+000003c0: 2066 6f72 6d61 7420 6966 2074 6861 7420   format if that 
+000003d0: 6865 2070 6f6c 7967 6f6e 7320 6361 6e20  he polygons can 
+000003e0: 6265 2064 6563 6f64 6564 2069 6e74 6f20  be decoded into 
+000003f0: 6120 6d61 736b 206f 6620 7468 6520 7361  a mask of the sa
+00000400: 6d65 2061 7320 7468 6520 696e 7075 7420  me as the input 
+00000410: 696d 6167 6520 7769 7468 6f75 7420 6861  image without ha
+00000420: 7669 6e67 2074 6f20 6c6f 6f6b 2075 7020  ving to look up 
+00000430: 6974 7320 7369 7a65 2e20 486f 7765 7665  its size. Howeve
+00000440: 7220 6974 2073 686f 756c 6420 6e6f 7420  r it should not 
+00000450: 6265 2077 7269 7474 656e 2074 6f20 6120  be written to a 
+00000460: 6a73 6f6e 2066 696c 6520 2861 7320 6974  json file (as it
+00000470: 2069 7320 6e6f 6e2d 7374 616e 6461 7264   is non-standard
+00000480: 292e 0a0a 4465 636f 6465 206d 6173 6b73  )...Decode masks
+00000490: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+000004a0: 2d0a 0a2e 2e20 6675 6e63 7469 6f6e 3a3a  -.... function::
+000004b0: 2072 7079 636f 636f 746f 6f6c 732e 6d61   rpycocotools.ma
+000004c0: 736b 2e64 6563 6f64 6528 656e 636f 6465  sk.decode(encode
+000004d0: 645f 6d61 736b 3a20 524c 4520 7c20 434f  d_mask: RLE | CO
+000004e0: 434f 5f52 4c45 207c 2050 6f6c 7967 6f6e  CO_RLE | Polygon
+000004f0: 7320 7c20 506f 6c79 676f 6e73 5253 2c20  s | PolygonsRS, 
+00000500: 7769 6474 683a 204e 6f6e 6520 7c20 696e  width: None | in
+00000510: 742c 2068 6569 6768 743a 204e 6f6e 6520  t, height: None 
+00000520: 7c20 696e 7429 202d 3e20 6e70 742e 4e44  | int) -> npt.ND
+00000530: 4172 7261 795b 6e70 2e75 696e 7438 5d0a  Array[np.uint8].
+00000540: 0a20 2044 6563 6f64 6520 6120 6d61 736b  .  Decode a mask
+00000550: 2074 6f20 6120 3a63 6c61 7373 3a60 6e75   to a :class:`nu
+00000560: 6d70 792e 6e64 6172 7261 7960 2e0a 0a20  mpy.ndarray`... 
+00000570: 203a 7061 7261 6d20 524c 4520 7c20 434f   :param RLE | CO
+00000580: 434f 5f52 4c45 207c 2050 6f6c 7967 6f6e  CO_RLE | Polygon
+00000590: 7320 7c20 506f 6c79 676f 6e73 5253 2065  s | PolygonsRS e
+000005a0: 6e63 6f64 6564 5f6d 6173 6b3a 2054 6865  ncoded_mask: The
+000005b0: 2065 6e63 6f64 6564 206d 6173 6b2e 0a20   encoded mask.. 
+000005c0: 203a 7061 7261 6d20 696e 7420 7769 6474   :param int widt
+000005d0: 683a 2055 7365 206f 6e6c 7920 7768 656e  h: Use only when
+000005e0: 2074 6865 206d 6173 6b20 6973 2061 203a   the mask is a :
+000005f0: 7079 3a63 6c61 7373 3a60 506f 6c79 676f  py:class:`Polygo
+00000600: 6e60 2e20 5468 6520 7769 6474 6820 6f66  n`. The width of
+00000610: 2074 6865 2069 6d61 6765 2063 6f72 7265   the image corre
+00000620: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
+00000630: 706f 6c79 676f 6e73 2e0a 2020 3a70 6172  polygons..  :par
+00000640: 616d 2069 6e74 2068 6569 6768 743a 2055  am int height: U
+00000650: 7365 206f 6e6c 7920 7768 656e 2074 6865  se only when the
+00000660: 206d 6173 6b20 6973 2061 203a 7079 3a63   mask is a :py:c
+00000670: 6c61 7373 3a60 506f 6c79 676f 6e60 2e20  lass:`Polygon`. 
+00000680: 5468 6520 6865 6967 6874 206f 6620 7468  The height of th
+00000690: 6520 696d 6167 6520 636f 7272 6573 706f  e image correspo
+000006a0: 6e64 696e 6720 746f 2074 6865 2070 6f6c  nding to the pol
+000006b0: 7967 6f6e 732e 0a20 203a 7261 6973 6520  ygons..  :raise 
+000006c0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
+000006d0: 6865 206d 6173 6b20 636f 6e76 6572 7369  he mask conversi
+000006e0: 6f6e 2066 6169 6c65 642e 0a20 203a 7265  on failed..  :re
+000006f0: 7475 726e 3a20 5468 6520 6465 636f 6465  turn: The decode
+00000700: 6420 6d61 736b 2061 7320 6120 4e75 6d50  d mask as a NumP
+00000710: 7920 6172 7261 792e 0a20 203a 7274 7970  y array..  :rtyp
+00000720: 653a 2060 606e 7074 2e4e 4441 7272 6179  e: ``npt.NDArray
+00000730: 5b6e 702e 7569 6e74 385d 6060 0a0a 0a45  [np.uint8]``...E
+00000740: 6e63 6f64 6520 6d61 736b 730a 2d2d 2d2d  ncode masks.----
+00000750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e  ------------....
+00000760: 2066 756e 6374 696f 6e3a 3a20 7270 7963   function:: rpyc
+00000770: 6f63 6f74 6f6f 6c73 2e6d 6173 6b2e 656e  ocotools.mask.en
+00000780: 636f 6465 286d 6173 6b3a 206e 7074 2e4e  code(mask: npt.N
+00000790: 4441 7272 6179 5b6e 702e 7569 6e74 385d  DArray[np.uint8]
+000007a0: 2c20 7461 7267 6574 3a20 4c69 7465 7261  , target: Litera
+000007b0: 6c5b 2270 6f6c 7967 6f6e 7322 5d20 7c20  l["polygons"] | 
+000007c0: 4c69 7465 7261 6c5b 2272 6c65 225d 207c  Literal["rle"] |
+000007d0: 204c 6974 6572 616c 5b22 636f 636f 5f72   Literal["coco_r
+000007e0: 6c65 225d 207c 204c 6974 6572 616c 5b22  le"] | Literal["
+000007f0: 706f 6c79 676f 6e73 5f72 7322 5d29 202d  polygons_rs"]) -
+00000800: 3e20 506f 6c79 676f 6e73 207c 2052 4c45  > Polygons | RLE
+00000810: 207c 2043 4f43 4f5f 524c 4520 7c20 506f   | COCO_RLE | Po
+00000820: 6c79 676f 6e73 5253 3a0a 0a20 2045 6e63  lygonsRS:..  Enc
+00000830: 6f64 652f 636f 6d70 7265 7373 2061 203a  ode/compress a :
+00000840: 636c 6173 733a 606e 756d 7079 2e6e 6461  class:`numpy.nda
+00000850: 7272 6179 6020 6d61 736b 2074 6f20 7468  rray` mask to th
+00000860: 6520 6465 7369 7265 6420 666f 726d 6174  e desired format
+00000870: 2e0a 0a20 203a 7061 7261 6d20 6e70 742e  ...  :param npt.
+00000880: 4e44 4172 7261 795b 6e70 2e75 696e 7438  NDArray[np.uint8
+00000890: 5d20 656e 636f 6465 645f 6d61 736b 3a20  ] encoded_mask: 
+000008a0: 5468 6520 756e 636f 6d70 7265 7373 6564  The uncompressed
+000008b0: 206d 6173 6b2e 0a20 203a 7261 6973 6520   mask..  :raise 
+000008c0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
+000008d0: 6865 206d 6173 6b20 636f 6e76 6572 7369  he mask conversi
+000008e0: 6f6e 2066 6169 6c65 642e 0a20 203a 7265  on failed..  :re
+000008f0: 7475 726e 3a20 5468 6520 636f 6d70 7265  turn: The compre
+00000900: 7373 6564 206d 6173 6b2e 0a20 203a 7274  ssed mask..  :rt
+00000910: 7970 653a 2060 6050 6f6c 7967 6f6e 7320  ype: ``Polygons 
+00000920: 7c20 524c 4520 7c20 434f 434f 5f52 4c45  | RLE | COCO_RLE
+00000930: 207c 2050 6f6c 7967 6f6e 7352 5360 600a   | PolygonsRS``.
```

### Comparing `rpycocotools-0.0.4/pyproject.toml` & `rpycocotools-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "rpycocotools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{name="Bagard Hoel"}]
 description = "Package providing utilities to load, manipulate, convert and visualize COCO format datasets."
 keywords = ["COCO", "COCO dataset"]
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -19,15 +19,15 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 license = {text="MIT"}
-dependencies = ["numpy", "rpycocotools-stubs==0.0.4"]
+dependencies = ["numpy", "rpycocotools-stubs==0.0.5"]
 requires-python = ">=3.8"
 
 [project.urls]
 "Source Code" = "https://github.com/hoel-bagard/rust_coco_tools"
 
 [tool.maturin]
 sdist-include = ["LICENSE", "README.md"]
@@ -66,14 +66,15 @@
 [tool.ruff]
 select = ["ALL"]
 exclude = ["docs/conf.py"]
 line-length = 120
 
 [tool.ruff.isort]
 order-by-type = false
+known-first-party = ["rpycocotools"]
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.pylint]
 max-args = 10
```

### Comparing `rpycocotools-0.0.4/python/rpycocotools/mask.py` & `rpycocotools-0.0.5/python/rpycocotools/mask.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,7 +53,47 @@
         case "coco_rle":
             encoded_mask = _mask.encode_to_coco_rle(mask)
         case "polygons":
             encoded_mask = _mask.encode_to_polygons(mask)
         case _:  # "polygons_rs"
             encoded_mask = _mask.encode_to_polygons_rs(mask)
     return encoded_mask
+
+
+def area(encoded_mask: anns.RLE | anns.COCO_RLE | anns.PolygonsRS | anns.Polygons) -> int:
+    """Compute the area of the given mask.
+
+    Args:
+        encoded_mask: The mask whose area should be computed.
+
+    Returns:
+        The area
+    """
+    if isinstance(encoded_mask, anns.RLE):
+        area = _mask.area_rle(encoded_mask)
+    elif isinstance(encoded_mask, anns.COCO_RLE):
+        area = _mask.area_coco_rle(encoded_mask)
+    elif isinstance(encoded_mask, anns.PolygonsRS):
+        area = _mask.area_poly_rs(encoded_mask)
+    else:
+        area = _mask.area_poly(encoded_mask)
+    return area
+
+
+def to_bbox(encoded_mask: anns.RLE | anns.COCO_RLE | anns.PolygonsRS | anns.Polygons) -> anns.BBox:
+    """Compute the bounding box of the given mask.
+
+    Args:
+        encoded_mask: The mask whose bounding box should be computed.
+
+    Returns:
+        The bounding box
+    """
+    if isinstance(encoded_mask, anns.RLE):
+        bbox = _mask.rle_to_bbox(encoded_mask)
+    elif isinstance(encoded_mask, anns.COCO_RLE):
+        bbox = _mask.coco_rle_to_bbox(encoded_mask)
+    elif isinstance(encoded_mask, anns.PolygonsRS):
+        bbox = _mask.poly_rs_to_bbox(encoded_mask)
+    else:
+        bbox = _mask.poly_to_bbox(encoded_mask)
+    return bbox
```

### Comparing `rpycocotools-0.0.4/requirements/README.md` & `rpycocotools-0.0.5/requirements/README.md`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/requirements/requirements-build.txt` & `rpycocotools-0.0.5/requirements/requirements-build.txt`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     --hash=sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4 \
     --hash=sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02 \
     --hash=sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c \
     --hash=sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b
     # via
     #   rpycocotools (pyproject.toml)
     #   rpycocotools-stubs
-rpycocotools-stubs==0.0.4 \
-    --hash=sha256:7365cd07b99904f55ab41cc1ea6bd8828a08e9bd7eaa6989a7a74d85664bce1e \
-    --hash=sha256:f24151d78578d5ef180d30ab5820e098b9df283de878008fdbdb3d62ebdd8b11
+rpycocotools-stubs==0.0.5 \
+    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
+    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
     # via rpycocotools (pyproject.toml)
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via rpycocotools-stubs
```

### Comparing `rpycocotools-0.0.4/requirements/requirements-dev.txt` & `rpycocotools-0.0.5/requirements/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,17 @@
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via build
 pyright==1.1.306 \
     --hash=sha256:008eb2a29584ae274a154d749cf81476a3073fb562a462eac8d43a753378b9db \
     --hash=sha256:16d5d198be64de497d5f9002000a271176c381e21b977ca5566cf779b643c9ed
     # via rpycocotools (pyproject.toml)
-rpycocotools-stubs==0.0.4 \
-    --hash=sha256:7365cd07b99904f55ab41cc1ea6bd8828a08e9bd7eaa6989a7a74d85664bce1e \
-    --hash=sha256:f24151d78578d5ef180d30ab5820e098b9df283de878008fdbdb3d62ebdd8b11
+rpycocotools-stubs==0.0.5 \
+    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
+    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
     # via rpycocotools (pyproject.toml)
 ruff==0.0.265 \
     --hash=sha256:1d5a8de2fbaf91ea5699451a06f4074e7a312accfa774ad9327cde3e4fda2081 \
     --hash=sha256:2a9b38bdb40a998cbc677db55b6225a6c4fadcf8819eb30695e1b8470942426b \
     --hash=sha256:30ddfe22de6ce4eb1260408f4480bbbce998f954dbf470228a21a9b2c45955e4 \
     --hash=sha256:4057eb539a1d88eb84e9f6a36e0a999e0f261ed850ae5d5817e68968e7b89ed9 \
     --hash=sha256:5028950f7af9b119d43d91b215d5044976e43b96a0d1458d193ef0dd3c587bf8 \
```

### Comparing `rpycocotools-0.0.4/requirements/requirements-doc.txt` & `rpycocotools-0.0.5/requirements/requirements-doc.txt`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,17 @@
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via sphinx
 requests==2.30.0 \
     --hash=sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294 \
     --hash=sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4
     # via sphinx
-rpycocotools-stubs==0.0.4 \
-    --hash=sha256:7365cd07b99904f55ab41cc1ea6bd8828a08e9bd7eaa6989a7a74d85664bce1e \
-    --hash=sha256:f24151d78578d5ef180d30ab5820e098b9df283de878008fdbdb3d62ebdd8b11
+rpycocotools-stubs==0.0.5 \
+    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
+    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
     # via rpycocotools (pyproject.toml)
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
     # via sphinx
 soupsieve==2.4.1 \
     --hash=sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8 \
```

### Comparing `rpycocotools-0.0.4/requirements/requirements-flake8.txt` & `rpycocotools-0.0.5/requirements/requirements-flake8.txt`

 * *Files 3% similar despite different names*

```diff
@@ -111,17 +111,17 @@
     --hash=sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019 \
     --hash=sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1
     # via flake8-docstrings
 pyflakes==2.5.0 \
     --hash=sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2 \
     --hash=sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3
     # via flake8
-rpycocotools-stubs==0.0.4 \
-    --hash=sha256:7365cd07b99904f55ab41cc1ea6bd8828a08e9bd7eaa6989a7a74d85664bce1e \
-    --hash=sha256:f24151d78578d5ef180d30ab5820e098b9df283de878008fdbdb3d62ebdd8b11
+rpycocotools-stubs==0.0.5 \
+    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
+    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
     # via rpycocotools (pyproject.toml)
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
     # via pydocstyle
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
```

### Comparing `rpycocotools-0.0.4/requirements/requirements-test.txt` & `rpycocotools-0.0.5/requirements/requirements-test.txt`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
     # via pytest
 pytest==7.3.1 \
     --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
     --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
     # via rpycocotools (pyproject.toml)
-rpycocotools-stubs==0.0.4 \
-    --hash=sha256:7365cd07b99904f55ab41cc1ea6bd8828a08e9bd7eaa6989a7a74d85664bce1e \
-    --hash=sha256:f24151d78578d5ef180d30ab5820e098b9df283de878008fdbdb3d62ebdd8b11
+rpycocotools-stubs==0.0.5 \
+    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
+    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
     # via rpycocotools (pyproject.toml)
 sortedcontainers==2.4.0 \
     --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
     --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
     # via hypothesis
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
```

### Comparing `rpycocotools-0.0.4/requirements/requirements.txt` & `rpycocotools-0.0.5/requirements/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     --hash=sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4 \
     --hash=sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02 \
     --hash=sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c \
     --hash=sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b
     # via
     #   rpycocotools (pyproject.toml)
     #   rpycocotools-stubs
-rpycocotools-stubs==0.0.4 \
-    --hash=sha256:7365cd07b99904f55ab41cc1ea6bd8828a08e9bd7eaa6989a7a74d85664bce1e \
-    --hash=sha256:f24151d78578d5ef180d30ab5820e098b9df283de878008fdbdb3d62ebdd8b11
+rpycocotools-stubs==0.0.5 \
+    --hash=sha256:7fa8935a1833bf98b27b39839ae07042175e31c04809a1842bde6ac988f8bcb7 \
+    --hash=sha256:8c5ddbad0b6ba72afa83dfe7b1cbaae5e8de12ae19a1694baeef8e1a586ef728
     # via rpycocotools (pyproject.toml)
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via rpycocotools-stubs
```

### Comparing `rpycocotools-0.0.4/src/coco.rs` & `rpycocotools-0.0.5/src/coco.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/src/errors.rs` & `rpycocotools-0.0.5/src/errors.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.4/src/lib.rs` & `rpycocotools-0.0.5/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     module.add_wrapped(wrap_pymodule!(mask::py_mask))?;
 
     // Inserting to sys.modules allows importing submodules nicely from Python
     // e.g. from rpycocotools.mask import decode_rle
     let sys = PyModule::import(py, "sys")?;
     let sys_modules: &PyDict = sys.getattr("modules")?.downcast()?;
     sys_modules.set_item("_rpycocotools.mask", module.getattr("mask")?)?;
-    sys_modules.set_item("_rpycocotools.anns", module.getattr("anns")?)?;
+    sys_modules.set_item("rpycocotools.anns", module.getattr("anns")?)?;
 
     Ok(())
 }
```

### Comparing `rpycocotools-0.0.4/src/mask.rs` & `rpycocotools-0.0.5/src/mask.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+#![allow(clippy::needless_pass_by_value)]
 use anyhow::{Context, Result};
 use cocotools::errors::MaskError;
+use cocotools::mask::utils::Area;
 use numpy::ndarray::Array;
 use numpy::ndarray::ShapeBuilder;
 use numpy::IntoPyArray;
 use numpy::PyArray2;
 use numpy::PyReadonlyArray2;
 use pyo3::prelude::*;
 use pyo3::pyfunction;
@@ -11,14 +13,37 @@
 use cocotools::coco::object_detection;
 use cocotools::mask;
 use cocotools::mask::conversions;
 
 use crate::coco::PyPolygons;
 use crate::errors::PyMaskError;
 
+#[allow(clippy::module_name_repetitions, clippy::missing_errors_doc)]
+#[pymodule]
+#[pyo3(name = "mask")]
+pub fn py_mask(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+    m.add_function(wrap_pyfunction!(decode_rle, m)?)?;
+    m.add_function(wrap_pyfunction!(decode_coco_rle, m)?)?;
+    m.add_function(wrap_pyfunction!(decode_poly_rs, m)?)?;
+    m.add_function(wrap_pyfunction!(decode_poly, m)?)?;
+    m.add_function(wrap_pyfunction!(encode_to_rle, m)?)?;
+    m.add_function(wrap_pyfunction!(encode_to_coco_rle, m)?)?;
+    m.add_function(wrap_pyfunction!(encode_to_polygons, m)?)?;
+    m.add_function(wrap_pyfunction!(encode_to_polygons_rs, m)?)?;
+    m.add_function(wrap_pyfunction!(area_rle, m)?)?;
+    m.add_function(wrap_pyfunction!(area_coco_rle, m)?)?;
+    m.add_function(wrap_pyfunction!(area_poly_rs, m)?)?;
+    m.add_function(wrap_pyfunction!(area_poly, m)?)?;
+    m.add_function(wrap_pyfunction!(rle_to_bbox, m)?)?;
+    m.add_function(wrap_pyfunction!(coco_rle_to_bbox, m)?)?;
+    m.add_function(wrap_pyfunction!(poly_rs_to_bbox, m)?)?;
+    m.add_function(wrap_pyfunction!(poly_to_bbox, m)?)?;
+    Ok(())
+}
+
 fn decode<T>(py: Python<'_>, encoded_mask: T) -> Result<&PyArray2<u8>, PyMaskError>
 where
     mask::Mask: TryFrom<T>,
     <mask::Mask as TryFrom<T>>::Error: Into<PyMaskError>,
 {
     match mask::Mask::try_from(encoded_mask) {
         Ok(mask) => {
@@ -41,29 +66,14 @@
             let mask = mask.into_pyarray(py);
             Ok(mask)
         }
         Err(error) => Err(error.into()),
     }
 }
 
-#[allow(clippy::module_name_repetitions, clippy::missing_errors_doc)]
-#[pymodule]
-#[pyo3(name = "mask")]
-pub fn py_mask(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(decode_rle, m)?)?;
-    m.add_function(wrap_pyfunction!(decode_coco_rle, m)?)?;
-    m.add_function(wrap_pyfunction!(decode_poly_rs, m)?)?;
-    m.add_function(wrap_pyfunction!(decode_poly, m)?)?;
-    m.add_function(wrap_pyfunction!(encode_to_rle, m)?)?;
-    m.add_function(wrap_pyfunction!(encode_to_coco_rle, m)?)?;
-    m.add_function(wrap_pyfunction!(encode_to_polygons, m)?)?;
-    m.add_function(wrap_pyfunction!(encode_to_polygons_rs, m)?)?;
-    Ok(())
-}
-
 #[pyfunction]
 fn decode_rle(py: Python<'_>, encoded_mask: object_detection::Rle) -> PyResult<&PyArray2<u8>> {
     Ok(decode(
         py,
         &object_detection::Segmentation::Rle(encoded_mask),
     )?)
 }
@@ -152,7 +162,47 @@
     py: Python<'_>,
     mask: PyReadonlyArray2<u8>,
 ) -> PyResult<Py<object_detection::PolygonsRS>> {
     let mask = mask.to_owned_array();
     let encoded_mask = object_detection::PolygonsRS::from(&mask);
     Py::new(py, encoded_mask)
 }
+
+#[pyfunction]
+fn area_rle(rle: object_detection::Rle) -> u32 {
+    rle.area()
+}
+
+#[pyfunction]
+fn area_coco_rle(coco_rle: object_detection::CocoRle) -> u32 {
+    coco_rle.area()
+}
+
+#[pyfunction]
+fn area_poly_rs(poly: object_detection::PolygonsRS) -> u32 {
+    poly.area()
+}
+
+#[pyfunction]
+fn area_poly(poly: object_detection::Polygons) -> u32 {
+    poly.area()
+}
+
+#[pyfunction]
+fn rle_to_bbox(rle: object_detection::Rle) -> object_detection::Bbox {
+    object_detection::Bbox::from(&rle)
+}
+
+#[pyfunction]
+fn coco_rle_to_bbox(coco_rle: object_detection::CocoRle) -> object_detection::Bbox {
+    object_detection::Bbox::from(&coco_rle)
+}
+
+#[pyfunction]
+fn poly_rs_to_bbox(poly: object_detection::PolygonsRS) -> object_detection::Bbox {
+    object_detection::Bbox::from(&poly)
+}
+
+#[pyfunction]
+fn poly_to_bbox(poly: object_detection::Polygons) -> object_detection::Bbox {
+    object_detection::Bbox::from(&poly)
+}
```

### Comparing `rpycocotools-0.0.4/tests/test_coco.py` & `rpycocotools-0.0.5/tests/test_coco.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import rpycocotools
 from hypothesis import given
 from hypothesis import strategies as st
 
+import rpycocotools
+
 u32_max = 4_294_967_295
 u32_st = st.integers(min_value=0, max_value=u32_max)
 
 
 def test_access_cats(coco_dataset: rpycocotools.COCO) -> None:
     cats = coco_dataset.get_cats()
     assert len(cats) == 80
```

### Comparing `rpycocotools-0.0.4/PKG-INFO` & `rpycocotools-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rpycocotools
-Version: 0.0.4
+Version: 0.0.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy
-Requires-Dist: rpycocotools-stubs ==0.0.4
+Requires-Dist: rpycocotools-stubs ==0.0.5
 Requires-Dist: maturin ; extra == 'build'
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: hypothesis ; extra == 'test'
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
 Requires-Dist: pyright ; extra == 'dev'
 Requires-Dist: sphinx ; extra == 'doc'
@@ -53,24 +53,29 @@
 
 [![PyPI](https://img.shields.io/pypi/v/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rpycocotools?style=flat-square)](https://pypistats.org/packages/rpycocotools)
 [![PyPI - License](https://img.shields.io/pypi/l/rpycocotools?style=flat)](https://opensource.org/licenses/MIT)
 
-The `rpycocotools` package provides tools to load, manipulate, convert and visualize COCO format datasets.
+The `rpycocotools` package provides tools to load, manipulate, convert and visualize COCO format datasets. The documentation is available [here](https://cocotools-rs.readthedocs.io/en/latest/index.html).
 
 ### Installation
 
 You can install the package through pip:
 ```
 pip install rpycocotools
 ```
 
-You can also build and install it into a virtualenv with `pip install .` (do not use `maturin develop`, the imports will not work).
+You can also git clone this repo and build it yourself with:
+```
+pip install -r requirements/requirements-build.txt
+pip install .
+```
+(do not use `maturin develop`, the imports will not work).
 
 ### Usage example
 
 Visualize image with a given `id`:
 ```python
 import rpycocotools
 coco_dataset = rpycocotools.COCO("../data_samples/coco_25k/annotations.json", "../data_samples/coco_25k/images")
@@ -91,10 +96,9 @@
 
 <p align="center">
   <img alt="bike_segmentation" src="https://user-images.githubusercontent.com/34478245/226691842-8a11cde1-905d-434e-b287-0c3c685e01d1.png">
 </p>
 
 
 ## TODO list:
-- Make it possible to get the dataset as a json (in order to be able to save/print it).
-- Make it possible to get the visualization image as a numpy array.
+- [ ] Make it possible to get the dataset as a json (in order to be able to save/print it).
```


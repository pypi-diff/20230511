# Comparing `tmp/sumtree-0.2.2.tar.gz` & `tmp/sumtree-0.2.3.tar.gz`

## Comparing `sumtree-0.2.2.tar` & `sumtree-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 sumtree-0.2.2/Cargo.toml
--rw-rw-r--   0     1000     1000       41 2023-02-03 16:05:18.000000 sumtree-0.2.2/.gitignore
--rw-rw-r--   0     1000     1000     1027 2023-02-10 09:04:01.000000 sumtree-0.2.2/README.md
--rw-rw-r--   0     1000     1000      464 2023-01-19 14:43:58.000000 sumtree-0.2.2/pyproject.toml
--rw-rw-r--   0     1000     1000       54 2023-02-23 14:50:49.000000 sumtree-0.2.2/python/sumtree/__init__.py
--rw-rw-r--   0     1000     1000        0 2022-10-24 17:17:43.000000 sumtree-0.2.2/python/sumtree/py.typed
--rw-rw-r--   0     1000     1000     1730 2023-02-23 14:49:47.000000 sumtree-0.2.2/python/sumtree/sumtree.pyi
--rw-rw-r--   0     1000     1000      818 2023-02-03 14:08:41.000000 sumtree-0.2.2/readme_pypi.md
--rw-rw-r--   0     1000     1000     9232 2023-02-03 16:04:49.000000 sumtree-0.2.2/src/lib.rs
--rw-rw-r--   0     1000     1000      590 2023-01-19 14:27:20.000000 sumtree-0.2.2/tests/benchmark.py
--rw-rw-r--   0     1000     1000     2627 2023-02-03 16:01:39.000000 sumtree-0.2.2/tests/sumtree_python.py
--rw-rw-r--   0     1000     1000      604 2023-02-03 16:02:29.000000 sumtree-0.2.2/tests/tests.py
--rw-rw-r--   0     1000     1000     8784 2023-02-23 14:50:53.000000 sumtree-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 sumtree-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 sumtree-0.2.3/Cargo.toml
+-rw-rw-r--   0     1000     1000        0 2023-05-11 16:36:05.000000 sumtree-0.2.3/.github/workflows/pytest.yaml
+-rw-rw-r--   0     1000     1000       41 2023-02-03 16:05:18.000000 sumtree-0.2.3/.gitignore
+-rw-rw-r--   0     1000     1000      147 2023-05-11 16:32:56.000000 sumtree-0.2.3/.vscode/settings.json
+-rw-rw-r--   0     1000     1000     1027 2023-02-10 09:04:01.000000 sumtree-0.2.3/README.md
+-rw-rw-r--   0     1000     1000     6316 2023-05-11 16:31:40.000000 sumtree-0.2.3/poetry.lock
+-rw-rw-r--   0     1000     1000      754 2023-05-11 16:31:44.000000 sumtree-0.2.3/pyproject.toml
+-rw-rw-r--   0     1000     1000       54 2023-02-23 14:50:49.000000 sumtree-0.2.3/python/sumtree/__init__.py
+-rw-rw-r--   0     1000     1000        0 2022-10-24 17:17:43.000000 sumtree-0.2.3/python/sumtree/py.typed
+-rw-rw-r--   0     1000     1000     1730 2023-02-23 14:49:47.000000 sumtree-0.2.3/python/sumtree/sumtree.pyi
+-rw-rw-r--   0     1000     1000      818 2023-02-03 14:08:41.000000 sumtree-0.2.3/readme_pypi.md
+-rw-rw-r--   0     1000     1000     9361 2023-05-11 16:20:16.000000 sumtree-0.2.3/src/lib.rs
+-rw-rw-r--   0     1000     1000      590 2023-01-19 14:27:20.000000 sumtree-0.2.3/tests/benchmark.py
+-rw-rw-r--   0     1000     1000     2627 2023-02-03 16:01:39.000000 sumtree-0.2.3/tests/sumtree_python.py
+-rw-rw-r--   0     1000     1000      958 2023-05-11 16:33:44.000000 sumtree-0.2.3/tests/test_sumtree.py
+-rw-rw-r--   0     1000     1000     8784 2023-05-11 16:12:07.000000 sumtree-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 sumtree-0.2.3/PKG-INFO
```

### Comparing `sumtree-0.2.2/Cargo.toml` & `sumtree-0.2.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "sumtree"
 authors = ["Yannick Molinghen <yannick.molinghen@ulb.be>"]
-version = "0.2.2"
+version = "0.2.3"
 edition = "2021"
 repository = "https://github.com/yamoling/sumtree"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### Comparing `sumtree-0.2.2/README.md` & `sumtree-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sumtree-0.2.2/python/sumtree/sumtree.pyi` & `sumtree-0.2.3/python/sumtree/sumtree.pyi`

 * *Files identical despite different names*

### Comparing `sumtree-0.2.2/readme_pypi.md` & `sumtree-0.2.3/readme_pypi.md`

 * *Files identical despite different names*

### Comparing `sumtree-0.2.2/src/lib.rs` & `sumtree-0.2.3/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-use pyo3::prelude::{pymodule, pyclass, pymethods, Python, PyResult, PyModule};
-use rand::{rngs::StdRng, SeedableRng, Rng};
+use pyo3::{
+    prelude::{pyclass, pymethods, pymodule, PyModule, PyResult, Python},
+    types::PyDict,
+};
+use rand::{rngs::StdRng, Rng, SeedableRng};
 
 #[pyclass]
+#[derive(Clone)]
 /// SumTree class
 /// A SumTree is a binary tree in which the value of a node is the sum of its direct children.
 /// As such, only leaves retain useful information.
 pub struct SumTree {
     /// The number of leaves in the SumTree
     n_leaves: usize,
     /// The tree nodes
@@ -14,33 +18,31 @@
     num_items: usize,
     /// The maximal number of items (leaves) in the tree
     capacity: usize,
     /// First leaf index
     first_leaf: usize,
     /// Next index to write
     write_index: usize,
-    rng: StdRng
+    rng: StdRng,
 }
 
-
-
 #[pymethods]
 impl SumTree {
     #[new]
     pub fn new(capacity: usize) -> Self {
-        let num_nodes = 2 * capacity -1;
+        let num_nodes = 2 * capacity - 1;
 
-        SumTree { 
-            n_leaves: capacity, 
+        SumTree {
+            n_leaves: capacity,
             tree: vec![0f64; num_nodes],
             num_items: 0,
             first_leaf: capacity - 1,
             capacity,
             write_index: 0,
-            rng: StdRng::seed_from_u64(rand::random())
+            rng: StdRng::seed_from_u64(rand::random()),
         }
     }
 
     /// The total cumulative sum
     #[getter]
     pub fn total(&self) -> f64 {
         self.tree[0]
@@ -79,15 +81,15 @@
     pub fn get(&self, mut cumsum: f64) -> (usize, f64) {
         if self.num_items == 0 {
             return (0, 0f64);
         }
         let mut idx = 0;
         while idx < self.first_leaf {
             let left = 2 * idx + 1;
-            if cumsum <= self.tree[left]{
+            if cumsum <= self.tree[left] {
                 // Left child
                 idx = left;
             } else {
                 // Right child
                 idx = left + 1;
                 cumsum = cumsum - self.tree[left];
             }
@@ -132,14 +134,17 @@
         (indices, values)
     }
 
     pub fn seed(&mut self, seed_value: u64) {
         self.rng = StdRng::seed_from_u64(seed_value);
     }
 
+    pub fn __deepcopy__(&self, _memo: &PyDict) -> Self {
+        self.clone()
+    }
 
     pub fn __len__(&self) -> usize {
         self.num_items
     }
 
     pub fn __getitem__(&self, leaf_num: usize) -> f64 {
         self.tree[self.first_leaf + leaf_num]
@@ -165,15 +170,14 @@
 /// A Python module implemented in Rust.
 #[pymodule]
 fn sumtree(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<SumTree>()?;
     Ok(())
 }
 
-
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn new_ok() {
         let st = SumTree::new(8);
@@ -204,15 +208,15 @@
         let st = SumTree::new(4);
         let (index, value) = st.get(50.);
         assert_eq!(index, 0);
         assert_eq!(value, 0.);
     }
 
     #[test]
-    fn sumtree_get(){
+    fn sumtree_get() {
         let mut st = SumTree::new(4);
         st.add(20.);
         st.add(20.);
         st.add(20.);
         st.add(20.);
         for (i, cumsum) in (0..80).step_by(20).enumerate() {
             let (index, value) = st.get(cumsum as f64);
@@ -224,41 +228,40 @@
             }
         }
         let (index, value) = st.get(80.);
         assert_eq!(value, 20.);
         assert_eq!(index, 3);
     }
 
-
     #[test]
-    fn sumtree_get_above_cumsum(){
+    fn sumtree_get_above_cumsum() {
         let mut st = SumTree::new(4);
         st.add(20.);
         st.add(20.);
         st.add(20.);
         st.add(20.);
         let (index, value) = st.get(100000.);
         assert_eq!(value, 20.);
         assert_eq!(index, 3);
     }
 
     #[test]
-    fn sumtree_get_below_min(){
+    fn sumtree_get_below_min() {
         let mut st = SumTree::new(4);
         st.add(20.);
         st.add(20.);
         st.add(20.);
         st.add(20.);
         let (index, value) = st.get(-100000.);
         assert_eq!(value, 20.);
         assert_eq!(index, 0);
     }
 
     #[test]
-    fn sumtree_get_plenty(){
+    fn sumtree_get_plenty() {
         use rand::random;
         let mut st = SumTree::new(50_000);
         for _ in 0..1_000_000 {
             st.add(random());
             let cumsum: f64 = random::<f64>() * st.total();
             let (index, _) = st.get(cumsum);
             assert!(index < st.num_items);
@@ -326,10 +329,8 @@
             st1.add(i as f64);
             st2.add(i as f64);
         }
         let (idx1, _) = st1.sample(20);
         let (idx2, _) = st2.sample(20);
         assert_ne!(idx1, idx2)
     }
-
-
 }
```

### Comparing `sumtree-0.2.2/tests/benchmark.py` & `sumtree-0.2.3/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `sumtree-0.2.2/tests/sumtree_python.py` & `sumtree-0.2.3/tests/sumtree_python.py`

 * *Files identical despite different names*

### Comparing `sumtree-0.2.2/Cargo.lock` & `sumtree-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "sumtree"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "pyo3",
  "rand",
 ]
 
 [[package]]
 name = "syn"
```

### Comparing `sumtree-0.2.2/PKG-INFO` & `sumtree-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumtree
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Fast and simple SumTree implementation in Rust
 Author: Yannick Molinghen <yannick.molinghen@ulb.be>
 Author-email: Yannick Molinghen <yannick.molinghen@ulb.be>
 Requires-Python: >=3.7
```


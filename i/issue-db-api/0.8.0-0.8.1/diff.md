# Comparing `tmp/issue_db_api-0.8.0.tar.gz` & `tmp/issue_db_api-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.8.0.tar", last modified: Thu May 11 10:19:34 2023, max compression
+gzip compressed data, was "issue_db_api-0.8.1.tar", last modified: Thu May 11 12:12:20 2023, max compression
```

## Comparing `issue_db_api-0.8.0.tar` & `issue_db_api-0.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.8.0/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.987801 issue_db_api-0.8.0/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-11 10:12:58.000000 issue_db_api-0.8.0/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.8.0/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8716 2023-05-11 10:14:20.000000 issue_db_api-0.8.0/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    44902 2023-05-11 10:01:47.000000 issue_db_api-0.8.0/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.8.0/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    39893 2023-05-11 10:14:19.000000 issue_db_api-0.8.0/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.8.0/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6964 2023-05-11 10:03:52.000000 issue_db_api-0.8.0/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2554 2023-05-11 10:04:43.000000 issue_db_api-0.8.0/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.987801 issue_db_api-0.8.0/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.8.0/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-11 10:12:58.000000 issue_db_api-0.8.0/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.8.1/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.393800 issue_db_api-0.8.1/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-11 12:10:29.000000 issue_db_api-0.8.1/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.8.1/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8716 2023-05-11 10:14:20.000000 issue_db_api-0.8.1/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    44902 2023-05-11 10:01:47.000000 issue_db_api-0.8.1/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.8.1/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.8.1/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.8.1/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    39893 2023-05-11 10:14:19.000000 issue_db_api-0.8.1/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.8.1/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6964 2023-05-11 10:03:52.000000 issue_db_api-0.8.1/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.8.1/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.8.1/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-11 12:10:29.000000 issue_db_api-0.8.1/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/setup.py
```

### Comparing `issue_db_api-0.8.0/LICENSE` & `issue_db_api-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/PKG-INFO` & `issue_db_api-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.8.0
+Version: 0.8.1
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.8.0/issue_db_api/Cargo.toml` & `issue_db_api-0.8.1/issue_db_api/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.8.0"
+version = "0.8.1"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.8.0/issue_db_api/issue_api.pyi` & `issue_db_api-0.8.1/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/api_core.rs` & `issue_db_api-0.8.1/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/comments.rs` & `issue_db_api-0.8.1/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/config.rs` & `issue_db_api-0.8.1/issue_db_api/src/config.rs`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         )?;
         let issues = ids.into_iter()
             .map(|id| Issue::new(
                 api.clone(),
                 id.clone(),
                 data.get(&id).unwrap().clone(),
                 label_caching_policy,
-                labels.get(&id).cloned()))
+                if self.preload_labels { Some(labels.get(&id).cloned()) } else { None }))
             .collect();
         Ok(issues)
     }
 
     pub fn load_issue(self,
                       api: Arc<IssueAPI>,
                       id: String,
```

### Comparing `issue_db_api-0.8.0/issue_db_api/src/embedding.rs` & `issue_db_api-0.8.1/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/errors.rs` & `issue_db_api-0.8.1/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/issues.rs` & `issue_db_api-0.8.1/issue_db_api/src/issues.rs`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
 #[allow(unused)]
 impl Issue {
     pub(crate) fn new(api: Arc<IssueAPI>,
                       ident: String,
                       data: IssueData,
                       caching: CachingPolicy,
-                      label: Option<Label>) -> Self {
-         Self{
-             api, ident, data,
-             caching_policy: caching,
-             label: CacheContainer::new(Some(label)),
-             dirty: AtomicBool::new(false)
+                      label: Option<Option<Label>>) -> Self {
+        Self{
+            api, ident, data,
+            caching_policy: caching,
+            label: CacheContainer::new(label),
+            dirty: AtomicBool::new(false)
         }
     }
 
     #[inline(always)]
     pub fn ident(&self) -> &String {
         &self.ident
     }
```

### Comparing `issue_db_api-0.8.0/issue_db_api/src/labels.rs` & `issue_db_api-0.8.1/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/lib.rs` & `issue_db_api-0.8.1/issue_db_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/models.rs` & `issue_db_api-0.8.1/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/query.rs` & `issue_db_api-0.8.1/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/repository.rs` & `issue_db_api-0.8.1/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.8.1/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/tags.rs` & `issue_db_api-0.8.1/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/issue_db_api/src/util.rs` & `issue_db_api-0.8.1/issue_db_api/src/util.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::fmt::Debug;
 use std::sync::atomic::{AtomicBool, Ordering};
 use std::sync::RwLock;
 use crate::errors::{APIResult};
 
 
 macro_rules! initialize_lazy_field {
     ($e:expr) => {
@@ -41,15 +42,15 @@
 #[derive(Debug)]
 pub struct CacheContainer<T: Clone> {
     value: RwLock<Option<T>>,
     dirty: AtomicBool
 }
 
 
-impl<T: Clone> CacheContainer<T> {
+impl<T: Clone + Debug> CacheContainer<T> {
     pub fn new(initial: Option<T>) -> Self {
         let dirty = initial.is_none();
         CacheContainer{
             value: RwLock::new(initial),
             dirty: AtomicBool::new(dirty)
         }
     }
```

### Comparing `issue_db_api-0.8.0/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.8.1/issue_db_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.8.0
+Version: 0.8.1
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.8.0/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.8.1/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.0/pyproject.toml` & `issue_db_api-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```


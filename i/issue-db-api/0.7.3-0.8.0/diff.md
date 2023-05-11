# Comparing `tmp/issue_db_api-0.7.3.tar.gz` & `tmp/issue_db_api-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.7.3.tar", last modified: Tue May  9 14:48:59 2023, max compression
+gzip compressed data, was "issue_db_api-0.8.0.tar", last modified: Thu May 11 10:19:34 2023, max compression
```

## Comparing `issue_db_api-0.7.3.tar` & `issue_db_api-0.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.7.3/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.033291 issue_db_api-0.7.3/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-09 14:48:21.000000 issue_db_api-0.7.3/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.7.3/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8397 2023-05-04 14:07:06.000000 issue_db_api-0.7.3/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    44641 2023-05-09 14:47:42.000000 issue_db_api-0.7.3/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.7.3/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    38608 2023-05-04 13:59:32.000000 issue_db_api-0.7.3/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.7.3/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6387 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2514 2023-05-05 12:20:10.000000 issue_db_api-0.7.3/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.033291 issue_db_api-0.7.3/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.7.3/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-09 14:48:21.000000 issue_db_api-0.7.3/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.8.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.987801 issue_db_api-0.8.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-11 10:12:58.000000 issue_db_api-0.8.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.8.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8716 2023-05-11 10:14:20.000000 issue_db_api-0.8.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    44902 2023-05-11 10:01:47.000000 issue_db_api-0.8.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.8.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    39893 2023-05-11 10:14:19.000000 issue_db_api-0.8.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.8.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6964 2023-05-11 10:03:52.000000 issue_db_api-0.8.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.8.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2554 2023-05-11 10:04:43.000000 issue_db_api-0.8.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 10:19:34.987801 issue_db_api-0.8.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.8.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-11 10:19:34.000000 issue_db_api-0.8.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-11 10:12:58.000000 issue_db_api-0.8.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-11 10:19:34.991801 issue_db_api-0.8.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.8.0/setup.py
```

### Comparing `issue_db_api-0.7.3/LICENSE` & `issue_db_api-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/PKG-INFO` & `issue_db_api-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.7.3
+Version: 0.8.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.7.3/issue_db_api/Cargo.toml` & `issue_db_api-0.8.0/issue_db_api/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.7.3"
+version = "0.8.0"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.7.3/issue_db_api/issue_api.pyi` & `issue_db_api-0.8.0/issue_db_api/issue_api.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,23 @@
                  url: str, *,
                  credentials: tuple[str, str] | None = None,
                  label_caching_policy: str = 'no_caching',
                  config_handling_policy: str = 'read_fetch_write_fetch',
                  allow_self_signed_certificates: bool = False):
         ...
 
+    @classmethod
+    def from_token(cls,
+                   url: str, *,
+                   token: str,
+                   label_caching_policy: str = 'no_caching',
+                   config_handling_policy: str = 'read_fetch_write_fetch',
+                   allow_self_signed_certificates: bool = False):
+        ...
+
     def __repr__(self) -> str:
         ...
 
     def search(self, /,
                q: Query, *,
                attributes: list[str] = (),
                load_labels: bool = False) -> list[Issue]:
```

### Comparing `issue_db_api-0.7.3/issue_db_api/src/api_core.rs` & `issue_db_api-0.8.0/issue_db_api/src/api_core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,20 @@
                 url,
                 token: None,
                 client,
                 allow_unsafe_ssl: allow_self_signed
             }
         )
     }
+    
+    pub(crate) fn with_token(url: String, token: String, allow_self_signed: bool) -> APIResult<Self> {
+        let mut read_only_api = Self::new_read_only(url, allow_self_signed)?;
+        read_only_api.token = Some(token);
+        Ok(read_only_api)
+    }
 
     fn login(&mut self, username: String, password: String) -> APIResult<()> {
         #[derive(serde::Deserialize)]
         struct TokenResponse {
             access_token: String,
             #[allow(dead_code)] token_type: String
         }
```

### Comparing `issue_db_api-0.7.3/issue_db_api/src/comments.rs` & `issue_db_api-0.8.0/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/config.rs` & `issue_db_api-0.8.0/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/embedding.rs` & `issue_db_api-0.8.0/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/errors.rs` & `issue_db_api-0.8.0/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/issues.rs` & `issue_db_api-0.8.0/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/labels.rs` & `issue_db_api-0.8.0/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/lib.rs` & `issue_db_api-0.8.0/issue_db_api/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 mod python {
     use std::collections::HashMap;
     use std::hash::{Hash, Hasher};
     use pyo3::basic::CompareOp;
     use pyo3::prelude::*;
     use pyo3::create_exception;
     use pyo3::exceptions::{PyException, PyTypeError, PyValueError};
-    use pyo3::types::{IntoPyDict, PyBool, PyDict, PyFloat, PyInt, PyList, PyLong, PyString, PyTuple};
+    use pyo3::types::{IntoPyDict, PyBool, PyDict, PyFloat, PyInt, PyList, PyLong, PyString, PyTuple, PyType};
     use serde_json::{Map, Number, Value};
     use crate::comments::Comment;
     use crate::config::{CachingPolicy, ConfigHandlingPolicy, IssueAttribute, IssueLoadingSettings};
     use crate::embedding::Embedding;
     use crate::errors::APIError;
     use crate::issues::Issue;
     use crate::labels::Label;
@@ -150,14 +150,37 @@
     #[allow(unused)]
     struct PyIssueRepository {
         url: String,
         authenticated: bool,
         repo: IssueRepository
     }
 
+    fn parse_caching_handling(label_caching_policy: &str) -> PyResult<CachingPolicy> {
+        match label_caching_policy {
+            "no_caching" => Ok(CachingPolicy::NoCaching),
+            "use_local_after_load" => Ok(CachingPolicy::UseLocalAfterLoad),
+            _ => {
+                let text = format!("Invalid caching policy: {}", label_caching_policy);
+                Err(IssueAPIError::new_err(text))
+            }
+        }
+    }
+
+    fn parse_config_policy(config_handling_policy: &str) -> PyResult<ConfigHandlingPolicy> {
+        match config_handling_policy {
+            "read_fetch_write_fetch" => Ok(ConfigHandlingPolicy::ReadFetchWriteWithFetch),
+            "read_local_write_fetch" => Ok(ConfigHandlingPolicy::ReadLocalWriteWithFetch),
+            "read_local_write_local" => Ok(ConfigHandlingPolicy::ReadLocalWriteNoFetch),
+            _ => {
+                let text = format!("Invalid config handling policy: {}", config_handling_policy);
+                Err(IssueAPIError::new_err(text))
+            }
+        }
+    }
+
     #[pymethods]
     impl PyIssueRepository {
         #[new]
         #[pyo3(signature=(
             url, *,
             credentials=None,
             label_caching_policy="no_caching",
@@ -165,31 +188,16 @@
             allow_self_signed_certificates=false
         ))]
         fn __new__(url: String,
                    credentials: Option<(String, String)>,
                    label_caching_policy: &str,
                    config_handling_policy: &str,
                    allow_self_signed_certificates: bool) -> PyResult<Self> {
-            let caching = match label_caching_policy {
-                "no_caching" => CachingPolicy::NoCaching,
-                "use_local_after_load" => CachingPolicy::UseLocalAfterLoad,
-                _ => {
-                    let text = format!("Invalid caching policy: {}", label_caching_policy);
-                    return Err(IssueAPIError::new_err(text));
-                }
-            };
-            let config_handling = match config_handling_policy {
-                "read_fetch_write_fetch" => ConfigHandlingPolicy::ReadFetchWriteWithFetch,
-                "read_local_write_fetch" => ConfigHandlingPolicy::ReadLocalWriteWithFetch,
-                "read_local_write_local" => ConfigHandlingPolicy::ReadLocalWriteNoFetch,
-                _ => {
-                    let text = format!("Invalid config handling policy: {}", config_handling_policy);
-                    return Err(IssueAPIError::new_err(text));
-                }
-            };
+            let caching = parse_caching_handling(label_caching_policy)?;
+            let config_handling = parse_config_policy(config_handling_policy)?;
             let (repo, auth) = if let Some((username, password)) = credentials {
                 (
                     IssueRepository::new(url.clone(),
                                          username,
                                          password,
                                          caching,
                                          config_handling,
@@ -204,14 +212,40 @@
                                                    allow_self_signed_certificates),
                     false
                 )
             };
             Ok(Self{url, authenticated: auth, repo: api2py_error(repo)?})
         }
 
+        #[classmethod]
+        #[pyo3(signature=(
+            url, *,
+            token,
+            label_caching_policy="no_caching",
+            config_handling_policy="read_fetch_write_fetch",
+            allow_self_signed_certificates=false
+            ))]
+        fn from_token(_cls: &PyType,
+                      url: String,
+                      token: String,
+                      label_caching_policy: &str,
+                      config_handling_policy: &str,
+                      allow_self_signed_certificates: bool) -> PyResult<Self> {
+            let caching = parse_caching_handling(label_caching_policy)?;
+            let config_handling = parse_config_policy(config_handling_policy)?;
+            let repo = IssueRepository::new_with_token(
+                url.clone(),
+                token,
+                caching,
+                config_handling,
+                allow_self_signed_certificates
+            );
+            Ok(PyIssueRepository{url, authenticated: true, repo: api2py_error(repo)?})
+        }
+
         fn __repr__(&self) -> PyResult<String> {
             let text = format!(
                 "<IssueRepository|url={}, authenticated={}>", self.url, self.authenticated
             );
             Ok(text)
         }
```

### Comparing `issue_db_api-0.7.3/issue_db_api/src/models.rs` & `issue_db_api-0.8.0/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/query.rs` & `issue_db_api-0.8.0/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/repository.rs` & `issue_db_api-0.8.0/issue_db_api/src/repository.rs`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,29 @@
             Self{
                 api,
                 label_caching: label_caching_policy,
                 config_handling: config_handling_policy
             }
         )
     }
+    
+    pub fn new_with_token(url: String,
+                          token: String, 
+                          label_caching_policy: CachingPolicy,
+                          config_handling_policy: ConfigHandlingPolicy,
+                          allow_self_signed_certs: bool) -> APIResult<Self> {
+        let api = Arc::new(IssueAPI::with_token(url, token, allow_self_signed_certs)?);
+        Ok(
+            Self{
+                api,
+                label_caching: label_caching_policy,
+                config_handling: config_handling_policy
+            }
+        )
+    }
 
     pub fn search(&self,
                   query: Query,
                   issue_loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
         let ids = self.api.search(query)?;
         if ids.is_empty() {
             return Ok(Vec::new());
```

### Comparing `issue_db_api-0.7.3/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.8.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/tags.rs` & `issue_db_api-0.8.0/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/issue_db_api/src/util.rs` & `issue_db_api-0.8.0/issue_db_api/src/util.rs`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,18 @@
     value: RwLock<Option<T>>,
     dirty: AtomicBool
 }
 
 
 impl<T: Clone> CacheContainer<T> {
     pub fn new(initial: Option<T>) -> Self {
+        let dirty = initial.is_none();
         CacheContainer{
             value: RwLock::new(initial),
-            dirty: AtomicBool::new(true)
+            dirty: AtomicBool::new(dirty)
         }
     }
 
     pub fn get<F: FnOnce() -> APIResult<T>>(&self, f: F) -> APIResult<T> {
         let obj = self.value
             .read()
             .map_err(|_| CacheLockError{})?;
```

### Comparing `issue_db_api-0.7.3/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.8.0/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.7.3
+Version: 0.8.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.7.3/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.8.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.3/pyproject.toml` & `issue_db_api-0.8.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.7.3"
+version = "0.8.0"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```


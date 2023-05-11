# Comparing `tmp/rnapykin-0.1.0.tar.gz` & `tmp/rnapykin-0.2.0.tar.gz`

## Comparing `rnapykin-0.1.0.tar` & `rnapykin-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 rnapykin-0.1.0/Cargo.toml
--rw-rw-r--   0     1000     1000      370 2023-05-10 19:23:45.000000 rnapykin-0.1.0/pyproject.toml
--rw-rw-r--   0     1000     1000     4667 2023-05-10 19:27:05.000000 rnapykin-0.1.0/src/lib.rs
--rw-rw-r--   0     1000     1000    36897 2023-05-10 19:24:50.000000 rnapykin-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 rnapykin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 rnapykin-0.2.0/Cargo.toml
+-rw-rw-r--   0     1000     1000    71220 2023-05-10 20:09:02.000000 rnapykin-0.2.0/mxflip.svg
+-rw-rw-r--   0     1000     1000    71388 2023-05-10 20:10:07.000000 rnapykin-0.2.0/myflip.svg
+-rw-rw-r--   0     1000     1000      370 2023-05-10 19:57:37.000000 rnapykin-0.2.0/pyproject.toml
+-rw-rw-r--   0     1000     1000    71244 2023-05-10 20:10:34.000000 rnapykin-0.2.0/reg.svg
+-rw-rw-r--   0     1000     1000    70737 2023-05-10 20:03:18.000000 rnapykin-0.2.0/res.svg
+-rw-rw-r--   0     1000     1000     3752 2023-05-10 20:11:41.000000 rnapykin-0.2.0/src/lib.rs
+-rw-rw-r--   0     1000     1000    36897 2023-05-10 19:57:53.000000 rnapykin-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 rnapykin-0.2.0/PKG-INFO
```

### Comparing `rnapykin-0.1.0/Cargo.lock` & `rnapykin-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -935,15 +935,15 @@
  "atty",
  "clap",
  "plotters",
 ]
 
 [[package]]
 name = "rnapykin"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "rnapkin",
 ]
 
 [[package]]
 name = "rustc_version"
```


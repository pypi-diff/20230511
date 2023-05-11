# Comparing `tmp/os2ds-rules-0.0.5.tar.gz` & `tmp/os2ds-rules-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2ds-rules-0.0.5.tar", last modified: Mon Apr 24 16:01:41 2023, max compression
+gzip compressed data, was "os2ds-rules-0.0.6.tar", last modified: Thu May 11 12:31:16 2023, max compression
```

## Comparing `os2ds-rules-0.0.5.tar` & `os2ds-rules-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:41.627310 os2ds-rules-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-24 16:01:41.627310 os2ds-rules-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:41.623310 os2ds-rules-0.0.5/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/include/cpr-detector.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:41.623310 os2ds-rules-0.0.5/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/lib/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/lib/cpr-detector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/lib/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/lib/wordlist_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:01:41.627310 os2ds-rules-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:41.623310 os2ds-rules-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:41.623310 os2ds-rules-0.0.5/src/os2ds_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/src/os2ds_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/src/os2ds_rules/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/src/os2ds_rules/cpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/src/os2ds_rules/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-24 16:01:28.000000 os2ds-rules-0.0.5/src/os2ds_rules/wordlist_rule.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:41.627310 os2ds-rules-0.0.5/src/os2ds_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-24 16:01:41.000000 os2ds-rules-0.0.5/src/os2ds_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-24 16:01:41.000000 os2ds-rules-0.0.5/src/os2ds_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:01:41.000000 os2ds-rules-0.0.5/src/os2ds_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 16:01:41.000000 os2ds-rules-0.0.5/src/os2ds_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:16.940144 os2ds-rules-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-11 12:31:16.940144 os2ds-rules-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:16.936144 os2ds-rules-0.0.6/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/include/cpr-detector.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:16.936144 os2ds-rules-0.0.6/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/lib/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/lib/cpr-detector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/lib/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/lib/wordlist_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:31:16.940144 os2ds-rules-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:16.936144 os2ds-rules-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:16.940144 os2ds-rules-0.0.6/src/os2ds_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/src/os2ds_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/src/os2ds_rules/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/src/os2ds_rules/cpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/src/os2ds_rules/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-11 12:31:04.000000 os2ds-rules-0.0.6/src/os2ds_rules/wordlist_rule.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:31:16.940144 os2ds-rules-0.0.6/src/os2ds_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-11 12:31:16.000000 os2ds-rules-0.0.6/src/os2ds_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 12:31:16.000000 os2ds-rules-0.0.6/src/os2ds_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:31:16.000000 os2ds-rules-0.0.6/src/os2ds_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 12:31:16.000000 os2ds-rules-0.0.6/src/os2ds_rules.egg-info/top_level.txt
```

### Comparing `os2ds-rules-0.0.5/LICENSE` & `os2ds-rules-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/PKG-INFO` & `os2ds-rules-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.5
+Version: 0.0.6
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `os2ds-rules-0.0.5/README.md` & `os2ds-rules-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/include/cpr-detector.hpp` & `os2ds-rules-0.0.6/include/cpr-detector.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 namespace CPRDetector {
 
 constexpr bool is_nonzero_digit(char c) noexcept { return '0' < c && c <= '9'; }
 
 constexpr bool is_digit(char c) noexcept { return '0' <= c && c <= '9'; }
 
-const auto is_separator = make_predicate(' ', '-', '/');
+const auto is_separator = make_predicate(' ', '-', '/', '\t');
 
 const auto is_previous_ok = make_predicate(char(0), ' ', '\n', '\t', '\0');
 
 constexpr bool is_space(const char c) noexcept { return c == ' '; }
 
 static constexpr std::array<int, 10> modulus11_factors = {4, 3, 2, 7, 6,
                                                           5, 4, 3, 2, 1};
```

### Comparing `os2ds-rules-0.0.5/lib/address_rule.cpp` & `os2ds-rules-0.0.6/lib/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/lib/cpr-detector.cpp` & `os2ds-rules-0.0.6/lib/cpr-detector.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/lib/name_rule.cpp` & `os2ds-rules-0.0.6/lib/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/lib/wordlist_rule.cpp` & `os2ds-rules-0.0.6/lib/wordlist_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/pyproject.toml` & `os2ds-rules-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os2ds-rules"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="HackTheOxidation", email="tomas.hagenau@protonmail.ch" },
 ]
 description = "Text processing tool for detecting Danish CPR-numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `os2ds-rules-0.0.5/setup.py` & `os2ds-rules-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/src/os2ds_rules/__init__.py` & `os2ds-rules-0.0.6/src/os2ds_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/src/os2ds_rules/address_rule.cpp` & `os2ds-rules-0.0.6/src/os2ds_rules/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/src/os2ds_rules/cpr.cpp` & `os2ds-rules-0.0.6/src/os2ds_rules/cpr.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/src/os2ds_rules/name_rule.cpp` & `os2ds-rules-0.0.6/src/os2ds_rules/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/src/os2ds_rules/wordlist_rule.cpp` & `os2ds-rules-0.0.6/src/os2ds_rules/wordlist_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.5/src/os2ds_rules.egg-info/PKG-INFO` & `os2ds-rules-0.0.6/src/os2ds_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.5
+Version: 0.0.6
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```


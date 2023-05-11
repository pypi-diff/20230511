# Comparing `tmp/pywencai-0.8.3.tar.gz` & `tmp/pywencai-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.8.3.tar", max compression
+gzip compressed data, was "pywencai-0.8.4.tar", max compression
```

## Comparing `pywencai-0.8.3.tar` & `pywencai-0.8.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-11 04:49:50.410360 pywencai-0.8.3/LICENSE
--rw-r--r--   0        0        0     2446 2023-05-11 04:49:50.410360 pywencai-0.8.3/README.md
--rw-r--r--   0        0        0      612 2023-05-11 04:49:50.410360 pywencai-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-11 04:49:50.410360 pywencai-0.8.3/pywencai/__init__.py
--rw-r--r--   0        0        0     3559 2023-05-11 04:49:50.414360 pywencai-0.8.3/pywencai/convert.py
--rw-r--r--   0        0        0    39677 2023-05-11 04:49:50.414360 pywencai-0.8.3/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4477 2023-05-11 04:49:50.414360 pywencai-0.8.3/pywencai/wencai.py
--rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 pywencai-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-11 04:59:27.411391 pywencai-0.8.4/LICENSE
+-rw-r--r--   0        0        0     2446 2023-05-11 04:59:27.411391 pywencai-0.8.4/README.md
+-rw-r--r--   0        0        0      612 2023-05-11 04:59:27.411391 pywencai-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-11 04:59:27.411391 pywencai-0.8.4/pywencai/__init__.py
+-rw-r--r--   0        0        0     3559 2023-05-11 04:59:27.411391 pywencai-0.8.4/pywencai/convert.py
+-rw-r--r--   0        0        0    39677 2023-05-11 04:59:27.411391 pywencai-0.8.4/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4477 2023-05-11 04:59:27.415391 pywencai-0.8.4/pywencai/wencai.py
+-rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 pywencai-0.8.4/PKG-INFO
```

### Comparing `pywencai-0.8.3/LICENSE` & `pywencai-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.3/README.md` & `pywencai-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.3/pyproject.toml` & `pywencai-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.8.3"
+version = "0.8.4"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.8.3/pywencai/convert.py` & `pywencai-0.8.4/pywencai/convert.py`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.3/pywencai/hexin-v.js` & `pywencai-0.8.4/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.3/pywencai/wencai.py` & `pywencai-0.8.4/pywencai/wencai.py`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.3/PKG-INFO` & `pywencai-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.8.3
+Version: 0.8.4
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


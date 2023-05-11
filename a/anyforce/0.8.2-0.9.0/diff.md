# Comparing `tmp/anyforce-0.8.2.tar.gz` & `tmp/anyforce-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyforce-0.8.2.tar", last modified: Thu Nov  4 12:13:57 2021, max compression
+gzip compressed data, was "anyforce-0.9.0.tar", last modified: Thu Nov  4 15:34:02 2021, max compression
```

## Comparing `anyforce-0.8.2.tar` & `anyforce-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-11-04 12:09:29.844592 anyforce-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17193 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6691 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/g.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/security/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/security/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/api/security/session.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/bl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-11-04 12:09:29.844592 anyforce-0.8.2/anyforce/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/logging/colorful.py
--rw-r--r--   0 runner    (1001) docker     (121)     5608 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/logging/context.py
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/logging/level.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6629 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/model/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/model/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/model/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/model/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/model/recoverialbe.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/model/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/test/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     3608 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/test/request.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-11-04 12:09:29.848593 anyforce-0.8.2/anyforce/typing/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2021-11-04 12:09:29.848593 anyforce-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-04 12:09:29.848593 anyforce-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2021-11-04 12:09:29.848593 anyforce-0.8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2021-11-04 12:09:29.848593 anyforce-0.8.2/tests/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6064 2021-11-04 12:09:29.848593 anyforce-0.8.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-04 12:09:29.848593 anyforce-0.8.2/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-11-04 12:09:29.848593 anyforce-0.8.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2021-11-04 12:09:29.848593 anyforce-0.8.2/tests/test_security.py
--rw-------   0 runner    (1001) docker     (121)      451 2021-11-04 12:13:57.921629 anyforce-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-11-04 15:32:01.503093 anyforce-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17193 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6691 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/g.py
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/security/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3197 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/security/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/api/security/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/bl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/logging/colorful.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5608 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/logging/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/logging/level.py
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6629 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/model/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4883 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/model/patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/model/recoverialbe.py
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/model/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6533 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/test/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3608 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/test/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-11-04 15:32:01.503093 anyforce-0.9.0/anyforce/typing/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-11-04 15:32:01.507093 anyforce-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-04 15:32:01.507093 anyforce-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2021-11-04 15:32:01.507093 anyforce-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2021-11-04 15:32:01.507093 anyforce-0.9.0/tests/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6064 2021-11-04 15:32:01.507093 anyforce-0.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-04 15:32:01.507093 anyforce-0.9.0/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-11-04 15:32:01.507093 anyforce-0.9.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2021-11-04 15:32:01.507093 anyforce-0.9.0/tests/test_security.py
+-rw-------   0 runner    (1001) docker     (121)      451 2021-11-04 15:34:02.620654 anyforce-0.9.0/PKG-INFO
```

### Comparing `anyforce-0.8.2/anyforce/__init__.py` & `anyforce-0.9.0/anyforce/__init__.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/api/api.py` & `anyforce-0.9.0/anyforce/api/api.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/api/exceptions.py` & `anyforce-0.9.0/anyforce/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/api/security/jwt.py` & `anyforce-0.9.0/anyforce/api/security/jwt.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/api/security/oauth2.py` & `anyforce-0.9.0/anyforce/api/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/bl/__init__.py` & `anyforce-0.9.0/anyforce/bl/__init__.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/json/__init__.py` & `anyforce-0.9.0/anyforce/json/__init__.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/logging/__init__.py` & `anyforce-0.9.0/anyforce/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/logging/colorful.py` & `anyforce-0.9.0/anyforce/logging/colorful.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/logging/context.py` & `anyforce-0.9.0/anyforce/logging/context.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/model/base.py` & `anyforce-0.9.0/anyforce/model/base.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/model/enum.py` & `anyforce-0.9.0/anyforce/model/enum.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/model/fields.py` & `anyforce-0.9.0/anyforce/model/fields.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/model/patch.py` & `anyforce-0.9.0/anyforce/model/patch.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/model/recoverialbe.py` & `anyforce-0.9.0/anyforce/model/recoverialbe.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/test/api.py` & `anyforce-0.9.0/anyforce/test/api.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/test/fixtures.py` & `anyforce-0.9.0/anyforce/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/anyforce/test/request.py` & `anyforce-0.9.0/anyforce/test/request.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/tests/conftest.py` & `anyforce-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/tests/model.py` & `anyforce-0.9.0/tests/model.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/tests/test_api.py` & `anyforce-0.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/tests/test_exception.py` & `anyforce-0.9.0/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `anyforce-0.8.2/tests/test_security.py` & `anyforce-0.9.0/tests/test_security.py`

 * *Files identical despite different names*


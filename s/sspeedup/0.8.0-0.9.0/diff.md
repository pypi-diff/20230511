# Comparing `tmp/sspeedup-0.8.0.tar.gz` & `tmp/sspeedup-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspeedup-0.8.0.tar", max compression
+gzip compressed data, was "sspeedup-0.9.0.tar", max compression
```

## Comparing `sspeedup-0.8.0.tar` & `sspeedup-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,32 @@
--rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.8.0/LICENSE
--rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.8.0/README.md
--rw-r--r--   0        0        0     1337 2023-04-14 23:08:51.965326 sspeedup-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      552 2023-04-14 22:27:40.256275 sspeedup-0.8.0/sspeedup/ability/exceptions.py
--rw-r--r--   0        0        0     2031 2023-04-14 22:27:40.256275 sspeedup-0.8.0/sspeedup/ability/word_split/_base.py
--rw-r--r--   0        0        0     7639 2023-04-14 23:07:38.449428 sspeedup-0.8.0/sspeedup/ability/word_split/jieba.py
--rw-r--r--   0        0        0     2311 2023-04-14 22:08:58.626733 sspeedup-0.8.0/sspeedup/api.py
--rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.8.0/sspeedup/cache/timeout.py
--rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.8.0/sspeedup/colorful_print.py
--rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.8.0/sspeedup/dict_helper.py
--rw-r--r--   0        0        0    12985 2023-04-14 22:09:36.418433 sspeedup-0.8.0/sspeedup/logging/run_logger.py
--rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.8.0/sspeedup/make_qrcode.py
--rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.8.0/sspeedup/pywebio/callbacks.py
--rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/require.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.8.0/sspeedup/retry/__init__.py
--rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/retry/deco.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.8.0/sspeedup/retry/event.py
--rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/retry/policy.py
--rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/time_helper.py
--rw-r--r--   0        0        0     2202 2023-04-14 22:27:40.256275 sspeedup-0.8.0/sspeedup/word_split/_base.py
--rw-r--r--   0        0        0     4363 2023-04-14 22:27:40.259608 sspeedup-0.8.0/sspeedup/word_split/jieba.py
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 sspeedup-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.9.0/LICENSE
+-rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.9.0/README.md
+-rw-r--r--   0        0        0     1337 2023-04-22 00:16:05.906192 sspeedup-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      553 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/ability/exceptions.py
+-rw-r--r--   0        0        0     2031 2023-04-14 22:27:40.256275 sspeedup-0.9.0/sspeedup/ability/word_split/_base.py
+-rw-r--r--   0        0        0     7641 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/ability/word_split/jieba.py
+-rw-r--r--   0        0        0     2312 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/api.py
+-rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.9.0/sspeedup/cache/timeout.py
+-rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.9.0/sspeedup/colorful_print.py
+-rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.9.0/sspeedup/dict_helper.py
+-rw-r--r--   0        0        0    12985 2023-04-14 22:09:36.418433 sspeedup-0.9.0/sspeedup/logging/run_logger.py
+-rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.9.0/sspeedup/make_qrcode.py
+-rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.9.0/sspeedup/pywebio/callbacks.py
+-rw-r--r--   0        0        0      492 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/pywebio/clipboard.py
+-rw-r--r--   0        0        0      577 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/pywebio/cookies.py
+-rw-r--r--   0        0        0      114 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/pywebio/footer.py
+-rw-r--r--   0        0        0      932 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/pywebio/html.py
+-rw-r--r--   0        0        0      174 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/pywebio/loading.py
+-rw-r--r--   0        0        0      565 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/pywebio/navigation.py
+-rw-r--r--   0        0        0      177 2023-04-22 00:16:05.906192 sspeedup-0.9.0/sspeedup/pywebio/patch.py
+-rw-r--r--   0        0        0      250 2023-04-22 00:16:05.909526 sspeedup-0.9.0/sspeedup/pywebio/query_params.py
+-rw-r--r--   0        0        0      167 2023-04-22 00:16:05.909526 sspeedup-0.9.0/sspeedup/pywebio/scope.py
+-rw-r--r--   0        0        0      250 2023-04-22 00:16:05.909526 sspeedup-0.9.0/sspeedup/pywebio/toast.py
+-rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.9.0/sspeedup/require.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.9.0/sspeedup/retry/__init__.py
+-rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.9.0/sspeedup/retry/deco.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.9.0/sspeedup/retry/event.py
+-rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.9.0/sspeedup/retry/policy.py
+-rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.9.0/sspeedup/time_helper.py
+-rw-r--r--   0        0        0     2202 2023-04-14 22:27:40.256275 sspeedup-0.9.0/sspeedup/word_split/_base.py
+-rw-r--r--   0        0        0     4363 2023-04-21 22:56:58.414571 sspeedup-0.9.0/sspeedup/word_split/jieba.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 sspeedup-0.9.0/PKG-INFO
```

### Comparing `sspeedup-0.8.0/LICENSE` & `sspeedup-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/pyproject.toml` & `sspeedup-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sspeedup"
-version = "0.8.0"
+version = "0.9.0"
 description = "开发工具箱"
 authors = ["yezi <yehaowei20060411@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FHU-yezi/sspeedup"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -14,20 +14,20 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pymongo = { version = "^4.3.3", optional = true }
 jieba = { version = "^0.42.1", optional = true }
 qrcode = { version = "^7.4.2", optional = true }
-pywebio = { version = "^1.7.1", optional = true }
+pywebio = { version = "^1.8.1", optional = true }
 sanic = { version = "^23.3.0", optional = true }
 httpx = { version = "^0.24.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.260"
+ruff = "^0.0.262"
 pyright = "^1.1.293"
 black = "^23.1.0"
 
 [tool.poetry.extras]
 logging = ["pymongo"]
 word-split-jieba = ["jieba"]
 qrcode = ["qrcode"]
```

### Comparing `sspeedup-0.8.0/sspeedup/ability/exceptions.py` & `sspeedup-0.9.0/sspeedup/ability/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     def __init__(self, code: int, message: str = "") -> None:
         self.code = code
         self.message = message
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}(code={self.code}, message={self.message})"
 
+
 class AbilityCallServiceError(Exception):
     def __init__(self, code: int, message: str = "") -> None:
         self.code = code
         self.message = message
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}(code={self.code}, message={self.message})"
```

### Comparing `sspeedup-0.8.0/sspeedup/ability/word_split/_base.py` & `sspeedup-0.9.0/sspeedup/ability/word_split/_base.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/ability/word_split/jieba.py` & `sspeedup-0.9.0/sspeedup/ability/word_split/jieba.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             {
                 key: value
                 for key, value in response_json["data"]["word_freq"].items()
                 if key not in self.stopwords
             }
         )
 
+
 class AbilityJiebaSearchSplitterV1(AbilitySplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
         self.stopwords = word_list_to_add
@@ -157,14 +158,15 @@
             {
                 key: value
                 for key, value in response_json["data"]["word_freq"].items()
                 if key not in self.stopwords
             }
         )
 
+
 class AbilityJiebaPossegSplitterV1(AbilitySplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
         self.stopwords = word_list_to_add
```

### Comparing `sspeedup-0.8.0/sspeedup/api.py` & `sspeedup-0.9.0/sspeedup/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     4：配额
     5：接口维护状态
     6：流控
     7：上游服务
     8：服务器状态
     9：保留
     """
+
     SUCCESS = 0
 
     CLOSE_TO_QUOTA_LIMIT = 141
     DEPRECATED = 151
     UPCOMING_MAINTENANCE = 181
 
     UNKNOWN_DATA_FORMAT = 411
```

### Comparing `sspeedup-0.8.0/sspeedup/cache/timeout.py` & `sspeedup-0.9.0/sspeedup/cache/timeout.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/colorful_print.py` & `sspeedup-0.9.0/sspeedup/colorful_print.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/logging/run_logger.py` & `sspeedup-0.9.0/sspeedup/logging/run_logger.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/make_qrcode.py` & `sspeedup-0.9.0/sspeedup/make_qrcode.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/pywebio/callbacks.py` & `sspeedup-0.9.0/sspeedup/pywebio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/retry/deco.py` & `sspeedup-0.9.0/sspeedup/retry/deco.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/retry/policy.py` & `sspeedup-0.9.0/sspeedup/retry/policy.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/time_helper.py` & `sspeedup-0.9.0/sspeedup/time_helper.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/word_split/_base.py` & `sspeedup-0.9.0/sspeedup/word_split/_base.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/sspeedup/word_split/jieba.py` & `sspeedup-0.9.0/sspeedup/word_split/jieba.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.8.0/PKG-INFO` & `sspeedup-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspeedup
-Version: 0.8.0
+Version: 0.9.0
 Summary: 开发工具箱
 Home-page: https://github.com/FHU-yezi/sspeedup
 License: MIT
 Author: yezi
 Author-email: yehaowei20060411@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Provides-Extra: logging
 Provides-Extra: pywebio
 Provides-Extra: qrcode
 Provides-Extra: word-split-jieba
 Requires-Dist: httpx (>=0.24.0,<0.25.0) ; extra == "ability-word-split"
 Requires-Dist: jieba (>=0.42.1,<0.43.0) ; extra == "word-split-jieba"
 Requires-Dist: pymongo (>=4.3.3,<5.0.0) ; extra == "logging"
-Requires-Dist: pywebio (>=1.7.1,<2.0.0) ; extra == "pywebio"
+Requires-Dist: pywebio (>=1.8.1,<2.0.0) ; extra == "pywebio"
 Requires-Dist: qrcode (>=7.4.2,<8.0.0) ; extra == "qrcode"
 Requires-Dist: sanic (>=23.3.0,<24.0.0) ; extra == "api-response-sanic"
 Project-URL: Repository, https://github.com/FHU-yezi/sspeedup
 Description-Content-Type: text/markdown
 
 # sspeedup
```


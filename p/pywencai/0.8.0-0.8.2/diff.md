# Comparing `tmp/pywencai-0.8.0.tar.gz` & `tmp/pywencai-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.8.0.tar", max compression
+gzip compressed data, was "pywencai-0.8.2.tar", max compression
```

## Comparing `pywencai-0.8.0.tar` & `pywencai-0.8.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-10 05:11:57.659710 pywencai-0.8.0/LICENSE
--rw-r--r--   0        0        0     2446 2023-05-10 05:11:57.659710 pywencai-0.8.0/README.md
--rw-r--r--   0        0        0      613 2023-05-10 05:11:57.659710 pywencai-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/__init__.py
--rw-r--r--   0        0        0     3559 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/convert.py
--rw-r--r--   0        0        0    39677 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4262 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/wencai.py
--rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 pywencai-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-11 04:43:20.364685 pywencai-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2446 2023-05-11 04:43:20.364685 pywencai-0.8.2/README.md
+-rw-r--r--   0        0        0      612 2023-05-11 04:43:20.364685 pywencai-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-11 04:43:20.364685 pywencai-0.8.2/pywencai/__init__.py
+-rw-r--r--   0        0        0     3559 2023-05-11 04:43:20.364685 pywencai-0.8.2/pywencai/convert.py
+-rw-r--r--   0        0        0    39677 2023-05-11 04:43:20.364685 pywencai-0.8.2/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4477 2023-05-11 04:43:20.364685 pywencai-0.8.2/pywencai/wencai.py
+-rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 pywencai-0.8.2/PKG-INFO
```

### Comparing `pywencai-0.8.0/LICENSE` & `pywencai-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.0/README.md` & `pywencai-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.0/pyproject.toml` & `pywencai-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.8.0"
+version = "0.8.2"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
@@ -22,8 +22,8 @@
 notebook = "^6.4.12"
 mypy = "^1.2.0"
 autopep8 = "^2.0.2"
 types-requests = "^2.30.0.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pywencai-0.8.0/pywencai/convert.py` & `pywencai-0.8.2/pywencai/convert.py`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.0/pywencai/hexin-v.js` & `pywencai-0.8.2/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.0/pywencai/wencai.py` & `pywencai-0.8.2/pywencai/wencai.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,27 @@
     '''获取token'''
     with open(os.path.join(os.path.dirname(__file__), 'hexin-v.js'), 'r') as f:
         jscontent = f.read()
     context = execjs.compile(jscontent)
     return context.call("v")
 
 
+def while_do(do, retry=10, sleep=0, log=False):
+    count = 0
+    while count < retry:
+        time.sleep(sleep)
+        try:
+            return do()
+        except:
+            log and logging.warning(f'{count+1}次尝试失败')
+            count += 1
+    # log and logging.info(f'获取get_robot_data失败')
+    return None
+
+
 def get_robot_data(**kwargs):
     '''获取condition'''
     retry = kwargs.get('retry', 10)
     sleep = kwargs.get('sleep', 0)
     question = kwargs.get('query')
     log = kwargs.get('log', False)
     query_type = kwargs.get('query_type', 'stock')
@@ -40,31 +53,35 @@
         'secondary_intent': query_type,
         'question': question
     }
 
     count = 0
     log and logging.info(f'获取condition开始')
 
-    while count < retry:
-        time.sleep(sleep)
+    def do():
         res = rq.request(
             method='POST',
             url='http://www.iwencai.com/customized/chart/get-robot-data',
             json=data,
             headers={
                 'hexin-v': get_token(),
                 'User-Agent': ua.random,
                 'cookie': cookie
             }
         )
         params = convert_params(res)
         log and logging.info(f'获取get_robot_data成功')
         return params
-    log and logging.info(f'获取get_robot_data失败')
-    return None
+
+    result = while_do(do, retry, sleep, log)
+
+    if result is None:
+        log and logging.info(f'获取get_robot_data失败')
+
+    return result
 
 
 def replace_key(key):
     '''替换key'''
     key_map = {
         'question': 'query',
         'sort_key': 'urp_sort_index',
@@ -85,37 +102,37 @@
         'page': 1,
         'source': 'Ths_iwencai_Xuangu',
         **kwargs
     }
     count = 0
     log and logging.info(f'第{data.get("page")}页开始')
 
-    while count < retry:
-        time.sleep(sleep)
-        try:
-            res = rq.request(
-                method='POST',
-                url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
-                data=data,
-                headers={
-                    'hexin-v': get_token(),
-                    'User-Agent': ua.random,
-                    'cookie': cookie
-                },
-                timeout=(5, 10)
-            )
-            result = json.loads(res.text)
-            list = result['answer']['components'][0]['data']['datas']
-            log and logging.info(f'第{data.get("page")}页成功')
-            return pd.DataFrame.from_dict(list)
-        except:
-            log and logging.warning(f'{count+1}次尝试失败')
-            count += 1
-    log and logging.error(f'第{data.get("page")}页失败')
-    return pd.DataFrame.from_dict([])
+    def do():
+        res = rq.request(
+            method='POST',
+            url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
+            data=data,
+            headers={
+                'hexin-v': get_token(),
+                'User-Agent': ua.random,
+                'cookie': cookie
+            },
+            timeout=(5, 10)
+        )
+        result = json.loads(res.text)
+        list = result['answer']['components'][0]['data']['datas']
+        log and logging.info(f'第{data.get("page")}页成功')
+        return pd.DataFrame.from_dict(list)
+    
+    result = while_do(do, retry, sleep, log)
+
+    if result is None:
+        log and logging.error(f'第{data.get("page")}页失败')
+
+    return result
 
 
 def can_loop(loop, count):
     '''是否继续循环'''
     if (loop is True):
         return True
     else:
```

### Comparing `pywencai-0.8.0/PKG-INFO` & `pywencai-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.8.0
+Version: 0.8.2
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


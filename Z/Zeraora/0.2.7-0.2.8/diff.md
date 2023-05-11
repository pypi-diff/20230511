# Comparing `tmp/Zeraora-0.2.7.tar.gz` & `tmp/Zeraora-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.7.tar", last modified: Tue May  9 01:58:15 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.8.tar", last modified: Thu May 11 07:36:58 2023, max compression
```

## Comparing `Zeraora-0.2.7.tar` & `Zeraora-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:15.000000 Zeraora-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-09 01:58:15.000000 Zeraora-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-09 01:58:05.000000 Zeraora-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:15.000000 Zeraora-0.2.7/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-09 01:58:15.000000 Zeraora-0.2.7/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 01:58:15.000000 Zeraora-0.2.7/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:58:15.000000 Zeraora-0.2.7/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 01:58:15.000000 Zeraora-0.2.7/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:58:15.000000 Zeraora-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-09 01:58:05.000000 Zeraora-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:15.000000 Zeraora-0.2.7/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/divisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:15.000000 Zeraora-0.2.7/zeraora/djangobase/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/djangobase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/djangobase/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/typeclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-09 01:58:05.000000 Zeraora-0.2.7/zeraora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-11 07:36:58.000000 Zeraora-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-11 07:36:39.000000 Zeraora-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 07:36:57.000000 Zeraora-0.2.8/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:36:58.000000 Zeraora-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-11 07:36:39.000000 Zeraora-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/divisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:36:58.000000 Zeraora-0.2.8/zeraora/djangobase/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/djangobase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/djangobase/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/typeclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-11 07:36:39.000000 Zeraora-0.2.8/zeraora/utils.py
```

### Comparing `Zeraora-0.2.7/PKG-INFO` & `Zeraora-0.2.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.7
+Version: 0.2.8
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
@@ -17,14 +17,15 @@
             <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
         </div>
         <div align="center">
             <i>长期维护的个人开源工具库</i>
             <br>
             <i>An utility Python package supports for my personal and company projects</i>
         </div>
+        
         ## 特点
         
         - 支持with、注解和实例化三种方式调用的计时器 [`BearTimer`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/BearTimer.md) ；
         - 生成通用representation方便调试时查看对象内部信息的 [`ReprMixin`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md) ；
         - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 [`OnionObject`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/OnionObject.md) ；
         - 安全转换的 `casting()` 和链式调用安全转换的 `Cast` ；
         - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
@@ -60,34 +61,14 @@
         
         ## 兼容性
         
         [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
         
         项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
         
-        ## 更新
-        
-        > 仅列出不兼容旧版的修改，其余变动见git历史。
-        
-        ### 0.2.7（2023-5-09）
-        
-        - 快捷函数 `casting` 更名为 `safecast` ，调用参数一致。
-        - 更改了内部结构，导致使用了 `ReprMixin` 的 Django 模型的迁移文件（migration）中 `CreateModel` 的 `base` 参数传入了错误值。点击[这里](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md)查看解决方案。
-        
-        ### 0.2.5（2023-5-02）
-        
-        - `OnionObject.__repr__()` 不再进行嵌套递归，因为在调试模式中可以展开嵌套，在此递归并无意义。现在OnionObject对象内的OnionObject对象在 `repr()` 后会显示为 `OnionObject(...)` 。
-        - 去除 `OnionObject.__str__()` 方法，可以用 `import json` 后 `json.dumps(OnionObject())` 实现原来的效果。
-        - 更改 `BearTimer` 的默认打印格式。
-        - 将 `BearTimer.output()` 拆分为负责准备打印的 `record()` 和实现打印的 `handle()` 。
-        
-        ### 0.2.0（2023-4-12）
-        
-        - 将递归转化的 `JSONObject` 与仅表层转化的 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
-        
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.2.7 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.2.8 Summary:
 ä¸ä¸ªåå«ååå·¥å·ç±»åå¿«æ·å½æ°çå·¥å·åºãA original utility
 Python package. Home-page: https://github.com/aixcyi/zeraora Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com License: MIT Project-
 URL: Source, https://github.com/aixcyi/zeraora Project-URL: Tracker, https://
 github.com/aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
                 [https://img.shields.io/badge/Python-3.7%20%2B-
@@ -38,31 +38,16 @@
 docstring)ï¼[reStructuredText](https://zh.wikipedia.org/wiki/
 ReStructuredText)æ ¼å¼ï¼ï¼ææ¡£æªå°½äºå®è¯·ç§»æ­¥æºä»£ç æµè§ã ##
 å¼å®¹æ§ [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/
 3.7.html#summary-release-highlights) å¼å§ `dict`
 æ­£å¼æç§æå¥é¡ºåºå­å¨ï¼èèå° `dict` æ¯ Python
 çåºç³ï¼ä¸ºäºé¿ååºç°é¾ä»¥å¯è§çéè¯¯ï¼å èå°è¯¥çæ¬å®ä¸ºå¼å®¹ä¸éãè¿ä¹æ¯ææ¥è§¦è¿çé¡¹ç®ä¸­çæä½è¿è¡çæ¬ï¼æèä¸å¤ªå¸æç»´æ¤å¯¹æ´ä½çæ¬çå¼å®¹ã
 é¡¹ç®ä¼å°½åä¿è¯ååå¼å®¹æ§ï¼ä½è¿æ¯å»ºè®®å¨requirementsä¸­åæç¹å®ççæ¬å·ï¼é¿åå ä¸ºçæ¬æ´æ°æåéèåºç°æ£æçéè¯¯ã
-## æ´æ° > ä»ååºä¸å¼å®¹æ§ççä¿®æ¹ï¼å¶ä½åå¨è§gitåå²ã ###
-0.2.7ï¼2023-5-09ï¼ - å¿«æ·å½æ° `casting` æ´åä¸º `safecast`
-ï¼è°ç¨åæ°ä¸è´ã - æ´æ¹äºåé¨ç»æï¼å¯¼è´ä½¿ç¨äº `ReprMixin`
-ç Django æ¨¡åçè¿ç§»æä»¶ï¼migrationï¼ä¸­ `CreateModel` ç `base`
-åæ°ä¼ å¥äºéè¯¯å¼ãç¹å»[è¿é](https://github.com/aixcyi/zeraora/
-blob/master/docs/zeraora/ReprMixin.md)æ¥çè§£å³æ¹æ¡ã ### 0.2.5ï¼2023-5-
-02ï¼ - `OnionObject.__repr__()`
-ä¸åè¿è¡åµå¥éå½ï¼å ä¸ºå¨è°è¯æ¨¡å¼ä¸­å¯ä»¥å±å¼åµå¥ï¼å¨æ­¤éå½å¹¶æ æä¹ãç°å¨OnionObjectå¯¹è±¡åçOnionObjectå¯¹è±¡å¨
-`repr()` åä¼æ¾ç¤ºä¸º `OnionObject(...)` ã - å»é¤ `OnionObject.__str__
-()` æ¹æ³ï¼å¯ä»¥ç¨ `import json` å `json.dumps(OnionObject())`
-å®ç°åæ¥çææã - æ´æ¹ `BearTimer` çé»è®¤æå°æ ¼å¼ã - å°
-`BearTimer.output()` æåä¸ºè´è´£åå¤æå°ç `record()`
-åå®ç°æå°ç `handle()` ã ### 0.2.0ï¼2023-4-12ï¼ - å°éå½è½¬åç
-`JSONObject` ä¸ä»è¡¨å±è½¬åç `JsonObject` åå¹¶ä¸º `OnionObject`
-ï¼å¹¶å å»åè¿°ä¸¤ä¸ªç±»ã Platform: UNKNOWN Classifier: Development Status
-:: 4 - Beta Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Developers Classifier:
-Operating System :: OS Independent Classifier: Natural Language :: Chinese
-(Simplified) Classifier: License :: OSI Approved :: MIT License Classifier:
-Topic :: Utilities Classifier: Typing :: Typed Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: Chinese (Simplified) Classifier: License :: OSI
+Approved :: MIT License Classifier: Topic :: Utilities Classifier: Typing ::
+Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `Zeraora-0.2.7/README.md` & `Zeraora-0.2.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
 </div>
 <div align="center">
     <i>长期维护的个人开源工具库</i>
     <br>
     <i>An utility Python package supports for my personal and company projects</i>
 </div>
+
 ## 特点
 
 - 支持with、注解和实例化三种方式调用的计时器 [`BearTimer`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/BearTimer.md) ；
 - 生成通用representation方便调试时查看对象内部信息的 [`ReprMixin`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md) ；
 - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 [`OnionObject`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/OnionObject.md) ；
 - 安全转换的 `casting()` 和链式调用安全转换的 `Cast` ；
 - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
@@ -50,27 +51,7 @@
 
 ## 兼容性
 
 [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
 
 项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
 
-## 更新
-
-> 仅列出不兼容旧版的修改，其余变动见git历史。
-
-### 0.2.7（2023-5-09）
-
-- 快捷函数 `casting` 更名为 `safecast` ，调用参数一致。
-- 更改了内部结构，导致使用了 `ReprMixin` 的 Django 模型的迁移文件（migration）中 `CreateModel` 的 `base` 参数传入了错误值。点击[这里](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md)查看解决方案。
-
-### 0.2.5（2023-5-02）
-
-- `OnionObject.__repr__()` 不再进行嵌套递归，因为在调试模式中可以展开嵌套，在此递归并无意义。现在OnionObject对象内的OnionObject对象在 `repr()` 后会显示为 `OnionObject(...)` 。
-- 去除 `OnionObject.__str__()` 方法，可以用 `import json` 后 `json.dumps(OnionObject())` 实现原来的效果。
-- 更改 `BearTimer` 的默认打印格式。
-- 将 `BearTimer.output()` 拆分为负责准备打印的 `record()` 和实现打印的 `handle()` 。
-
-### 0.2.0（2023-4-12）
-
-- 将递归转化的 `JSONObject` 与仅表层转化的 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
-
```

#### html2text {}

```diff
@@ -32,22 +32,7 @@
 docstring)ï¼[reStructuredText](https://zh.wikipedia.org/wiki/
 ReStructuredText)æ ¼å¼ï¼ï¼ææ¡£æªå°½äºå®è¯·ç§»æ­¥æºä»£ç æµè§ã ##
 å¼å®¹æ§ [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/
 3.7.html#summary-release-highlights) å¼å§ `dict`
 æ­£å¼æç§æå¥é¡ºåºå­å¨ï¼èèå° `dict` æ¯ Python
 çåºç³ï¼ä¸ºäºé¿ååºç°é¾ä»¥å¯è§çéè¯¯ï¼å èå°è¯¥çæ¬å®ä¸ºå¼å®¹ä¸éãè¿ä¹æ¯ææ¥è§¦è¿çé¡¹ç®ä¸­çæä½è¿è¡çæ¬ï¼æèä¸å¤ªå¸æç»´æ¤å¯¹æ´ä½çæ¬çå¼å®¹ã
 é¡¹ç®ä¼å°½åä¿è¯ååå¼å®¹æ§ï¼ä½è¿æ¯å»ºè®®å¨requirementsä¸­åæç¹å®ççæ¬å·ï¼é¿åå ä¸ºçæ¬æ´æ°æåéèåºç°æ£æçéè¯¯ã
-## æ´æ° > ä»ååºä¸å¼å®¹æ§ççä¿®æ¹ï¼å¶ä½åå¨è§gitåå²ã ###
-0.2.7ï¼2023-5-09ï¼ - å¿«æ·å½æ° `casting` æ´åä¸º `safecast`
-ï¼è°ç¨åæ°ä¸è´ã - æ´æ¹äºåé¨ç»æï¼å¯¼è´ä½¿ç¨äº `ReprMixin`
-ç Django æ¨¡åçè¿ç§»æä»¶ï¼migrationï¼ä¸­ `CreateModel` ç `base`
-åæ°ä¼ å¥äºéè¯¯å¼ãç¹å»[è¿é](https://github.com/aixcyi/zeraora/
-blob/master/docs/zeraora/ReprMixin.md)æ¥çè§£å³æ¹æ¡ã ### 0.2.5ï¼2023-5-
-02ï¼ - `OnionObject.__repr__()`
-ä¸åè¿è¡åµå¥éå½ï¼å ä¸ºå¨è°è¯æ¨¡å¼ä¸­å¯ä»¥å±å¼åµå¥ï¼å¨æ­¤éå½å¹¶æ æä¹ãç°å¨OnionObjectå¯¹è±¡åçOnionObjectå¯¹è±¡å¨
-`repr()` åä¼æ¾ç¤ºä¸º `OnionObject(...)` ã - å»é¤ `OnionObject.__str__
-()` æ¹æ³ï¼å¯ä»¥ç¨ `import json` å `json.dumps(OnionObject())`
-å®ç°åæ¥çææã - æ´æ¹ `BearTimer` çé»è®¤æå°æ ¼å¼ã - å°
-`BearTimer.output()` æåä¸ºè´è´£åå¤æå°ç `record()`
-åå®ç°æå°ç `handle()` ã ### 0.2.0ï¼2023-4-12ï¼ - å°éå½è½¬åç
-`JSONObject` ä¸ä»è¡¨å±è½¬åç `JsonObject` åå¹¶ä¸º `OnionObject`
-ï¼å¹¶å å»åè¿°ä¸¤ä¸ªç±»ã
```

### Comparing `Zeraora-0.2.7/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.8/Zeraora.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.7
+Version: 0.2.8
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
@@ -17,14 +17,15 @@
             <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
         </div>
         <div align="center">
             <i>长期维护的个人开源工具库</i>
             <br>
             <i>An utility Python package supports for my personal and company projects</i>
         </div>
+        
         ## 特点
         
         - 支持with、注解和实例化三种方式调用的计时器 [`BearTimer`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/BearTimer.md) ；
         - 生成通用representation方便调试时查看对象内部信息的 [`ReprMixin`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md) ；
         - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 [`OnionObject`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/OnionObject.md) ；
         - 安全转换的 `casting()` 和链式调用安全转换的 `Cast` ；
         - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
@@ -60,34 +61,14 @@
         
         ## 兼容性
         
         [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
         
         项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
         
-        ## 更新
-        
-        > 仅列出不兼容旧版的修改，其余变动见git历史。
-        
-        ### 0.2.7（2023-5-09）
-        
-        - 快捷函数 `casting` 更名为 `safecast` ，调用参数一致。
-        - 更改了内部结构，导致使用了 `ReprMixin` 的 Django 模型的迁移文件（migration）中 `CreateModel` 的 `base` 参数传入了错误值。点击[这里](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md)查看解决方案。
-        
-        ### 0.2.5（2023-5-02）
-        
-        - `OnionObject.__repr__()` 不再进行嵌套递归，因为在调试模式中可以展开嵌套，在此递归并无意义。现在OnionObject对象内的OnionObject对象在 `repr()` 后会显示为 `OnionObject(...)` 。
-        - 去除 `OnionObject.__str__()` 方法，可以用 `import json` 后 `json.dumps(OnionObject())` 实现原来的效果。
-        - 更改 `BearTimer` 的默认打印格式。
-        - 将 `BearTimer.output()` 拆分为负责准备打印的 `record()` 和实现打印的 `handle()` 。
-        
-        ### 0.2.0（2023-4-12）
-        
-        - 将递归转化的 `JSONObject` 与仅表层转化的 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
-        
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.2.7 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.2.8 Summary:
 ä¸ä¸ªåå«ååå·¥å·ç±»åå¿«æ·å½æ°çå·¥å·åºãA original utility
 Python package. Home-page: https://github.com/aixcyi/zeraora Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com License: MIT Project-
 URL: Source, https://github.com/aixcyi/zeraora Project-URL: Tracker, https://
 github.com/aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
                 [https://img.shields.io/badge/Python-3.7%20%2B-
@@ -38,31 +38,16 @@
 docstring)ï¼[reStructuredText](https://zh.wikipedia.org/wiki/
 ReStructuredText)æ ¼å¼ï¼ï¼ææ¡£æªå°½äºå®è¯·ç§»æ­¥æºä»£ç æµè§ã ##
 å¼å®¹æ§ [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/
 3.7.html#summary-release-highlights) å¼å§ `dict`
 æ­£å¼æç§æå¥é¡ºåºå­å¨ï¼èèå° `dict` æ¯ Python
 çåºç³ï¼ä¸ºäºé¿ååºç°é¾ä»¥å¯è§çéè¯¯ï¼å èå°è¯¥çæ¬å®ä¸ºå¼å®¹ä¸éãè¿ä¹æ¯ææ¥è§¦è¿çé¡¹ç®ä¸­çæä½è¿è¡çæ¬ï¼æèä¸å¤ªå¸æç»´æ¤å¯¹æ´ä½çæ¬çå¼å®¹ã
 é¡¹ç®ä¼å°½åä¿è¯ååå¼å®¹æ§ï¼ä½è¿æ¯å»ºè®®å¨requirementsä¸­åæç¹å®ççæ¬å·ï¼é¿åå ä¸ºçæ¬æ´æ°æåéèåºç°æ£æçéè¯¯ã
-## æ´æ° > ä»ååºä¸å¼å®¹æ§ççä¿®æ¹ï¼å¶ä½åå¨è§gitåå²ã ###
-0.2.7ï¼2023-5-09ï¼ - å¿«æ·å½æ° `casting` æ´åä¸º `safecast`
-ï¼è°ç¨åæ°ä¸è´ã - æ´æ¹äºåé¨ç»æï¼å¯¼è´ä½¿ç¨äº `ReprMixin`
-ç Django æ¨¡åçè¿ç§»æä»¶ï¼migrationï¼ä¸­ `CreateModel` ç `base`
-åæ°ä¼ å¥äºéè¯¯å¼ãç¹å»[è¿é](https://github.com/aixcyi/zeraora/
-blob/master/docs/zeraora/ReprMixin.md)æ¥çè§£å³æ¹æ¡ã ### 0.2.5ï¼2023-5-
-02ï¼ - `OnionObject.__repr__()`
-ä¸åè¿è¡åµå¥éå½ï¼å ä¸ºå¨è°è¯æ¨¡å¼ä¸­å¯ä»¥å±å¼åµå¥ï¼å¨æ­¤éå½å¹¶æ æä¹ãç°å¨OnionObjectå¯¹è±¡åçOnionObjectå¯¹è±¡å¨
-`repr()` åä¼æ¾ç¤ºä¸º `OnionObject(...)` ã - å»é¤ `OnionObject.__str__
-()` æ¹æ³ï¼å¯ä»¥ç¨ `import json` å `json.dumps(OnionObject())`
-å®ç°åæ¥çææã - æ´æ¹ `BearTimer` çé»è®¤æå°æ ¼å¼ã - å°
-`BearTimer.output()` æåä¸ºè´è´£åå¤æå°ç `record()`
-åå®ç°æå°ç `handle()` ã ### 0.2.0ï¼2023-4-12ï¼ - å°éå½è½¬åç
-`JSONObject` ä¸ä»è¡¨å±è½¬åç `JsonObject` åå¹¶ä¸º `OnionObject`
-ï¼å¹¶å å»åè¿°ä¸¤ä¸ªç±»ã Platform: UNKNOWN Classifier: Development Status
-:: 4 - Beta Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Developers Classifier:
-Operating System :: OS Independent Classifier: Natural Language :: Chinese
-(Simplified) Classifier: License :: OSI Approved :: MIT License Classifier:
-Topic :: Utilities Classifier: Typing :: Typed Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: Chinese (Simplified) Classifier: License :: OSI
+Approved :: MIT License Classifier: Topic :: Utilities Classifier: Typing ::
+Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `Zeraora-0.2.7/setup.py` & `Zeraora-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.7/zeraora/__init__.py` & `Zeraora-0.2.8/zeraora/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,39 +9,42 @@
     datasize as dsz,
     true,
     SafeCaster,
     safecast,
     safecasts,
 )
 from .divisions import (
+    Region,
     Province,
-    REGIONS,
 )
 from .generators import (
     randbytes,
     randb62,
     randb64,
     SnowflakeWorker,
     SnowflakeMultiWorker,
     SnowflakeSingleWorker,
 )
 from .typeclasses import (
     OnionObject,
+    RadixInteger,
     ChoicesMeta,
     Choices,
     IntegerChoices,
     TextChoices,
+    ItemsMeta,
+    Items,
 )
 from .utils import (
     BearTimer,
     ReprMixin,
 )
 
 __author__ = 'aixcyi'
-__version__ = (0, 2, 7)
-version = '0.2.7'
+__version__ = (0, 2, 8)
+version = '0.2.8'
 
 # Django makemigrations 会在 CreateModel 里插入参数
 # bases=(zeraora.utils.ReprMixin, models.Model)
 # 导致对 zeraora 产生依赖，这里改变 ReprMixin 所在包地址，
 # 尽量减少因为改变内部包结构导致对外部的影响。
 ReprMixin.__module__ = 'zeraora'
```

### Comparing `Zeraora-0.2.7/zeraora/charsets.py` & `Zeraora-0.2.8/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.7/zeraora/checkers.py` & `Zeraora-0.2.8/zeraora/checkers.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.7/zeraora/converters.py` & `Zeraora-0.2.8/zeraora/converters.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.7/zeraora/djangobase/mixins.py` & `Zeraora-0.2.8/zeraora/djangobase/mixins.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.7/zeraora/generators.py` & `Zeraora-0.2.8/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.7/zeraora/utils.py` & `Zeraora-0.2.8/zeraora/utils.py`

 * *Files identical despite different names*


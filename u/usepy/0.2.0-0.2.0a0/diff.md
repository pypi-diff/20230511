# Comparing `tmp/usepy-0.2.0.tar.gz` & `tmp/usepy-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy-0.2.0.tar", max compression
+gzip compressed data, was "usepy-0.2.0a0.tar", max compression
```

## Comparing `usepy-0.2.0.tar` & `usepy-0.2.0a0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1656 2023-05-11 01:48:14.370578 usepy-0.2.0/README.md
--rw-r--r--   0        0        0      539 2023-05-11 01:48:14.382578 usepy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/contrib/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/contrib/pydantic_.py
--rw-r--r--   0        0        0     2039 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/contrib/tenacity_.py
--rw-r--r--   0        0        0     1290 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/__init__.py
--rw-r--r--   0        0        0     5214 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useAddict.py
--rw-r--r--   0        0        0     2075 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useBloomFilter.py
--rw-r--r--   0        0        0      467 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useCachedProperty.py
--rw-r--r--   0        0        0      417 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useCatchError.py
--rw-r--r--   0        0        0      883 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useCleanHtml.py
--rw-r--r--   0        0        0     1059 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useCounter.py
--rw-r--r--   0        0        0     6379 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useDateTime.py
--rw-r--r--   0        0        0     8165 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useDict.py
--rw-r--r--   0        0        0     1529 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useImport.py
--rw-r--r--   0        0        0      692 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useIs.py
--rw-r--r--   0        0        0     8934 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useList.py
--rw-r--r--   0        0        0      419 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useListify.py
--rw-r--r--   0        0        0     2909 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/usePath.py
--rw-r--r--   0        0        0      596 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useRandom.py
--rw-r--r--   0        0        0     1814 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useRetry.py
--rw-r--r--   0        0        0      379 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useRunInThread.py
--rw-r--r--   0        0        0      522 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useSingleton.py
--rw-r--r--   0        0        0     3146 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useString.py
--rw-r--r--   0        0        0      552 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useStringDecode.py
--rw-r--r--   0        0        0      534 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useStringEncode.py
--rw-r--r--   0        0        0      229 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useStringReverse.py
--rw-r--r--   0        0        0     1158 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useThread.py
--rw-r--r--   0        0        0      352 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useTimeIt.py
--rw-r--r--   0        0        0      840 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useTimeout.py
--rw-r--r--   0        0        0     4748 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useTimer.py
--rw-r--r--   0        0        0     1971 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/core/useTo.py
--rw-r--r--   0        0        0      226 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/crawl/__init__.py
--rw-r--r--   0        0        0      221 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/crawl/useCookieToDict.py
--rw-r--r--   0        0        0     3405 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/crawl/useCurl.py
--rw-r--r--   0        0        0      239 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/crawl/useDataToDict.py
--rw-r--r--   0        0        0      267 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/crawl/useHeaderToDict.py
--rw-r--r--   0        0        0     1382 2023-05-11 01:48:14.382578 usepy-0.2.0/src/usepy/crawl/useUrl.py
--rw-r--r--   0        0        0   711543 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/crawl/useUserAgent.py
--rw-r--r--   0        0        0        9 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/__init__.py
--rw-r--r--   0        0        0      266 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useLogger/__init__.py
--rw-r--r--   0        0        0     2042 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useLogger/formatters.py
--rw-r--r--   0        0        0     1149 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useLogger/handlers.py
--rw-r--r--   0        0        0     2791 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useLogger/intercept.py
--rw-r--r--   0        0        0     2087 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useLogger/logger.py
--rw-r--r--   0        0        0       84 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/__init__.py
--rw-r--r--   0        0        0      219 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/__init__.py
--rw-r--r--   0        0        0      508 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/bark.py
--rw-r--r--   0        0        0      271 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/base.py
--rw-r--r--   0        0        0      597 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/chanify.py
--rw-r--r--   0        0        0      897 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/ding.py
--rw-r--r--   0        0        0     1027 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/email.py
--rw-r--r--   0        0        0      578 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/pushdeer.py
--rw-r--r--   0        0        0      688 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/pushover.py
--rw-r--r--   0        0        0      675 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/channels/wechat.py
--rw-r--r--   0        0        0      534 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/integrations/useNotify/notification.py
--rw-r--r--   0        0        0       82 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/utils/__init__.py
--rw-r--r--   0        0        0      410 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/utils/useFormatSizeof.py
--rw-r--r--   0        0        0      306 2023-05-11 01:48:14.386578 usepy-0.2.0/src/usepy/utils/useFuncName.py
--rw-r--r--   0        0        0     2119 1970-01-01 00:00:00.000000 usepy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      825 2023-05-03 08:20:39.256238 usepy-0.2.0a0/README.md
+-rw-r--r--   0        0        0      541 2023-05-03 08:20:39.268238 usepy-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/contrib/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/contrib/pydantic_.py
+-rw-r--r--   0        0        0     2039 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/contrib/tenacity_.py
+-rw-r--r--   0        0        0     1173 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/__init__.py
+-rw-r--r--   0        0        0     5214 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useAddict.py
+-rw-r--r--   0        0        0     1945 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useBloomFilter.py
+-rw-r--r--   0        0        0      467 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useCachedProperty.py
+-rw-r--r--   0        0        0      417 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useCatchError.py
+-rw-r--r--   0        0        0      883 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useCleanHtml.py
+-rw-r--r--   0        0        0     1059 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useCounter.py
+-rw-r--r--   0        0        0     6379 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useDateTime.py
+-rw-r--r--   0        0        0     8165 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useDict.py
+-rw-r--r--   0        0        0     1529 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useImport.py
+-rw-r--r--   0        0        0      692 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useIs.py
+-rw-r--r--   0        0        0     7116 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useList.py
+-rw-r--r--   0        0        0      419 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useListify.py
+-rw-r--r--   0        0        0     2909 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/usePath.py
+-rw-r--r--   0        0        0      596 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useRandom.py
+-rw-r--r--   0        0        0     1814 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useRetry.py
+-rw-r--r--   0        0        0      379 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useRunInThread.py
+-rw-r--r--   0        0        0      522 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useSingleton.py
+-rw-r--r--   0        0        0     3146 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useString.py
+-rw-r--r--   0        0        0      552 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useStringDecode.py
+-rw-r--r--   0        0        0      534 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useStringEncode.py
+-rw-r--r--   0        0        0      229 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useStringReverse.py
+-rw-r--r--   0        0        0     1158 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useThread.py
+-rw-r--r--   0        0        0      412 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useTimeIt.py
+-rw-r--r--   0        0        0      840 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useTimeout.py
+-rw-r--r--   0        0        0     4748 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useTimer.py
+-rw-r--r--   0        0        0     1971 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/core/useTo.py
+-rw-r--r--   0        0        0      226 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/crawl/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/crawl/useCookieToDict.py
+-rw-r--r--   0        0        0     3405 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/crawl/useCurl.py
+-rw-r--r--   0        0        0      239 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/crawl/useDataToDict.py
+-rw-r--r--   0        0        0      267 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/crawl/useHeaderToDict.py
+-rw-r--r--   0        0        0     1382 2023-05-03 08:20:39.268238 usepy-0.2.0a0/src/usepy/crawl/useUrl.py
+-rw-r--r--   0        0        0   711543 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/crawl/useUserAgent.py
+-rw-r--r--   0        0        0        9 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useLogger/__init__.py
+-rw-r--r--   0        0        0     2042 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useLogger/formatters.py
+-rw-r--r--   0        0        0     1149 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useLogger/handlers.py
+-rw-r--r--   0        0        0     2791 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useLogger/intercept.py
+-rw-r--r--   0        0        0     2087 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useLogger/logger.py
+-rw-r--r--   0        0        0       84 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/__init__.py
+-rw-r--r--   0        0        0      508 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/bark.py
+-rw-r--r--   0        0        0      271 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/base.py
+-rw-r--r--   0        0        0      597 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/chanify.py
+-rw-r--r--   0        0        0      897 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/ding.py
+-rw-r--r--   0        0        0     1027 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/email.py
+-rw-r--r--   0        0        0      578 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/pushdeer.py
+-rw-r--r--   0        0        0      688 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/pushover.py
+-rw-r--r--   0        0        0      675 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/wechat.py
+-rw-r--r--   0        0        0      534 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/integrations/useNotify/notification.py
+-rw-r--r--   0        0        0       82 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/utils/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/utils/useFormatSizeof.py
+-rw-r--r--   0        0        0      306 2023-05-03 08:20:39.272238 usepy-0.2.0a0/src/usepy/utils/useFuncName.py
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 usepy-0.2.0a0/PKG-INFO
```

### Comparing `usepy-0.2.0/pyproject.toml` & `usepy-0.2.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usepy"
-version = "0.2.0"
+version = "0.2.0a0"
 description = "usepy"
 homepage = "https://usepy.code05.com/"
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'usepy', from = 'src' }
 ]
```

### Comparing `usepy-0.2.0/src/usepy/contrib/pydantic_.py` & `usepy-0.2.0a0/src/usepy/contrib/pydantic_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/contrib/tenacity_.py` & `usepy-0.2.0a0/src/usepy/contrib/tenacity_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/__init__.py` & `usepy-0.2.0a0/src/usepy/core/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 from .useStringEncode import useStringEncode
 
 from .useAddict import useAdDict
 
 from .useCounter import useCounter
 
 from .useDict import useDict
-from .useList import (
-    useList,
-    useListFilter, useListFlatten, useListDifference, useListEvery, useListSome, useListSort, useListUnique
-)
+from .useList import useList
 
 from .useCatchError import useCatchError
 from .useListify import useListify
 from .useCachedProperty import useCachedProperty
 from .useRetry import useRetry
 from .useBloomFilter import useBloomFilter
 from .useRunInThread import useRunInThread
```

### Comparing `usepy-0.2.0/src/usepy/core/useAddict.py` & `usepy-0.2.0a0/src/usepy/core/useAddict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useBloomFilter.py` & `usepy-0.2.0a0/src/usepy/core/useBloomFilter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
 reference
 - https://github.com/LiuXingMing/Scrapy_Redis_Bloomfilter/blob/master/bloomfilterOnRedis.py
 - https://github.com/MuggleK/CrawlersTools/blob/main/CrawlersTools/preprocess/bloom_filter.py
 """
-from typing import Tuple
-
 from .useTo import useToSHA1
 
 
 class SimpleHash(object):
 
     def __init__(self, cap, seed):
         self.cap = cap
@@ -49,22 +47,18 @@
         input_value = useToSHA1(input_value)
         name = f"{self.key}{int(input_value[0:2], 16) % self.block_num}"
         for f in self.hash_func:
             loc = f.hash(input_value)
             ret = ret & self.client.getbit(name, loc)
         return bool(ret)
 
-    def _add(self, input_value: str):
-        input_value = useToSHA1(input_value)
-        name = f"{self.key}{str(int(input_value[0:2], 16) % self.block_num)}"
-        for f in self.hash_func:
-            loc = f.hash(input_value)
-            self.client.setbit(name, loc, 1)
-
-    def add(self, *input_value: Tuple[str]) -> None:
+    def add(self, input_value: str) -> None:
         """
         插入字符串
         :param input_value: 输入值
         :return:
         """
-        for iv in input_value:
-            self._add(iv)
+        input_value = useToSHA1(input_value)
+        name = f"{self.key}{str(int(input_value[0:2], 16) % self.block_num)}"
+        for f in self.hash_func:
+            loc = f.hash(input_value)
+            self.client.setbit(name, loc, 1)
```

### Comparing `usepy-0.2.0/src/usepy/core/useCleanHtml.py` & `usepy-0.2.0a0/src/usepy/core/useCleanHtml.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useCounter.py` & `usepy-0.2.0a0/src/usepy/core/useCounter.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useDateTime.py` & `usepy-0.2.0a0/src/usepy/core/useDateTime.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useDict.py` & `usepy-0.2.0a0/src/usepy/core/useDict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useImport.py` & `usepy-0.2.0a0/src/usepy/core/useImport.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useIs.py` & `usepy-0.2.0a0/src/usepy/core/useIs.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useList.py` & `usepy-0.2.0a0/src/usepy/core/useList.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from typing import List, Generator, Dict, Optional, Callable, Literal, Any, Tuple, Union
-from functools import reduce
-from operator import and_, or_
 
 SortType = Optional[
     Literal["quick", "bubble", "select"]
 ]
 
 ListType = Union[List, Tuple]
 
@@ -216,84 +214,7 @@
         >>> useList.difference([{'a': 1, 'b': 2}, {'a': 2, 'b': 3}], [{'a': 1, 'b': 2}])
         [{'a': 2, 'b': 3}]
         >>> useList.difference([1, 2, 3], [1, 4], fn=lambda x: x ** 2)
         [3]
         """
         fn = fn or (lambda x: x)
         return [item for item in original_list if fn(item) not in exclude_list]
-
-
-def useListFilter(array: List, fn: Callable):
-    """
-    数组过滤
-    :param array: 数组
-    :param fn: 函数
-    :return:
-    """
-    return list(filter(fn, array))
-
-
-def useListFlatten(array: List):
-    """
-    数组扁平化
-    :param array: 数组
-    :return:
-    """
-    return useList.flatten(array)
-
-
-def useListDifference(original_array: List, exclude_array: List, fn: Optional[Callable] = None):
-    """
-    求差集
-    :param original_array: 原数组
-    :param exclude_array: 排除数组
-    :param fn: 函数
-    :return: 差集
-
-    >>> useListDifference([1, 2, 3], [1, 4])
-    [2, 3]
-    >>> useListDifference([{'a': 1, 'b': 2}, {'a': 2, 'b': 3}], [{'a': 1, 'b': 2}])
-    [{'a': 2, 'b': 3}]
-    >>> useListDifference([1, 2, 3], [1, 4], fn=lambda x: x ** 2)
-    [3]
-    """
-    return useList.difference(original_array, exclude_array, fn)
-
-
-def useListEvery(array: List, fn: Callable):
-    """
-    数组每一项都满足条件
-    :param array: 数组
-    :param fn: 函数
-    :return:
-    """
-    return reduce(and_, [fn(element) for element in array])
-
-
-def useListSome(array: List, fn: Callable):
-    """
-    数组有一项满足条件
-    :param array: 数组
-    :param fn: 函数
-    :return:
-    """
-    return reduce(or_, [fn(element) for element in array])
-
-
-def useListSort(array: List, algorithm: SortType = 'bubble'):
-    """
-    数组排序
-    :param array: 数组
-    :param algorithm: 排序算法, 默认冒泡排序
-    :return: 排序后数组
-    """
-    return useList.sort(array, algorithm)
-
-
-def useListUnique(array: List, fn: Optional[Callable] = None):
-    """
-    数组去重
-    :param fn:
-    :param array: 数组
-    :return: 去重后数组
-    """
-    return list(useList.dedupe(array, fn))
```

### Comparing `usepy-0.2.0/src/usepy/core/usePath.py` & `usepy-0.2.0a0/src/usepy/core/usePath.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useRandom.py` & `usepy-0.2.0a0/src/usepy/core/useRandom.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useRetry.py` & `usepy-0.2.0a0/src/usepy/core/useRetry.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useSingleton.py` & `usepy-0.2.0a0/src/usepy/core/useSingleton.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useString.py` & `usepy-0.2.0a0/src/usepy/core/useString.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useStringDecode.py` & `usepy-0.2.0a0/src/usepy/core/useStringDecode.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useStringEncode.py` & `usepy-0.2.0a0/src/usepy/core/useStringEncode.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useThread.py` & `usepy-0.2.0a0/src/usepy/core/useThread.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useTimeout.py` & `usepy-0.2.0a0/src/usepy/core/useTimeout.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useTimer.py` & `usepy-0.2.0a0/src/usepy/core/useTimer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/core/useTo.py` & `usepy-0.2.0a0/src/usepy/core/useTo.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/crawl/useCurl.py` & `usepy-0.2.0a0/src/usepy/crawl/useCurl.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/crawl/useUrl.py` & `usepy-0.2.0a0/src/usepy/crawl/useUrl.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/crawl/useUserAgent.py` & `usepy-0.2.0a0/src/usepy/crawl/useUserAgent.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useLogger/formatters.py` & `usepy-0.2.0a0/src/usepy/integrations/useLogger/formatters.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useLogger/handlers.py` & `usepy-0.2.0a0/src/usepy/integrations/useLogger/handlers.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useLogger/intercept.py` & `usepy-0.2.0a0/src/usepy/integrations/useLogger/intercept.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useLogger/logger.py` & `usepy-0.2.0a0/src/usepy/integrations/useLogger/logger.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useNotify/channels/chanify.py` & `usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/chanify.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useNotify/channels/ding.py` & `usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/ding.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useNotify/channels/email.py` & `usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/email.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useNotify/channels/pushdeer.py` & `usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/pushdeer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useNotify/channels/pushover.py` & `usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/pushover.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useNotify/channels/wechat.py` & `usepy-0.2.0a0/src/usepy/integrations/useNotify/channels/wechat.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.0/src/usepy/integrations/useNotify/notification.py` & `usepy-0.2.0a0/src/usepy/integrations/useNotify/notification.py`

 * *Files identical despite different names*


# Comparing `tmp/eyes_soatra-0.0.19.tar.gz` & `tmp/eyes_soatra-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.19.tar", last modified: Tue May  2 07:38:02 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.20.tar", last modified: Thu May 11 09:50:35 2023, max compression
```

## Comparing `eyes_soatra-0.0.19.tar` & `eyes_soatra-0.0.20.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 07:38:02.139417 eyes_soatra-0.0.19/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.19/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      552 2023-05-02 07:38:02.139200 eyes_soatra-0.0.19/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       47 2023-05-02 03:38:24.000000 eyes_soatra-0.0.19/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 07:38:02.137628 eyes_soatra-0.0.19/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.19/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 07:38:02.138879 eyes_soatra-0.0.19/eyes_soatra/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-02 07:07:54.000000 eyes_soatra-0.0.19/eyes_soatra/depends/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     7664 2023-05-02 03:37:05.000000 eyes_soatra-0.0.19/eyes_soatra/depends/depends_404.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.19/eyes_soatra/depends/depends_no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)    11092 2023-05-02 07:05:45.000000 eyes_soatra-0.0.19/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 07:38:02.138395 eyes_soatra-0.0.19/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      552 2023-05-02 07:38:02.000000 eyes_soatra-0.0.19/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      350 2023-05-02 07:38:02.000000 eyes_soatra-0.0.19/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 07:38:02.000000 eyes_soatra-0.0.19/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-02 07:38:02.000000 eyes_soatra-0.0.19/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-02 07:38:02.000000 eyes_soatra-0.0.19/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-02 07:38:02.139469 eyes_soatra-0.0.19/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-02 07:38:01.000000 eyes_soatra-0.0.19/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.232869 eyes_soatra-0.0.20/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.20/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-11 09:50:35.232741 eyes_soatra-0.0.20/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.20/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.228375 eyes_soatra-0.0.20/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.20/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.229434 eyes_soatra-0.0.20/eyes_soatra/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-02 07:07:54.000000 eyes_soatra-0.0.20/eyes_soatra/depends/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.20/eyes_soatra/depends/depends_404.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.20/eyes_soatra/depends/depends_no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)    12902 2023-05-11 09:41:42.000000 eyes_soatra-0.0.20/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.229786 eyes_soatra-0.0.20/eyes_soatra/needs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-11 07:51:47.000000 eyes_soatra-0.0.20/eyes_soatra/needs/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.20/eyes_soatra/needs/user_agends.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.228970 eyes_soatra-0.0.20/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      440 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-11 09:50:35.232912 eyes_soatra-0.0.20/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-10 03:53:31.000000 eyes_soatra-0.0.20/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.232351 eyes_soatra-0.0.20/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2464 2023-05-11 09:35:34.000000 eyes_soatra-0.0.20/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1495 2023-05-11 09:30:34.000000 eyes_soatra-0.0.20/test/test2.py
```

### Comparing `eyes_soatra-0.0.19/PKG-INFO` & `eyes_soatra-0.0.20/eyes_soatra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: eyes_soatra
-Version: 0.0.19
+Name: eyes-soatra
+Version: 0.0.20
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-You can use this package to achieve to purpose.
+You can use this package to achieve your purpose.
```

### Comparing `eyes_soatra-0.0.19/eyes_soatra/depends/depends_404.py` & `eyes_soatra-0.0.20/eyes_soatra/depends/depends_404.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "The page you were looking for doesn't exist.",
     "Web ページが見つかりません。",
     "【404 NOT FOUND】 ご指定のページは見つかりませんでした",
     "【NOT FOUND】 ご指定のページは見つかりませんでした。",
     "お手数ですが、再度キーワードを入力してください",
     "お探しのコンテンツはみつかりませんでした。",
     "お探しのページ、またはファイルは見つかりませんでした。",
-    "お探しのページが",
+    # "お探しのページが", the page you looking for
     "お探しのページが見つかりません",
     "お探しのページが見つかりません / NotFound",
     "お探しのページが見つかりません。",
     "お探しのページが見つかりませんでした",
     "お探しのページが見つかりませんでした。",
     "お探しのページが見つかりませんでした！",
     "お探しのページが見つかりません（サイト内検索をご利用ください）",
```

### Comparing `eyes_soatra-0.0.19/eyes_soatra/eyes.py` & `eyes_soatra-0.0.20/eyes_soatra/eyes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!python3
-from eyes_soatra.depends.depends_404 import depends as __depends_no_data
-from eyes_soatra.depends.depends_no_data import depends as __depends_404
+from eyes_soatra.depends.depends_404 import depends as __depends_404
+from eyes_soatra.depends.depends_no_data import depends as __depends_no_data
+from eyes_soatra.needs.user_agents import User_Agents as __User_Agents
 from translate import Translator as __Translator
 from requests_html import HTML as __HTML
 import requests as __requests
 import jellyfish as __jellyfish
 import re as __re
+import time as __time
+import random
 
 # Suppress only the single warning from urllib3 needed.
 __requests.packages.urllib3.disable_warnings()
 __requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 try:
     __requests.packages.urllib3.contrib.pyopenssl.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 except AttributeError:
     # no pyopenssl support used / needed / available
     pass
 
 # private global variables
-
-__headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/50.0.2661.102 Safari/537.36'}
 __separator = '\||-|:'
 __header_min_length = 3
 __paragraph_min_length = 7
 __container = 'self::div or self::span or self::table'
 __header_xpaths = [
     '//title',
     '//h1[self::*//text() and last()=1]',
@@ -31,23 +32,18 @@
 __paragraph_xpaths = [
     '//p[@class="no_data"]',
     '//h1[self::*//text()]/following-sibling::p[1]',
     '//h1[self::*//text()]/following-sibling::*//p[1]',
     f'//*[({__container}) and self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1][{__container}]//p[1]'
 ]
 __content_xpaths = [
-    '''
-        //h1[self::*//text()]/following-sibling::*|
-        //h1[self::*//text()]/following-sibling::*//*|
-        //*[self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1]//*
-    '''
+    '//h1[self::*//text()]/following-sibling::*|//h1[self::*//text()]/following-sibling::*//*|//*[self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1]//*'
 ]
-# //h1[self::*//text()]/following-sibling::p[1]|//h1[self::*//text()]/following-sibling::*//p[1]|//*[({self::div or self::span}) and self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1][{self::div or self::span}]//p[1]
-# ---------------------- helpers
 
+# private functions
 def __sort_dict(dict):
     keys = list(dict.keys())
     keys.sort()
     new_dict = {}
     
     for key in keys:
         new_dict[key] = dict[key]
@@ -81,44 +77,45 @@
 ):
     header_texts = []
     paragraph_texts = []
     content_texts = []
     
     for xpath in __header_xpaths + (header_xpath if type(header_xpath) == list else []):
         header_list = html.xpath(f'({xpath})//text()')
+        header = ' '.join(header_list)
+        header = __strip(header)
         
-        for header in header_list:
-            header = __strip(header)
-            
-            if len(header) >= __header_min_length:
-                header_texts.append(header)
+        if len(header) >= __header_min_length:
+            header_texts.append(header)
+        # for header in header_list:
     
     for xpath in __paragraph_xpaths + (paragraph_xpath if type(paragraph_xpath) == list else []):
         paragraph_list = html.xpath(f'({xpath})//text()')
+        paragraph = ' '.join(paragraph_list)
+        paragraph = __strip(paragraph)
         
-        for paragraph in paragraph_list:
-            paragraph = __strip(paragraph)
-            
-            if len(paragraph) >= __paragraph_min_length:
-                paragraph_texts.append(paragraph)
+        if len(paragraph) >= __paragraph_min_length:
+            paragraph_texts.append(paragraph)
 
         if len(paragraph_texts):
             break
+        # for paragraph in paragraph_list:
     
     for xpath in __content_xpaths + (content_xpath if type(content_xpath) == list else []):
         content_list = html.xpath(f'({xpath})//text()')
+        content = ' '.join(content_list)
+        content = __strip(content)
         
-        for content in content_list:
-            content = __strip(content)
-            
-            if len(content) > 0:
-                content_texts.append(content)
+        if len(content) > 0:
+            content_texts.append(content)
 
         if len(content_texts):
             break
+        # for content in content_list:
+            
 
     return {
         'headers': header_texts,
         'paragraphs': paragraph_texts,
         'contents': content_texts,
     }
 
@@ -158,17 +155,18 @@
         for depend in __depends_404 + (depends if type(depends) == list else []):
             for header in headers:                
                 for token_header in __re.split(__separator + (separator if separator else ''), header):
                     token_header = __strip(token_header)
                     
                     if len(token_header) >= __header_min_length:
                         s1 = __jellyfish.jaro_similarity(depend, token_header)
-                        s2 = __jellyfish.jaro_winkler_similarity(depend, token_header)
+                        # s2 = __jellyfish.jaro_winkler_similarity(depend, token_header)
                         
-                        points = (s1 + s2) / 2
+                        # points = (s1 + s2) / 2
+                        points = s1
                         
                         if points > header_high_point:
                             header_high_point = points
                             header_similar = depend
                             header_keyword = token_header
                             
                         if points >= header_min_point:
@@ -201,17 +199,18 @@
         for depend in __depends_no_data + (depends if type(depends) == list else []):
             for paragraph in paragraphs:
                 for token_paragraph in __re.split(__separator + (separator if separator else ''), paragraph):
                     token_paragraph = __strip(token_paragraph)
                     
                     if len(token_paragraph) >= __paragraph_min_length:
                         s1 = __jellyfish.jaro_similarity(depend, token_paragraph)
-                        s2 = __jellyfish.jaro_winkler_similarity(depend, token_paragraph)
+                        # s2 = __jellyfish.jaro_winkler_similarity(depend, token_paragraph)
                         
-                        points = (s1 + s2) / 2
+                        # points = (s1 + s2) / 2
+                        points = s1
                         
                         if points > paragraph_high_point:
                             paragraph_high_point = points
                             paragraph_similar = depend
                             paragraph_keyword = token_paragraph
                             
                         if points >= paragraph_min_point:
@@ -242,108 +241,148 @@
             'blank': True,
             'content': contents
         }
         
     return result
 
 # ------------------------ public function
-
 def view_page(
     url,
     lang='ja',
-    timeout=10,
+    sleep=2,
+    timeout=20,
     verify=False,
+    headers=None,
     depends=None,
     separator=None,
+    tries_reject=50,
+    tries_timeout=3,
     header_xpath=None,
     paragraph_xpath=None,
     content_xpath=None,
     allow_redirects=True,
     header_min_point=0.8,
     paragraph_min_point=0.85,
     
     show_highlight = False,
     show_header = False,
     show_paragraph = False,
     show_content = False,
     
     **requests_options
 ):
-    try:
-        response = __requests.get(
-            url,
-            timeout=timeout,
-            allow_redirects=allow_redirects,
-            verify=verify,
-            headers=__headers,
-            **requests_options
-        )
-        status_code = response.status_code
-        redirected = response.is_redirect
-        expired = response.headers.get('Expires')
-        expired = expired if expired else (response.headers.get('expires') or False)
-        expired_obj = {'expired': expired} if expired else {}
-        
-        if status_code >= 400 and status_code <= 499:
-            return __sort_dict({
-                'active': False,
-                'checked': False,
-                **expired_obj,
-                'error': f'Client error responses',
-                'redirected': redirected,
-                'url': response.url,
-                'status': status_code
-            })
+    tried = 0
+    agents = []
+    
+    while True:
+        try:
+            tried += 1
+            user_agent = random.choice(__User_Agents)
+            
+            while user_agent in agents:
+                user_agent = random.choice(__User_Agents)
+                
+            agents.append(user_agent)
+                
+            response = __requests.get(
+                **requests_options,
+                url=url,
+                timeout=timeout,
+                allow_redirects=allow_redirects,
+                verify=verify,
+                headers={
+                    **(headers if headers else {}),
+                    'USER-AGENT': user_agent,
+                    'ACCEPT' : 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
+                    'ACCEPT-ENCODING' : 'gzip, deflate, br',
+                    'ACCEPT-LANGUAGE' : 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,km-KH;q=0.6,km;q=0.5,ja-JP;q=0.4,ja;q=0.3',
+                    'REFERER' : 'https://www.google.com/'
+                },
+            )
+            status_code = response.status_code
+            redirected = response.is_redirect
+            expired = response.headers.get('Expires')
+            expired = expired if expired else (response.headers.get('expires') or False)
+            expired_obj = {'expired': expired} if expired else {}
+            
+            if status_code >= 400 and status_code <= 499:
+                return __sort_dict({
+                    'active': False,
+                    'checked': False,
+                    **expired_obj,
+                    'error': f'Client error responses: {status_code}',
+                    'redirected': redirected,
+                    'url': response.url,
+                    'status': status_code,
+                    'tried': tried,
+                })
+                
+            if status_code >= 500 and status_code <= 599:
+                return __sort_dict({
+                    'active': False,
+                    'checked': False,
+                    **expired_obj,
+                    'error': f'Server error responses: {status_code}',
+                    'redirected': redirected,
+                    'url': response.url,
+                    'status': status_code,
+                    'tried': tried,
+                })
+    
+            html = response.content
+            highlight = __get_highlight(
+                html,
+                header_xpath,
+                paragraph_xpath,
+                content_xpath,
+            )
+            
+            if not (lang == 'ja' or lang == 'en'):
+                translate = __Translator(from_lang=lang, to_lang='en')
+                
+                for key in highlight:
+                    for i in range(0, len(highlight[key])):
+                        highlight[key][i] = translate.translate(highlight[key][i])
             
-        if status_code >= 500 and status_code <= 599:
             return __sort_dict({
-                'active': False,
-                'checked': False,
+                **__bad_page(
+                    highlight,
+                    separator,
+                    depends,
+                    header_min_point,
+                    paragraph_min_point,
+                    
+                    show_highlight,
+                    show_header,
+                    show_paragraph,
+                    show_content,
+                ),
                 **expired_obj,
-                'error': f'Server error responses',
                 'redirected': redirected,
                 'url': response.url,
-                'status': status_code
+                'status': status_code,
+                'tried': tried,
             })
- 
-        html = response.content
-        highlight = __get_highlight(
-            html,
-            header_xpath,
-            paragraph_xpath,
-            content_xpath,
-        )
-        
-        if not (lang == 'ja' or lang == 'en'):
-            translate = __Translator(from_lang=lang, to_lang='en')
-            
-            for key in highlight:
-                for i in range(0, len(highlight[key])):
-                    highlight[key][i] = translate.translate(highlight[key][i])
-        
-        return __sort_dict({
-            **__bad_page(
-                highlight,
-                separator,
-                depends,
-                header_min_point,
-                paragraph_min_point,
+
+        except Exception as error:                    
+            if type(error) == __requests.exceptions.ConnectionError:
+                if tried >= tries_reject:
+                    return __sort_dict({
+                        'active': None,
+                        'checked': False,
+                        'error': error,
+                        'redirected': False,
+                        'url': url,
+                        'tried': tried
+                    })
+                __time.sleep(sleep)
                 
-                show_highlight,
-                show_header,
-                show_paragraph,
-                show_content,
-            ),
-            **expired_obj,
-            'redirected': redirected,
-            'url': response.url,
-            'status': status_code
-        })
-
-    except Exception as error:
-        return __sort_dict({
-            'active': False,
-            'checked': False,
-            'error': error,
-            'redirected': False,
-            'url': url,
-        })
+            else :
+                if tried >= tries_timeout:
+                    return __sort_dict({
+                        'active': None,
+                        'checked': False,
+                        'error': error,
+                        'redirected': False,
+                        'url': url,
+                        'tried': tried
+                    })
```

### Comparing `eyes_soatra-0.0.19/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.20/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: eyes-soatra
-Version: 0.0.19
+Name: eyes_soatra
+Version: 0.0.20
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-You can use this package to achieve to purpose.
+You can use this package to achieve your purpose.
```

### Comparing `eyes_soatra-0.0.19/setup.py` & `eyes_soatra-0.0.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.19'
+VERSION = '0.0.20'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```


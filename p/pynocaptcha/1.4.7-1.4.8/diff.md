# Comparing `tmp/pynocaptcha-1.4.7.tar.gz` & `tmp/pynocaptcha-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.4.7.tar", last modified: Tue May  9 07:34:03 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.4.8.tar", last modified: Thu May 11 08:44:56 2023, max compression
```

## Comparing `pynocaptcha-1.4.7.tar` & `pynocaptcha-1.4.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-09 07:34:03.000000 pynocaptcha-1.4.7/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-09 07:34:03.000000 pynocaptcha-1.4.7/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-09 07:34:03.000000 pynocaptcha-1.4.7/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.7/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-09 07:34:03.000000 pynocaptcha-1.4.7/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.4.7/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4539 2023-05-09 07:33:22.000000 pynocaptcha-1.4.7/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.7/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.7/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.7/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.7/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-09 07:33:53.000000 pynocaptcha-1.4.7/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-11 08:44:56.000000 pynocaptcha-1.4.8/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-11 08:44:56.000000 pynocaptcha-1.4.8/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-11 08:44:56.000000 pynocaptcha-1.4.8/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.8/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-11 08:44:56.000000 pynocaptcha-1.4.8/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.4.8/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4573 2023-05-11 08:44:17.000000 pynocaptcha-1.4.8/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.8/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.8/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.8/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.8/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-11 08:30:56.000000 pynocaptcha-1.4.8/setup.py
```

### Comparing `pynocaptcha-1.4.7/PKG-INFO` & `pynocaptcha-1.4.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.4.7
+Version: 1.4.8
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.4.7/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.4.8/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.7/pynocaptcha/crackers/base.py` & `pynocaptcha-1.4.8/pynocaptcha/crackers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,27 +98,28 @@
         
         if self.user_agent:
             self.wanda_args["user_agent"] = self.user_agent
         if self.proxy:
             self.wanda_args["proxy"] = self.proxy
 
         retry_times = 0        
+        resp = {}
         while retry_times < self.max_retry_times:
             try:
                 resp = requests.post(
                     f"http://{'xn--fjqs46frol.com' if self.internal_api else 'api.nocaptcha.io' }/api/wanda/{self.cracker_name}/{self.cracker_version}", 
                     headers=headers, json=self.wanda_args, timeout=self.timeout
                 ).json()
+                if self.debug:
+                    logger.info(resp)
                 break
             except Exception as e:
                 if self.debug:
                     logger.error(e)
                 retry_times += 1
-        if self.debug:
-            logger.info(resp)
         wanda_ret = resp.get("data")
         if not wanda_ret:
             if self.debug:
                 logger.error(resp.get("msg"))
             return
         ret = self.response(wanda_ret)
         if self.check_useful:
```

### Comparing `pynocaptcha-1.4.7/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.4.8/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.7/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.4.8/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.7/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.4.8/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.7/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.4.8/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.7/setup.py` & `pynocaptcha-1.4.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.4.7',
+    version='1.4.8',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```


# Comparing `tmp/platform-library-0.0.5.tar.gz` & `tmp/platform-library-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-library-0.0.5.tar", last modified: Mon Mar  6 08:11:54 2023, max compression
+gzip compressed data, was "platform-library-0.0.6.tar", last modified: Thu May 11 06:40:19 2023, max compression
```

## Comparing `platform-library-0.0.5.tar` & `platform-library-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-03-06 08:11:54.321204 platform-library-0.0.5/
--rw-r--r--   0 Artyom     (501) staff       (20)     1078 2022-11-08 13:08:16.000000 platform-library-0.0.5/LICENSE
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-03-06 08:11:54.321092 platform-library-0.0.5/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.0.5/README-public.md
--rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.0.5/README.md
--rw-r--r--   0 Artyom     (501) staff       (20)      552 2023-03-06 08:11:49.000000 platform-library-0.0.5/pyproject.toml
--rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-03-06 08:11:54.321237 platform-library-0.0.5/setup.cfg
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-03-06 08:11:54.319089 platform-library-0.0.5/src/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-03-06 08:11:54.320184 platform-library-0.0.5/src/platform_library.egg-info/
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-03-06 08:11:54.000000 platform-library-0.0.5/src/platform_library.egg-info/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)      454 2023-03-06 08:11:54.000000 platform-library-0.0.5/src/platform_library.egg-info/SOURCES.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-03-06 08:11:54.000000 platform-library-0.0.5/src/platform_library.egg-info/dependency_links.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       15 2023-03-06 08:11:54.000000 platform-library-0.0.5/src/platform_library.egg-info/requires.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-03-06 08:11:54.000000 platform-library-0.0.5/src/platform_library.egg-info/top_level.txt
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-03-06 08:11:54.319202 platform-library-0.0.5/src/plib/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-03-06 08:11:54.320624 platform-library-0.0.5/src/plib/auth/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.0.5/src/plib/auth/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.0.5/src/plib/auth/encrypt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.0.5/src/plib/auth/jwt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.0.5/src/plib/auth/o2auth.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-03-06 08:11:54.320956 platform-library-0.0.5/src/plib/licensing/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.0.5/src/plib/licensing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     4027 2023-03-06 07:29:21.000000 platform-library-0.0.5/src/plib/licensing/api.py
--rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.0.5/src/plib/licensing/exceptions.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.675411 platform-library-0.0.6/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1078 2022-11-08 13:08:16.000000 platform-library-0.0.6/LICENSE
+-rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-11 06:40:19.675289 platform-library-0.0.6/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.0.6/README-public.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.0.6/README.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      552 2023-05-11 06:38:46.000000 platform-library-0.0.6/pyproject.toml
+-rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-05-11 06:40:19.675449 platform-library-0.0.6/setup.cfg
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.673208 platform-library-0.0.6/src/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.674349 platform-library-0.0.6/src/platform_library.egg-info/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)      454 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/SOURCES.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/dependency_links.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)       15 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/requires.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/top_level.txt
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.673323 platform-library-0.0.6/src/plib/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.674767 platform-library-0.0.6/src/plib/auth/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/encrypt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/jwt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/o2auth.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.675145 platform-library-0.0.6/src/plib/licensing/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.0.6/src/plib/licensing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     4037 2023-05-11 06:38:08.000000 platform-library-0.0.6/src/plib/licensing/api.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.0.6/src/plib/licensing/exceptions.py
```

### Comparing `platform-library-0.0.5/LICENSE` & `platform-library-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.5/PKG-INFO` & `platform-library-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
         Copyright (c) 2022 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.0.5/README.md` & `platform-library-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.5/pyproject.toml` & `platform-library-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "platform-library"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Artyom Vakilov", email="a.vakilov@3divi.com" },
 ]
 
 description = "A library for easy developing 3DiVi Platform"
 readme = "README-public.md"
 license = { file="LICENSE" }
```

### Comparing `platform-library-0.0.5/src/platform_library.egg-info/PKG-INFO` & `platform-library-0.0.6/src/platform_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
         Copyright (c) 2022 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.0.5/src/plib/auth/encrypt.py` & `platform-library-0.0.6/src/plib/auth/encrypt.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.5/src/plib/auth/o2auth.py` & `platform-library-0.0.6/src/plib/auth/o2auth.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.5/src/plib/licensing/api.py` & `platform-library-0.0.6/src/plib/licensing/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 import requests
 
-from plib.encrypt import Encryptor
-from plib.jwt import encode_payload
+from plib.auth.encrypt import Encryptor
+from plib.auth.jwt import encode_payload
 
 from .exceptions import LicenseLimitAttribute, LicenseServiceError, LicenseSignatureCorrupted
 
 
 class License:
     def __init__(self,
                  url: str,
```

### Comparing `platform-library-0.0.5/src/plib/licensing/exceptions.py` & `platform-library-0.0.6/src/plib/licensing/exceptions.py`

 * *Files identical despite different names*


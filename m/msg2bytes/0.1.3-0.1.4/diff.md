# Comparing `tmp/msg2bytes-0.1.3.tar.gz` & `tmp/msg2bytes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msg2bytes-0.1.3.tar", last modified: Fri Apr 28 11:50:55 2023, max compression
+gzip compressed data, was "msg2bytes-0.1.4.tar", last modified: Thu May 11 14:39:11 2023, max compression
```

## Comparing `msg2bytes-0.1.3.tar` & `msg2bytes-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-28 11:50:55.678440 msg2bytes-0.1.3/
--rw-r--r--   0 test       (501) staff       (20)     1067 2023-04-26 05:03:42.000000 msg2bytes-0.1.3/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      167 2023-04-26 05:03:46.000000 msg2bytes-0.1.3/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     2984 2023-04-28 11:50:55.678324 msg2bytes-0.1.3/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2286 2023-04-28 11:46:21.000000 msg2bytes-0.1.3/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-28 11:50:55.677471 msg2bytes-0.1.3/msg2bytes/
--rw-r--r--   0 test       (501) staff       (20)       20 2023-04-26 04:58:02.000000 msg2bytes-0.1.3/msg2bytes/__init__.py
--rw-r--r--   0 test       (501) staff       (20)    35495 2023-04-28 04:25:50.000000 msg2bytes-0.1.3/msg2bytes/core.py
--rw-r--r--   0 test       (501) staff       (20)     7756 2023-04-28 04:25:07.000000 msg2bytes-0.1.3/msg2bytes/tests.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-28 11:50:55.678144 msg2bytes-0.1.3/msg2bytes.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     2984 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      310 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       16 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       10 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       15 2023-04-26 05:04:22.000000 msg2bytes-0.1.3/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-04-28 11:50:55.678473 msg2bytes-0.1.3/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1395 2023-04-28 04:26:27.000000 msg2bytes-0.1.3/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-11 14:39:11.373468 msg2bytes-0.1.4/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2023-04-26 05:03:42.000000 msg2bytes-0.1.4/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      167 2023-04-26 05:03:46.000000 msg2bytes-0.1.4/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3099 2023-05-11 14:39:11.373350 msg2bytes-0.1.4/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2401 2023-05-11 13:44:55.000000 msg2bytes-0.1.4/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-11 14:39:11.372497 msg2bytes-0.1.4/msg2bytes/
+-rw-r--r--   0 test       (501) staff       (20)       20 2023-04-26 04:58:02.000000 msg2bytes-0.1.4/msg2bytes/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)    35513 2023-05-11 13:39:16.000000 msg2bytes-0.1.4/msg2bytes/core.py
+-rw-r--r--   0 test       (501) staff       (20)     7756 2023-04-28 04:25:07.000000 msg2bytes-0.1.4/msg2bytes/tests.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-11 14:39:11.373201 msg2bytes-0.1.4/msg2bytes.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3099 2023-05-11 14:39:11.000000 msg2bytes-0.1.4/msg2bytes.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      310 2023-05-11 14:39:11.000000 msg2bytes-0.1.4/msg2bytes.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-05-11 14:39:11.000000 msg2bytes-0.1.4/msg2bytes.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-05-11 14:39:11.000000 msg2bytes-0.1.4/msg2bytes.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       16 2023-05-11 14:39:11.000000 msg2bytes-0.1.4/msg2bytes.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       10 2023-05-11 14:39:11.000000 msg2bytes-0.1.4/msg2bytes.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       15 2023-04-26 05:04:22.000000 msg2bytes-0.1.4/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-05-11 14:39:11.373500 msg2bytes-0.1.4/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1395 2023-05-11 13:45:02.000000 msg2bytes-0.1.4/setup.py
```

### Comparing `msg2bytes-0.1.3/LICENSE` & `msg2bytes-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msg2bytes-0.1.3/PKG-INFO` & `msg2bytes-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msg2bytes
-Version: 0.1.3
+Version: 0.1.4
 Summary: MessageToBytes(msg2bytes) is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller.
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: msg2bytes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -98,7 +98,11 @@
 - First release.
 
 ### v0.1.3
 
 - Use more friendly exception names.
 - Add datetime.date codec.
 - Add datetime.time codec.
+
+### v0.1.4
+
+- Fixed async keyword missing before virtual method problem. This wasn't actually cause any problems.
```

### Comparing `msg2bytes-0.1.3/README.md` & `msg2bytes-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -81,7 +81,11 @@
 - First release.
 
 ### v0.1.3
 
 - Use more friendly exception names.
 - Add datetime.date codec.
 - Add datetime.time codec.
+
+### v0.1.4
+
+- Fixed async keyword missing before virtual method problem. This wasn't actually cause any problems.
```

### Comparing `msg2bytes-0.1.3/msg2bytes/core.py` & `msg2bytes-0.1.4/msg2bytes/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,19 +315,19 @@
         pass
 
     @classmethod
     def load(cls, rfile, **kwargs):
         pass
 
     @classmethod
-    def async_dump(cls, data, wfile, **kwargs):
+    async def async_dump(cls, data, wfile, **kwargs):
         pass
 
     @classmethod
-    def async_load(cls, rfile, **kwargs):
+    async def async_load(cls, rfile, **kwargs):
         pass
 
 
 class NoneCodec(Msg2bytesCodec):
     type = type(None)
     code = NONE
 
@@ -367,15 +367,15 @@
     async def async_dump(cls, data, wfile, **kwargs):
         if data is True:
             await TrueCodec.async_dump(data, wfile, **kwargs)
         else:
             await FalseCodec.async_dump(data, wfile, **kwargs)
 
     @classmethod
-    def async_load(cls, rfile, **kwargs):
+    async def async_load(cls, rfile, **kwargs):
         return None
 
 
 class TrueCodec(Msg2bytesCodec):
     type = bool
     code = TRUE
```

### Comparing `msg2bytes-0.1.3/msg2bytes/tests.py` & `msg2bytes-0.1.4/msg2bytes/tests.py`

 * *Files identical despite different names*

### Comparing `msg2bytes-0.1.3/msg2bytes.egg-info/PKG-INFO` & `msg2bytes-0.1.4/msg2bytes.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msg2bytes
-Version: 0.1.3
+Version: 0.1.4
 Summary: MessageToBytes(msg2bytes) is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller.
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: msg2bytes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -98,7 +98,11 @@
 - First release.
 
 ### v0.1.3
 
 - Use more friendly exception names.
 - Add datetime.date codec.
 - Add datetime.time codec.
+
+### v0.1.4
+
+- Fixed async keyword missing before virtual method problem. This wasn't actually cause any problems.
```

### Comparing `msg2bytes-0.1.3/setup.py` & `msg2bytes-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 requires = []
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="msg2bytes",
-    version="0.1.3",
+    version="0.1.4",
     description="MessageToBytes(msg2bytes) is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
```


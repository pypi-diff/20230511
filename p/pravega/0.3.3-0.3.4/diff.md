# Comparing `tmp/pravega-0.3.3-cp39-none-win_amd64.whl.zip` & `tmp/pravega-0.3.4-cp39-cp39-manylinux_2_35_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5413002 bytes, number of entries: 5
--rw-r--r--  4.6 unx     3301 b- defN 23-Apr-21 04:51 pravega-0.3.3.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Apr-21 04:51 pravega-0.3.3.dist-info/WHEEL
--rw-r--r--  4.6 unx       64 b- defN 23-Apr-21 04:51 pravega_client/__init__.py
--rwxr-xr-x  4.6 unx 15856128 b- defN 23-Apr-21 04:51 pravega_client/pravega_client.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      396 b- defN 23-Apr-21 04:51 pravega-0.3.3.dist-info/RECORD
-5 files, 15859984 bytes uncompressed, 5412270 bytes compressed:  65.9%
+Zip file size: 6122149 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2788 b- defN 23-May-11 05:37 pravega-0.3.4.dist-info/METADATA
+-rw-r--r--  4.6 unx      108 b- defN 23-May-11 05:37 pravega-0.3.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx      139 b- defN 23-May-11 05:37 pravega_client/__init__.py
+-rwxr-xr-x  4.6 unx 18030976 b- defN 23-May-11 05:37 pravega_client/pravega_client.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      410 b- defN 23-May-11 05:37 pravega-0.3.4.dist-info/RECORD
+5 files, 18034421 bytes uncompressed, 6121393 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: pravega-0.3.3.dist-info/METADATA
+Filename: pravega-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: pravega-0.3.3.dist-info/WHEEL
+Filename: pravega-0.3.4.dist-info/WHEEL
 Comment: 
 
 Filename: pravega_client/__init__.py
 Comment: 
 
-Filename: pravega_client/pravega_client.cp39-win_amd64.pyd
+Filename: pravega_client/pravega_client.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: pravega-0.3.3.dist-info/RECORD
+Filename: pravega-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pravega_client/__init__.py

```diff
@@ -1,3 +1,5 @@
 from .pravega_client import *
 
 __doc__ = pravega_client.__doc__
+if hasattr(pravega_client, "__all__"):
+    __all__ = pravega_client.__all__
```

## Comparing `pravega-0.3.3.dist-info/METADATA` & `pravega-0.3.4.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,71 @@
 Metadata-Version: 2.1
 Name: pravega
-Version: 0.3.3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Version: 0.3.4
 Summary: Pravega client
 Keywords: streaming,client,pravega
 Author: Pravega Community
 License: Apache-2.0
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/pravega/pravega-client-rust
-Project-URL: Homepage, https://pravega.github.io/pravega-client-rust/
 
-![CIbuild](https://github.com/pravega/pravega-client-rust/workflows/CIbuild/badge.svg)
-[![codecov](https://codecov.io/gh/pravega/pravega-client-rust/branch/master/graph/badge.svg?token=XEjqMkINCV)](https://codecov.io/gh/pravega/pravega-client-rust)
-
-# Pravega Python client.
-
-This project provides a way to interact with [Pravega](http://pravega.io) using Python client.
-
-Pravega is an open source distributed storage service implementing Streams. It offers Stream as the main primitive for 
-the foundation of reliable storage systems: a high-performance, durable, elastic, and unlimited append-only byte stream 
-with strict ordering and consistency.
-
-This project supports interaction with Pravega for Python versions 3.8+. For a quick tutorial on the Python bindings 
-visit the [book](https://pravega.github.io/pravega-client-rust/Python/PythonBindings.html).
-
-Also check out the Pravega Python client [API documents](https://pravega.github.io/pravega-client-rust/python/pravega_client.html).
-## Install
-
-The client library can be installed using pip.
-```shell
-pip install pravega
-```
-The users can also choose to generate the bindings using the commands specified at [PythonBinding](./PythonBinding.md) .
-
-## Example
-### Write events
-```python
-import pravega_client
-# assuming Pravega controller is listening at 127.0.0.1:9090
-stream_manager = pravega_client.StreamManager("tcp://127.0.0.1:9090")
-
-scope_result = stream_manager.create_scope("scope_foo")
-self.assertEqual(True, scope_result, "Scope creation status")
-
-stream_result = stream_manager.create_stream("scope_foo", "stream_bar", 1) # initially stream contains 1 segment
-self.assertEqual(True, stream_result, "Stream creation status")
-
-writer = stream_manager.create_writer("scope_foo","stream_bar")
-writer.write_event("hello world")
-```
-### Read events
-```python
-import pravega_client
-# assuming Pravega controller is listening at 127.0.0.1:9090
-stream_manager = pravega_client.StreamManager("tcp://127.0.0.1:9090")
-
-reader_group = stream_manager.create_reader_group("my_reader_group", "scope_foo", "stream_bar")
-
-reader = reader_group.create_reader("my_reader");
-
-# acquire a segment slice to read
-slice = await reader.get_segment_slice_async()
-for event in slice:
-    print(event.data())
-    
-# after calling release segment, data in this segment slice will not be read again by
-# readers in the same reader group.
-reader.release_segment(slice)
-
-# remember to mark the finished reader as offline.
-reader.reader_offline()
+![CIbuild](https://github.com/pravega/pravega-client-rust/workflows/CIbuild/badge.svg)
+[![codecov](https://codecov.io/gh/pravega/pravega-client-rust/branch/master/graph/badge.svg?token=XEjqMkINCV)](https://codecov.io/gh/pravega/pravega-client-rust)
+
+# Pravega Python client.
+
+This project provides a way to interact with [Pravega](http://pravega.io) using Python client.
+
+Pravega is an open source distributed storage service implementing Streams. It offers Stream as the main primitive for 
+the foundation of reliable storage systems: a high-performance, durable, elastic, and unlimited append-only byte stream 
+with strict ordering and consistency.
+
+This project supports interaction with Pravega for Python versions 3.8+. For a quick tutorial on the Python bindings 
+visit the [book](https://pravega.github.io/pravega-client-rust/Python/PythonBindings.html).
+
+Also check out the Pravega Python client [API documents](https://pravega.github.io/pravega-client-rust/python/pravega_client.html).
+## Install
+
+The client library can be installed using pip.
+```shell
+pip install pravega
+```
+The users can also choose to generate the bindings using the commands specified at [PythonBinding](./PythonBinding.md) .
+
+## Example
+### Write events
+```python
+import pravega_client
+# assuming Pravega controller is listening at 127.0.0.1:9090
+stream_manager = pravega_client.StreamManager("tcp://127.0.0.1:9090")
+
+scope_result = stream_manager.create_scope("scope_foo")
+self.assertEqual(True, scope_result, "Scope creation status")
+
+stream_result = stream_manager.create_stream("scope_foo", "stream_bar", 1) # initially stream contains 1 segment
+self.assertEqual(True, stream_result, "Stream creation status")
+
+writer = stream_manager.create_writer("scope_foo","stream_bar")
+writer.write_event("hello world")
+```
+### Read events
+```python
+import pravega_client
+# assuming Pravega controller is listening at 127.0.0.1:9090
+stream_manager = pravega_client.StreamManager("tcp://127.0.0.1:9090")
+
+reader_group = stream_manager.create_reader_group("my_reader_group", "scope_foo", "stream_bar")
+
+reader = reader_group.create_reader("my_reader");
+
+# acquire a segment slice to read
+slice = await reader.get_segment_slice_async()
+for event in slice:
+    print(event.data())
+    
+# after calling release segment, data in this segment slice will not be read again by
+# readers in the same reader group.
+reader.release_segment(slice)
+
+# remember to mark the finished reader as offline.
+reader.reader_offline()
 ```
```


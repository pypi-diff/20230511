# Comparing `tmp/pure_protobuf-3.0.0a3.tar.gz` & `tmp/pure_protobuf-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_protobuf-3.0.0a3.tar", max compression
+gzip compressed data, was "pure_protobuf-3.0.0a4.tar", max compression
```

## Comparing `pure_protobuf-3.0.0a3.tar` & `pure_protobuf-3.0.0a4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1089 2023-04-25 14:26:30.317963 pure_protobuf-3.0.0a3/LICENSE
--rw-r--r--   0        0        0     3210 2023-04-25 14:26:30.317963 pure_protobuf-3.0.0a3/README.md
--rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/__init__.py
--rw-r--r--   0        0        0     2375 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/_accumulators.py
--rw-r--r--   0        0        0     1679 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/_mergers.py
--rw-r--r--   0        0        0     3259 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/annotations.py
--rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/descriptors/__init__.py
--rw-r--r--   0        0        0     4769 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/descriptors/_field.py
--rw-r--r--   0        0        0     7833 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/descriptors/record.py
--rw-r--r--   0        0        0      685 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/__init__.py
--rw-r--r--   0        0        0      211 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/_dataclasses.py
--rw-r--r--   0        0        0     1085 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/_typing.py
--rw-r--r--   0        0        0      441 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/datetime.py
--rw-r--r--   0        0        0      589 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/io.py
--rw-r--r--   0        0        0      635 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/itertools.py
--rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/__init__.py
--rw-r--r--   0        0        0      935 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_repr.py
--rw-r--r--   0        0        0      620 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_skip.py
--rw-r--r--   0        0        0      522 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_vars.py
--rw-r--r--   0        0        0      716 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/accumulate.py
--rw-r--r--   0        0        0      486 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/merge.py
--rw-r--r--   0        0        0      818 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/read.py
--rw-r--r--   0        0        0      402 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/write.py
--rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/__init__.py
--rw-r--r--   0        0        0     1420 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/bytes_.py
--rw-r--r--   0        0        0      269 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/fixed32.py
--rw-r--r--   0        0        0      250 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/fixed64.py
--rw-r--r--   0        0        0     1112 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/struct_.py
--rw-r--r--   0        0        0     1446 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/tag.py
--rw-r--r--   0        0        0      619 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/url.py
--rw-r--r--   0        0        0     4541 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/varint.py
--rw-r--r--   0        0        0     1204 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/wire_type.py
--rw-r--r--   0        0        0     4976 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/wrappers.py
--rw-r--r--   0        0        0     5180 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/message.py
--rw-r--r--   0        0        0     2376 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/one_of.py
--rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/py.typed
--rw-r--r--   0        0        0     3720 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/well_known.py
--rw-r--r--   0        0        0     3425 2023-04-25 14:26:48.458065 pure_protobuf-3.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 pure_protobuf-3.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/LICENSE
+-rw-r--r--   0        0        0     3323 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/__init__.py
+-rw-r--r--   0        0        0     2375 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/_accumulators.py
+-rw-r--r--   0        0        0     1679 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/_mergers.py
+-rw-r--r--   0        0        0     3041 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/annotations.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/descriptors/__init__.py
+-rw-r--r--   0        0        0     4769 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/descriptors/_field.py
+-rw-r--r--   0        0        0     7339 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/descriptors/record.py
+-rw-r--r--   0        0        0      685 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/helpers/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/helpers/_dataclasses.py
+-rw-r--r--   0        0        0     1085 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/helpers/_typing.py
+-rw-r--r--   0        0        0      441 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/helpers/datetime.py
+-rw-r--r--   0        0        0      589 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/helpers/io.py
+-rw-r--r--   0        0        0      635 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/helpers/itertools.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:37:03.440747 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/__init__.py
+-rw-r--r--   0        0        0      935 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/_repr.py
+-rw-r--r--   0        0        0      620 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/_skip.py
+-rw-r--r--   0        0        0      522 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/_vars.py
+-rw-r--r--   0        0        0      716 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/accumulate.py
+-rw-r--r--   0        0        0      486 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/merge.py
+-rw-r--r--   0        0        0      818 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/read.py
+-rw-r--r--   0        0        0      402 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/interfaces/write.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/__init__.py
+-rw-r--r--   0        0        0     1372 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/bytes_.py
+-rw-r--r--   0        0        0      269 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/fixed32.py
+-rw-r--r--   0        0        0      250 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/fixed64.py
+-rw-r--r--   0        0        0     1112 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/struct_.py
+-rw-r--r--   0        0        0     1397 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/tag.py
+-rw-r--r--   0        0        0      619 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/url.py
+-rw-r--r--   0        0        0     4119 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/varint.py
+-rw-r--r--   0        0        0     1204 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/wire_type.py
+-rw-r--r--   0        0        0     4976 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/io/wrappers.py
+-rw-r--r--   0        0        0     5180 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/message.py
+-rw-r--r--   0        0        0     2376 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/one_of.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/py.typed
+-rw-r--r--   0        0        0     3720 2023-05-10 21:37:03.444748 pure_protobuf-3.0.0a4/pure_protobuf/well_known.py
+-rw-r--r--   0        0        0     3425 2023-05-10 21:37:24.196341 pure_protobuf-3.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     4868 1970-01-01 00:00:00.000000 pure_protobuf-3.0.0a4/PKG-INFO
```

### Comparing `pure_protobuf-3.0.0a3/LICENSE` & `pure_protobuf-3.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/README.md` & `pure_protobuf-3.0.0a4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,63 +19,67 @@
     <img alt="Documentation" height="30em" src="https://img.shields.io/github/actions/workflow/status/eigenein/protobuf/docs.yml?label=documentation&logo=github">
 </a>
 
 ## Quick examples
 
 ### `.proto` definition
 
+It's not needed for `pure-protobuf`, but for the sake of an example, let's consider the following definition:
+
 ```protobuf
 syntax = "proto3";
 
 message SearchRequest {
   string query = 1;
   int32 page_number = 2;
   int32 result_per_page = 3;
 }
 ```
 
+And here's the same via `pure-protobuf`:
+
 ### With [dataclasses](https://docs.python.org/3/library/dataclasses.html)
 
 ```python title="dataclass_example.py"
 from dataclasses import dataclass
 from io import BytesIO
 
-from pure_protobuf.annotations import Field, uint
+from pure_protobuf.annotations import Field
 from pure_protobuf.message import BaseMessage
 from typing_extensions import Annotated
 
 
 @dataclass
 class SearchRequest(BaseMessage):
     query: Annotated[str, Field(1)] = ""
-    page_number: Annotated[uint, Field(2)] = 0
-    result_per_page: Annotated[uint, Field(3)] = 0
+    page_number: Annotated[int, Field(2)] = 0
+    result_per_page: Annotated[int, Field(3)] = 0
 
 
-request = SearchRequest(query="hello", page_number=uint(1), result_per_page=uint(10))
+request = SearchRequest(query="hello", page_number=1, result_per_page=10)
 buffer = bytes(request)
 assert buffer == b"\x0A\x05hello\x10\x01\x18\x0A"
 assert SearchRequest.read_from(BytesIO(buffer)) == request
 ```
 
 ### With [`pydantic`](https://docs.pydantic.dev/)
 
 ```python title="pydantic_example.py"
 from io import BytesIO
 
-from pure_protobuf.annotations import Field, uint
+from pure_protobuf.annotations import Field
 from pure_protobuf.message import BaseMessage
 from pydantic import BaseModel
 from typing_extensions import Annotated
 
 
 class SearchRequest(BaseMessage, BaseModel):
     query: Annotated[str, Field(1)] = ""
-    page_number: Annotated[uint, Field(2)] = 0
-    result_per_page: Annotated[uint, Field(3)] = 0
+    page_number: Annotated[int, Field(2)] = 0
+    result_per_page: Annotated[int, Field(3)] = 0
 
 
-request = SearchRequest(query="hello", page_number=uint(1), result_per_page=uint(10))
+request = SearchRequest(query="hello", page_number=1, result_per_page=10)
 buffer = bytes(request)
 assert buffer == b"\x0A\x05hello\x10\x01\x18\x0A"
 assert SearchRequest.read_from(BytesIO(buffer)) == request
 ```
```

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/_accumulators.py` & `pure_protobuf-3.0.0a4/pure_protobuf/_accumulators.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/_mergers.py` & `pure_protobuf-3.0.0a4/pure_protobuf/_mergers.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/annotations.py` & `pure_protobuf-3.0.0a4/pure_protobuf/annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,25 +97,14 @@
 Fixed signed 64-bit integer.
 
 See Also:
     - https://developers.google.com/protocol-buffers/docs/proto3#scalar
     - https://developers.google.com/protocol-buffers/docs/encoding#non-varint-nums
 """
 
-uint = NewType("uint", int)
-"""Unsigned variable-length integer."""
-
-int32 = NewType("int32", int)
-"""
-Two's compliment integer.
-
-See Also:
-    - https://developers.google.com/protocol-buffers/docs/encoding#signed-ints
-"""
-
-int64 = NewType("int64", int)
+ZigZagInt = NewType("ZigZagInt", int)
 """
-Two's compliment integer.
+ZigZag-encoded integer.
 
 See Also:
     - https://developers.google.com/protocol-buffers/docs/encoding#signed-ints
 """
```

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/descriptors/_field.py` & `pure_protobuf-3.0.0a4/pure_protobuf/descriptors/_field.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/descriptors/record.py` & `pure_protobuf-3.0.0a4/pure_protobuf/descriptors/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, Any, ByteString, ClassVar, Dict, Generic, Type
 from urllib.parse import ParseResult
 
 from typing_extensions import Self
 
 from pure_protobuf._accumulators import AccumulateLastOneWins
 from pure_protobuf._mergers import MergeLastOneWins
-from pure_protobuf.annotations import double, fixed32, fixed64, int32, int64, sfixed32, sfixed64, uint
+from pure_protobuf.annotations import ZigZagInt, double, fixed32, fixed64, sfixed32, sfixed64
 from pure_protobuf.exceptions import UnsupportedAnnotationError
 from pure_protobuf.helpers._dataclasses import KW_ONLY, SLOTS
 from pure_protobuf.helpers.itertools import ReadCallback
 from pure_protobuf.interfaces._vars import RecordT
 from pure_protobuf.interfaces.accumulate import Accumulate
 from pure_protobuf.interfaces.merge import Merge
 from pure_protobuf.interfaces.read import ReadTyped
@@ -23,19 +23,17 @@
 from pure_protobuf.io.url import ReadUrl, WriteUrl
 from pure_protobuf.io.varint import (
     ReadEnum,
     ReadTwosComplimentVarint,
     WriteEnum,
     WriteTwosComplimentVarint,
     read_bool,
-    read_signed_varint,
-    read_unsigned_varint,
+    read_zigzag_varint,
     write_bool,
-    write_signed_varint,
-    write_unsigned_varint,
+    write_zigzag_varint,
 )
 from pure_protobuf.io.wire_type import WireType
 from pure_protobuf.io.wrappers import ReadMaybePacked, ReadStrictlyTyped
 
 if TYPE_CHECKING:
     from pure_protobuf.message import BaseMessage
 
@@ -174,35 +172,25 @@
     ByteString: BYTES_DESCRIPTOR,
     fixed32: UNSIGNED_INT32_DESCRIPTOR,
     fixed64: UNSIGNED_INT64_DESCRIPTOR,
     float: FLOAT_DESCRIPTOR,
     double: DOUBLE_DESCRIPTOR,
     int: RecordDescriptor(
         wire_type=WireType.VARINT,
-        write=write_signed_varint,
-        read=ReadMaybePacked[int](ReadCallback(read_signed_varint), WireType.VARINT),
-    ),
-    int32: RecordDescriptor(
-        wire_type=WireType.VARINT,
-        write=WriteTwosComplimentVarint[int32](),
-        read=ReadMaybePacked[int32](ReadCallback(ReadTwosComplimentVarint[int32]()), WireType.VARINT),
-    ),
-    int64: RecordDescriptor(
-        wire_type=WireType.VARINT,
-        write=WriteTwosComplimentVarint[int64](),
-        read=ReadMaybePacked[int64](ReadCallback(ReadTwosComplimentVarint[int64]()), WireType.VARINT),
+        write=WriteTwosComplimentVarint(),
+        read=ReadMaybePacked[int](ReadCallback(ReadTwosComplimentVarint()), WireType.VARINT),
     ),
     memoryview: BYTES_DESCRIPTOR,
     ParseResult: URL_DESCRIPTOR,
     sfixed32: SIGNED_INT32_DESCRIPTOR,
     sfixed64: UNSIGNED_INT64_DESCRIPTOR,
     str: RecordDescriptor(
         wire_type=WireType.LEN,
         write=write_string,
         read=ReadStrictlyTyped(ReadCallback(read_string), WireType.LEN),
     ),
-    uint: RecordDescriptor(
+    ZigZagInt: RecordDescriptor(
         wire_type=WireType.VARINT,
-        write=write_unsigned_varint,
-        read=ReadMaybePacked[uint](ReadCallback(read_unsigned_varint), WireType.VARINT),
+        write=write_zigzag_varint,
+        read=ReadMaybePacked[int](ReadCallback(read_zigzag_varint), WireType.VARINT),
     ),
 }
```

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/exceptions.py` & `pure_protobuf-3.0.0a4/pure_protobuf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/helpers/_typing.py` & `pure_protobuf-3.0.0a4/pure_protobuf/helpers/_typing.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/helpers/io.py` & `pure_protobuf-3.0.0a4/pure_protobuf/helpers/io.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/helpers/itertools.py` & `pure_protobuf-3.0.0a4/pure_protobuf/helpers/itertools.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_repr.py` & `pure_protobuf-3.0.0a4/pure_protobuf/interfaces/_repr.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_skip.py` & `pure_protobuf-3.0.0a4/pure_protobuf/interfaces/_skip.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_vars.py` & `pure_protobuf-3.0.0a4/pure_protobuf/interfaces/_vars.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/accumulate.py` & `pure_protobuf-3.0.0a4/pure_protobuf/interfaces/accumulate.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/read.py` & `pure_protobuf-3.0.0a4/pure_protobuf/interfaces/read.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/io/bytes_.py` & `pure_protobuf-3.0.0a4/pure_protobuf/io/bytes_.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Reading and writing scalar length-delimited values.
 
 See Also:
     - https://developers.google.com/protocol-buffers/docs/encoding#length-types
+
 """
 
 from io import SEEK_CUR
 from typing import IO
 
-from pure_protobuf.annotations import uint
 from pure_protobuf.helpers.io import read_checked
 from pure_protobuf.interfaces._skip import Skip
 from pure_protobuf.interfaces.read import ReadSingular
 from pure_protobuf.interfaces.write import Write
 from pure_protobuf.io.varint import read_unsigned_varint, write_unsigned_varint
 
 
@@ -20,15 +20,15 @@
     def __call__(self, io: IO[bytes]) -> None:
         length = read_unsigned_varint(io)
         io.seek(length, SEEK_CUR)
 
 
 class WriteBytes(Write[bytes]):
     def __call__(self, value: bytes, io: IO[bytes]) -> None:
-        write_unsigned_varint(uint(len(value)), io)
+        write_unsigned_varint(len(value), io)
         io.write(value)
 
 
 class ReadBytes(ReadSingular[bytes]):
     def __call__(self, io: IO[bytes]) -> bytes:
         length = read_unsigned_varint(io)
         return read_checked(io, length)
```

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/io/struct_.py` & `pure_protobuf-3.0.0a4/pure_protobuf/io/struct_.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/io/tag.py` & `pure_protobuf-3.0.0a4/pure_protobuf/io/tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass
 from typing import IO
 
 from typing_extensions import Self
 
-from pure_protobuf.annotations import uint
 from pure_protobuf.exceptions import IncorrectWireTypeError
 from pure_protobuf.helpers._dataclasses import KW_ONLY, SLOTS
 from pure_protobuf.io.varint import read_unsigned_varint, write_unsigned_varint
 from pure_protobuf.io.wire_type import WireType
 
 
 @dataclass(frozen=True, **KW_ONLY, **SLOTS)
@@ -35,8 +34,8 @@
 
     def encode(self) -> int:
         """Convert the tag into its encoded format."""
         return (self.field_number << 3) | self.wire_type.value  # type: ignore
 
     def write_to(self, io: IO[bytes]) -> None:
         """Write the tag into the file object."""
-        write_unsigned_varint(uint(self.encode()), io)
+        write_unsigned_varint(self.encode(), io)
```

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/io/url.py` & `pure_protobuf-3.0.0a4/pure_protobuf/io/url.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/io/varint.py` & `pure_protobuf-3.0.0a4/pure_protobuf/io/varint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,134 +1,127 @@
 """
 Reading and writing varints and the derivative types.
 
 See Also:
     - https://developers.google.com/protocol-buffers/docs/encoding#varints
+
 """
 
 from enum import IntEnum
 from itertools import count
 from sys import byteorder
-from typing import IO, Generic, Iterator, Type, TypeVar, cast
+from typing import IO, Iterator, Type, TypeVar
 
-from pure_protobuf.annotations import int32, int64, uint
 from pure_protobuf.exceptions import IncorrectValueError
 from pure_protobuf.helpers.io import read_byte_checked
 from pure_protobuf.interfaces._skip import Skip
 from pure_protobuf.interfaces.read import Read, ReadSingular
 from pure_protobuf.interfaces.write import Write
 
 
 class SkipVarint(Skip):
     def __call__(self, io: IO[bytes]) -> None:
         while read_byte_checked(io) & 0x80:
             pass
 
 
-class ReadUnsignedVarint(ReadSingular[uint]):
+class ReadUnsignedVarint(ReadSingular[int]):
     """Reads unsigned varint from the stream."""
 
-    def __call__(self, io: IO[bytes]) -> uint:
+    def __call__(self, io: IO[bytes]) -> int:
         value = 0
         for shift in count(0, 7):
             byte = read_byte_checked(io)
             value |= (byte & 0x7F) << shift
             if not byte & 0x80:
-                return uint(value)
+                return value
         raise AssertionError("unreachable code")
 
 
-class WriteUnsignedVarint(Write[uint]):
+class WriteUnsignedVarint(Write[int]):
     """Writes unsigned varint to the stream."""
 
-    def __call__(self, value: uint, io: IO[bytes]) -> None:
-        value = int(value)
+    def __call__(self, value: int, io: IO[bytes]) -> None:
         while value > 0x7F:
             io.write(bytes((value & 0x7F | 0x80,)))
             value >>= 7
         io.write(bytes((value,)))
 
 
 skip_varint = SkipVarint()
 read_unsigned_varint = ReadUnsignedVarint()
 write_unsigned_varint = WriteUnsignedVarint()
 
 
-class ReadSignedVarint(ReadSingular[int]):
+class ReadZigZagVarint(ReadSingular[int]):
     """
-    Reads a **signed** varint.
+    Reads a ZigZag-encoded varint.
 
     See Also:
         - https://stackoverflow.com/a/2211086/359730.
     """
 
     def __call__(self, io: IO[bytes]) -> int:
         value = read_unsigned_varint(io)
         return (value >> 1) ^ (-(value & 1))
 
 
-class WriteSignedVarint(Write[int]):
-    """Writes a **signed** varint."""
+class WriteZigZagVarint(Write[int]):
+    """Writes a ZigZag-encoded varint."""
 
     def __call__(self, value: int, io: IO[bytes]) -> None:
-        write_unsigned_varint(uint(abs(value) * 2 - (value < 0)), io)
-
+        write_unsigned_varint(abs(value) * 2 - (value < 0), io)
 
-read_signed_varint = ReadSignedVarint()
-write_signed_varint = WriteSignedVarint()
 
+read_zigzag_varint = ReadZigZagVarint()
+write_zigzag_varint = WriteZigZagVarint()
 
-TwosComplimentIntegerT = TypeVar("TwosComplimentIntegerT", int32, int64, int)
 
-
-class ReadTwosComplimentVarint(Generic[TwosComplimentIntegerT], ReadSingular[TwosComplimentIntegerT]):
+class ReadTwosComplimentVarint(ReadSingular[int]):
     """
     Reads a two's compliment varint.
 
     See Also:
         - https://protobuf.dev/programming-guides/encoding/#signed-ints
     """
 
-    def __call__(self, io: IO[bytes]) -> TwosComplimentIntegerT:
+    def __call__(self, io: IO[bytes]) -> int:
         varint = read_unsigned_varint(io)
-        return cast(
-            TwosComplimentIntegerT,
-            int.from_bytes(
-                varint.to_bytes(8, byteorder, signed=False),
-                byteorder,
-                signed=True,
-            ),
+        return int.from_bytes(
+            varint.to_bytes(8, byteorder, signed=False),
+            byteorder,
+            signed=True,
         )
 
 
-class WriteTwosComplimentVarint(Generic[TwosComplimentIntegerT], Write[TwosComplimentIntegerT]):
+class WriteTwosComplimentVarint(Write[int]):
     """
     Writes a two's compliment varint.
 
     See Also:
         - https://protobuf.dev/programming-guides/encoding/#signed-ints
     """
 
-    def __call__(self, value: TwosComplimentIntegerT, io: IO[bytes]) -> None:
+    def __call__(self, value: int, io: IO[bytes]) -> None:
         compliment = int.from_bytes(
             value.to_bytes(8, byteorder, signed=True),
             byteorder,
             signed=False,
         )
-        return write_unsigned_varint(uint(compliment), io)
+        return write_unsigned_varint(compliment, io)
 
 
 class ReadBool(ReadSingular[bool]):
     def __call__(self, io: IO[bytes]) -> bool:
         return bool(read_unsigned_varint(io))
 
 
 class WriteBool(Write[bool]):
     def __call__(self, value: bool, io: IO[bytes]) -> None:
-        write_unsigned_varint(uint(value), io)
+        write_unsigned_varint(int(value), io)
 
 
 read_bool = ReadBool()
 write_bool = WriteBool()
 
 
 EnumT = TypeVar("EnumT", bound=IntEnum)
@@ -155,8 +148,8 @@
 
 
 class WriteEnum(Write[EnumT]):
     __slots__ = ()
 
     def __call__(self, value: EnumT, io: IO[bytes]) -> None:
         # noinspection PyTypeChecker
-        write_unsigned_varint(uint(value.value), io)
+        write_unsigned_varint(value.value, io)
```

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/io/wire_type.py` & `pure_protobuf-3.0.0a4/pure_protobuf/io/wire_type.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/io/wrappers.py` & `pure_protobuf-3.0.0a4/pure_protobuf/io/wrappers.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/message.py` & `pure_protobuf-3.0.0a4/pure_protobuf/message.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/one_of.py` & `pure_protobuf-3.0.0a4/pure_protobuf/one_of.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pure_protobuf/well_known.py` & `pure_protobuf-3.0.0a4/pure_protobuf/well_known.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a3/pyproject.toml` & `pure_protobuf-3.0.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "Protocol Buffers using Python type annotations"
 keywords = ["protobuf", "protocol-buffers"]
 license = "MIT"
 name = "pure-protobuf"
 readme = "README.md"
 repository = "https://github.com/eigenein/protobuf"
-version = "3.0.0a3"
+version = "3.0.0a4"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3 :: Only",
@@ -39,26 +39,26 @@
 typing-extensions = "^4.4.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
+cairosvg = "^2.6.0"
+mkdocs-autorefs = "^0.4.1"
+mkdocs-git-revision-date-localized-plugin = "^1.1.0"
+mkdocs-material = "^9.1.11"
+mkdocstrings = { version = "^0.21.2", extras = ["python"] }
 mypy = "^1.2.0"
+pillow = "^9.4.0"
 pydantic = "^1.10.4"
 pytest = "^7.2.0"
 pytest-benchmark = "^4.0.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.247"
-mkdocs-material = "^9.0.12"
-pillow = "^9.4.0"
-cairosvg = "^2.6.0"
-mkdocs-git-revision-date-localized-plugin = "^1.1.0"
-mkdocstrings = { version = "^0.20.0", extras = ["python"] }
-mkdocs-autorefs = "^0.4.1"
+ruff = "^0.0.265"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/eigenein/protobuf/blob/master/CHANGELOG.md"
 "Homepage" = "https://github.com/eigenein/protobuf"
 "Issues" = "https://github.com/eigenein/protobuf/issues"
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `pure_protobuf-3.0.0a3/PKG-INFO` & `pure_protobuf-3.0.0a4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-protobuf
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Protocol Buffers using Python type annotations
 Home-page: https://github.com/eigenein/protobuf
 License: MIT
 Keywords: protobuf,protocol-buffers
 Author: Pavel Perestoronin
 Author-email: eigenein@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -53,64 +53,68 @@
     <img alt="Documentation" height="30em" src="https://img.shields.io/github/actions/workflow/status/eigenein/protobuf/docs.yml?label=documentation&logo=github">
 </a>
 
 ## Quick examples
 
 ### `.proto` definition
 
+It's not needed for `pure-protobuf`, but for the sake of an example, let's consider the following definition:
+
 ```protobuf
 syntax = "proto3";
 
 message SearchRequest {
   string query = 1;
   int32 page_number = 2;
   int32 result_per_page = 3;
 }
 ```
 
+And here's the same via `pure-protobuf`:
+
 ### With [dataclasses](https://docs.python.org/3/library/dataclasses.html)
 
 ```python title="dataclass_example.py"
 from dataclasses import dataclass
 from io import BytesIO
 
-from pure_protobuf.annotations import Field, uint
+from pure_protobuf.annotations import Field
 from pure_protobuf.message import BaseMessage
 from typing_extensions import Annotated
 
 
 @dataclass
 class SearchRequest(BaseMessage):
     query: Annotated[str, Field(1)] = ""
-    page_number: Annotated[uint, Field(2)] = 0
-    result_per_page: Annotated[uint, Field(3)] = 0
+    page_number: Annotated[int, Field(2)] = 0
+    result_per_page: Annotated[int, Field(3)] = 0
 
 
-request = SearchRequest(query="hello", page_number=uint(1), result_per_page=uint(10))
+request = SearchRequest(query="hello", page_number=1, result_per_page=10)
 buffer = bytes(request)
 assert buffer == b"\x0A\x05hello\x10\x01\x18\x0A"
 assert SearchRequest.read_from(BytesIO(buffer)) == request
 ```
 
 ### With [`pydantic`](https://docs.pydantic.dev/)
 
 ```python title="pydantic_example.py"
 from io import BytesIO
 
-from pure_protobuf.annotations import Field, uint
+from pure_protobuf.annotations import Field
 from pure_protobuf.message import BaseMessage
 from pydantic import BaseModel
 from typing_extensions import Annotated
 
 
 class SearchRequest(BaseMessage, BaseModel):
     query: Annotated[str, Field(1)] = ""
-    page_number: Annotated[uint, Field(2)] = 0
-    result_per_page: Annotated[uint, Field(3)] = 0
+    page_number: Annotated[int, Field(2)] = 0
+    result_per_page: Annotated[int, Field(3)] = 0
 
 
-request = SearchRequest(query="hello", page_number=uint(1), result_per_page=uint(10))
+request = SearchRequest(query="hello", page_number=1, result_per_page=10)
 buffer = bytes(request)
 assert buffer == b"\x0A\x05hello\x10\x01\x18\x0A"
 assert SearchRequest.read_from(BytesIO(buffer)) == request
 ```
```


# Comparing `tmp/pyodc-1.1.4.tar.gz` & `tmp/pyodc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodc-1.1.4.tar", last modified: Wed Aug 24 12:29:11 2022, max compression
+gzip compressed data, was "pyodc-1.2.0.tar", last modified: Thu May 11 13:05:42 2023, max compression
```

## Comparing `pyodc-1.1.4.tar` & `pyodc-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 12:29:11.241690 pyodc-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-08-24 12:28:44.000000 pyodc-1.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-24 12:28:44.000000 pyodc-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-24 12:28:44.000000 pyodc-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2022-08-24 12:29:11.241690 pyodc-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-08-24 12:28:44.000000 pyodc-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 12:29:11.237690 pyodc-1.1.4/codc/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-08-24 12:28:44.000000 pyodc-1.1.4/codc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-08-24 12:28:44.000000 pyodc-1.1.4/codc/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4308 2022-08-24 12:28:44.000000 pyodc-1.1.4/codc/encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     8996 2022-08-24 12:28:44.000000 pyodc-1.1.4/codc/frame.py
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-08-24 12:28:44.000000 pyodc-1.1.4/codc/lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-08-24 12:28:44.000000 pyodc-1.1.4/codc/processed_odc.h
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-08-24 12:28:44.000000 pyodc-1.1.4/codc/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 12:29:11.241690 pyodc-1.1.4/pyodc/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyodc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14938 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyodc/codec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyodc/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6391 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyodc/encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)    10385 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyodc/frame.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyodc/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2807 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyodc/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 12:29:11.241690 pyodc-1.1.4/pyodc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2022-08-24 12:29:11.000000 pyodc-1.1.4/pyodc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-08-24 12:29:11.000000 pyodc-1.1.4/pyodc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 12:29:11.000000 pyodc-1.1.4/pyodc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-24 12:29:11.000000 pyodc-1.1.4/pyodc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-24 12:29:11.000000 pyodc-1.1.4/pyodc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 12:29:11.000000 pyodc-1.1.4/pyodc.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-24 12:28:44.000000 pyodc-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 12:29:11.241690 pyodc-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-08-24 12:28:44.000000 pyodc-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-05-11 13:05:18.000000 pyodc-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-11 13:05:18.000000 pyodc-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-11 13:05:18.000000 pyodc-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-11 13:05:42.730787 pyodc-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2923 2023-05-11 13:05:18.000000 pyodc-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/codc/
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4308 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11079 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4718 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/lib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/processed_odc.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/pyodc/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14921 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6386 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/pyodc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 13:05:42.730787 pyodc-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-11 13:05:18.000000 pyodc-1.2.0/setup.py
```

### Comparing `pyodc-1.1.4/CHANGELOG.md` & `pyodc-1.2.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyodc-1.1.4/LICENSE` & `pyodc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodc-1.1.4/PKG-INFO` & `pyodc-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodc
-Version: 1.1.4
+Version: 1.2.0
 Summary: A Python interface to odc for encoding/decoding ODB-2 files.
 Home-page: https://github.com/ecmwf/pyodc
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: odc odb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyodc-1.1.4/README.md` & `pyodc-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodc-1.1.4/codc/encoder.py` & `pyodc-1.2.0/codc/encoder.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.1.4/codc/frame.py` & `pyodc-1.2.0/codc/frame.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,21 @@
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
 import codecs
 import os
 
-import numpy
+import numpy as np
 import pandas
 
 
 # A null-terminated UTF-8 decoder
 def null_utf_decoder(name):
     if name == "utf_8_null":
-
         utf8_decoder = codecs.getdecoder("utf-8")
 
         return codecs.CodecInfo(
             name="utf_8_null",
             encode=None,
             decode=lambda b, e: utf8_decoder(b.split(b"\x00", 1)[0], e),
             incrementalencoder=None,
@@ -36,14 +35,20 @@
 class ColumnInfo:
     class Bitfield:
         def __init__(self, name, size, offset):
             self.name = name
             self.size = size
             self.offset = offset
 
+        def __eq__(self, other):
+            return self.name == other.name and self.size == other.size and self.offset == other.offset
+
+        def __str__(self):
+            return f"bits(name={self.name}, size={self.size}, offset={self.offset})"
+
     def __init__(self, name, idx, dtype, datasize, bitfields):
         self.name = name
         self.dtype = dtype
         self.index = idx
         self.datasize = datasize
         self.bitfields = bitfields
         assert (dtype == BITFIELD) != (bitfields is None)
@@ -68,15 +73,14 @@
         self.__columns = None
 
     @property
     @memoize_constant
     def columns(self):
         columns = []
         for col in range(self.ncolumns):
-
             pname = ffi.new("const char**")
             ptype = ffi.new("int*")
             pdatasize = ffi.new("int*")
             pbitfield_count = ffi.new("int*")
             lib.odc_frame_column_attributes(self.__frame, col, pname, ptype, pdatasize, pbitfield_count)
             name = ffi.string(pname[0]).decode("utf-8")
             dtype = DataType(int(ptype[0]))
@@ -88,15 +92,14 @@
                 assert datasize % 8 == 0
             else:
                 assert datasize == 8
 
             if dtype == BITFIELD:
                 bitfields = []
                 for n in range(bitfield_count):
-
                     pbitfield_name = ffi.new("const char**")
                     poffset = ffi.new("int*")
                     psize = ffi.new("int*")
                     lib.odc_frame_bitfield_attributes(self.__frame, col, n, pbitfield_name, poffset, psize)
 
                     bitfields.append(
                         ColumnInfo.Bitfield(
@@ -161,24 +164,70 @@
             key = ffi.string(key_temp[0]).decode("utf-8")
             value = ffi.string(value_temp[0]).decode("utf-8")
             properties[key] = value
 
         return properties
 
     def dataframe(self, columns=None):
+        # Are there any bitfield columns we need to consider?
+        original_columns = columns
+        bitfields = []
+
+        if columns is not None:
+            final_columns = set()
+            for colname in columns:
+                dotpos = colname.find(".")
+                if dotpos == -1:
+                    final_columns.add(colname)
+                else:
+                    column_name = colname[:dotpos]
+                    sp = colname[dotpos + 1 :].split("@")
+                    bitfield_name = sp[0]
+                    if len(sp) > 1:
+                        column_name += "@" + sp[1]
+                    final_columns.add(column_name)
+                    bitfields.append((bitfield_name, column_name, colname))
+            columns = list(final_columns)
+
+        df = self._dataframe_internal(columns)
+
+        # If there are any bitfields that need extraction, do it here, and remove any temporarily
+        # decoded columns as is possible
+
+        if bitfields:
+            extracted_columns = set()
+            for bitfield_name, column_name, output_name in bitfields:
+                assert df[column_name].dtype == np.int64
+                col = self.column_dict[column_name]
+                bf = next((b for b in col.bitfields if b.name == bitfield_name))
+                mask = (1 << bf.size) - 1
+                new_column = np.right_shift(df[column_name], bf.offset) & mask
+                if bf.size == 1:
+                    new_column = new_column.astype(bool)
+                df[output_name] = new_column
+                extracted_columns.add(column_name)
+
+            for column in extracted_columns:
+                if column not in original_columns:
+                    del df[column]
 
+        return df
+
+    def _dataframe_internal(self, columns=None):
         # Some constants that are useful
 
         pmissing_integer = ffi.new("long*")
         pmissing_double = ffi.new("double*")
         lib.odc_missing_integer(pmissing_integer)
         lib.odc_missing_double(pmissing_double)
         missing_integer = pmissing_integer[0]
         missing_double = pmissing_double[0]
 
+        # If no column info specified, use the defaults
+
         if columns is None:
             columns = [c.name for c in self.columns]
 
         assert columns is not None
 
         cd = self.column_dict
         scd, ambiguous_columns = self._simple_column_dict_ambiguous
@@ -208,28 +257,25 @@
 
         lib.odc_decoder_set_row_count(decoder, self.nrows)
 
         dataframes = []
         pos = 0
         string_seq = tuple((cols, "|S{}".format(dataSize), dataSize) for dataSize, cols in string_cols.items())
         for cols, dtype, dsize in (
-            (integer_cols, numpy.int64, 8),
-            (double_cols, numpy.double, 8),
+            (integer_cols, np.int64, 8),
+            (double_cols, np.double, 8),
         ) + string_seq:
-
             if len(cols) > 0:
-
-                array = numpy.empty((self.nrows, len(cols)), dtype=dtype, order="C")
+                array = np.empty((self.nrows, len(cols)), dtype=dtype, order="C")
 
                 pointer = array.ctypes.data
                 strides = array.ctypes.strides
 
                 colnames = []
                 for i, (name, col) in enumerate(cols):
-
                     colnames.append(name)
                     lib.odc_decoder_add_column(decoder, col.name.encode("utf-8"))
                     lib.odc_decoder_column_set_data_array(
                         decoder,
                         pos,
                         dsize,
                         strides[0],
@@ -248,17 +294,17 @@
         lib.odc_decode_threaded(decoder, self.__frame, prows_decoded, threads)
         assert prows_decoded[0] == self.nrows
 
         # Update the missing values (n.b., still sorted by type), and decode strings
 
         for i in range(len(dataframes)):
             df = dataframes[i]
-            if df.dtypes[0] == numpy.int64:
+            if df.dtypes[0] == np.int64:
                 df.mask(df == missing_integer, inplace=True)
-            elif df.dtypes[0] == numpy.double:
+            elif df.dtypes[0] == np.double:
                 df.mask(df == missing_double, inplace=True)
             else:
                 # This is a bit yucky, but I haven't found any other way to decode from b'' strings to real ones
                 # Also note, result_type added to work around bug in pandas
                 # https://github.com/pandas-dev/pandas/issues/34529
                 dataframes[i] = df.apply(
                     lambda x: x.astype("object").str.decode("utf_8_null"),
```

### Comparing `pyodc-1.1.4/codc/lib.py` & `pyodc-1.2.0/codc/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     Finds the header file associated with the ODC C API and parses it, loads the shared library,
     and patches the accessors with automatic python-C error handling.
     """
 
     __type_names = {}
 
     def __init__(self):
-
         ffi.cdef(self.__read_header())
 
         libnames = [
             "odccore",
         ]
         for env_var in ("ODC_DIR", "odc_DIR"):
             if os.environ.get(env_var):
```

### Comparing `pyodc-1.1.4/codc/processed_odc.h` & `pyodc-1.2.0/codc/processed_odc.h`

 * *Files identical despite different names*

### Comparing `pyodc-1.1.4/codc/reader.py` & `pyodc-1.2.0/codc/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 class Reader:
     """This is the main container class for reading ODBs"""
 
     __reader = None
     __frames = None
 
     def __init__(self, source, aggregated=True, max_aggregated=-1):
-
         self.__aggregated = aggregated
         self.__max_aggregated = max_aggregated
 
         reader = ffi.new("odc_reader_t**")
         if isinstance(source, io.IOBase):
             lib.odc_open_file_descriptor(reader, source.fileno())
         else:
@@ -36,15 +35,14 @@
             lib.odc_new_frame(frame, self.__reader)
             frame = ffi.gc(frame[0], lib.odc_free_frame)
             while (
                 lib.odc_next_frame_aggregated(frame, self.__max_aggregated)
                 if self.__aggregated
                 else lib.odc_next_frame(frame)
             ) != lib.ODC_ITERATION_COMPLETE:
-
                 copy_frame = ffi.new("odc_frame_t**")
                 lib.odc_copy_frame(frame, copy_frame)
                 self.__frames.append(Frame(ffi.gc(copy_frame[0], lib.odc_free_frame)))
 
         return self.__frames
 
 
@@ -52,15 +50,15 @@
     r = Reader(source, aggregated=aggregated, max_aggregated=max_aggregated)
     for f in r.frames:
         yield f.dataframe(columns)
 
 
 def _read_odb_oneshot(source, columns=None):
     reduced = pandas.concat(_read_odb_generator(source, columns), sort=False, ignore_index=True)
-    for name, data in reduced.iteritems():
+    for name, data in reduced.items():
         if data.dtype == "object":
             data.where(pandas.notnull(data), None, inplace=True)
     return reduced
 
 
 def read_odb(source, columns=None, aggregated=True, single=False, max_aggregated=-1):
     if single:
```

### Comparing `pyodc-1.1.4/pyodc/codec.py` & `pyodc-1.2.0/pyodc/codec.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,15 +138,14 @@
         return cls(column_name, value, value, data_type)
 
     def decode(self, stream):
         return struct.pack("<d", self.min).split(b"\x00", 1)[0].decode("utf-8")
 
 
 class NumericBase(Codec):
-
     _numChanges = None
     _data = None
     accepted_types = None
 
     @classmethod
     def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
         assert data_type in cls.accepted_types
@@ -159,15 +158,14 @@
         if self._numChanges is None:
             assert self._data is not None
             self._numChanges = (self._data.fillna(self.missing_value).diff() != 0).sum() - 1
         return self._numChanges
 
 
 class ConstantOrMissing(NumericBase):
-
     internal_missing_value = 0xFF
     accepted_types = (DataType.INTEGER, DataType.BITFIELD)
 
     @classmethod
     def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
         assert data.nunique() == 1 and data.hasnans
         return super().from_dataframe(column_name, data, data_type)
@@ -185,20 +183,18 @@
         else:
             return {DataType.INTEGER: int, DataType.REAL: float, DataType.DOUBLE: float, DataType.BITFIELD: int}[
                 self.type
             ](self.min)
 
 
 class RealConstantOrMissing(ConstantOrMissing):
-
     accepted_types = (DataType.DOUBLE, DataType.REAL)
 
 
 class OffsetInteger(NumericBase):
-
     internal_missing_value = None
     max_range = 0
     accepted_types = (DataType.INTEGER, DataType.BITFIELD)
 
     @staticmethod
     def _encode(stream, value):
         raise NotImplementedError
@@ -217,15 +213,14 @@
 
     def decode(self, stream):
         value = self._decode(stream)
         return None if value == self.internal_missing_value else int(value + self.min)
 
 
 class Int8(OffsetInteger):
-
     max_range = 0xFF
     accepts_missing = False
 
     @staticmethod
     def _encode(stream, value):
         stream.encodeUInt8(value)
 
@@ -237,15 +232,14 @@
 class Int8Missing(Int8):
     max_range = 0xFE
     accepts_missing = True
     internal_missing_value = 0xFF
 
 
 class Int16(OffsetInteger):
-
     max_range = 0xFFFF
     accepts_missing = False
 
     @staticmethod
     def _encode(stream, value):
         stream.encodeUInt16(value)
 
@@ -257,15 +251,14 @@
 class Int16Missing(Int16):
     max_range = 0xFFFE
     accepts_missing = True
     internal_missing_value = 0xFFFF
 
 
 class Int32(NumericBase):
-
     max_range = 0xFFFFFFFE
     accepts_missing = True
     internal_missing_value = 0x7FFFFFFF
     accepted_types = (DataType.INTEGER, DataType.BITFIELD)
 
     @classmethod
     def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
@@ -283,26 +276,24 @@
 
     def decode(self, stream):
         value = stream.readInt32()
         return None if value == self.internal_missing_value else value
 
 
 class LongReal(NumericBase):
-
     accepted_types = (DataType.DOUBLE, DataType.REAL)
 
     def encode(self, stream, value):
         stream.encodeReal64(value)
 
     def decode(self, stream):
         return stream.readReal64()
 
 
 class ShortReal(NumericBase):
-
     internal_missing_value = INTERNAL_REAL_MISSING[0]
     accepted_types = (DataType.DOUBLE, DataType.REAL)
 
     def encode(self, stream, value):
         if pd.isnull(value) is None:
             stream.encodeReal32(self.internal_missing_value)
         else:
@@ -315,31 +306,28 @@
 
 
 class ShortReal2(ShortReal):
     internal_missing_value = INTERNAL_REAL_MISSING[1]
 
 
 class Int8String(Codec):
-
     missing_value = MISSING_INTEGER
     type = DataType.STRING
     _numChanges = None
 
     def __init__(self, *args, values=None, data=None, **kwargs):
-
         self._data = data
         assert values is not None
         self.values = values
         self.value_map = {value: i for i, value in enumerate(values)}
 
         super().__init__(*args, **kwargs)
 
     @classmethod
     def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
-
         assert not data.hasnans
         assert data_type == DataType.STRING
         return cls(column_name, 0, 0, data_type, values=data.unique(), data=data)
 
     @classmethod
     def from_stream(cls, stream, column_name: str, data_type: DataType, bitfield_names, bitfield_sizes):
         has_missing, minval, maxval, missing_value = cls.read_core_header(stream)
@@ -401,15 +389,14 @@
 
     @staticmethod
     def _decode(stream):
         return stream.readUInt16()
 
 
 def select_codec(column_name: str, data: pd.Series, data_type):
-
     # If data types are not specified, determine them from the pandas Series
 
     if data_type is None:
         if data.dtype in ["{}int{}".format(s, b) for s in ("", "u") for b in (8, 16, 32, 64)]:
             data_type = DataType.INTEGER
         elif data.dtype == "float64":
             if not data.isnull().all() and all(pd.isnull(v) or float(v).is_integer() for v in data):
@@ -426,15 +413,14 @@
         raise RuntimeError("Unknown data type {} not supported".format(data.dtype))
 
     # And now the logic for selecting the codec
 
     codec_class = None
 
     if data_type in (DataType.INTEGER, DataType.BITFIELD):
-
         range = data.max() - data.min()
         has_missing = data.hasnans
 
         if data.nunique() == 1:
             if data.hasnans:
                 codec_class = ConstantOrMissing
             else:
@@ -442,39 +428,36 @@
         else:
             for c in [Int8, Int8Missing, Int16, Int16Missing, Int32]:
                 if range <= c.max_range and (c.accepts_missing or not has_missing):
                     codec_class = c
                     break
 
     elif data_type == DataType.DOUBLE:
-
         if data.nunique() == 1:
             if data.hasnans:
                 codec_class = RealConstantOrMissing
             else:
                 codec_class = Constant
         else:
             codec_class = LongReal
 
     elif data_type == DataType.REAL:
-
         if data.nunique() == 1:
             if data.hasnans:
                 codec_class = RealConstantOrMissing
             else:
                 codec_class = Constant
         elif INTERNAL_REAL_MISSING[1] in data:
             if INTERNAL_REAL_MISSING[0] in data:
                 raise ValueError("Cannot encode a float data series with both internal missing values")
             codec_class = ShortReal
         else:
             codec_class = ShortReal2
 
     elif data_type == DataType.STRING:
-
         if data.nunique() == 1 and not data.hasnans:
             codec_class = ConstantString
         elif data.nunique() <= 256:
             codec_class = Int8String
         else:
             assert data.nunique() <= 32767
             codec_class = Int16String
```

### Comparing `pyodc-1.1.4/pyodc/constants.py` & `pyodc-1.2.0/pyodc/constants.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.1.4/pyodc/encoder.py` & `pyodc-1.2.0/pyodc/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         list: The column order used for encoding as a list of column names
 
     :meta private:
     """
 
     stream_class = BigEndianStream if bigendian else LittleEndianStream
 
-    codecs = [select_codec(name, data, (types or {}).get(name, None)) for name, data in dataframe.iteritems()]
+    codecs = [select_codec(name, data, (types or {}).get(name, None)) for name, data in dataframe.items()]
 
     # If a column order has been specified, sort the codecs according to it. otherwise sort
     # the codecs for the most efficient use of the given data
 
     if column_order:
         assert len(column_order) == len(set(column_order))
         assert set(column_order) == set(c.column_name for c in codecs)
@@ -121,15 +121,14 @@
 
     # Iterate over rows
 
     last_row = None
     codec_indexes = list(zip(codecs, column_indexes))
 
     for row in dataframe.itertuples(index=False):
-
         for i, (codec, index) in enumerate(codec_indexes):
             if last_row is None or (
                 row[index] != last_row[index] and not (pd.isnull(row[index]) and pd.isnull(last_row[index]))
             ):
                 break
 
         stream.encodeMarker(i)
```

### Comparing `pyodc-1.1.4/pyodc/frame.py` & `pyodc-1.2.0/pyodc/frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
 from itertools import accumulate, chain
 
+import numpy as np
 import pandas as pd
 
 
 class MismatchedFramesError(ValueError):
     pass
 
 
@@ -74,14 +75,17 @@
             self.name = name
             self.size = size
             self.offset = offset
 
         def __eq__(self, other):
             return self.name == other.name and self.size == other.size and self.offset == other.offset
 
+        def __str__(self):
+            return f"bits(name={self.name}, size={self.size}, offset={self.offset})"
+
     def __init__(self, name, idx, dtype, datasize, bitfields):
         self.name = name
         self.dtype = dtype
         self.index = idx
         self.datasize = datasize
         self.bitfields = bitfields
 
@@ -121,15 +125,14 @@
         properties(dict): Dictionary of additional properties that can contain arbitrary metadata
         columns(list): A list of :class:`.ColumnInfo` objects describing the column structure of the frame
         nrows(int): Number of rows of data within the frame
         ncolumns(int): Number of data columns within the frame
     """
 
     def __init__(self, source):
-
         # Read marker and magic
 
         m = source.read(2)
         if len(m) == 0:
             raise EOFError()
         assert int.from_bytes(m, byteorder="big", signed=False) == NEW_HEADER
 
@@ -246,14 +249,70 @@
 
         Parameters:
             columns: List of columns to decode
 
         Returns:
             DataFrame
         """
+
+        # Are there any bitfield columns we need to consider?
+
+        original_columns = columns
+        bitfields = []
+
+        if columns is not None:
+            final_columns = set()
+            for colname in columns:
+                dotpos = colname.find(".")
+                if dotpos == -1:
+                    final_columns.add(colname)
+                else:
+                    column_name = colname[:dotpos]
+                    sp = colname[dotpos + 1 :].split("@")
+                    bitfield_name = sp[0]
+                    if len(sp) > 1:
+                        column_name += "@" + sp[1]
+                    final_columns.add(column_name)
+                    bitfields.append((bitfield_name, column_name, colname))
+            columns = list(final_columns)
+
+        df = self._dataframe_internal(columns)
+
+        # If there are any bitfields that need extraction, do it here, and remove any temporarily
+        # decoded columns as is possible
+
+        if bitfields:
+            extracted_columns = set()
+            for bitfield_name, column_name, output_name in bitfields:
+                assert df[column_name].dtype == np.int64
+                col = self.column_dict[column_name]
+                bf = next((b for b in col.bitfields if b.name == bitfield_name))
+                mask = (1 << bf.size) - 1
+                new_column = np.right_shift(df[column_name], bf.offset) & mask
+                if bf.size == 1:
+                    new_column = new_column.astype(bool)
+                df[output_name] = new_column
+                extracted_columns.add(column_name)
+
+            for column in extracted_columns:
+                if column not in original_columns:
+                    del df[column]
+
+        return df
+
+    def _dataframe_internal(self, columns=None):
+        """
+        Decodes the frame into a pandas dataframe
+
+        Parameters:
+            columns: List of columns to decode
+
+        Returns:
+            DataFrame
+        """
         # TODO: Properly skip decoding columns that aren't needed
         column_codecs = self._column_codecs
 
         self._stream.seek(self._dataStartPosition)
 
         output_cols = [[] for _ in range(self._numberOfColumns)]
 
@@ -273,15 +332,14 @@
                             raise KeyError("Ambiguous short column name '{}' requested".format(name))
                         output[name] = output_col
 
         lastDecoded = [0] * self._numberOfColumns
 
         lastStartCol = None
         for row in range(self._numberOfRows):
-
             startCol = self._stream.readMarker()
 
             if lastStartCol is None:
                 if startCol > 0:
                     for col in range(startCol):
                         output_cols[col].append(column_codecs[col].typed_missing_value)
 
@@ -304,14 +362,15 @@
         df = pd.DataFrame(output)
 
         if len(self._trailingAggregatedFrames) > 0:
             return pd.concat(
                 [df] + [f.dataframe(columns) for f in self._trailingAggregatedFrames],
                 copy=False,
                 axis=0,
+                ignore_index=True,
             )
         else:
             return df
 
     def _append(self, frame: "Frame"):
         if self.column_dict != frame.column_dict:
             raise MismatchedFramesError
```

### Comparing `pyodc-1.1.4/pyodc/reader.py` & `pyodc-1.2.0/pyodc/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     r = Reader(source, aggregated=aggregated)
     for f in r.frames:
         yield f.dataframe(columns)
 
 
 def _read_odb_oneshot(source, columns=None):
     reduced = pandas.concat(_read_odb_generator(source, columns), sort=False, ignore_index=True)
-    for name, data in reduced.iteritems():
+    for name, data in reduced.items():
         if data.dtype == "object":
             data.where(pandas.notnull(data), None, inplace=True)
     return reduced
 
 
 def read_odb(source, columns=None, aggregated=True, single=False):
     """
```

### Comparing `pyodc-1.1.4/pyodc/stream.py` & `pyodc-1.2.0/pyodc/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 That may be useful at some point
 """
 import struct
 from io import SEEK_SET
 
 
 class Stream:
-
     byteOrder = None
     floatMarker = None
     doubleMarker = None
 
     def __init__(self, f):
         self.f = f
         assert self.byteOrder in ["big", "little"]
@@ -88,18 +87,16 @@
         return struct.unpack(self.floatMarker, self.read(4))[0]
 
     def readReal64(self):
         return struct.unpack(self.doubleMarker, self.read(8))[0]
 
 
 class LittleEndianStream(Stream):
-
     byteOrder = "little"
     floatMarker = "<f"
     doubleMarker = "<d"
 
 
 class BigEndianStream(Stream):
-
     byteOrder = "big"
     floatMarker = ">f"
     doubleMarker = ">d"
```

### Comparing `pyodc-1.1.4/pyodc.egg-info/PKG-INFO` & `pyodc-1.2.0/pyodc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodc
-Version: 1.1.4
+Version: 1.2.0
 Summary: A Python interface to odc for encoding/decoding ODB-2 files.
 Home-page: https://github.com/ecmwf/pyodc
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: odc odb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyodc-1.1.4/setup.py` & `pyodc-1.2.0/setup.py`

 * *Files identical despite different names*


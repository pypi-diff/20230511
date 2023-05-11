# Comparing `tmp/wsgi_lineprof-0.8.0.tar.gz` & `tmp/wsgi_lineprof-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wsgi_lineprof-0.8.0.tar", last modified: Mon Aug 12 04:48:47 2019, max compression
+gzip compressed data, was "dist/wsgi_lineprof-0.9.0.tar", last modified: Sat Oct 12 13:34:19 2019, max compression
```

## Comparing `wsgi_lineprof-0.8.0.tar` & `wsgi_lineprof-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yusuke     (501) staff       (20)        0 2019-08-12 04:48:47.000000 wsgi_lineprof-0.8.0/
--rw-r--r--   0 yusuke     (501) staff       (20)      123 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/MANIFEST.in
--rw-r--r--   0 yusuke     (501) staff       (20)     4262 2019-08-12 04:48:47.000000 wsgi_lineprof-0.8.0/PKG-INFO
--rw-r--r--   0 yusuke     (501) staff       (20)     2328 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/README.rst
-drwxr-xr-x   0 yusuke     (501) staff       (20)        0 2019-08-12 04:48:47.000000 wsgi_lineprof-0.8.0/extensions/
--rw-r--r--   0 yusuke     (501) staff       (20)   344576 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/extensions/extensions.c
--rw-r--r--   0 yusuke     (501) staff       (20)     2967 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/extensions/extensions.pyx
--rw-r--r--   0 yusuke     (501) staff       (20)     1254 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/extensions/header.pxd
--rw-r--r--   0 yusuke     (501) staff       (20)     2089 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/extensions/timer.c
--rw-r--r--   0 yusuke     (501) staff       (20)      116 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/extensions/timer.h
--rw-r--r--   0 yusuke     (501) staff       (20)       73 2019-08-12 04:48:47.000000 wsgi_lineprof-0.8.0/setup.cfg
--rw-r--r--   0 yusuke     (501) staff       (20)     3259 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/setup.py
-drwxr-xr-x   0 yusuke     (501) staff       (20)        0 2019-08-12 04:48:47.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/
--rw-r--r--   0 yusuke     (501) staff       (20)        0 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/__init__.py
--rw-r--r--   0 yusuke     (501) staff       (20)      641 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/extensions.pyi
--rw-r--r--   0 yusuke     (501) staff       (20)     2364 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/filters.py
--rw-r--r--   0 yusuke     (501) staff       (20)     2274 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/middleware.py
--rw-r--r--   0 yusuke     (501) staff       (20)      596 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/profiler.py
--rw-r--r--   0 yusuke     (501) staff       (20)        0 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/py.typed
--rw-r--r--   0 yusuke     (501) staff       (20)     3595 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/stats.py
--rw-r--r--   0 yusuke     (501) staff       (20)       71 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/types.py
--rw-r--r--   0 yusuke     (501) staff       (20)     1552 2019-08-12 04:43:23.000000 wsgi_lineprof-0.8.0/wsgi_lineprof/writers.py
-drwxr-xr-x   0 yusuke     (501) staff       (20)        0 2019-08-12 04:48:47.000000 wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/
--rw-r--r--   0 yusuke     (501) staff       (20)     4262 2019-08-12 04:48:46.000000 wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/PKG-INFO
--rw-r--r--   0 yusuke     (501) staff       (20)      563 2019-08-12 04:48:47.000000 wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/SOURCES.txt
--rw-r--r--   0 yusuke     (501) staff       (20)        1 2019-08-12 04:48:46.000000 wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/dependency_links.txt
--rw-r--r--   0 yusuke     (501) staff       (20)      440 2019-08-12 04:48:46.000000 wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/requires.txt
--rw-r--r--   0 yusuke     (501) staff       (20)       25 2019-08-12 04:48:46.000000 wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-12 13:34:19.000000 wsgi_lineprof-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (115)      123 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (115)     4470 2019-10-12 13:34:19.000000 wsgi_lineprof-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2512 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-12 13:34:19.000000 wsgi_lineprof-0.9.0/extensions/
+-rw-r--r--   0 runner    (1001) docker     (115)   346631 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/extensions/extensions.c
+-rw-r--r--   0 runner    (1001) docker     (115)     3163 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/extensions/extensions.pyx
+-rw-r--r--   0 runner    (1001) docker     (115)     1254 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/extensions/header.pxd
+-rw-r--r--   0 runner    (1001) docker     (115)     2089 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/extensions/timer.c
+-rw-r--r--   0 runner    (1001) docker     (115)      201 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/extensions/timer.h
+-rw-r--r--   0 runner    (1001) docker     (115)       73 2019-10-12 13:34:19.000000 wsgi_lineprof-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     3286 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-12 13:34:19.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      641 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (115)     2336 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/filters.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2245 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (115)      596 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/py.typed
+-rw-r--r--   0 runner    (1001) docker     (115)     4367 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/stats.py
+-rw-r--r--   0 runner    (1001) docker     (115)       71 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/types.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1623 2019-10-12 13:34:02.000000 wsgi_lineprof-0.9.0/wsgi_lineprof/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-12 13:34:19.000000 wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     4470 2019-10-12 13:34:18.000000 wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)      563 2019-10-12 13:34:19.000000 wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-12 13:34:18.000000 wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      456 2019-10-12 13:34:18.000000 wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       25 2019-10-12 13:34:18.000000 wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/top_level.txt
```

### Comparing `wsgi_lineprof-0.8.0/PKG-INFO` & `wsgi_lineprof-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsgi_lineprof
-Version: 0.8.0
+Version: 0.9.0
 Summary: WSGI middleware for line-by-line profiling
 Home-page: https://github.com/ymyzk/wsgi_lineprof
 Author: Yusuke Miyazaki
 Author-email: miyazaki.dev@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/ymyzk/wsgi_lineprof/issues
 Project-URL: Source, https://github.com/ymyzk/wsgi_lineprof
@@ -12,14 +12,17 @@
         =============
         .. image:: https://badge.fury.io/py/wsgi-lineprof.svg
            :target: https://pypi.python.org/pypi/wsgi-lineprof/
            :alt: PyPI version
         .. image:: https://img.shields.io/pypi/pyversions/wsgi_lineprof.svg
            :target: https://pypi.python.org/pypi/wsgi-lineprof/
            :alt: PyPI Supported Python Versions
+        .. image:: https://github.com/ymyzk/tox-gh-actions/workflows/Tests/badge.svg
+           :target: https://github.com/ymyzk/tox-gh-actions/actions?workflow=Tests
+           :alt: GitHub Actions (Tests)
         .. image:: https://travis-ci.org/ymyzk/wsgi_lineprof.svg?branch=master
            :target: https://travis-ci.org/ymyzk/wsgi_lineprof
            :alt: Build Status
         .. image:: https://ci.appveyor.com/api/projects/status/cjhft69q2hq1gdoj?svg=true
            :target: https://ci.appveyor.com/project/ymyzk/wsgi-lineprof
            :alt: AppVeyor Build Status
         .. image:: https://readthedocs.org/projects/wsgi_lineprof/badge/?version=latest
@@ -89,11 +92,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Benchmark
 Provides-Extra: benchmark
+Provides-Extra: benchmark-deps
 Provides-Extra: build
-Provides-Extra: test
 Provides-Extra: docs
-Provides-Extra: benchmark-deps
+Provides-Extra: test
```

### Comparing `wsgi_lineprof-0.8.0/README.rst` & `wsgi_lineprof-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 =============
 .. image:: https://badge.fury.io/py/wsgi-lineprof.svg
    :target: https://pypi.python.org/pypi/wsgi-lineprof/
    :alt: PyPI version
 .. image:: https://img.shields.io/pypi/pyversions/wsgi_lineprof.svg
    :target: https://pypi.python.org/pypi/wsgi-lineprof/
    :alt: PyPI Supported Python Versions
+.. image:: https://github.com/ymyzk/tox-gh-actions/workflows/Tests/badge.svg
+   :target: https://github.com/ymyzk/tox-gh-actions/actions?workflow=Tests
+   :alt: GitHub Actions (Tests)
 .. image:: https://travis-ci.org/ymyzk/wsgi_lineprof.svg?branch=master
    :target: https://travis-ci.org/ymyzk/wsgi_lineprof
    :alt: Build Status
 .. image:: https://ci.appveyor.com/api/projects/status/cjhft69q2hq1gdoj?svg=true
    :target: https://ci.appveyor.com/project/ymyzk/wsgi-lineprof
    :alt: AppVeyor Build Status
 .. image:: https://readthedocs.org/projects/wsgi_lineprof/badge/?version=latest
```

### Comparing `wsgi_lineprof-0.8.0/extensions/extensions.c` & `wsgi_lineprof-0.9.0/extensions/extensions.c`

 * *Files 2% similar despite different names*

```diff
@@ -611,15 +611,14 @@
 
 #define __PYX_HAVE__extensions
 #define __PYX_HAVE_API__extensions
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "pythread.h"
-#include <stdint.h>
 #include "frameobject.h"
 #include "timer.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
@@ -829,75 +828,84 @@
   "extensions/extensions.pyx",
   "stringsource",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
 
+/* "extensions.pyx":13
+ * # Old Windows compilers don't support this.
+ * # from libc.stdint cimport uint64_t
+ * ctypedef unsigned long long uint64_t             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+typedef unsigned PY_LONG_LONG __pyx_t_10extensions_uint64_t;
+
 /*--- Type declarations ---*/
 struct __pyx_obj_10extensions_LineProfiler;
 struct __pyx_obj_10extensions_LineTiming;
 struct __pyx_obj_10extensions_LastTime;
 
-/* "extensions.pyx":16
+/* "extensions.pyx":22
  * 
  * 
  * cdef class LineProfiler:             # <<<<<<<<<<<<<<
  *     cdef public dict results
  *     cdef public dict last_time
  */
 struct __pyx_obj_10extensions_LineProfiler {
   PyObject_HEAD
   PyObject *results;
   PyObject *last_time;
 };
 
 
-/* "extensions.pyx":49
+/* "extensions.pyx":55
  * 
  * 
  * cdef class LineTiming:             # <<<<<<<<<<<<<<
  *     cdef public object code
  *     cdef public int lineno
  */
 struct __pyx_obj_10extensions_LineTiming {
   PyObject_HEAD
   struct __pyx_vtabstruct_10extensions_LineTiming *__pyx_vtab;
   PyObject *code;
   int lineno;
-  uint64_t total_time;
+  __pyx_t_10extensions_uint64_t total_time;
   long n_hits;
 };
 
 
-/* "extensions.pyx":73
+/* "extensions.pyx":79
  * 
  * 
  * cdef class LastTime:             # <<<<<<<<<<<<<<
  *     cdef int f_lineno
  *     cdef uint64_t time
  */
 struct __pyx_obj_10extensions_LastTime {
   PyObject_HEAD
   int f_lineno;
-  uint64_t time;
+  __pyx_t_10extensions_uint64_t time;
 };
 
 
 
-/* "extensions.pyx":49
+/* "extensions.pyx":55
  * 
  * 
  * cdef class LineTiming:             # <<<<<<<<<<<<<<
  *     cdef public object code
  *     cdef public int lineno
  */
 
 struct __pyx_vtabstruct_10extensions_LineTiming {
-  PyObject *(*hit)(struct __pyx_obj_10extensions_LineTiming *, uint64_t);
+  PyObject *(*hit)(struct __pyx_obj_10extensions_LineTiming *, __pyx_t_10extensions_uint64_t);
 };
 static struct __pyx_vtabstruct_10extensions_LineTiming *__pyx_vtabptr_10extensions_LineTiming;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
@@ -1277,24 +1285,24 @@
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint64_t(uint64_t value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_PY_LONG_LONG(unsigned PY_LONG_LONG value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *);
+static CYTHON_INLINE unsigned PY_LONG_LONG __Pyx_PyInt_As_unsigned_PY_LONG_LONG(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
@@ -1307,15 +1315,15 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static PyObject *__pyx_f_10extensions_10LineTiming_hit(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, uint64_t __pyx_v_dt); /* proto*/
+static PyObject *__pyx_f_10extensions_10LineTiming_hit(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, __pyx_t_10extensions_uint64_t __pyx_v_dt); /* proto*/
 
 /* Module declarations from 'cpython.version' */
 
 /* Module declarations from '__builtin__' */
 
 /* Module declarations from 'cpython.type' */
 static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
@@ -1392,16 +1400,14 @@
 
 /* Module declarations from 'cpython.bytes' */
 
 /* Module declarations from 'cpython.pycapsule' */
 
 /* Module declarations from 'cpython' */
 
-/* Module declarations from 'libc.stdint' */
-
 /* Module declarations from 'header' */
 
 /* Module declarations from 'extensions' */
 static PyTypeObject *__pyx_ptype_10extensions_LineProfiler = 0;
 static PyTypeObject *__pyx_ptype_10extensions_LineTiming = 0;
 static PyTypeObject *__pyx_ptype_10extensions_LastTime = 0;
 static int __pyx_f_10extensions_python_trace_callback(PyObject *, PyFrameObject *, int, PyObject *); /*proto*/
@@ -1525,15 +1531,15 @@
 static int __pyx_pf_10extensions_10LineTiming_6lineno_2__set__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10extensions_10LineTiming_10total_time___get__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self); /* proto */
 static int __pyx_pf_10extensions_10LineTiming_10total_time_2__set__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10extensions_10LineTiming_6n_hits___get__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self); /* proto */
 static int __pyx_pf_10extensions_10LineTiming_6n_hits_2__set__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10extensions_10LineTiming_6__reduce_cython__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10extensions_10LineTiming_8__setstate_cython__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_10extensions_8LastTime___cinit__(struct __pyx_obj_10extensions_LastTime *__pyx_v_self, int __pyx_v_f_lineno, uint64_t __pyx_v_time); /* proto */
+static int __pyx_pf_10extensions_8LastTime___cinit__(struct __pyx_obj_10extensions_LastTime *__pyx_v_self, int __pyx_v_f_lineno, __pyx_t_10extensions_uint64_t __pyx_v_time); /* proto */
 static PyObject *__pyx_pf_10extensions_8LastTime_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10extensions_LastTime *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10extensions_8LastTime_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10extensions_LastTime *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10extensions___pyx_unpickle_LineProfiler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10extensions_2__pyx_unpickle_LineTiming(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_10extensions_LineProfiler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10extensions_LineTiming(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10extensions_LastTime(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -1546,15 +1552,15 @@
 static PyObject *__pyx_codeobj__3;
 static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__5;
 static PyObject *__pyx_codeobj__7;
 static PyObject *__pyx_codeobj__9;
 /* Late includes */
 
-/* "extensions.pyx":20
+/* "extensions.pyx":26
  *     cdef public dict last_time
  * 
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.results = {}
  *         self.last_time = {}
  */
 
@@ -1576,45 +1582,45 @@
 
 static int __pyx_pf_10extensions_12LineProfiler___init__(struct __pyx_obj_10extensions_LineProfiler *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "extensions.pyx":21
+  /* "extensions.pyx":27
  * 
  *     def __init__(self):
  *         self.results = {}             # <<<<<<<<<<<<<<
  *         self.last_time = {}
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->results);
   __Pyx_DECREF(__pyx_v_self->results);
   __pyx_v_self->results = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "extensions.pyx":22
+  /* "extensions.pyx":28
  *     def __init__(self):
  *         self.results = {}
  *         self.last_time = {}             # <<<<<<<<<<<<<<
  * 
  *     def enable(self):
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->last_time);
   __Pyx_DECREF(__pyx_v_self->last_time);
   __pyx_v_self->last_time = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "extensions.pyx":20
+  /* "extensions.pyx":26
  *     cdef public dict last_time
  * 
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.results = {}
  *         self.last_time = {}
  */
 
@@ -1626,15 +1632,15 @@
   __Pyx_AddTraceback("extensions.LineProfiler.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":24
+/* "extensions.pyx":30
  *         self.last_time = {}
  * 
  *     def enable(self):             # <<<<<<<<<<<<<<
  *         PyEval_SetTrace(python_trace_callback, self)
  * 
  */
 
@@ -1652,39 +1658,39 @@
 }
 
 static PyObject *__pyx_pf_10extensions_12LineProfiler_2enable(struct __pyx_obj_10extensions_LineProfiler *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("enable", 0);
 
-  /* "extensions.pyx":25
+  /* "extensions.pyx":31
  * 
  *     def enable(self):
  *         PyEval_SetTrace(python_trace_callback, self)             # <<<<<<<<<<<<<<
  * 
  *     def disable(self):
  */
   PyEval_SetTrace(__pyx_f_10extensions_python_trace_callback, ((PyObject *)__pyx_v_self));
 
-  /* "extensions.pyx":24
+  /* "extensions.pyx":30
  *         self.last_time = {}
  * 
  *     def enable(self):             # <<<<<<<<<<<<<<
  *         PyEval_SetTrace(python_trace_callback, self)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":27
+/* "extensions.pyx":33
  *         PyEval_SetTrace(python_trace_callback, self)
  * 
  *     def disable(self):             # <<<<<<<<<<<<<<
  *         PyEval_SetTrace(NULL, <object>NULL)
  * 
  */
 
@@ -1702,39 +1708,39 @@
 }
 
 static PyObject *__pyx_pf_10extensions_12LineProfiler_4disable(CYTHON_UNUSED struct __pyx_obj_10extensions_LineProfiler *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("disable", 0);
 
-  /* "extensions.pyx":28
+  /* "extensions.pyx":34
  * 
  *     def disable(self):
  *         PyEval_SetTrace(NULL, <object>NULL)             # <<<<<<<<<<<<<<
  * 
  *     def reset(self):
  */
   PyEval_SetTrace(NULL, ((PyObject *)NULL));
 
-  /* "extensions.pyx":27
+  /* "extensions.pyx":33
  *         PyEval_SetTrace(python_trace_callback, self)
  * 
  *     def disable(self):             # <<<<<<<<<<<<<<
  *         PyEval_SetTrace(NULL, <object>NULL)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":30
+/* "extensions.pyx":36
  *         PyEval_SetTrace(NULL, <object>NULL)
  * 
  *     def reset(self):             # <<<<<<<<<<<<<<
  *         self.results = {}
  *         self.last_time = {}
  */
 
@@ -1753,45 +1759,45 @@
 
 static PyObject *__pyx_pf_10extensions_12LineProfiler_6reset(struct __pyx_obj_10extensions_LineProfiler *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("reset", 0);
 
-  /* "extensions.pyx":31
+  /* "extensions.pyx":37
  * 
  *     def reset(self):
  *         self.results = {}             # <<<<<<<<<<<<<<
  *         self.last_time = {}
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->results);
   __Pyx_DECREF(__pyx_v_self->results);
   __pyx_v_self->results = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "extensions.pyx":32
+  /* "extensions.pyx":38
  *     def reset(self):
  *         self.results = {}
  *         self.last_time = {}             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->last_time);
   __Pyx_DECREF(__pyx_v_self->last_time);
   __pyx_v_self->last_time = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "extensions.pyx":30
+  /* "extensions.pyx":36
  *         PyEval_SetTrace(NULL, <object>NULL)
  * 
  *     def reset(self):             # <<<<<<<<<<<<<<
  *         self.results = {}
  *         self.last_time = {}
  */
 
@@ -1804,15 +1810,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":35
+/* "extensions.pyx":41
  * 
  *     @staticmethod
  *     def get_timer():             # <<<<<<<<<<<<<<
  *         return hpTimer()
  * 
  */
 
@@ -1835,29 +1841,29 @@
 
 static PyObject *__pyx_pf_10extensions_12LineProfiler_8get_timer(void) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("get_timer", 0);
 
-  /* "extensions.pyx":36
+  /* "extensions.pyx":42
  *     @staticmethod
  *     def get_timer():
  *         return hpTimer()             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint64_t(hpTimer()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(hpTimer()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "extensions.pyx":35
+  /* "extensions.pyx":41
  * 
  *     @staticmethod
  *     def get_timer():             # <<<<<<<<<<<<<<
  *         return hpTimer()
  * 
  */
 
@@ -1868,15 +1874,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":39
+/* "extensions.pyx":45
  * 
  *     @staticmethod
  *     def get_timer_implementation():             # <<<<<<<<<<<<<<
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):
  *             return HP_TIMER_IMPLEMENTATION
  */
 
@@ -1901,66 +1907,66 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("get_timer_implementation", 0);
 
-  /* "extensions.pyx":40
+  /* "extensions.pyx":46
  *     @staticmethod
  *     def get_timer_implementation():
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):             # <<<<<<<<<<<<<<
  *             return HP_TIMER_IMPLEMENTATION
  *         return HP_TIMER_IMPLEMENTATION.decode("ascii")
  */
-  __pyx_t_1 = __Pyx_PyObject_FromString(HP_TIMER_IMPLEMENTATION); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_FromString(HP_TIMER_IMPLEMENTATION); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyString_Check(__pyx_t_1); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "extensions.pyx":41
+    /* "extensions.pyx":47
  *     def get_timer_implementation():
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):
  *             return HP_TIMER_IMPLEMENTATION             # <<<<<<<<<<<<<<
  *         return HP_TIMER_IMPLEMENTATION.decode("ascii")
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_FromString(HP_TIMER_IMPLEMENTATION); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FromString(HP_TIMER_IMPLEMENTATION); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "extensions.pyx":40
+    /* "extensions.pyx":46
  *     @staticmethod
  *     def get_timer_implementation():
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):             # <<<<<<<<<<<<<<
  *             return HP_TIMER_IMPLEMENTATION
  *         return HP_TIMER_IMPLEMENTATION.decode("ascii")
  */
   }
 
-  /* "extensions.pyx":42
+  /* "extensions.pyx":48
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):
  *             return HP_TIMER_IMPLEMENTATION
  *         return HP_TIMER_IMPLEMENTATION.decode("ascii")             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_c_string(HP_TIMER_IMPLEMENTATION, 0, strlen(HP_TIMER_IMPLEMENTATION), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_c_string(HP_TIMER_IMPLEMENTATION, 0, strlen(HP_TIMER_IMPLEMENTATION), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "extensions.pyx":39
+  /* "extensions.pyx":45
  * 
  *     @staticmethod
  *     def get_timer_implementation():             # <<<<<<<<<<<<<<
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):
  *             return HP_TIMER_IMPLEMENTATION
  */
 
@@ -1971,15 +1977,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":45
+/* "extensions.pyx":51
  * 
  *     @staticmethod
  *     def get_unit():             # <<<<<<<<<<<<<<
  *         return hpTimerUnit()
  * 
  */
 
@@ -2002,29 +2008,29 @@
 
 static PyObject *__pyx_pf_10extensions_12LineProfiler_12get_unit(void) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("get_unit", 0);
 
-  /* "extensions.pyx":46
+  /* "extensions.pyx":52
  *     @staticmethod
  *     def get_unit():
  *         return hpTimerUnit()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(hpTimerUnit()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(hpTimerUnit()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "extensions.pyx":45
+  /* "extensions.pyx":51
  * 
  *     @staticmethod
  *     def get_unit():             # <<<<<<<<<<<<<<
  *         return hpTimerUnit()
  * 
  */
 
@@ -2035,15 +2041,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":17
+/* "extensions.pyx":23
  * 
  * cdef class LineProfiler:
  *     cdef public dict results             # <<<<<<<<<<<<<<
  *     cdef public dict last_time
  * 
  */
 
@@ -2090,15 +2096,15 @@
 }
 
 static int __pyx_pf_10extensions_12LineProfiler_7results_2__set__(struct __pyx_obj_10extensions_LineProfiler *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyDict_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 23, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->results);
   __Pyx_DECREF(__pyx_v_self->results);
   __pyx_v_self->results = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -2140,15 +2146,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":18
+/* "extensions.pyx":24
  * cdef class LineProfiler:
  *     cdef public dict results
  *     cdef public dict last_time             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self):
  */
 
@@ -2195,15 +2201,15 @@
 }
 
 static int __pyx_pf_10extensions_12LineProfiler_9last_time_2__set__(struct __pyx_obj_10extensions_LineProfiler *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyDict_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 24, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->last_time);
   __Pyx_DECREF(__pyx_v_self->last_time);
   __pyx_v_self->last_time = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -2546,15 +2552,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":55
+/* "extensions.pyx":61
  *     cdef public long n_hits
  * 
  *     def __init__(self, object code, int lineno):             # <<<<<<<<<<<<<<
  *         self.code = code
  *         self.lineno = lineno
  */
 
@@ -2585,32 +2591,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_code)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lineno)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 55, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 61, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 55, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 61, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_code = values[0];
-    __pyx_v_lineno = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L3_error)
+    __pyx_v_lineno = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 55, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 61, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("extensions.LineTiming.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10extensions_10LineTiming___init__(((struct __pyx_obj_10extensions_LineTiming *)__pyx_v_self), __pyx_v_code, __pyx_v_lineno);
 
@@ -2620,115 +2626,115 @@
 }
 
 static int __pyx_pf_10extensions_10LineTiming___init__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v_code, int __pyx_v_lineno) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "extensions.pyx":56
+  /* "extensions.pyx":62
  * 
  *     def __init__(self, object code, int lineno):
  *         self.code = code             # <<<<<<<<<<<<<<
  *         self.lineno = lineno
  *         self.total_time = 0
  */
   __Pyx_INCREF(__pyx_v_code);
   __Pyx_GIVEREF(__pyx_v_code);
   __Pyx_GOTREF(__pyx_v_self->code);
   __Pyx_DECREF(__pyx_v_self->code);
   __pyx_v_self->code = __pyx_v_code;
 
-  /* "extensions.pyx":57
+  /* "extensions.pyx":63
  *     def __init__(self, object code, int lineno):
  *         self.code = code
  *         self.lineno = lineno             # <<<<<<<<<<<<<<
  *         self.total_time = 0
  *         self.n_hits = 0
  */
   __pyx_v_self->lineno = __pyx_v_lineno;
 
-  /* "extensions.pyx":58
+  /* "extensions.pyx":64
  *         self.code = code
  *         self.lineno = lineno
  *         self.total_time = 0             # <<<<<<<<<<<<<<
  *         self.n_hits = 0
  * 
  */
   __pyx_v_self->total_time = 0;
 
-  /* "extensions.pyx":59
+  /* "extensions.pyx":65
  *         self.lineno = lineno
  *         self.total_time = 0
  *         self.n_hits = 0             # <<<<<<<<<<<<<<
  * 
  *     cdef hit(self, uint64_t dt):
  */
   __pyx_v_self->n_hits = 0;
 
-  /* "extensions.pyx":55
+  /* "extensions.pyx":61
  *     cdef public long n_hits
  * 
  *     def __init__(self, object code, int lineno):             # <<<<<<<<<<<<<<
  *         self.code = code
  *         self.lineno = lineno
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":61
+/* "extensions.pyx":67
  *         self.n_hits = 0
  * 
  *     cdef hit(self, uint64_t dt):             # <<<<<<<<<<<<<<
  *             self.n_hits += 1
  *             self.total_time += dt
  */
 
-static PyObject *__pyx_f_10extensions_10LineTiming_hit(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, uint64_t __pyx_v_dt) {
+static PyObject *__pyx_f_10extensions_10LineTiming_hit(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, __pyx_t_10extensions_uint64_t __pyx_v_dt) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("hit", 0);
 
-  /* "extensions.pyx":62
+  /* "extensions.pyx":68
  * 
  *     cdef hit(self, uint64_t dt):
  *             self.n_hits += 1             # <<<<<<<<<<<<<<
  *             self.total_time += dt
  * 
  */
   __pyx_v_self->n_hits = (__pyx_v_self->n_hits + 1);
 
-  /* "extensions.pyx":63
+  /* "extensions.pyx":69
  *     cdef hit(self, uint64_t dt):
  *             self.n_hits += 1
  *             self.total_time += dt             # <<<<<<<<<<<<<<
  * 
  *     def as_tuple(self):
  */
   __pyx_v_self->total_time = (__pyx_v_self->total_time + __pyx_v_dt);
 
-  /* "extensions.pyx":61
+  /* "extensions.pyx":67
  *         self.n_hits = 0
  * 
  *     cdef hit(self, uint64_t dt):             # <<<<<<<<<<<<<<
  *             self.n_hits += 1
  *             self.total_time += dt
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":65
+/* "extensions.pyx":71
  *             self.total_time += dt
  * 
  *     def as_tuple(self):             # <<<<<<<<<<<<<<
  *         return self.lineno, self.n_hits, self.total_time
  * 
  */
 
@@ -2750,44 +2756,44 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("as_tuple", 0);
 
-  /* "extensions.pyx":66
+  /* "extensions.pyx":72
  * 
  *     def as_tuple(self):
  *         return self.lineno, self.n_hits, self.total_time             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_self->n_hits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_self->n_hits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_self->total_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_self->total_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "extensions.pyx":65
+  /* "extensions.pyx":71
  *             self.total_time += dt
  * 
  *     def as_tuple(self):             # <<<<<<<<<<<<<<
  *         return self.lineno, self.n_hits, self.total_time
  * 
  */
 
@@ -2801,15 +2807,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":68
+/* "extensions.pyx":74
  *         return self.lineno, self.n_hits, self.total_time
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return '<LineTiming for %r lineno: %r n_hits: %r total_time: %r>' % (
  *             self.code, self.lineno, self.n_hits, <long>self.total_time)
  */
 
@@ -2831,66 +2837,66 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "extensions.pyx":69
+  /* "extensions.pyx":75
  * 
  *     def __repr__(self):
  *         return '<LineTiming for %r lineno: %r n_hits: %r total_time: %r>' % (             # <<<<<<<<<<<<<<
  *             self.code, self.lineno, self.n_hits, <long>self.total_time)
  * 
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "extensions.pyx":70
+  /* "extensions.pyx":76
  *     def __repr__(self):
  *         return '<LineTiming for %r lineno: %r n_hits: %r total_time: %r>' % (
  *             self.code, self.lineno, self.n_hits, <long>self.total_time)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_self->n_hits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_self->n_hits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_long(((long)__pyx_v_self->total_time)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long(((long)__pyx_v_self->total_time)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_self->code);
   __Pyx_GIVEREF(__pyx_v_self->code);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_self->code);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "extensions.pyx":69
+  /* "extensions.pyx":75
  * 
  *     def __repr__(self):
  *         return '<LineTiming for %r lineno: %r n_hits: %r total_time: %r>' % (             # <<<<<<<<<<<<<<
  *             self.code, self.lineno, self.n_hits, <long>self.total_time)
  * 
  */
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_LineTiming_for_r_lineno_r_n_hit, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_LineTiming_for_r_lineno_r_n_hit, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "extensions.pyx":68
+  /* "extensions.pyx":74
  *         return self.lineno, self.n_hits, self.total_time
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return '<LineTiming for %r lineno: %r n_hits: %r total_time: %r>' % (
  *             self.code, self.lineno, self.n_hits, <long>self.total_time)
  */
 
@@ -2904,15 +2910,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":50
+/* "extensions.pyx":56
  * 
  * cdef class LineTiming:
  *     cdef public object code             # <<<<<<<<<<<<<<
  *     cdef public int lineno
  *     cdef public uint64_t total_time
  */
 
@@ -2999,15 +3005,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":51
+/* "extensions.pyx":57
  * cdef class LineTiming:
  *     cdef public object code
  *     cdef public int lineno             # <<<<<<<<<<<<<<
  *     cdef public uint64_t total_time
  *     cdef public long n_hits
  */
 
@@ -3026,15 +3032,15 @@
 
 static PyObject *__pyx_pf_10extensions_10LineTiming_6lineno___get__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3061,29 +3067,29 @@
 }
 
 static int __pyx_pf_10extensions_10LineTiming_6lineno_2__set__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
   __pyx_v_self->lineno = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("extensions.LineTiming.lineno.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":52
+/* "extensions.pyx":58
  *     cdef public object code
  *     cdef public int lineno
  *     cdef public uint64_t total_time             # <<<<<<<<<<<<<<
  *     cdef public long n_hits
  * 
  */
 
@@ -3102,15 +3108,15 @@
 
 static PyObject *__pyx_pf_10extensions_10LineTiming_10total_time___get__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_self->total_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_self->total_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3135,31 +3141,31 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_10extensions_10LineTiming_10total_time_2__set__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  uint64_t __pyx_t_1;
+  __pyx_t_10extensions_uint64_t __pyx_t_1;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_uint64_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(__pyx_v_value); if (unlikely((__pyx_t_1 == (unsigned PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
   __pyx_v_self->total_time = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("extensions.LineTiming.total_time.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":53
+/* "extensions.pyx":59
  *     cdef public int lineno
  *     cdef public uint64_t total_time
  *     cdef public long n_hits             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, object code, int lineno):
  */
 
@@ -3178,15 +3184,15 @@
 
 static PyObject *__pyx_pf_10extensions_10LineTiming_6n_hits___get__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->n_hits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->n_hits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3213,15 +3219,15 @@
 }
 
 static int __pyx_pf_10extensions_10LineTiming_6n_hits_2__set__(struct __pyx_obj_10extensions_LineTiming *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   long __pyx_t_1;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_long(__pyx_v_value); if (unlikely((__pyx_t_1 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_long(__pyx_v_value); if (unlikely((__pyx_t_1 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 59, __pyx_L1_error)
   __pyx_v_self->n_hits = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("extensions.LineTiming.n_hits.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -3271,15 +3277,15 @@
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_self->n_hits); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_self->total_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_self->total_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_self->code);
   __Pyx_GIVEREF(__pyx_v_self->code);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_self->code);
   __Pyx_GIVEREF(__pyx_t_1);
@@ -3531,27 +3537,27 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":77
+/* "extensions.pyx":83
  *     cdef uint64_t time
  * 
  *     def __cinit__(self, int f_lineno, uint64_t time):             # <<<<<<<<<<<<<<
  *         self.f_lineno = f_lineno
  *         self.time = time
  */
 
 /* Python wrapper */
 static int __pyx_pw_10extensions_8LastTime_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_10extensions_8LastTime_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_f_lineno;
-  uint64_t __pyx_v_time;
+  __pyx_t_10extensions_uint64_t __pyx_v_time;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_f_lineno,&__pyx_n_s_time,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -3570,68 +3576,68 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_f_lineno)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_time)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 77, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 83, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 77, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_f_lineno = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_f_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L3_error)
-    __pyx_v_time = __Pyx_PyInt_As_uint64_t(values[1]); if (unlikely((__pyx_v_time == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L3_error)
+    __pyx_v_f_lineno = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_f_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L3_error)
+    __pyx_v_time = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(values[1]); if (unlikely((__pyx_v_time == (unsigned PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 77, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 83, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("extensions.LastTime.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10extensions_8LastTime___cinit__(((struct __pyx_obj_10extensions_LastTime *)__pyx_v_self), __pyx_v_f_lineno, __pyx_v_time);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_10extensions_8LastTime___cinit__(struct __pyx_obj_10extensions_LastTime *__pyx_v_self, int __pyx_v_f_lineno, uint64_t __pyx_v_time) {
+static int __pyx_pf_10extensions_8LastTime___cinit__(struct __pyx_obj_10extensions_LastTime *__pyx_v_self, int __pyx_v_f_lineno, __pyx_t_10extensions_uint64_t __pyx_v_time) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "extensions.pyx":78
+  /* "extensions.pyx":84
  * 
  *     def __cinit__(self, int f_lineno, uint64_t time):
  *         self.f_lineno = f_lineno             # <<<<<<<<<<<<<<
  *         self.time = time
  * 
  */
   __pyx_v_self->f_lineno = __pyx_v_f_lineno;
 
-  /* "extensions.pyx":79
+  /* "extensions.pyx":85
  *     def __cinit__(self, int f_lineno, uint64_t time):
  *         self.f_lineno = f_lineno
  *         self.time = time             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_self->time = __pyx_v_time;
 
-  /* "extensions.pyx":77
+  /* "extensions.pyx":83
  *     cdef uint64_t time
  * 
  *     def __cinit__(self, int f_lineno, uint64_t time):             # <<<<<<<<<<<<<<
  *         self.f_lineno = f_lineno
  *         self.time = time
  */
 
@@ -3744,15 +3750,15 @@
   __Pyx_AddTraceback("extensions.LastTime.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "extensions.pyx":82
+/* "extensions.pyx":88
  * 
  * 
  * cdef int python_trace_callback(object self_, PyFrameObject *py_frame, int what,             # <<<<<<<<<<<<<<
  *                                PyObject *arg):
  *     cdef LineProfiler self
  */
 
@@ -3760,27 +3766,27 @@
   struct __pyx_obj_10extensions_LineProfiler *__pyx_v_self = 0;
   PyObject *__pyx_v_results = 0;
   PyObject *__pyx_v_result_code = 0;
   PyObject *__pyx_v_last_time = 0;
   struct __pyx_obj_10extensions_LineTiming *__pyx_v_entry = 0;
   struct __pyx_obj_10extensions_LastTime *__pyx_v_old = 0;
   PyObject *__pyx_v_code = 0;
-  uint64_t __pyx_v_time;
+  __pyx_t_10extensions_uint64_t __pyx_v_time;
   int __pyx_v_lineno;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("python_trace_callback", 0);
 
-  /* "extensions.pyx":94
+  /* "extensions.pyx":100
  *     cdef int lineno
  * 
  *     if what != PyTrace_LINE and what != PyTrace_RETURN:             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
   __pyx_t_2 = ((__pyx_v_what != PyTrace_LINE) != 0);
@@ -3790,381 +3796,381 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_what != PyTrace_RETURN) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "extensions.pyx":95
+    /* "extensions.pyx":101
  * 
  *     if what != PyTrace_LINE and what != PyTrace_RETURN:
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     time = hpTimer()
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "extensions.pyx":94
+    /* "extensions.pyx":100
  *     cdef int lineno
  * 
  *     if what != PyTrace_LINE and what != PyTrace_RETURN:             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
   }
 
-  /* "extensions.pyx":97
+  /* "extensions.pyx":103
  *         return 0
  * 
  *     time = hpTimer()             # <<<<<<<<<<<<<<
  * 
  *     self = <LineProfiler>self_
  */
   __pyx_v_time = hpTimer();
 
-  /* "extensions.pyx":99
+  /* "extensions.pyx":105
  *     time = hpTimer()
  * 
  *     self = <LineProfiler>self_             # <<<<<<<<<<<<<<
  *     last_time = self.last_time
  *     results = self.results
  */
   __pyx_t_3 = __pyx_v_self_;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_self = ((struct __pyx_obj_10extensions_LineProfiler *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "extensions.pyx":100
+  /* "extensions.pyx":106
  * 
  *     self = <LineProfiler>self_
  *     last_time = self.last_time             # <<<<<<<<<<<<<<
  *     results = self.results
  *     code = <object>py_frame.f_code
  */
   __pyx_t_3 = __pyx_v_self->last_time;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_last_time = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "extensions.pyx":101
+  /* "extensions.pyx":107
  *     self = <LineProfiler>self_
  *     last_time = self.last_time
  *     results = self.results             # <<<<<<<<<<<<<<
  *     code = <object>py_frame.f_code
  * 
  */
   __pyx_t_3 = __pyx_v_self->results;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_results = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "extensions.pyx":102
+  /* "extensions.pyx":108
  *     last_time = self.last_time
  *     results = self.results
  *     code = <object>py_frame.f_code             # <<<<<<<<<<<<<<
  * 
  *     if code not in results:
  */
   __pyx_t_3 = ((PyObject *)__pyx_v_py_frame->f_code);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_code = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "extensions.pyx":104
+  /* "extensions.pyx":110
  *     code = <object>py_frame.f_code
  * 
  *     if code not in results:             # <<<<<<<<<<<<<<
  *         results[code] = {}
  * 
  */
   if (unlikely(__pyx_v_results == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 104, __pyx_L1_error)
+    __PYX_ERR(0, 110, __pyx_L1_error)
   }
-  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_code, __pyx_v_results, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_code, __pyx_v_results, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "extensions.pyx":105
+    /* "extensions.pyx":111
  * 
  *     if code not in results:
  *         results[code] = {}             # <<<<<<<<<<<<<<
  * 
  *     if code in last_time:
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (unlikely(__pyx_v_results == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 105, __pyx_L1_error)
+      __PYX_ERR(0, 111, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__pyx_v_results, __pyx_v_code, __pyx_t_3) < 0)) __PYX_ERR(0, 105, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_results, __pyx_v_code, __pyx_t_3) < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "extensions.pyx":104
+    /* "extensions.pyx":110
  *     code = <object>py_frame.f_code
  * 
  *     if code not in results:             # <<<<<<<<<<<<<<
  *         results[code] = {}
  * 
  */
   }
 
-  /* "extensions.pyx":107
+  /* "extensions.pyx":113
  *         results[code] = {}
  * 
  *     if code in last_time:             # <<<<<<<<<<<<<<
  *         result_code = results[code]
  *         old = last_time[code]
  */
   if (unlikely(__pyx_v_last_time == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 107, __pyx_L1_error)
+    __PYX_ERR(0, 113, __pyx_L1_error)
   }
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_v_code, __pyx_v_last_time, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_v_code, __pyx_v_last_time, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "extensions.pyx":108
+    /* "extensions.pyx":114
  * 
  *     if code in last_time:
  *         result_code = results[code]             # <<<<<<<<<<<<<<
  *         old = last_time[code]
  *         lineno = old.f_lineno
  */
     if (unlikely(__pyx_v_results == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 108, __pyx_L1_error)
+      __PYX_ERR(0, 114, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_results, __pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_results, __pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyDict_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 108, __pyx_L1_error)
+    if (!(likely(PyDict_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 114, __pyx_L1_error)
     __pyx_v_result_code = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "extensions.pyx":109
+    /* "extensions.pyx":115
  *     if code in last_time:
  *         result_code = results[code]
  *         old = last_time[code]             # <<<<<<<<<<<<<<
  *         lineno = old.f_lineno
  * 
  */
     if (unlikely(__pyx_v_last_time == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 109, __pyx_L1_error)
+      __PYX_ERR(0, 115, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_last_time, __pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_last_time, __pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_10extensions_LastTime))))) __PYX_ERR(0, 109, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_10extensions_LastTime))))) __PYX_ERR(0, 115, __pyx_L1_error)
     __pyx_v_old = ((struct __pyx_obj_10extensions_LastTime *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "extensions.pyx":110
+    /* "extensions.pyx":116
  *         result_code = results[code]
  *         old = last_time[code]
  *         lineno = old.f_lineno             # <<<<<<<<<<<<<<
  * 
  *         if lineno not in result_code:
  */
     __pyx_t_4 = __pyx_v_old->f_lineno;
     __pyx_v_lineno = __pyx_t_4;
 
-    /* "extensions.pyx":112
+    /* "extensions.pyx":118
  *         lineno = old.f_lineno
  * 
  *         if lineno not in result_code:             # <<<<<<<<<<<<<<
  *             result_code[lineno] = entry = LineTiming(code, lineno)
  *         else:
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (unlikely(__pyx_v_result_code == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 112, __pyx_L1_error)
+      __PYX_ERR(0, 118, __pyx_L1_error)
     }
-    __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_t_3, __pyx_v_result_code, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_t_3, __pyx_v_result_code, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "extensions.pyx":113
+      /* "extensions.pyx":119
  * 
  *         if lineno not in result_code:
  *             result_code[lineno] = entry = LineTiming(code, lineno)             # <<<<<<<<<<<<<<
  *         else:
  *             entry = result_code[lineno]
  */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_v_code);
       __Pyx_GIVEREF(__pyx_v_code);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_code);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10extensions_LineTiming), __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10extensions_LineTiming), __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (unlikely(__pyx_v_result_code == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 113, __pyx_L1_error)
+        __PYX_ERR(0, 119, __pyx_L1_error)
       }
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(PyDict_SetItem(__pyx_v_result_code, __pyx_t_5, __pyx_t_3) < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_result_code, __pyx_t_5, __pyx_t_3) < 0)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_3);
       __pyx_v_entry = ((struct __pyx_obj_10extensions_LineTiming *)__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "extensions.pyx":112
+      /* "extensions.pyx":118
  *         lineno = old.f_lineno
  * 
  *         if lineno not in result_code:             # <<<<<<<<<<<<<<
  *             result_code[lineno] = entry = LineTiming(code, lineno)
  *         else:
  */
       goto __pyx_L8;
     }
 
-    /* "extensions.pyx":115
+    /* "extensions.pyx":121
  *             result_code[lineno] = entry = LineTiming(code, lineno)
  *         else:
  *             entry = result_code[lineno]             # <<<<<<<<<<<<<<
  * 
  *         entry.hit(time - old.time)
  */
     /*else*/ {
       if (unlikely(__pyx_v_result_code == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 115, __pyx_L1_error)
+        __PYX_ERR(0, 121, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_lineno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_result_code, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 115, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_result_code, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_10extensions_LineTiming))))) __PYX_ERR(0, 115, __pyx_L1_error)
+      if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_10extensions_LineTiming))))) __PYX_ERR(0, 121, __pyx_L1_error)
       __pyx_v_entry = ((struct __pyx_obj_10extensions_LineTiming *)__pyx_t_5);
       __pyx_t_5 = 0;
     }
     __pyx_L8:;
 
-    /* "extensions.pyx":117
+    /* "extensions.pyx":123
  *             entry = result_code[lineno]
  * 
  *         entry.hit(time - old.time)             # <<<<<<<<<<<<<<
  * 
  *         if what == PyTrace_RETURN:
  */
-    __pyx_t_5 = ((struct __pyx_vtabstruct_10extensions_LineTiming *)__pyx_v_entry->__pyx_vtab)->hit(__pyx_v_entry, (__pyx_v_time - __pyx_v_old->time)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __pyx_t_5 = ((struct __pyx_vtabstruct_10extensions_LineTiming *)__pyx_v_entry->__pyx_vtab)->hit(__pyx_v_entry, (__pyx_v_time - __pyx_v_old->time)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "extensions.pyx":119
+    /* "extensions.pyx":125
  *         entry.hit(time - old.time)
  * 
  *         if what == PyTrace_RETURN:             # <<<<<<<<<<<<<<
  *             del last_time[code]
  * 
  */
     __pyx_t_2 = ((__pyx_v_what == PyTrace_RETURN) != 0);
     if (__pyx_t_2) {
 
-      /* "extensions.pyx":120
+      /* "extensions.pyx":126
  * 
  *         if what == PyTrace_RETURN:
  *             del last_time[code]             # <<<<<<<<<<<<<<
  * 
  *     if what == PyTrace_LINE:
  */
       if (unlikely(__pyx_v_last_time == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 120, __pyx_L1_error)
+        __PYX_ERR(0, 126, __pyx_L1_error)
       }
-      if (unlikely(PyDict_DelItem(__pyx_v_last_time, __pyx_v_code) < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
+      if (unlikely(PyDict_DelItem(__pyx_v_last_time, __pyx_v_code) < 0)) __PYX_ERR(0, 126, __pyx_L1_error)
 
-      /* "extensions.pyx":119
+      /* "extensions.pyx":125
  *         entry.hit(time - old.time)
  * 
  *         if what == PyTrace_RETURN:             # <<<<<<<<<<<<<<
  *             del last_time[code]
  * 
  */
     }
 
-    /* "extensions.pyx":107
+    /* "extensions.pyx":113
  *         results[code] = {}
  * 
  *     if code in last_time:             # <<<<<<<<<<<<<<
  *         result_code = results[code]
  *         old = last_time[code]
  */
   }
 
-  /* "extensions.pyx":122
+  /* "extensions.pyx":128
  *             del last_time[code]
  * 
  *     if what == PyTrace_LINE:             # <<<<<<<<<<<<<<
  *         last_time[code] = LastTime(py_frame.f_lineno, hpTimer())
  * 
  */
   __pyx_t_2 = ((__pyx_v_what == PyTrace_LINE) != 0);
   if (__pyx_t_2) {
 
-    /* "extensions.pyx":123
+    /* "extensions.pyx":129
  * 
  *     if what == PyTrace_LINE:
  *         last_time[code] = LastTime(py_frame.f_lineno, hpTimer())             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_py_frame->f_lineno); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_py_frame->f_lineno); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(hpTimer()); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(hpTimer()); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10extensions_LastTime), __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10extensions_LastTime), __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v_last_time == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 123, __pyx_L1_error)
+      __PYX_ERR(0, 129, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__pyx_v_last_time, __pyx_v_code, __pyx_t_3) < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_last_time, __pyx_v_code, __pyx_t_3) < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "extensions.pyx":122
+    /* "extensions.pyx":128
  *             del last_time[code]
  * 
  *     if what == PyTrace_LINE:             # <<<<<<<<<<<<<<
  *         last_time[code] = LastTime(py_frame.f_lineno, hpTimer())
  * 
  */
   }
 
-  /* "extensions.pyx":125
+  /* "extensions.pyx":131
  *         last_time[code] = LastTime(py_frame.f_lineno, hpTimer())
  * 
  *     return 0             # <<<<<<<<<<<<<<
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "extensions.pyx":82
+  /* "extensions.pyx":88
  * 
  * 
  * cdef int python_trace_callback(object self_, PyFrameObject *py_frame, int what,             # <<<<<<<<<<<<<<
  *                                PyObject *arg):
  *     cdef LineProfiler self
  */
 
@@ -4857,15 +4863,15 @@
 
 static PyObject *__pyx_f_10extensions___pyx_unpickle_LineTiming__set_state(struct __pyx_obj_10extensions_LineTiming *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   long __pyx_t_3;
-  uint64_t __pyx_t_4;
+  __pyx_t_10extensions_uint64_t __pyx_t_4;
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
@@ -4909,15 +4915,15 @@
   __pyx_v___pyx_result->n_hits = __pyx_t_3;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_As_uint64_t(__pyx_t_1); if (unlikely((__pyx_t_4 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_4 == (unsigned PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->total_time = __pyx_t_4;
 
   /* "(tree fragment)":13
  * cdef __pyx_unpickle_LineTiming__set_state(LineTiming __pyx_result, tuple __pyx_state):
  *     __pyx_result.code = __pyx_state[0]; __pyx_result.lineno = __pyx_state[1]; __pyx_result.n_hits = __pyx_state[2]; __pyx_result.total_time = __pyx_state[3]
  *     if len(__pyx_state) > 4 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
@@ -5519,15 +5525,15 @@
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 40, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -5549,40 +5555,40 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "extensions.pyx":35
+  /* "extensions.pyx":41
  * 
  *     @staticmethod
  *     def get_timer():             # <<<<<<<<<<<<<<
  *         return hpTimer()
  * 
  */
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_extensions_extensions_pyx, __pyx_n_s_get_timer, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_extensions_extensions_pyx, __pyx_n_s_get_timer, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 41, __pyx_L1_error)
 
-  /* "extensions.pyx":39
+  /* "extensions.pyx":45
  * 
  *     @staticmethod
  *     def get_timer_implementation():             # <<<<<<<<<<<<<<
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):
  *             return HP_TIMER_IMPLEMENTATION
  */
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_extensions_extensions_pyx, __pyx_n_s_get_timer_implementation, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_extensions_extensions_pyx, __pyx_n_s_get_timer_implementation, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 45, __pyx_L1_error)
 
-  /* "extensions.pyx":45
+  /* "extensions.pyx":51
  * 
  *     @staticmethod
  *     def get_unit():             # <<<<<<<<<<<<<<
  *         return hpTimerUnit()
  * 
  */
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_extensions_extensions_pyx, __pyx_n_s_get_unit, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_extensions_extensions_pyx, __pyx_n_s_get_unit, 51, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 51, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_LineProfiler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -5641,46 +5647,46 @@
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_10extensions_LineProfiler) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10extensions_LineProfiler) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10extensions_LineProfiler.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10extensions_LineProfiler.tp_dictoffset && __pyx_type_10extensions_LineProfiler.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10extensions_LineProfiler.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LineProfiler, (PyObject *)&__pyx_type_10extensions_LineProfiler) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10extensions_LineProfiler) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LineProfiler, (PyObject *)&__pyx_type_10extensions_LineProfiler) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10extensions_LineProfiler) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __pyx_ptype_10extensions_LineProfiler = &__pyx_type_10extensions_LineProfiler;
   __pyx_vtabptr_10extensions_LineTiming = &__pyx_vtable_10extensions_LineTiming;
-  __pyx_vtable_10extensions_LineTiming.hit = (PyObject *(*)(struct __pyx_obj_10extensions_LineTiming *, uint64_t))__pyx_f_10extensions_10LineTiming_hit;
-  if (PyType_Ready(&__pyx_type_10extensions_LineTiming) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_vtable_10extensions_LineTiming.hit = (PyObject *(*)(struct __pyx_obj_10extensions_LineTiming *, __pyx_t_10extensions_uint64_t))__pyx_f_10extensions_10LineTiming_hit;
+  if (PyType_Ready(&__pyx_type_10extensions_LineTiming) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10extensions_LineTiming.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10extensions_LineTiming.tp_dictoffset && __pyx_type_10extensions_LineTiming.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10extensions_LineTiming.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_10extensions_LineTiming.tp_dict, __pyx_vtabptr_10extensions_LineTiming) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LineTiming, (PyObject *)&__pyx_type_10extensions_LineTiming) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10extensions_LineTiming) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_10extensions_LineTiming.tp_dict, __pyx_vtabptr_10extensions_LineTiming) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LineTiming, (PyObject *)&__pyx_type_10extensions_LineTiming) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10extensions_LineTiming) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
   __pyx_ptype_10extensions_LineTiming = &__pyx_type_10extensions_LineTiming;
-  if (PyType_Ready(&__pyx_type_10extensions_LastTime) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10extensions_LastTime) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10extensions_LastTime.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10extensions_LastTime.tp_dictoffset && __pyx_type_10extensions_LastTime.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10extensions_LastTime.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LastTime, (PyObject *)&__pyx_type_10extensions_LastTime) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10extensions_LastTime) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LastTime, (PyObject *)&__pyx_type_10extensions_LastTime) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10extensions_LastTime) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
   __pyx_ptype_10extensions_LastTime = &__pyx_type_10extensions_LastTime;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -5929,98 +5935,98 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "extensions.pyx":35
+  /* "extensions.pyx":41
  * 
  *     @staticmethod
  *     def get_timer():             # <<<<<<<<<<<<<<
  *         return hpTimer()
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10extensions_12LineProfiler_9get_timer, NULL, __pyx_n_s_extensions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10extensions_12LineProfiler_9get_timer, NULL, __pyx_n_s_extensions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer, __pyx_t_1) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer, __pyx_t_1) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_10extensions_LineProfiler);
 
-  /* "extensions.pyx":34
+  /* "extensions.pyx":40
  *         self.last_time = {}
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def get_timer():
  *         return hpTimer()
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_10extensions_LineProfiler, __pyx_n_s_get_timer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_10extensions_LineProfiler, __pyx_n_s_get_timer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer, __pyx_t_2) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_10extensions_LineProfiler);
 
-  /* "extensions.pyx":39
+  /* "extensions.pyx":45
  * 
  *     @staticmethod
  *     def get_timer_implementation():             # <<<<<<<<<<<<<<
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):
  *             return HP_TIMER_IMPLEMENTATION
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_10extensions_12LineProfiler_11get_timer_implementation, NULL, __pyx_n_s_extensions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_10extensions_12LineProfiler_11get_timer_implementation, NULL, __pyx_n_s_extensions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer_implementation, __pyx_t_2) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer_implementation, __pyx_t_2) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_10extensions_LineProfiler);
 
-  /* "extensions.pyx":38
+  /* "extensions.pyx":44
  *         return hpTimer()
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def get_timer_implementation():
  *         if isinstance(HP_TIMER_IMPLEMENTATION, str):
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_10extensions_LineProfiler, __pyx_n_s_get_timer_implementation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_10extensions_LineProfiler, __pyx_n_s_get_timer_implementation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer_implementation, __pyx_t_1) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_timer_implementation, __pyx_t_1) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_10extensions_LineProfiler);
 
-  /* "extensions.pyx":45
+  /* "extensions.pyx":51
  * 
  *     @staticmethod
  *     def get_unit():             # <<<<<<<<<<<<<<
  *         return hpTimerUnit()
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10extensions_12LineProfiler_13get_unit, NULL, __pyx_n_s_extensions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10extensions_12LineProfiler_13get_unit, NULL, __pyx_n_s_extensions); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_unit, __pyx_t_1) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_unit, __pyx_t_1) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_10extensions_LineProfiler);
 
-  /* "extensions.pyx":44
+  /* "extensions.pyx":50
  *         return HP_TIMER_IMPLEMENTATION.decode("ascii")
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def get_unit():
  *         return hpTimerUnit()
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_10extensions_LineProfiler, __pyx_n_s_get_unit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_10extensions_LineProfiler, __pyx_n_s_get_unit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_unit, __pyx_t_2) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_10extensions_LineProfiler->tp_dict, __pyx_n_s_get_unit, __pyx_t_2) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_10extensions_LineProfiler);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_LineProfiler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -6041,15 +6047,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_LineTiming, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "extensions.pyx":1
  * # cython: language_level=2             # <<<<<<<<<<<<<<
  * from cpython cimport PyObject
- * from libc.stdint cimport uint64_t
+ * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
@@ -7662,40 +7668,40 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint64_t(uint64_t value) {
-    const uint64_t neg_one = (uint64_t) ((uint64_t) 0 - (uint64_t) 1), const_zero = (uint64_t) 0;
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_PY_LONG_LONG(unsigned PY_LONG_LONG value) {
+    const unsigned PY_LONG_LONG neg_one = (unsigned PY_LONG_LONG) ((unsigned PY_LONG_LONG) 0 - (unsigned PY_LONG_LONG) 1), const_zero = (unsigned PY_LONG_LONG) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(uint64_t) < sizeof(long)) {
+        if (sizeof(unsigned PY_LONG_LONG) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(uint64_t) <= sizeof(unsigned long)) {
+        } else if (sizeof(unsigned PY_LONG_LONG) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint64_t) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(unsigned PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(uint64_t) <= sizeof(long)) {
+        if (sizeof(unsigned PY_LONG_LONG) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint64_t) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(unsigned PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(uint64_t),
+        return _PyLong_FromByteArray(bytes, sizeof(unsigned PY_LONG_LONG),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
     const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
@@ -8071,163 +8077,163 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *x) {
-    const uint64_t neg_one = (uint64_t) ((uint64_t) 0 - (uint64_t) 1), const_zero = (uint64_t) 0;
+static CYTHON_INLINE unsigned PY_LONG_LONG __Pyx_PyInt_As_unsigned_PY_LONG_LONG(PyObject *x) {
+    const unsigned PY_LONG_LONG neg_one = (unsigned PY_LONG_LONG) ((unsigned PY_LONG_LONG) 0 - (unsigned PY_LONG_LONG) 1), const_zero = (unsigned PY_LONG_LONG) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(uint64_t) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(uint64_t, long, PyInt_AS_LONG(x))
+        if (sizeof(unsigned PY_LONG_LONG) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (uint64_t) val;
+            return (unsigned PY_LONG_LONG) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (uint64_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(uint64_t, digit, digits[0])
+                case  0: return (unsigned PY_LONG_LONG) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(uint64_t) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) >= 2 * PyLong_SHIFT) {
-                            return (uint64_t) (((((uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) >= 2 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(uint64_t) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) >= 3 * PyLong_SHIFT) {
-                            return (uint64_t) (((((((uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) >= 3 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(uint64_t) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
-                            return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (uint64_t) -1;
+                    return (unsigned PY_LONG_LONG) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(uint64_t) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(uint64_t, unsigned long, PyLong_AsUnsignedLong(x))
+            if (sizeof(unsigned PY_LONG_LONG) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned PY_LONG_LONG, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(uint64_t) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(uint64_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if (sizeof(unsigned PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned PY_LONG_LONG, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (uint64_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(uint64_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(uint64_t,  digit, +digits[0])
+                case  0: return (unsigned PY_LONG_LONG) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(uint64_t) - 1 > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (uint64_t) (((uint64_t)-1)*(((((uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) (((unsigned PY_LONG_LONG)-1)*(((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(uint64_t) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (uint64_t) ((((((uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) ((((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(uint64_t) - 1 > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (uint64_t) (((uint64_t)-1)*(((((((uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) (((unsigned PY_LONG_LONG)-1)*(((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(uint64_t) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (uint64_t) ((((((((uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) ((((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(uint64_t) - 1 > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (uint64_t) (((uint64_t)-1)*(((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) (((unsigned PY_LONG_LONG)-1)*(((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(uint64_t) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(unsigned PY_LONG_LONG) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(uint64_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(uint64_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (uint64_t) ((((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(unsigned PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                            return (unsigned PY_LONG_LONG) ((((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(uint64_t) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(uint64_t, long, PyLong_AsLong(x))
+            if (sizeof(unsigned PY_LONG_LONG) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned PY_LONG_LONG, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(uint64_t) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(uint64_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if (sizeof(unsigned PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(unsigned PY_LONG_LONG, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
 #if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
                             "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
 #else
-            uint64_t val;
+            unsigned PY_LONG_LONG val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -8239,32 +8245,32 @@
                                               bytes, sizeof(val),
                                               is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
 #endif
-            return (uint64_t) -1;
+            return (unsigned PY_LONG_LONG) -1;
         }
     } else {
-        uint64_t val;
+        unsigned PY_LONG_LONG val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (uint64_t) -1;
-        val = __Pyx_PyInt_As_uint64_t(tmp);
+        if (!tmp) return (unsigned PY_LONG_LONG) -1;
+        val = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to uint64_t");
-    return (uint64_t) -1;
+        "value too large to convert to unsigned PY_LONG_LONG");
+    return (unsigned PY_LONG_LONG) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to uint64_t");
-    return (uint64_t) -1;
+        "can't convert negative value to unsigned PY_LONG_LONG");
+    return (unsigned PY_LONG_LONG) -1;
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
```

### Comparing `wsgi_lineprof-0.8.0/extensions/extensions.pyx` & `wsgi_lineprof-0.9.0/extensions/extensions.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # cython: language_level=2
 from cpython cimport PyObject
-from libc.stdint cimport uint64_t
 
 from header cimport (
     PyEval_SetTrace, PyFrameObject, PyTrace_LINE, PyTrace_RETURN
 )
 
 
+# It's better if we can use libc.stdint.uint64_t
+# but it produces #include <stdint.h> in the generated C code
+# Old Windows compilers don't support this.
+# from libc.stdint cimport uint64_t
+ctypedef unsigned long long uint64_t
+
+
 cdef extern from "timer.h":
     uint64_t hpTimer()
     double hpTimerUnit()
     char[] HP_TIMER_IMPLEMENTATION
 
 
 cdef class LineProfiler:
```

### Comparing `wsgi_lineprof-0.8.0/extensions/header.pxd` & `wsgi_lineprof-0.9.0/extensions/header.pxd`

 * *Files identical despite different names*

### Comparing `wsgi_lineprof-0.8.0/extensions/timer.c` & `wsgi_lineprof-0.9.0/extensions/timer.c`

 * *Files identical despite different names*

### Comparing `wsgi_lineprof-0.8.0/setup.py` & `wsgi_lineprof-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     if not path.exists(path.join(root, source)):
         raise Exception("No Cython installation, no generated C file")
     warn("Could not import Cython, using generated C source code instead")
 
 setup(
     name="wsgi_lineprof",
 
-    version="0.8.0",
+    version="0.9.0",
 
     description="WSGI middleware for line-by-line profiling",
     long_description=long_description,
 
     url="https://github.com/ymyzk/wsgi_lineprof",
 
     author="Yusuke Miyazaki",
@@ -73,14 +73,15 @@
     ext_package="wsgi_lineprof",
     ext_modules=cythonize([
         Extension("extensions",
                   sources=[source, "extensions/timer.c"])
     ]),
 
     install_requires=[
+        "colorama>=0.4.1",
         "six>=1.10.0",
     ],
 
     extras_require={
         ":python_version < '3.5'": ["typing"],
         "benchmark": [
             "asv>=0.3.1,<0.4",
```

### Comparing `wsgi_lineprof-0.8.0/wsgi_lineprof/extensions.pyi` & `wsgi_lineprof-0.9.0/wsgi_lineprof/extensions.pyi`

 * *Files identical despite different names*

### Comparing `wsgi_lineprof-0.8.0/wsgi_lineprof/filters.py` & `wsgi_lineprof-0.9.0/wsgi_lineprof/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from abc import ABCMeta, abstractmethod
 from itertools import islice
 from operator import attrgetter
 import re
-from typing import Iterable, TYPE_CHECKING  # noqa: F401
+from typing import Iterable, TYPE_CHECKING
 
 from six import add_metaclass
 from six.moves import filter
 
 
 if TYPE_CHECKING:
-    from wsgi_lineprof.stats import LineProfilerStat  # noqa: F401
+    from wsgi_lineprof.stats import LineProfilerStat
 
 
 @add_metaclass(ABCMeta)
 class BaseFilter(object):
     @abstractmethod
     def filter(self, stats):
         # type: (Iterable[LineProfilerStat]) -> Iterable[LineProfilerStat]
```

### Comparing `wsgi_lineprof-0.8.0/wsgi_lineprof/middleware.py` & `wsgi_lineprof-0.9.0/wsgi_lineprof/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import atexit
 import sys
-from typing import (Any, Callable, Iterable, Optional,  # noqa: F401
-                    TYPE_CHECKING)  # noqa: F401
+from typing import Any, Iterable, Optional, TYPE_CHECKING
 
 from wsgi_lineprof.profiler import LineProfiler
-from wsgi_lineprof.stats import FilterType  # noqa: F401
-from wsgi_lineprof.types import Stream  # noqa: F401
-from wsgi_lineprof.writers import (AsyncWriter, BaseWriter,  # noqa: F401
-                                   SyncWriter)  # noqa: F401
+from wsgi_lineprof.stats import FilterType
+from wsgi_lineprof.types import Stream
+from wsgi_lineprof.writers import AsyncWriter, BaseWriter, SyncWriter
 
 
 if TYPE_CHECKING:
-    from wsgiref.types import (StartResponse, WSGIApplication,  # noqa: F401
-                               WSGIEnvironment)  # noqa: F401
+    from wsgiref.types import StartResponse, WSGIApplication, WSGIEnvironment
 
 
 class LineProfilerMiddleware(object):
     def __init__(self,
                  app,  # type: WSGIApplication
                  stream=None,  # type: Optional[Stream]
                  filters=tuple(),  # type: Iterable[FilterType]
                  async_stream=False,  # type: bool
                  accumulate=False,  # type: bool
+                 color=True,  # type: bool
                  ):
         # type: (...) -> None
         self.app = app
         # A hack to suppress unexpected mypy error on Python 2
         # error: Incompatible types in assignment
         # (expression has type "object", variable has type "TextIO")
         stdout = sys.stdout  # type: Any
@@ -36,21 +34,23 @@
         # Cannot use AsyncWriter with atexit
         if async_stream and not accumulate:
             self.writer = AsyncWriter(self.stream)  # type: BaseWriter
         else:
             self.writer = SyncWriter(self.stream)
         if accumulate:
             atexit.register(self._write_stats)
+        # Enable colorization only for stdout/stderr
+        self.color = color and self.stream in {sys.stdout, sys.stderr}
 
     def _write_stats(self):
         # type: () -> None
         stats = self.profiler.get_stats()
         for f in self.filters:
             stats = stats.filter(f)
-        self.writer.write(stats)
+        self.writer.write(stats, color=self.color)
 
     def __call__(self, env, start_response):
         # type: (WSGIEnvironment, StartResponse) -> Iterable[bytes]
         if not self.accumulate:
             self.profiler.reset()
         self.profiler.enable()
         result = self.app(env, start_response)
```

### Comparing `wsgi_lineprof-0.8.0/wsgi_lineprof/profiler.py` & `wsgi_lineprof-0.9.0/wsgi_lineprof/profiler.py`

 * *Files identical despite different names*

### Comparing `wsgi_lineprof-0.8.0/wsgi_lineprof/writers.py` & `wsgi_lineprof-0.9.0/wsgi_lineprof/writers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from abc import ABCMeta, abstractmethod
 from six import add_metaclass
-from six.moves import queue
+from six.moves.queue import Queue
 from threading import Thread
-from typing import Any  # noqa: F401
+from typing import Any, Tuple
 
-from wsgi_lineprof.stats import LineProfilerStats  # noqa: F401
-from wsgi_lineprof.types import Stream  # noqa: F401
+from wsgi_lineprof.stats import LineProfilerStats
+from wsgi_lineprof.types import Stream
 
 
 @add_metaclass(ABCMeta)
 class BaseWriter(object):
     @abstractmethod
     def __init__(self,
                  stream,  # type: Stream
                  *kwargs  # type: Any
                  ):
         # type: (...) -> None
         return
 
     @abstractmethod
-    def write(self, stats):
-        # type: (LineProfilerStats) -> None
+    def write(self, stats, color=False):
+        # type: (LineProfilerStats, bool) -> None
         return
 
 
 class SyncWriter(BaseWriter):
     def __init__(self,
                  stream,  # type: Stream
                  ):
         # type: (...) -> None
         self.stream = stream
 
-    def write(self, stats):
-        # type: (LineProfilerStats) -> None
-        stats.write_text(self.stream)
+    def write(self, stats, color=False):
+        # type: (LineProfilerStats, bool) -> None
+        stats.write_text(self.stream, color=color)
 
 
 class AsyncWriter(BaseWriter):
     def __init__(self,
                  stream,  # type: Stream
                  ):
         # type: (...) -> None
         self.stream = stream
-        self.queue = queue.Queue()  # type: queue.Queue[LineProfilerStats]
+        self.queue = Queue()  # type: Queue[Tuple[LineProfilerStats, bool]]
         self.writer_thread = Thread(target=self._write)
         self.writer_thread.setDaemon(True)
         self.writer_thread.start()
 
-    def write(self, stats):
-        # type: (LineProfilerStats) -> None
-        self.queue.put(stats)
+    def write(self, stats, color=False):
+        # type: (LineProfilerStats, bool) -> None
+        self.queue.put((stats, color))
 
     def _write(self):
         # type: () -> None
         while True:
-            stats = self.queue.get()
-            stats.write_text(self.stream)
+            stats, color = self.queue.get()
+            stats.write_text(self.stream, color=color)
```

### Comparing `wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/PKG-INFO` & `wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsgi-lineprof
-Version: 0.8.0
+Version: 0.9.0
 Summary: WSGI middleware for line-by-line profiling
 Home-page: https://github.com/ymyzk/wsgi_lineprof
 Author: Yusuke Miyazaki
 Author-email: miyazaki.dev@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/ymyzk/wsgi_lineprof/issues
 Project-URL: Source, https://github.com/ymyzk/wsgi_lineprof
@@ -12,14 +12,17 @@
         =============
         .. image:: https://badge.fury.io/py/wsgi-lineprof.svg
            :target: https://pypi.python.org/pypi/wsgi-lineprof/
            :alt: PyPI version
         .. image:: https://img.shields.io/pypi/pyversions/wsgi_lineprof.svg
            :target: https://pypi.python.org/pypi/wsgi-lineprof/
            :alt: PyPI Supported Python Versions
+        .. image:: https://github.com/ymyzk/tox-gh-actions/workflows/Tests/badge.svg
+           :target: https://github.com/ymyzk/tox-gh-actions/actions?workflow=Tests
+           :alt: GitHub Actions (Tests)
         .. image:: https://travis-ci.org/ymyzk/wsgi_lineprof.svg?branch=master
            :target: https://travis-ci.org/ymyzk/wsgi_lineprof
            :alt: Build Status
         .. image:: https://ci.appveyor.com/api/projects/status/cjhft69q2hq1gdoj?svg=true
            :target: https://ci.appveyor.com/project/ymyzk/wsgi-lineprof
            :alt: AppVeyor Build Status
         .. image:: https://readthedocs.org/projects/wsgi_lineprof/badge/?version=latest
@@ -89,11 +92,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Benchmark
 Provides-Extra: benchmark
+Provides-Extra: benchmark-deps
 Provides-Extra: build
-Provides-Extra: test
 Provides-Extra: docs
-Provides-Extra: benchmark-deps
+Provides-Extra: test
```

### Comparing `wsgi_lineprof-0.8.0/wsgi_lineprof.egg-info/SOURCES.txt` & `wsgi_lineprof-0.9.0/wsgi_lineprof.egg-info/SOURCES.txt`

 * *Files identical despite different names*


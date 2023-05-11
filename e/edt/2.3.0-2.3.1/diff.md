# Comparing `tmp/edt-2.3.0.tar.gz` & `tmp/edt-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edt-2.3.0.tar", last modified: Fri May 20 06:04:16 2022, max compression
+gzip compressed data, was "edt-2.3.1.tar", last modified: Thu May 11 19:08:30 2023, max compression
```

## Comparing `edt-2.3.0.tar` & `edt-2.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-05-20 06:04:16.067589 edt-2.3.0/
--rw-r--r--   0 wms        (501) staff       (20)       92 2022-05-20 06:04:15.000000 edt-2.3.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     8102 2022-05-20 06:04:15.000000 edt-2.3.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    35147 2021-01-11 02:45:13.000000 edt-2.3.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       81 2021-04-21 23:11:13.000000 edt-2.3.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     3627 2022-05-20 06:04:16.067752 edt-2.3.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     2222 2021-01-11 02:45:13.000000 edt-2.3.0/README.md
--rw-r--r--   0 wms        (501) staff       (20)  2121971 2022-05-20 06:03:09.000000 edt-2.3.0/edt.cpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-05-20 06:04:16.067355 edt-2.3.0/edt.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     3627 2022-05-20 06:04:15.000000 edt-2.3.0/edt.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      297 2022-05-20 06:04:16.000000 edt-2.3.0/edt.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2022-05-20 06:04:15.000000 edt-2.3.0/edt.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 00:03:37.000000 edt-2.3.0/edt.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2022-05-20 06:04:15.000000 edt-2.3.0/edt.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)        6 2022-05-20 06:04:15.000000 edt-2.3.0/edt.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)        4 2022-05-20 06:04:15.000000 edt-2.3.0/edt.egg-info/top_level.txt
--rw-r--r--   0 wms        (501) staff       (20)    24068 2022-05-20 06:02:29.000000 edt-2.3.0/edt.hpp
--rw-r--r--   0 wms        (501) staff       (20)     8449 2022-05-07 04:25:23.000000 edt-2.3.0/edt_voxel_graph.hpp
--rw-r--r--   0 wms        (501) staff       (20)     1011 2022-05-20 06:04:16.068237 edt-2.3.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      779 2022-01-18 06:20:03.000000 edt-2.3.0/setup.py
--rw-r--r--   0 wms        (501) staff       (20)     3948 2021-01-11 02:45:13.000000 edt-2.3.0/threadpool.h
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-05-11 19:08:30.446776 edt-2.3.1/
+-rw-r--r--   0 wms        (501) staff       (20)       92 2023-05-11 19:08:28.000000 edt-2.3.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     8268 2023-05-11 19:08:28.000000 edt-2.3.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    35147 2021-01-11 02:45:13.000000 edt-2.3.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       81 2021-04-21 23:11:13.000000 edt-2.3.1/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     3630 2023-05-11 19:08:30.446959 edt-2.3.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     2222 2021-01-11 02:45:13.000000 edt-2.3.1/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-05-11 19:08:30.446584 edt-2.3.1/edt.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     3630 2023-05-11 19:08:28.000000 edt-2.3.1/edt.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      297 2023-05-11 19:08:30.000000 edt-2.3.1/edt.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-05-11 19:08:28.000000 edt-2.3.1/edt.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 00:03:37.000000 edt-2.3.1/edt.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-05-11 19:08:28.000000 edt-2.3.1/edt.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 19:08:28.000000 edt-2.3.1/edt.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)        4 2023-05-11 19:08:28.000000 edt-2.3.1/edt.egg-info/top_level.txt
+-rw-r--r--   0 wms        (501) staff       (20)    24068 2023-03-25 22:37:18.000000 edt-2.3.1/edt.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    29159 2023-05-06 20:03:38.000000 edt-2.3.1/edt.pyx
+-rw-r--r--   0 wms        (501) staff       (20)     8449 2022-05-07 04:25:23.000000 edt-2.3.1/edt_voxel_graph.hpp
+-rw-r--r--   0 wms        (501) staff       (20)     1011 2023-05-11 19:08:30.447650 edt-2.3.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      873 2023-05-06 20:02:52.000000 edt-2.3.1/setup.py
+-rw-r--r--   0 wms        (501) staff       (20)     3948 2021-01-11 02:45:13.000000 edt-2.3.1/threadpool.h
```

### Comparing `edt-2.3.0/ChangeLog` & `edt-2.3.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+2.3.1
+-----
+
+* release(2.3.1): update build system
+* fix: update build for py311
+* build: add py311 to tox
+* chore: update edt.cpp
+* install: delay numpy invocation
+
 2.3.0
 -----
 
 * release(2.3.0): adds sdf, sdfsq functions + fixes trailing zero bug
 * feat(sdf): adds signed distance function  (#44)
 
 2.2.0
```

### Comparing `edt-2.3.0/LICENSE` & `edt-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edt-2.3.0/PKG-INFO` & `edt-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edt
-Version: 2.3.0
+Version: 2.3.1
 Summary: Multi-Label Anisotropic Euclidean Distance Transform 3D
 Home-page: https://github.com/seung-lab/euclidean-distance-transform-3d/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: UNKNOWN
 Description: ## Python Instructions for MLAEDT-3D
         
@@ -67,9 +67,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
```

### Comparing `edt-2.3.0/README.md` & `edt-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `edt-2.3.0/edt.egg-info/PKG-INFO` & `edt-2.3.1/edt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edt
-Version: 2.3.0
+Version: 2.3.1
 Summary: Multi-Label Anisotropic Euclidean Distance Transform 3D
 Home-page: https://github.com/seung-lab/euclidean-distance-transform-3d/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: UNKNOWN
 Description: ## Python Instructions for MLAEDT-3D
         
@@ -67,9 +67,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
```

### Comparing `edt-2.3.0/edt.hpp` & `edt-2.3.1/edt.hpp`

 * *Files identical despite different names*

### Comparing `edt-2.3.0/edt_voxel_graph.hpp` & `edt-2.3.1/edt_voxel_graph.hpp`

 * *Files identical despite different names*

### Comparing `edt-2.3.0/setup.cfg` & `edt-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `edt-2.3.0/setup.py` & `edt-2.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import setuptools
 import sys
 
-import numpy as np
+class NumpyImport:
+  def __repr__(self):
+    import numpy as np
+
+    return np.get_include()
+
+  __fspath__ = __repr__
 
 # NOTE: If edt.cpp does not exist:
 # cython -3 --fast-fail -v --cplus edt.pyx
 
 extra_compile_args = []
 if sys.platform == 'win32':
   extra_compile_args += [
@@ -17,21 +23,21 @@
   ]
 
 if sys.platform == 'darwin':
   extra_compile_args += [ '-stdlib=libc++', '-mmacosx-version-min=10.9' ]
 
 
 setuptools.setup(
-  setup_requires=['pbr'],
-  python_requires="~=3.6", # >= 3.6 < 4.0
+  setup_requires=['pbr', 'cython'],
+  python_requires=">=3.7,<4",
   ext_modules=[
     setuptools.Extension(
       'edt',
-      sources=[ 'edt.cpp' ],
+      sources=[ 'edt.pyx' ],
       language='c++',
-      include_dirs=[ np.get_include() ],
+      include_dirs=[ NumpyImport() ],
       extra_compile_args=extra_compile_args,
     ),
   ],
   long_description_content_type='text/markdown',
   pbr=True
 )
```

### Comparing `edt-2.3.0/threadpool.h` & `edt-2.3.1/threadpool.h`

 * *Files identical despite different names*


# Comparing `tmp/gunicorn_uvicorn_runner-0.1.2-py3-none-any.whl.zip` & `tmp/gunicorn_uvicorn_runner-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 6825 bytes, number of entries: 6
 -rw-r--r--  2.0 unx      157 b- defN 80-Jan-01 00:00 gunicorn_uvicorn_runner/__init__.py
 -rw-r--r--  2.0 unx     1676 b- defN 80-Jan-01 00:00 gunicorn_uvicorn_runner/core.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.2.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1737 b- defN 16-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.2.dist-info/METADATA
-?rw-r--r--  2.0 unx      538 b- defN 16-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.2.dist-info/RECORD
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1737 b- defN 80-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx      538 b- defN 16-Jan-01 00:00 gunicorn_uvicorn_runner-0.1.3.dist-info/RECORD
 6 files, 15553 bytes uncompressed, 5843 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: gunicorn_uvicorn_runner/__init__.py
 Comment: 
 
 Filename: gunicorn_uvicorn_runner/core.py
 Comment: 
 
-Filename: gunicorn_uvicorn_runner-0.1.2.dist-info/LICENSE
+Filename: gunicorn_uvicorn_runner-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: gunicorn_uvicorn_runner-0.1.2.dist-info/WHEEL
+Filename: gunicorn_uvicorn_runner-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: gunicorn_uvicorn_runner-0.1.2.dist-info/METADATA
+Filename: gunicorn_uvicorn_runner-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: gunicorn_uvicorn_runner-0.1.2.dist-info/RECORD
+Filename: gunicorn_uvicorn_runner-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gunicorn_uvicorn_runner-0.1.2.dist-info/LICENSE` & `gunicorn_uvicorn_runner-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gunicorn_uvicorn_runner-0.1.2.dist-info/METADATA` & `gunicorn_uvicorn_runner-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunicorn-uvicorn-runner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Run either gunicorn or uvicorn depending on whether reloading is needed.
 Home-page: https://github.com/Jaza/gunicorn-uvicorn-runner
 License: Apache-2.0
 Author: Jeremy Epstein
 Author-email: jazepstein@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `gunicorn_uvicorn_runner-0.1.2.dist-info/RECORD` & `gunicorn_uvicorn_runner-0.1.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 gunicorn_uvicorn_runner/__init__.py,sha256=BC_b3eMB-CDojm9HiVCd0n4d_-H2th-CRT-3-udfwHU,157
 gunicorn_uvicorn_runner/core.py,sha256=t7H7upHFPF7IVEWR9iBSSX5H8bslOI_iqZwOQxuDl0Y,1676
-gunicorn_uvicorn_runner-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-gunicorn_uvicorn_runner-0.1.2.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-gunicorn_uvicorn_runner-0.1.2.dist-info/METADATA,sha256=5uIzaOB_Gd-aoil57iNtAWkoM9ApaFRlpng6aTPQI1o,1737
-gunicorn_uvicorn_runner-0.1.2.dist-info/RECORD,,
+gunicorn_uvicorn_runner-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+gunicorn_uvicorn_runner-0.1.3.dist-info/METADATA,sha256=mT5B6R1_Vi0TDyC252n-cK5NWzkNrLoIjiSjX_JVLo4,1737
+gunicorn_uvicorn_runner-0.1.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+gunicorn_uvicorn_runner-0.1.3.dist-info/RECORD,,
```


# Comparing `tmp/argus_toolbelt-6.9.2-py3-none-any.whl.zip` & `tmp/argus_toolbelt-6.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -53,13 +53,13 @@
 -rw-r--r--  2.0 unx     6104 b- defN 80-Jan-01 00:00 argus_plugins/events/filter.py
 -rw-r--r--  2.0 unx     7550 b- defN 80-Jan-01 00:00 argus_plugins/events/search.py
 -rw-r--r--  2.0 unx     3171 b- defN 80-Jan-01 00:00 argus_plugins/events/statistics.py
 -rw-r--r--  2.0 unx     2175 b- defN 80-Jan-01 00:00 argus_plugins/events/utils.py
 -rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 argus_plugins/reports/__init__.py
 -rw-r--r--  2.0 unx     2347 b- defN 80-Jan-01 00:00 argus_plugins/reports/status.py
 -rw-r--r--  2.0 unx      220 b- defN 80-Jan-01 00:00 argus_plugins/reports/utils.py
-?rw-r--r--  2.0 unx       57 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 argus_toolbelt-6.9.2.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2139 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.2.dist-info/METADATA
-?rw-r--r--  2.0 unx     5753 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.2.dist-info/RECORD
+?rw-r--r--  2.0 unx       57 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 argus_toolbelt-6.9.3.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2139 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.3.dist-info/METADATA
+?rw-r--r--  2.0 unx     5753 b- defN 16-Jan-01 00:00 argus_toolbelt-6.9.3.dist-info/RECORD
 63 files, 254416 bytes uncompressed, 77623 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -168,23 +168,23 @@
 
 Filename: argus_plugins/reports/status.py
 Comment: 
 
 Filename: argus_plugins/reports/utils.py
 Comment: 
 
-Filename: argus_toolbelt-6.9.2.dist-info/entry_points.txt
+Filename: argus_toolbelt-6.9.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: argus_toolbelt-6.9.2.dist-info/LICENSE
+Filename: argus_toolbelt-6.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: argus_toolbelt-6.9.2.dist-info/WHEEL
+Filename: argus_toolbelt-6.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: argus_toolbelt-6.9.2.dist-info/METADATA
+Filename: argus_toolbelt-6.9.3.dist-info/METADATA
 Comment: 
 
-Filename: argus_toolbelt-6.9.2.dist-info/RECORD
+Filename: argus_toolbelt-6.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `argus_toolbelt-6.9.2.dist-info/LICENSE` & `argus_toolbelt-6.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `argus_toolbelt-6.9.2.dist-info/METADATA` & `argus_toolbelt-6.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: argus-toolbelt
-Version: 6.9.2
+Version: 6.9.3
 Summary: A framework for creating interactive commands with Argus' APIs
 License: ISC
 Author: mnemonic
 Author-email: opensource@mnemonic.no
-Requires-Python: >=3.6.1,<4.0.0
+Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: includes
-Requires-Dist: argus-api (>=2.7.2,<3.0.0)
+Requires-Dist: argus-api (>=2.7.3,<3.0.0)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: colorlog (>=4.7,<5.0)
 Requires-Dist: dateparser (>=1.0.0,<2.0.0)
 Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: jinja2 (>=2.11.3)
 Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
 Requires-Dist: pyyaml-include (>=1.2,<2.0); extra == "includes"
```

## Comparing `argus_toolbelt-6.9.2.dist-info/RECORD` & `argus_toolbelt-6.9.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -52,12 +52,12 @@
 argus_plugins/events/filter.py,sha256=J2z8kRopKSM5ZqmqvAHJeXpzIdK_FHKR5DSBoXui-RU,6104
 argus_plugins/events/search.py,sha256=kd_BFt0ZZ0qk3hw3C9xwE2lcgB2pSvzsxnFfO3cEmxg,7550
 argus_plugins/events/statistics.py,sha256=FYMyAkkC5VjgJp2lNRAFanIt0mxTXjh2rldq5EdeSYo,3171
 argus_plugins/events/utils.py,sha256=aVPoiY6QkGa_bw5azLLlFgD4_facmgeY8FR8wXz0w9I,2175
 argus_plugins/reports/__init__.py,sha256=DdOjnA4gw9LfXn5JWMu87JaspOBaJ1Rg1TSTvMrcUu8,43
 argus_plugins/reports/status.py,sha256=gAxYcUBGQgy0-o_By2HMREDoIAjgKE3hqTW9fPZADJM,2347
 argus_plugins/reports/utils.py,sha256=V_VqNgJY3dgznbQBsRKyF01djb7cmE2H5KISnKyuvWg,220
-argus_toolbelt-6.9.2.dist-info/entry_points.txt,sha256=eiDXZaNwsMQ3-jDWVmADLwzW9ys_uaBycHyhjMGnz2g,57
-argus_toolbelt-6.9.2.dist-info/LICENSE,sha256=3gKWMM-A9eiFMMXG22JxEMXSvsxUCDabyzUILvw8mfk,767
-argus_toolbelt-6.9.2.dist-info/WHEEL,sha256=V7iVckP-GYreevsTDnv1eAinQt_aArwnAxmnP0gygBY,83
-argus_toolbelt-6.9.2.dist-info/METADATA,sha256=8GE6ZXlcDEKMh6Kr9m0k3SCawyLHIgcEz9Wkb0PZnyk,2139
-argus_toolbelt-6.9.2.dist-info/RECORD,,
+argus_toolbelt-6.9.3.dist-info/entry_points.txt,sha256=eiDXZaNwsMQ3-jDWVmADLwzW9ys_uaBycHyhjMGnz2g,57
+argus_toolbelt-6.9.3.dist-info/LICENSE,sha256=3gKWMM-A9eiFMMXG22JxEMXSvsxUCDabyzUILvw8mfk,767
+argus_toolbelt-6.9.3.dist-info/WHEEL,sha256=V7iVckP-GYreevsTDnv1eAinQt_aArwnAxmnP0gygBY,83
+argus_toolbelt-6.9.3.dist-info/METADATA,sha256=C6pnPHMVRplYNIdms26O0n6nF3YxEz_ix3c9YToIlWk,2139
+argus_toolbelt-6.9.3.dist-info/RECORD,,
```


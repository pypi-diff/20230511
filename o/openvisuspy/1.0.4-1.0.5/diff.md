# Comparing `tmp/openvisuspy-1.0.4-py3-none-any.whl.zip` & `tmp/openvisuspy-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25203 bytes, number of entries: 15
+Zip file size: 25329 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      239 b- defN 23-May-08 21:22 openvisuspy/__init__.py
 -rw-r--r--  2.0 unx     3757 b- defN 23-May-08 21:22 openvisuspy/app.py
--rw-r--r--  2.0 unx     6033 b- defN 23-May-08 21:22 openvisuspy/backend.py
+-rw-r--r--  2.0 unx     6056 b- defN 23-May-11 00:04 openvisuspy/backend.py
 -rw-r--r--  2.0 unx     7093 b- defN 23-May-08 21:22 openvisuspy/backend_cpp.py
 -rw-r--r--  2.0 unx    11577 b- defN 23-May-08 21:22 openvisuspy/backend_py.py
 -rw-r--r--  2.0 unx     4417 b- defN 23-May-08 21:22 openvisuspy/canvas.py
 -rw-r--r--  2.0 unx     6655 b- defN 23-May-08 21:22 openvisuspy/slice.py
 -rw-r--r--  2.0 unx     1498 b- defN 23-May-08 21:22 openvisuspy/slices.py
 -rw-r--r--  2.0 unx     7249 b- defN 23-May-08 21:22 openvisuspy/utils.py
 -rw-r--r--  2.0 unx    16756 b- defN 23-May-08 21:22 openvisuspy/widgets.py
--rwxrwxrwx  2.0 unx     1849 b- defN 23-May-10 19:20 openvisuspy-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2737 b- defN 23-May-10 19:20 openvisuspy-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 19:20 openvisuspy-1.0.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       12 b- defN 23-May-10 19:20 openvisuspy-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1195 b- defN 23-May-10 19:20 openvisuspy-1.0.4.dist-info/RECORD
-15 files, 71159 bytes uncompressed, 23247 bytes compressed:  67.3%
+-rwxrwxrwx  2.0 unx     1849 b- defN 23-May-10 22:20 openvisuspy-1.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2982 b- defN 23-May-10 22:20 openvisuspy-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 22:20 openvisuspy-1.0.5.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       12 b- defN 23-May-10 22:20 openvisuspy-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1195 b- defN 23-May-10 22:20 openvisuspy-1.0.5.dist-info/RECORD
+15 files, 71427 bytes uncompressed, 23373 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: openvisuspy/utils.py
 Comment: 
 
 Filename: openvisuspy/widgets.py
 Comment: 
 
-Filename: openvisuspy-1.0.4.dist-info/LICENSE
+Filename: openvisuspy-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: openvisuspy-1.0.4.dist-info/METADATA
+Filename: openvisuspy-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: openvisuspy-1.0.4.dist-info/WHEEL
+Filename: openvisuspy-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: openvisuspy-1.0.4.dist-info/top_level.txt
+Filename: openvisuspy-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: openvisuspy-1.0.4.dist-info/RECORD
+Filename: openvisuspy-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openvisuspy/backend.py

```diff
@@ -23,23 +23,24 @@
 		for I in range(pdim):
 			p1[I]=delta[I]*(p1[I]//delta[I])
 			p2[I]=delta[I]*(p2[I]//delta[I])
 			p2[I]=max(p1[I]+delta[I], p2[I])
 		
 		num_pixels=[(p2[I]-p1[I])//delta[I] for I in range(pdim)]
 
-		# print(f"getAlignedBox endh={endh} box={[p1,p2]} delta={delta} num_pixels={num_pixels}")
 
 		#  force to be a slice?
 		# REMOVE THIS!!!
 		if pdim==3 and slice_dir is not None:
 			offset=p1[slice_dir]
 			p2[slice_dir]=offset+0
 			p2[slice_dir]=offset+1
 		
+		# print(f"getAlignedBox logic_box={logic_box} endh={endh} slice_dir={slice_dir} (p1,p2)={(p1,p2)} delta={delta} num_pixels={num_pixels}")
+
 		return (p1,p2), delta, num_pixels
 
 	# createBoxQuery
 	def createBoxQuery(self,
 		timestep=None, 
 		field=None, 
 		logic_box=None,
@@ -109,17 +110,16 @@
 					logger.info(f"Guess resolution endh={endh} original_box={original_box} aligned_box={aligned_box} delta={delta} num_pixels={repr(num_pixels)} tot_pixels={tot_pixels:,} max_pixels={max_pixels:,} end={endh}")
 					logic_box=aligned_box
 					break
 
 		# this is the query I need
 		end_resolutions=list(reversed([endh-pdim*I for I in range(num_refinements) if endh-pdim*I>=0]))
 
-		# need to align to make sure I have all progression needed
-		# (i.e. the first resolution must get something!)
-		logic_box, delta, num_pixels=self.getAlignedBox(logic_box, end_resolutions[0], slice_dir=slice_dir)
+		# scrgiorgio: end_resolutions[0] is wrong, I need to align to the finest resolution
+		logic_box, delta, num_pixels=self.getAlignedBox(logic_box, end_resolutions[-1], slice_dir=slice_dir)
 
 		logic_box=[
 			[int(it) for it in logic_box[0]],
 			[int(it) for it in logic_box[1]]
 		]
 
 		query=types.SimpleNamespace()
```

## Comparing `openvisuspy-1.0.4.dist-info/LICENSE` & `openvisuspy-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openvisuspy-1.0.4.dist-info/METADATA` & `openvisuspy-1.0.5.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: openvisuspy
-Version: 1.0.4
+Version: 1.0.5
 Summary: openvisuspy
 Author: OpenVisus developers
 Project-URL: Homepage, https://github.com/sci-visus/openvisuspy
 Project-URL: Bug Tracker, https://github.com/sci-visus/openvisuspy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenViSUS Visualization project
 
 The official OpenVisus C++ GitHub repository is [here](https://github.com/sci-visus/OpenVisus).
 
+
 # Install openvisuspy
 
 Create a virtual environment. This step is optional, but best to avoid conflicts:
 
+- for windows users you can do `doskey python3=python $*` and `.venv/Scripts/activate.bat`
+
 ```
 python3 -m venv .venv
 source .venv/bin/activate
 python3 -m pip install --upgrade pip
 ```
 
 Install python packages, technically only `numpy` is stricly needed, but to access cloud storage and show dashboards/notebooks, you need additional packages too.
 
 ```
 python3 -m pip install numpy boto3 xmltodict colorcet requests scikit-image matplotlib bokeh panel itkwidgets[all] pyvista vtk jupyter
 ```
 
 Next, nstall Openvisus packages. 
 
+
 If you **do not need the OpenVisus viewer** (or if you are in Windows WSL):
 
 ```
 python3 -m pip install --upgrade OpenVisusNoGui
 python3 -m pip install --upgrade openvisuspy 
 ```
 
@@ -42,14 +46,20 @@
 
 ```
 python3 -m pip install --upgrade OpenVisus
 python3 -m OpenVisus configure 
 python3 -m pip install --upgrade openvisuspy 
 ```
 
+if you are in debugging mode you may want to reference your local packages:
+
+```
+export PYTHONPATH=./src;/projects/OpenVisus/build/RelWithDebInfo
+```
+
 # Examples
 
 ## Bokeh Dashboards 
 
 ```
 python3 -m bokeh serve "examples/dashboards/run.py"  --dev --address localhost --args --single
 python3 -m bokeh serve "examples/dashboards/run.py"  --dev --address localhost --args --multi
```

## Comparing `openvisuspy-1.0.4.dist-info/RECORD` & `openvisuspy-1.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 openvisuspy/__init__.py,sha256=XJQQQgf-N1nzohZPP5BHW2yFZB0ApRqELJMpioa6sow,239
 openvisuspy/app.py,sha256=L3qnxJhL6D3xCFdUjgUzZ-Blk9Ag4x-sz7HSjaGZefM,3757
-openvisuspy/backend.py,sha256=CJ3ChI0L8P5srnpoK_bI4eyCE07lRYNacUkK77BpPic,6033
+openvisuspy/backend.py,sha256=inp3MJswK7QcDFV4__zdGcJ-diWJsrOXiWp8DBkpqL4,6056
 openvisuspy/backend_cpp.py,sha256=ZukezVcj3DikB823ZvinWDb2Tlefke5CjRoSLCDjNTw,7093
 openvisuspy/backend_py.py,sha256=B-ns-tcnhhrE9AedVS6nrVICxZjkkYkqr_oa9mBd2uk,11577
 openvisuspy/canvas.py,sha256=oa42eKl7mQSRnagJ9Kz0uG8duJV0eKaaeG8fFLE6N3A,4417
 openvisuspy/slice.py,sha256=lrerqoE5fekQ0-D0KBWKk_dugRVHKFT-NavfJ3iR3-E,6655
 openvisuspy/slices.py,sha256=ijF00q4UpLMsYC1poXVjr2ZvZM2nl5OZnLh94scjWEM,1498
 openvisuspy/utils.py,sha256=DGfo09rGiKQdB6SHJiEWmOYeMTJnxRJFNUNWPUTxmVQ,7249
 openvisuspy/widgets.py,sha256=OADksn13PktE8giInU-IVH9Ti8skz_S6mdLrVMkzWeQ,16756
-openvisuspy-1.0.4.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
-openvisuspy-1.0.4.dist-info/METADATA,sha256=zx0J1ZvUeAL0PMwsQjQfExA0G5-CLYDNKgZ_p03mGrs,2737
-openvisuspy-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openvisuspy-1.0.4.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
-openvisuspy-1.0.4.dist-info/RECORD,,
+openvisuspy-1.0.5.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
+openvisuspy-1.0.5.dist-info/METADATA,sha256=oddADTu0Os5WxQMhVxfbyLDHWim0BR4pRaHYW4cwfEw,2982
+openvisuspy-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openvisuspy-1.0.5.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
+openvisuspy-1.0.5.dist-info/RECORD,,
```


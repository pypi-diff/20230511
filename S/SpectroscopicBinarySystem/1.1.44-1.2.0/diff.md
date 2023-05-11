# Comparing `tmp/SpectroscopicBinarySystem-1.1.44.tar.gz` & `tmp/SpectroscopicBinarySystem-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.1.44.tar", last modified: Fri May  5 09:13:18 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.2.0.tar", last modified: Thu May 11 11:33:03 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.1.44.tar` & `SpectroscopicBinarySystem-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:13:18.307776 SpectroscopicBinarySystem-1.1.44/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.44/LICENSE
--rw-rw-rw-   0        0        0     4732 2023-05-05 09:13:18.308875 SpectroscopicBinarySystem-1.1.44/PKG-INFO
--rw-rw-rw-   0        0        0     4340 2023-05-05 09:13:15.000000 SpectroscopicBinarySystem-1.1.44/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 09:13:18.305408 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.44/pyproject.toml
--rw-rw-rw-   0        0        0      725 2023-05-05 09:13:18.310326 SpectroscopicBinarySystem-1.1.44/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 09:13:18.306414 SpectroscopicBinarySystem-1.1.44/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    30236 2023-05-05 09:09:16.000000 SpectroscopicBinarySystem-1.1.44/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:33:03.806035 SpectroscopicBinarySystem-1.2.0/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4760 2023-05-11 11:33:03.806035 SpectroscopicBinarySystem-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4369 2023-05-11 11:30:08.000000 SpectroscopicBinarySystem-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 11:33:03.803369 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4760 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-05-11 11:33:03.815788 SpectroscopicBinarySystem-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 11:33:03.804376 SpectroscopicBinarySystem-1.2.0/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    31287 2023-05-11 11:02:14.000000 SpectroscopicBinarySystem-1.2.0/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.1.44/LICENSE` & `SpectroscopicBinarySystem-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.44/PKG-INFO` & `SpectroscopicBinarySystem-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.44
+Version: 1.2.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -68,47 +68,48 @@
 Download sample data (see **/examples/alphadra** directory) or from the **STAROS** database (https://alphadra.staros-projects.org/)
 
 And run this code :
 
 ```python
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
-# create SpectroscopicBinarySystem object
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
     conf={
         "LAMBDA_REF": 6562.82,
         "LINE_FIT_MODEL": "voigt",
         "LINE_FIT_WINDOW_WIDTH": 10,
-        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1.5,
-        "LINE_FIT_FWHM": .5,
+        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1,
         "RV_CORR_TYPE": "barycentric",
         "SB_TYPE": 1
     },
-    debug=True)
+    verbose=True
+    debug=False)
 
 # plot result with matplotlib and save the results
-sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", 
-                            subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
-                            savefig=True)
- 
-# display result with plotly
-sbs.plotlyRadialVelocityCurve(
-    title="α Dra - HD123299 - Phased radial velocities")
+sbs.plotRadialVelocityCurve(
+    title="α Dra - HD123299 - Phased radial velocities",
+    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
+    savefig=True)
 
 # plot 2d dynamic spectrum
 sbs.plotSpec2DFlux(
-    title="α Dra - HD123299 - 2d dynamic spectrum",
-    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
-    savefig=False
+    title="α Dra - HD123299 - Hα line 2d dynamic spectrum",
+    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
+    savefig=True
 )
+
+# display result with plotl
+sbs.plotlyRadialVelocityCurve(
+    title="α Dra - HD123299 - Phased radial velocities",
+    group_by_instrument=False)
+
 ```
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_phased_result.png)
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_2d_spectrum_result.png)
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
-
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_debug_result_page_4.png)
```

### Comparing `SpectroscopicBinarySystem-1.1.44/README.md` & `SpectroscopicBinarySystem-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -56,47 +56,48 @@
 Download sample data (see **/examples/alphadra** directory) or from the **STAROS** database (https://alphadra.staros-projects.org/)
 
 And run this code :
 
 ```python
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
-# create SpectroscopicBinarySystem object
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
     conf={
         "LAMBDA_REF": 6562.82,
         "LINE_FIT_MODEL": "voigt",
         "LINE_FIT_WINDOW_WIDTH": 10,
-        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1.5,
-        "LINE_FIT_FWHM": .5,
+        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1,
         "RV_CORR_TYPE": "barycentric",
         "SB_TYPE": 1
     },
-    debug=True)
+    verbose=True
+    debug=False)
 
 # plot result with matplotlib and save the results
-sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", 
-                            subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
-                            savefig=True)
- 
-# display result with plotly
-sbs.plotlyRadialVelocityCurve(
-    title="α Dra - HD123299 - Phased radial velocities")
+sbs.plotRadialVelocityCurve(
+    title="α Dra - HD123299 - Phased radial velocities",
+    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
+    savefig=True)
 
 # plot 2d dynamic spectrum
 sbs.plotSpec2DFlux(
-    title="α Dra - HD123299 - 2d dynamic spectrum",
-    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
-    savefig=False
+    title="α Dra - HD123299 - Hα line 2d dynamic spectrum",
+    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
+    savefig=True
 )
+
+# display result with plotl
+sbs.plotlyRadialVelocityCurve(
+    title="α Dra - HD123299 - Phased radial velocities",
+    group_by_instrument=False)
+
 ```
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_phased_result.png)
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_2d_spectrum_result.png)
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
-
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_debug_result_page_4.png)
```

### Comparing `SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.44
+Version: 1.2.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -68,47 +68,48 @@
 Download sample data (see **/examples/alphadra** directory) or from the **STAROS** database (https://alphadra.staros-projects.org/)
 
 And run this code :
 
 ```python
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
-# create SpectroscopicBinarySystem object
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
     conf={
         "LAMBDA_REF": 6562.82,
         "LINE_FIT_MODEL": "voigt",
         "LINE_FIT_WINDOW_WIDTH": 10,
-        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1.5,
-        "LINE_FIT_FWHM": .5,
+        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1,
         "RV_CORR_TYPE": "barycentric",
         "SB_TYPE": 1
     },
-    debug=True)
+    verbose=True
+    debug=False)
 
 # plot result with matplotlib and save the results
-sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", 
-                            subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
-                            savefig=True)
- 
-# display result with plotly
-sbs.plotlyRadialVelocityCurve(
-    title="α Dra - HD123299 - Phased radial velocities")
+sbs.plotRadialVelocityCurve(
+    title="α Dra - HD123299 - Phased radial velocities",
+    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
+    savefig=True)
 
 # plot 2d dynamic spectrum
 sbs.plotSpec2DFlux(
-    title="α Dra - HD123299 - 2d dynamic spectrum",
-    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
-    savefig=False
+    title="α Dra - HD123299 - Hα line 2d dynamic spectrum",
+    subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to may 2023\nhttps://alphadra.staros-projects.org/\n",
+    savefig=True
 )
+
+# display result with plotl
+sbs.plotlyRadialVelocityCurve(
+    title="α Dra - HD123299 - Phased radial velocities",
+    group_by_instrument=False)
+
 ```
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_phased_result.png)
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_2d_spectrum_result.png)
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
-
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_debug_result_page_4.png)
```

### Comparing `SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.44/setup.cfg` & `SpectroscopicBinarySystem-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 312e 3434 0d0a  rsion = 1.1.44..
-00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
-00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
-00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
-00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
-00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
-00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
-000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
-000000b0: 2062 696e 6172 7920 7379 7374 656d 0d0a   binary system..
-000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000d0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000e0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-000000f0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000100: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000110: 6e0d 0a6c 6963 656e 7365 203d 2042 5344  n..license = BSD
-00000120: 2d33 2d43 6c61 7573 650d 0a6c 6963 656e  -3-Clause..licen
-00000130: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
-00000140: 5345 0d0a 6b65 7977 6f72 6473 203d 2061  SE..keywords = a
-00000150: 7374 726f 6e6f 6d79 2c61 7374 726f 7068  stronomy,astroph
-00000160: 7973 6963 732c 7363 6965 6e63 652c 6669  ysics,science,fi
-00000170: 7473 2c6d 6f64 656c 732c 6669 7474 696e  ts,models,fittin
-00000180: 672c 7370 6563 7472 6f73 636f 7079 2c73  g,spectroscopy,s
-00000190: 7065 6374 7275 6d0d 0a0d 0a5b 6f70 7469  pectrum....[opti
-000001a0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
-000001b0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-000001c0: 6571 7569 7265 7320 3d20 3e3d 332e 3130  equires = >=3.10
-000001d0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-000001e0: 6573 203d 200d 0a09 6173 7472 6f70 793e  es = ...astropy>
-000001f0: 3d35 2e32 2e32 0d0a 0961 7374 726f 7175  =5.2.2...astroqu
-00000200: 6572 793e 3d30 2e34 2e36 0d0a 0942 696e  ery>=0.4.6...Bin
-00000210: 6172 7953 7461 7253 6f6c 7665 723e 3d31  aryStarSolver>=1
-00000220: 2e32 2e30 0d0a 096d 6174 706c 6f74 6c69  .2.0...matplotli
-00000230: 623e 3d33 2e37 2e31 0d0a 096e 756d 7079  b>=3.7.1...numpy
-00000240: 3e3d 312e 3234 2e32 0d0a 094f 7262 6974  >=1.24.2...Orbit
-00000250: 616c 5079 3e3d 302e 372e 300d 0a09 5079  alPy>=0.7.0...Py
-00000260: 5941 4d4c 3e3d 362e 300d 0a09 7370 6563  YAML>=6.0...spec
-00000270: 7574 696c 733e 3d31 2e39 2e31 0d0a 0942  utils>=1.9.1...B
-00000280: 696e 6172 7953 7461 7253 6f6c 7665 723e  inaryStarSolver>
-00000290: 3d31 2e32 2e30 0d0a 0970 6c6f 746c 793e  =1.2.0...plotly>
-000002a0: 3d35 2e31 342e 310d 0a0d 0a5b 6567 675f  =5.14.1....[egg_
-000002b0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000002c0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000002d0: 300d 0a0d 0a                             0....
+00000030: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
+00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
+00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
+00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
+00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
+00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
+00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
+000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic 
+000000b0: 6269 6e61 7279 2073 7973 7465 6d0d 0a6c  binary system..l
+000000c0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+000000d0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+000000e0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+000000f0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+00000100: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000110: 0d0a 6c69 6365 6e73 6520 3d20 4253 442d  ..license = BSD-
+00000120: 332d 436c 6175 7365 0d0a 6c69 6365 6e73  3-Clause..licens
+00000130: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
+00000140: 450d 0a6b 6579 776f 7264 7320 3d20 6173  E..keywords = as
+00000150: 7472 6f6e 6f6d 792c 6173 7472 6f70 6879  tronomy,astrophy
+00000160: 7369 6373 2c73 6369 656e 6365 2c66 6974  sics,science,fit
+00000170: 732c 6d6f 6465 6c73 2c66 6974 7469 6e67  s,models,fitting
+00000180: 2c73 7065 6374 726f 7363 6f70 792c 7370  ,spectroscopy,sp
+00000190: 6563 7472 756d 0d0a 0d0a 5b6f 7074 696f  ectrum....[optio
+000001a0: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
+000001b0: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+000001c0: 7175 6972 6573 203d 203e 3d33 2e31 300d  quires = >=3.10.
+000001d0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000001e0: 7320 3d20 0d0a 0961 7374 726f 7079 3e3d  s = ...astropy>=
+000001f0: 352e 322e 320d 0a09 6173 7472 6f71 7565  5.2.2...astroque
+00000200: 7279 3e3d 302e 342e 360d 0a09 4269 6e61  ry>=0.4.6...Bina
+00000210: 7279 5374 6172 536f 6c76 6572 3e3d 312e  ryStarSolver>=1.
+00000220: 322e 300d 0a09 6d61 7470 6c6f 746c 6962  2.0...matplotlib
+00000230: 3e3d 332e 372e 310d 0a09 6e75 6d70 793e  >=3.7.1...numpy>
+00000240: 3d31 2e32 342e 320d 0a09 4f72 6269 7461  =1.24.2...Orbita
+00000250: 6c50 793e 3d30 2e37 2e30 0d0a 0950 7959  lPy>=0.7.0...PyY
+00000260: 414d 4c3e 3d36 2e30 0d0a 0973 7065 6375  AML>=6.0...specu
+00000270: 7469 6c73 3e3d 312e 392e 310d 0a09 4269  tils>=1.9.1...Bi
+00000280: 6e61 7279 5374 6172 536f 6c76 6572 3e3d  naryStarSolver>=
+00000290: 312e 322e 300d 0a09 706c 6f74 6c79 3e3d  1.2.0...plotly>=
+000002a0: 352e 3134 2e31 0d0a 0d0a 5b65 6767 5f69  5.14.1....[egg_i
+000002b0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000002c0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000002d0: 0d0a 0d0a                                ....
```

### Comparing `SpectroscopicBinarySystem-1.1.44/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.2.0/spectroscopicbinarysystem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from astropy import constants as const
 
 # astroquery
 from astroquery.simbad import Simbad
 
 # specutils
 from specutils import Spectrum1D, SpectralRegion
-from specutils.manipulation import extract_region, LinearInterpolatedResampler
+from specutils.manipulation import extract_region, LinearInterpolatedResampler, gaussian_smooth
 from specutils.fitting import fit_lines, fit_generic_continuum
+from specutils.analysis import centroid
 
 # matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.ticker import (MultipleLocator)
 
 # plotly
 import plotly.graph_objects as go
@@ -47,14 +48,15 @@
     """
 
     def __init__(self, filename, skycoord, conf):
         self._filename = filename
         self._basename = os.path.basename(filename)
         self._skycoord = skycoord
         self._conf = conf
+        self._phase = None
 
         spectrum_file = fits.open(filename)
 
         self._header = spectrum_file[0].header
         self._jd = self._header['JD-OBS']
         self._observer = self._header['OBSERVER']
         with warnings.catch_warnings():  # Ignore warnings
@@ -174,52 +176,57 @@
         """
         Find the center of the line in a spectrum using a fit (models available : Gaussian1D, Lorentz1D, Voigt1D)
         :return: None
         """
         w1 = float(self._conf['LINE_FIT_WINDOW_WIDTH']) / 2
         w2 = float(self._conf['LINE_FIT_CONT_NORM_EXCLUDE_WIDTH']) / 2
         fwhm = float(self._conf['LINE_FIT_FWHM'])
+        gauss_smooth_std = float(self._conf['LINE_FIT_GAUSS_SMOOTH_STD'])
 
-        # > Hack to replace zero values of the spectra.
-        # Sometimes first value for the intensity is equal to 0.00 and prevents finding the true minima.
-        # Ex : sample/alphadra/_alphadra_20230406_856.fits
-        self.flux[self.flux == 0] = 1 * u.Jy
-        ipeak = self.flux.argmin()
-        xpeak = self.spectral_axis[ipeak].to(u.AA)
+        # Smooth the spectrum to make a first approximation of the center of the main line in absorption.
+        # Assume that the line to be measured is the broadest and deepest in the spectrum
+        spec1_gsmooth = gaussian_smooth(Spectrum1D(
+            flux=self.flux, wcs=self.wcs), stddev=gauss_smooth_std)
 
-        spec1d_line = extract_region(Spectrum1D(flux=self.flux, wcs=self.wcs),
-                                     SpectralRegion(xpeak - (w1 * u.AA), xpeak + (w1 * u.AA)))
+        ipeak = spec1_gsmooth.flux[50:-50].argmin()
+        xpeak = spec1_gsmooth.spectral_axis[50:-50][ipeak].to(u.AA)
 
-        s_fit = fit_generic_continuum(spec1d_line, exclude_regions=[
-                                      SpectralRegion(xpeak - (w2 * u.AA), xpeak + (w2 * u.AA))])
+        sr_w1 = SpectralRegion(xpeak - (w1 * u.AA), xpeak + (w1 * u.AA))
+        sr_w2 = SpectralRegion(xpeak - (w2 * u.AA), xpeak + (w2 * u.AA))
+
+        spec1d_line = extract_region(Spectrum1D(
+            flux=self.flux, wcs=self.wcs), sr_w1)
+
+        # continuum normalization of the extracted spectral region
+        s_fit = fit_generic_continuum(spec1d_line, exclude_regions=[sr_w2])
         spec1d_line = spec1d_line / s_fit(spec1d_line.spectral_axis)
         spec1d_line = spec1d_line - 1
 
+        # line fitting
         match self._conf['LINE_FIT_MODEL']:
             case 'gaussian':
                 g_init = models.Gaussian1D(
                     mean=xpeak, amplitude=spec1d_line.flux.argmin())
             case 'voigt':
                 g_init = models.Voigt1D(
                     x_0=xpeak, amplitude_L=spec1d_line.flux.argmin())
             case 'lorentz':
                 g_init = models.Lorentz1D(x_0=xpeak, fwhm=fwhm)
-        #
 
-        g_fit = fit_lines(spec1d_line, g_init, window=SpectralRegion(
-            xpeak - (w2 * u.AA), xpeak + (w2 * u.AA)))
+        g_fit = fit_lines(spec1d_line, g_init, window=sr_w2)
         y_fit = g_fit(spec1d_line.spectral_axis)
 
         match self._conf['LINE_FIT_MODEL']:
             case 'gaussian':
                 center = g_fit.mean
             case _:
                 center = g_fit.x_0
 
-        self._debug_line_fitting = (spec1d_line, y_fit)
+        self._debug_line_fitting = (spec1d_line, y_fit, extract_region(Spectrum1D(
+            flux=spec1_gsmooth.flux, wcs=self.wcs), sr_w1))
         self._center_of_line = center.value
 
     def __str__(self):
         return f"Spectrum : {self._basename}\n- obs: {self._observer}\n- jd: {self._jd}\n- center: {self._center_of_line} A\n- {self._conf['RV_CORR_TYPE']}: {self._rv_corr}\n- rv: {self._rv}\n "
 
 #
 
@@ -238,34 +245,37 @@
     :param t0: Allow to fix Periastron epoch T0 if known (julian date)
     :param period: If the period of the orbit is already known use this param (period in days).
     :param perdiod_guess: If the period is uncertain use this param (period in days).
     :param conf: Allow to customize additionnal parameters (see self._conf default value below)
     :param debug: Allow to activate log and some additional plots for debug purpose
     """
 
-    def __init__(self, object_name, spectra_path, t0=None, period=None, period_guess=None, conf=None, debug=False):
+    def __init__(self, object_name, spectra_path, t0=None, period=None, period_guess=None, conf=None, verbose=False, debug=False):
 
         self._conf = {"LAMBDA_REF": 6562.82,
                       "LINE_FIT_MODEL": "voigt",
                       "LINE_FIT_WINDOW_WIDTH": 10,
                       "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1.5,
                       "LINE_FIT_FWHM": .5,
+                      "LINE_FIT_GAUSS_SMOOTH_STD": 10,
                       "RV_CORR_TYPE": "barycentric",
                       "SB_TYPE": 1}
 
         self._sb_spectra = []
         self._spectra_filename = []
         self._orbital_solution = None
         self._spectra_path = spectra_path
         self._object_name = object_name
         self._type = type
         self._t0 = t0
         self._period = period
         self._period_guess = period_guess
         self._debug = debug
+        self._verbose = verbose
+        self._residuals = []
 
         # load user configuration or defaults
         if conf:
             self._conf.update(conf)
 
         print('** SpectroscopicBinarySystem **')
         self.__findObjectCoordinate()
@@ -285,40 +295,48 @@
             for file in files:
                 regex = re.compile('(.*).fit')
                 if (re.match(regex, file)):
                     spectrum_filename = os.path.join(self._spectra_path, file)
                     sbSpec1D = SBSpectrum1D(
                         spectrum_filename, self._skycoord, self._conf)
                     self._sb_spectra.append(sbSpec1D)
-                    if self._debug:
+                    if self._verbose:
                         print(sbSpec1D)
-        if self._debug:
+
+        if self._verbose:
             print(f'{len(self._sb_spectra)} processed spectra')
+        if self._debug:
             plt.rcParams['font.size'] = '6'
             plt.rcParams['font.family'] = 'monospace'
-            grid_size = math.ceil(len(self._sb_spectra)/6)
-            fig, axs = plt.subplots(6, grid_size, figsize=(
-                13, 7), sharex=True, sharey=True)
-            for i, s in enumerate(self._sb_spectra):
-                ax = axs.flat[i]
-                extracted_profil, line_fitting = s.getDebugLineFitting()
-                ax.set_title(
-                    f'{s.getBaseName()}\n{s.getObserver()} JD={s.getJD()}', fontsize="6")
-                ax.grid(True)
-                ax.tick_params(axis='both', which='major', labelsize=6)
-                ax.tick_params(axis='both', which='minor', labelsize=6)
-                ax.plot(extracted_profil.spectral_axis.to(
-                    u.AA), extracted_profil.flux, color="k")
-                ax.plot(extracted_profil.spectral_axis.to(
-                    u.AA), line_fitting, color="r")
-                ax.axvline(x=s.getCenterOfLine(),
-                           color='r', linestyle='-', lw=0.7)
-            plt.tight_layout(pad=0.8, w_pad=2, h_pad=1)
-            plt.savefig(f'{self._spectra_path}/sbs_debug_result.png', dpi=150)
-            plt.show()
+
+            paginate_sb_spectra = [self._sb_spectra[i:i+16]
+                                   for i in range(0, len(self._sb_spectra), 16)]
+            for page, spectra in enumerate(paginate_sb_spectra):
+                fig, axs = plt.subplots(4, 4, figsize=(
+                    10, 7), sharex=True, sharey=True)
+                for i, s in enumerate(spectra):
+                    ax = axs.flat[i]
+                    extracted_profil, line_fitting, gauss_smooth = s.getDebugLineFitting()
+                    ax.set_title(
+                        f'{s.getBaseName()}\n{s.getObserver()} JD={s.getJD()}', fontsize="6")
+                    ax.grid(True)
+                    ax.tick_params(axis='both', which='major', labelsize=6)
+                    ax.tick_params(axis='both', which='minor', labelsize=6)
+                    ax.plot(extracted_profil.spectral_axis.to(
+                        u.AA), extracted_profil.flux, color="k")
+                    ax.plot(gauss_smooth.spectral_axis.to(
+                        u.AA), gauss_smooth.flux-1*u.Jy, "b--")
+                    ax.plot(extracted_profil.spectral_axis.to(
+                        u.AA), line_fitting, color="r")
+                    ax.axvline(x=s.getCenterOfLine(),
+                               color='r', linestyle='-', lw=0.7)
+                plt.tight_layout(pad=0.8, w_pad=2, h_pad=1)
+                plt.savefig(
+                    f'{self._spectra_path}/{self._object_name}_debug_result_page_{page}.png', dpi=300)
+                plt.close(fig)
 
     def getObservationCount(self):
         """
         Return the count of processed spectra
         :return: count
         :rtype: int
         """
@@ -395,15 +413,15 @@
 
         period = self._orbital_solution[0][5]
         for s in self._sb_spectra:
             # compute phase of the sytem
             jd = s.getJD()
             phase = self.__getPhase(float(self._t0), period, jd)
             s.setPhase(phase)
-            if self._debug:
+            if self._verbose:
                 print(f"{s.getBaseName()} phase : {phase}")
 
         print(
             f'{self._object_name} orbital solution with {len(self._sb_spectra)} spectra',
             f'- γ = {params[0]} ± {err[0]}',
             f'- K = {params[1]} ± {err[1]}',
             f'- ω = {params[2]} ± {err[2]}',
@@ -477,18 +495,22 @@
                     axs[0].errorbar(s.getPhase(), s.getRV(
                     ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
                 else:
                     axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
                                     fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
             xindex = self.__findNearest(self._model_x, s.getPhase())
+            delta = s.getRV() - self._model_y[xindex]
+            self._residuals.append(delta)
             fmt = instruments[label] if group_by_instruments else 'o'
-            axs[1].errorbar(s.getPhase(), s.getRV() - self._model_y[xindex],
+            axs[1].errorbar(s.getPhase(), delta,
                             yerr=0, fmt=fmt, ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
+        print(f'- Residuals mean STD : {np.std(self._residuals)} km/s')
+
     def plotRadialVelocityCurve(self, title="", subtitle="", rv_y_multiple=10, residual_y_multiple=None, savefig=False, dpi=150, font_family='monospace', font_size=9, group_by_instruments=False):
         if not self._orbital_solution:
             self.__solveSystem()
 
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
         fig, axs = plt.subplots(2, 1, figsize=(11, 7), gridspec_kw={
```


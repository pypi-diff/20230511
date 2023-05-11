# Comparing `tmp/estival-0.2.3.tar.gz` & `tmp/estival-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estival-0.2.3.tar", max compression
+gzip compressed data, was "estival-0.2.4.tar", max compression
```

## Comparing `estival-0.2.3.tar` & `estival-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,26 @@
--rw-r--r--   0        0        0     3010 2023-04-04 20:46:52.692604 estival-0.2.3/estival/calibration/__pycache__/pymc.cpython-310.pyc
--rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.3/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
--rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.3/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
--rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.3/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
--rw-r--r--   0        0        0    23290 2023-05-03 06:12:36.018586 estival-0.2.3/estival/calibration/mcmc/adaptive.py
--rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.3/estival/calibration/mcmc/covariance.py
--rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.3/estival/calibration/mcmc/transformations.py
--rw-r--r--   0        0        0     2665 2023-04-04 20:12:53.083034 estival-0.2.3/estival/calibration/pymc.py
--rw-r--r--   0        0        0     2659 2023-05-03 20:42:06.724911 estival-0.2.3/estival/model.py
--rw-r--r--   0        0        0     2666 2023-05-03 21:37:51.092087 estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
--rw-r--r--   0        0        0     4492 2023-05-03 03:19:27.593270 estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
--rw-r--r--   0        0        0     2635 2023-05-03 21:00:19.800964 estival-0.2.3/estival/optimization/nevergrad.py
--rw-r--r--   0        0        0     3801 2023-04-04 20:15:44.189728 estival-0.2.3/estival/priors.py
--rw-r--r--   0        0        0    10790 2023-05-03 21:34:29.524110 estival-0.2.3/estival/targets.py
--rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.3/estival/utils.py
--rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.3/LICENSE
--rw-r--r--   0        0        0     1002 2023-05-03 23:14:40.994446 estival-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-03 23:21:51.163726 estival-0.2.3/README.md
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 estival-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3458 2023-05-10 03:44:23.083361 estival-0.2.4/estival/calibration/__pycache__/pymc.cpython-310.pyc
+-rw-r--r--   0        0        0     4772 2023-05-06 03:26:51.437183 estival-0.2.4/estival/calibration/__pycache__/pymc.cpython-311.pyc
+-rw-r--r--   0        0        0    14995 2023-05-05 04:48:51.863477 estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc
+-rw-r--r--   0        0        0    25353 2023-05-05 05:24:17.406283 estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc
+-rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
+-rw-r--r--   0        0        0     2324 2023-05-05 04:48:54.568004 estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc
+-rw-r--r--   0        0        0     3213 2023-05-05 05:24:18.633294 estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc
+-rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
+-rw-r--r--   0        0        0     3211 2023-05-05 04:48:54.551505 estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc
+-rw-r--r--   0        0        0     5303 2023-05-05 05:24:18.606294 estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc
+-rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
+-rw-r--r--   0        0        0    23290 2023-05-03 06:12:36.018586 estival-0.2.4/estival/calibration/mcmc/adaptive.py
+-rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.4/estival/calibration/mcmc/covariance.py
+-rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.4/estival/calibration/mcmc/transformations.py
+-rw-r--r--   0        0        0     3080 2023-05-11 03:41:35.661930 estival-0.2.4/estival/calibration/pymc.py
+-rw-r--r--   0        0        0     2683 2023-05-11 02:56:54.916427 estival-0.2.4/estival/model.py
+-rw-r--r--   0        0        0     2666 2023-05-03 21:37:51.092087 estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
+-rw-r--r--   0        0        0     4511 2023-05-05 05:24:18.926797 estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
+-rw-r--r--   0        0        0     2635 2023-05-03 21:00:19.800964 estival-0.2.4/estival/optimization/nevergrad.py
+-rw-r--r--   0        0        0     4222 2023-05-10 03:48:52.052508 estival-0.2.4/estival/priors.py
+-rw-r--r--   0        0        0    11364 2023-05-11 02:58:25.406441 estival-0.2.4/estival/targets.py
+-rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.4/estival/utils.py
+-rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1034 2023-05-11 03:44:56.420364 estival-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-05-11 03:57:10.793592 estival-0.2.4/README.md
+-rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 estival-0.2.4/PKG-INFO
```

### Comparing `estival-0.2.3/estival/calibration/__pycache__/pymc.cpython-310.pyc` & `estival-0.2.4/estival/calibration/__pycache__/pymc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 20:12:53 2023 UTC, .py size: 2665 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,189 +1,217 @@
-00000000: 6f0d 0d0a 0000 0000 c584 2c64 690a 0000  o.........,di...
+00000000: 6f0d 0d0a 0000 0000 0013 5b64 730c 0000  o.........[ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
+00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
-00000050: 6d08 5a08 0100 6403 6508 6602 6404 6405  m.Z...d.e.f.d.d.
-00000060: 8404 5a09 640a 6403 6508 6407 650a 6604  ..Z.d.d.e.d.e.f.
-00000070: 6408 6409 8405 5a0b 6401 5300 290b e900  d.d...Z.d.S.)...
-00000080: 0000 004e 2901 da1a 4261 7965 7369 616e  ...N)...Bayesian
-00000090: 436f 6d70 6172 746d 656e 7461 6c4d 6f64  CompartmentalMod
-000000a0: 656c da03 6263 6d63 0100 0000 0000 0000  el..bcmc........
-000000b0: 0000 0000 0200 0000 0400 0000 0300 0000  ................
-000000c0: 731a 0000 0047 0087 0066 0164 0164 0284  s....G...f.d.d..
-000000d0: 0864 0274 006a 0183 037d 017c 0153 0029  .d.t.j...}.|.S.)
-000000e0: 037a 745f 7375 6d6d 6172 795f 0a0a 2020  .zt_summary_..  
-000000f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00000100: 6263 6d3a 2054 6865 206d 6f64 656c 2074  bcm: The model t
-00000110: 6f20 7772 6170 0a0a 2020 2020 5265 7475  o wrap..    Retu
-00000120: 726e 733a 0a20 2020 2020 2020 2041 2077  rns:.        A w
-00000130: 7261 7070 6564 2070 7974 656e 736f 7220  rapped pytensor 
-00000140: 6f70 2066 6f72 2075 7365 2069 6e20 7079  op for use in py
-00000150: 6d63 0a20 2020 2063 0000 0000 0000 0000  mc.    c........
-00000160: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00000170: 733e 0000 0065 005a 0164 005a 0264 015a  s>...e.Z.d.Z.d.Z
-00000180: 0365 046a 0567 0165 0694 006a 0783 0114  .e.j.g.e...j....
-00000190: 005a 0865 046a 0567 015a 0987 0066 0164  .Z.e.j.g.Z...f.d
-000001a0: 0264 0384 085a 0a64 0464 0584 005a 0b64  .d...Z.d.d...Z.d
-000001b0: 0653 0029 077a 2267 6574 5f77 7261 7070  .S.).z"get_wrapp
-000001c0: 6564 5f6c 6c2e 3c6c 6f63 616c 733e 2e42  ed_ll.<locals>.B
-000001d0: 434d 4c6f 674c 696b 6561 1501 0000 0a20  CMLogLikea..... 
-000001e0: 2020 2020 2020 2053 7065 6369 6679 2077         Specify w
-000001f0: 6861 7420 7479 7065 206f 6620 6f62 6a65  hat type of obje
-00000200: 6374 2077 696c 6c20 6265 2070 6173 7365  ct will be passe
-00000210: 6420 616e 6420 7265 7475 726e 6564 2074  d and returned t
-00000220: 6f20 7468 6520 4f70 2077 6865 6e20 6974  o the Op when it
-00000230: 2069 730a 2020 2020 2020 2020 6361 6c6c   is.        call
-00000240: 6564 2e20 496e 206f 7572 2063 6173 6520  ed. In our case 
-00000250: 7765 2077 696c 6c20 6265 2070 6173 7369  we will be passi
-00000260: 6e67 2069 7420 6120 7665 6374 6f72 206f  ng it a vector o
-00000270: 6620 7661 6c75 6573 2028 7468 6520 7061  f values (the pa
-00000280: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00000290: 2074 6861 7420 6465 6669 6e65 206f 7572   that define our
-000002a0: 206d 6f64 656c 2920 616e 6420 7265 7475   model) and retu
-000002b0: 726e 696e 6720 6120 7369 6e67 6c65 2022  rning a single "
-000002c0: 7363 616c 6172 2220 7661 6c75 6520 2874  scalar" value (t
-000002d0: 6865 0a20 2020 2020 2020 206c 6f67 2d6c  he.        log-l
-000002e0: 696b 656c 6968 6f6f 6429 0a20 2020 2020  ikelihood).     
-000002f0: 2020 2063 0100 0000 0000 0000 0000 0000     c............
-00000300: 0100 0000 0200 0000 1300 0000 730a 0000  ............s...
-00000310: 0088 007c 005f 0064 0153 0029 0261 1e01  ...|._.d.S.).a..
-00000320: 0000 0a20 2020 2020 2020 2020 2020 2049  ...            I
-00000330: 6e69 7469 616c 6973 6520 7468 6520 4f70  nitialise the Op
-00000340: 2077 6974 6820 7661 7269 6f75 7320 7468   with various th
-00000350: 696e 6773 2074 6861 7420 6f75 7220 6c6f  ings that our lo
-00000360: 672d 6c69 6b65 6c69 686f 6f64 2066 756e  g-likelihood fun
-00000370: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00000380: 2020 7265 7175 6972 6573 2e20 4265 6c6f    requires. Belo
-00000390: 7720 6172 6520 7468 6520 7468 696e 6773  w are the things
-000003a0: 2074 6861 7420 6172 6520 6e65 6564 6564   that are needed
-000003b0: 2069 6e20 7468 6973 2070 6172 7469 6375   in this particu
-000003c0: 6c61 720a 2020 2020 2020 2020 2020 2020  lar.            
-000003d0: 6578 616d 706c 652e 0a0a 2020 2020 2020  example...      
-000003e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000003f0: 0a20 2020 2020 2020 2020 2020 202d 2d2d  .            ---
-00000400: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00000410: 2020 2020 6263 6d3a 2042 6179 6573 6961      bcm: Bayesia
-00000420: 6e43 6f6d 7061 7274 6d65 6e74 616c 4d6f  nCompartmentalMo
-00000430: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-00000440: 4ea9 0172 0300 0000 2901 da04 7365 6c66  N..r....)...self
-00000450: 7204 0000 00a9 00fa 322f 6d6e 742f 632f  r.......2/mnt/c/
-00000460: 6465 762f 454d 552f 6573 7469 7661 6c2f  dev/EMU/estival/
-00000470: 6573 7469 7661 6c2f 6361 6c69 6272 6174  estival/calibrat
-00000480: 696f 6e2f 7079 6d63 2e70 79da 085f 5f69  ion/pymc.py..__i
-00000490: 6e69 745f 5f1c 0000 0073 0200 0000 0a0c  nit__....s......
-000004a0: 7a2b 6765 745f 7772 6170 7065 645f 6c6c  z+get_wrapped_ll
-000004b0: 2e3c 6c6f 6361 6c73 3e2e 4243 4d4c 6f67  .<locals>.BCMLog
-000004c0: 4c69 6b65 2e5f 5f69 6e69 745f 5f63 0400  Like.__init__c..
-000004d0: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-000004e0: 0000 1300 0000 7346 0000 007c 0289 0087  ......sF...|....
-000004f0: 0066 0164 0164 0284 0874 007c 006a 016a  .f.d.d...t.|.j.j
-00000500: 0283 0144 0083 017d 047c 006a 016a 0364  ...D...}.|.j.j.d
-00000510: 0469 007c 04a4 018e 017d 0574 04a0 057c  .i.|.....}.t...|
-00000520: 05a1 017c 0364 0319 0064 033c 0064 0053  ...|.d...d.<.d.S
-00000530: 0029 054e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00000540: 0003 0000 0005 0000 0013 0000 0073 1a00  .............s..
-00000550: 0000 6900 7c00 5d09 5c02 7d01 7d02 7c02  ..i.|.].\.}.}.|.
-00000560: 8800 7c01 1900 9302 7102 5300 7206 0000  ..|.....q.S.r...
-00000570: 0072 0600 0000 2903 da02 2e30 da01 69da  .r....)....0..i.
-00000580: 016b a901 da06 7061 7261 6d73 7206 0000  .k....paramsr...
-00000590: 0072 0700 0000 da0a 3c64 6963 7463 6f6d  .r......<dictcom
-000005a0: 703e 2c00 0000 7302 0000 001a 007a 3e67  p>,...s......z>g
-000005b0: 6574 5f77 7261 7070 6564 5f6c 6c2e 3c6c  et_wrapped_ll.<l
-000005c0: 6f63 616c 733e 2e42 434d 4c6f 674c 696b  ocals>.BCMLogLik
-000005d0: 652e 7065 7266 6f72 6d2e 3c6c 6f63 616c  e.perform.<local
-000005e0: 733e 2e3c 6469 6374 636f 6d70 3e72 0100  s>.<dictcomp>r..
-000005f0: 0000 7206 0000 0029 06da 0965 6e75 6d65  ..r....)...enume
-00000600: 7261 7465 7203 0000 00da 0670 7269 6f72  rater......prior
-00000610: 73da 0d6c 6f67 6c69 6b65 6c69 686f 6f64  s..loglikelihood
-00000620: da02 6e70 da05 6172 7261 7929 0672 0500  ..np..array).r..
-00000630: 0000 da04 6e6f 6465 da06 696e 7075 7473  ....node..inputs
-00000640: da07 6f75 7470 7574 73da 066b 7761 7267  ..outputs..kwarg
-00000650: 73da 046c 6f67 6c72 0600 0000 720c 0000  s..loglr....r...
-00000660: 0072 0700 0000 da07 7065 7266 6f72 6d2a  .r......perform*
-00000670: 0000 0073 0800 0000 0401 1a01 1203 1602  ...s............
-00000680: 7a2a 6765 745f 7772 6170 7065 645f 6c6c  z*get_wrapped_ll
-00000690: 2e3c 6c6f 6361 6c73 3e2e 4243 4d4c 6f67  .<locals>.BCMLog
-000006a0: 4c69 6b65 2e70 6572 666f 726d 4e29 0cda  Like.performN)..
-000006b0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000006c0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000006d0: 655f 5fda 075f 5f64 6f63 5f5f da02 7074  e__..__doc__..pt
-000006e0: da07 6473 6361 6c61 72da 036c 656e 7210  ..dscalar..lenr.
-000006f0: 0000 00da 0669 7479 7065 73da 066f 7479  .....itypes..oty
-00000700: 7065 7372 0800 0000 7219 0000 0072 0600  pesr....r....r..
-00000710: 0000 7204 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00000720: 00da 0a42 434d 4c6f 674c 696b 6511 0000  ...BCMLogLike...
-00000730: 0073 0c00 0000 0800 0401 1207 0801 0c02  .s..............
-00000740: 0c0e 7223 0000 0029 0272 1e00 0000 da02  ..r#...).r......
-00000750: 4f70 2902 7203 0000 0072 2300 0000 7206  Op).r....r#...r.
-00000760: 0000 0072 0400 0000 7207 0000 00da 0e67  ...r....r......g
-00000770: 6574 5f77 7261 7070 6564 5f6c 6c07 0000  et_wrapped_ll...
-00000780: 0073 0400 0000 160a 0422 7225 0000 0046  .s......."r%...F
-00000790: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
-000007a0: 0000 0000 0008 0000 0005 0000 0043 0000  .............C..
-000007b0: 0073 6200 0000 7400 7c00 8301 8300 7d02  .sb...t.|.....}.
-000007c0: 6700 7d03 7c00 6a01 a002 a100 4400 5d0b  g.}.|.j.....D.].
-000007d0: 5c02 7d04 7d05 7c03 a003 7c05 a004 a100  \.}.}.|...|.....
-000007e0: a101 0100 710c 6401 6402 8400 7c03 4400  ....q.d.d...|.D.
-000007f0: 8301 7d06 7405 a006 6403 7c02 7c06 8e00  ..}.t...d.|.|...
-00000800: a102 7d07 7c01 722f 7405 a007 6404 7c07  ..}.|.r/t...d.|.
-00000810: a102 0100 7c03 5300 2905 61a7 0100 0055  ....|.S.).a....U
-00000820: 7365 2061 2067 6976 656e 2042 6179 6573  se a given Bayes
-00000830: 6961 6e43 6f6d 7061 7274 6d65 6e74 616c  ianCompartmental
-00000840: 4d6f 6465 6c20 666f 7220 7079 6d63 2073  Model for pymc s
-00000850: 616d 706c 696e 670a 2020 2020 5468 6973  ampling.    This
-00000860: 2073 686f 756c 6420 6265 2063 616c 6c65   should be calle
-00000870: 6420 696e 7369 6465 2061 206d 6f64 656c  d inside a model
-00000880: 2063 6f6e 7465 7874 206c 696b 6520 736f   context like so
-00000890: 0a20 2020 200a 2020 2020 7769 7468 2070  .    .    with p
-000008a0: 6d2e 4d6f 6465 6c28 293a 0a20 2020 2020  m.Model():.     
-000008b0: 2020 2076 6172 6961 626c 6573 203d 2075     variables = u
-000008c0: 7365 5f6d 6f64 656c 2862 636d 290a 2020  se_model(bcm).  
-000008d0: 2020 2020 2020 706d 2e73 616d 706c 6528        pm.sample(
-000008e0: 7374 6570 3d5b 706d 2e44 454d 6574 726f  step=[pm.DEMetro
-000008f0: 706f 6c69 7328 7661 7269 6162 6c65 7329  polis(variables)
-00000900: 5d29 0a0a 2020 2020 4172 6773 3a0a 2020  ])..    Args:.  
-00000910: 2020 2020 2020 6263 6d3a 2054 6865 2042        bcm: The B
-00000920: 434d 2074 6f20 7573 6520 666f 7220 7361  CM to use for sa
-00000930: 6d70 6c69 6e67 0a20 2020 2020 2020 2069  mpling.        i
-00000940: 6e63 6c75 6465 5f6c 6c3a 2049 6e63 6c75  nclude_ll: Inclu
-00000950: 6465 206c 6f67 6c69 6b65 6c69 686f 6f64  de loglikelihood
-00000960: 2069 6e20 7468 6520 7361 6d70 6c65 206f   in the sample o
-00000970: 7574 7075 7473 0a0a 2020 2020 5265 7475  utputs..    Retu
-00000980: 726e 733a 0a20 2020 2020 2020 2054 6865  rns:.        The
-00000990: 206c 6973 7420 6f66 2076 6172 6961 626c   list of variabl
-000009a0: 6573 2074 6f20 6265 2070 6173 7365 6420  es to be passed 
-000009b0: 746f 2061 2073 616d 706c 6572 2073 7465  to a sampler ste
-000009c0: 700a 2020 2020 6301 0000 0000 0000 0000  p.    c.........
-000009d0: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-000009e0: 1600 0000 6700 7c00 5d07 7d01 7400 a001  ....g.|.].}.t...
-000009f0: 7c01 a101 9102 7102 5300 7206 0000 0029  |.....q.S.r....)
-00000a00: 0272 1e00 0000 da12 6173 5f74 656e 736f  .r......as_tenso
-00000a10: 725f 7661 7269 6162 6c65 2902 7209 0000  r_variable).r...
-00000a20: 00da 0176 7206 0000 0072 0600 0000 7207  ...vr....r....r.
-00000a30: 0000 00da 0a3c 6c69 7374 636f 6d70 3e4b  .....<listcomp>K
-00000a40: 0000 0073 0200 0000 1600 7a1d 7573 655f  ...s......z.use_
-00000a50: 6d6f 6465 6c2e 3c6c 6f63 616c 733e 2e3c  model.<locals>.<
-00000a60: 6c69 7374 636f 6d70 3e72 1100 0000 da07  listcomp>r......
-00000a70: 6c6f 676c 696b 6529 0872 2500 0000 7210  loglike).r%...r.
-00000a80: 0000 00da 0569 7465 6d73 da06 6170 7065  .....items..appe
-00000a90: 6e64 da07 746f 5f70 796d 63da 0270 6dda  nd..to_pymc..pm.
-00000aa0: 0950 6f74 656e 7469 616c da0d 4465 7465  .Potential..Dete
-00000ab0: 726d 696e 6973 7469 6329 0872 0300 0000  rministic).r....
-00000ac0: 5a0a 696e 636c 7564 655f 6c6c 7218 0000  Z.include_llr...
-00000ad0: 005a 0b70 796d 635f 7072 696f 7273 720b  .Z.pymc_priorsr.
-00000ae0: 0000 00da 0570 7269 6f72 da06 696e 7661  .....prior..inva
-00000af0: 7273 da03 706f 7472 0600 0000 7206 0000  rs..potr....r...
-00000b00: 0072 0700 0000 da09 7573 655f 6d6f 6465  .r......use_mode
-00000b10: 6c35 0000 0073 1200 0000 0a0f 0402 1202  l5...s..........
-00000b20: 1001 0e02 1003 0402 0c01 0402 7234 0000  ............r4..
-00000b30: 0029 0146 290c da05 6e75 6d70 7972 1200  .).F)...numpyr..
-00000b40: 0000 da04 7079 6d63 722e 0000 00da 0f70  ....pymcr......p
-00000b50: 7974 656e 736f 722e 7465 6e73 6f72 da06  ytensor.tensor..
-00000b60: 7465 6e73 6f72 721e 0000 00da 0d65 7374  tensorr......est
-00000b70: 6976 616c 2e6d 6f64 656c 7202 0000 0072  ival.modelr....r
-00000b80: 2500 0000 da04 6c69 7374 7234 0000 0072  %.....listr4...r
-00000b90: 0600 0000 7206 0000 0072 0600 0000 7207  ....r....r....r.
-00000ba0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000bb0: 0073 0c00 0000 0800 0801 0c01 0c02 0e02  .s..............
-00000bc0: 182e                                     ..
+00000050: 6d08 5a08 0100 6400 6401 6c09 5a09 6403  m.Z...d.d.l.Z.d.
+00000060: 6508 6602 6404 6405 8404 5a0a 640c 6403  e.f.d.d...Z.d.d.
+00000070: 6508 6407 650b 6604 6408 6409 8405 5a0c  e.d.e.f.d.d...Z.
+00000080: 640a 640b 8400 5a0d 6401 5300 290d e900  d.d...Z.d.S.)...
+00000090: 0000 004e 2901 da1a 4261 7965 7369 616e  ...N)...Bayesian
+000000a0: 436f 6d70 6172 746d 656e 7461 6c4d 6f64  CompartmentalMod
+000000b0: 656c da03 6263 6d63 0100 0000 0000 0000  el..bcmc........
+000000c0: 0000 0000 0400 0000 0400 0000 0300 0000  ................
+000000d0: 7358 0000 0067 0089 0188 006a 00a0 01a1  sX...g.....j....
+000000e0: 0044 005d 165c 027d 017d 027c 026a 0264  .D.].\.}.}.|.j.d
+000000f0: 016b 0472 1788 01a0 0374 046a 05a1 0101  .k.r.....t.j....
+00000100: 0071 0788 01a0 0374 046a 06a1 0101 0071  .q.....t.j.....q
+00000110: 0747 0087 0087 0166 0264 0264 0384 0864  .G.....f.d.d...d
+00000120: 0374 046a 0783 037d 037c 0353 0029 047a  .t.j...}.|.S.).z
+00000130: 745f 7375 6d6d 6172 795f 0a0a 2020 2020  t_summary_..    
+00000140: 4172 6773 3a0a 2020 2020 2020 2020 6263  Args:.        bc
+00000150: 6d3a 2054 6865 206d 6f64 656c 2074 6f20  m: The model to 
+00000160: 7772 6170 0a0a 2020 2020 5265 7475 726e  wrap..    Return
+00000170: 733a 0a20 2020 2020 2020 2041 2077 7261  s:.        A wra
+00000180: 7070 6564 2070 7974 656e 736f 7220 6f70  pped pytensor op
+00000190: 2066 6f72 2075 7365 2069 6e20 7079 6d63   for use in pymc
+000001a0: 0a20 2020 20e9 0100 0000 6300 0000 0000  .    .....c.....
+000001b0: 0000 0000 0000 0000 0000 0003 0000 0000  ................
+000001c0: 0000 0073 3000 0000 6500 5a01 6400 5a02  ...s0...e.Z.d.Z.
+000001d0: 6401 5a03 9401 5a04 6505 6a06 6701 5a07  d.Z...Z.e.j.g.Z.
+000001e0: 8700 6601 6402 6403 8408 5a08 6404 6405  ..f.d.d...Z.d.d.
+000001f0: 8400 5a09 6406 5300 2907 7a22 6765 745f  ..Z.d.S.).z"get_
+00000200: 7772 6170 7065 645f 6c6c 2e3c 6c6f 6361  wrapped_ll.<loca
+00000210: 6c73 3e2e 4243 4d4c 6f67 4c69 6b65 6115  ls>.BCMLogLikea.
+00000220: 0100 000a 2020 2020 2020 2020 5370 6563  ....        Spec
+00000230: 6966 7920 7768 6174 2074 7970 6520 6f66  ify what type of
+00000240: 206f 626a 6563 7420 7769 6c6c 2062 6520   object will be 
+00000250: 7061 7373 6564 2061 6e64 2072 6574 7572  passed and retur
+00000260: 6e65 6420 746f 2074 6865 204f 7020 7768  ned to the Op wh
+00000270: 656e 2069 7420 6973 0a20 2020 2020 2020  en it is.       
+00000280: 2063 616c 6c65 642e 2049 6e20 6f75 7220   called. In our 
+00000290: 6361 7365 2077 6520 7769 6c6c 2062 6520  case we will be 
+000002a0: 7061 7373 696e 6720 6974 2061 2076 6563  passing it a vec
+000002b0: 746f 7220 6f66 2076 616c 7565 7320 2874  tor of values (t
+000002c0: 6865 2070 6172 616d 6574 6572 730a 2020  he parameters.  
+000002d0: 2020 2020 2020 7468 6174 2064 6566 696e        that defin
+000002e0: 6520 6f75 7220 6d6f 6465 6c29 2061 6e64  e our model) and
+000002f0: 2072 6574 7572 6e69 6e67 2061 2073 696e   returning a sin
+00000300: 676c 6520 2273 6361 6c61 7222 2076 616c  gle "scalar" val
+00000310: 7565 2028 7468 650a 2020 2020 2020 2020  ue (the.        
+00000320: 6c6f 672d 6c69 6b65 6c69 686f 6f64 290a  log-likelihood).
+00000330: 2020 2020 2020 2020 6301 0000 0000 0000          c.......
+00000340: 0000 0000 0001 0000 0002 0000 0013 0000  ................
+00000350: 0073 0a00 0000 8800 7c00 5f00 6401 5300  .s......|._.d.S.
+00000360: 2902 611e 0100 000a 2020 2020 2020 2020  ).a.....        
+00000370: 2020 2020 496e 6974 6961 6c69 7365 2074      Initialise t
+00000380: 6865 204f 7020 7769 7468 2076 6172 696f  he Op with vario
+00000390: 7573 2074 6869 6e67 7320 7468 6174 206f  us things that o
+000003a0: 7572 206c 6f67 2d6c 696b 656c 6968 6f6f  ur log-likelihoo
+000003b0: 6420 6675 6e63 7469 6f6e 0a20 2020 2020  d function.     
+000003c0: 2020 2020 2020 2072 6571 7569 7265 732e         requires.
+000003d0: 2042 656c 6f77 2061 7265 2074 6865 2074   Below are the t
+000003e0: 6869 6e67 7320 7468 6174 2061 7265 206e  hings that are n
+000003f0: 6565 6465 6420 696e 2074 6869 7320 7061  eeded in this pa
+00000400: 7274 6963 756c 6172 0a20 2020 2020 2020  rticular.       
+00000410: 2020 2020 2065 7861 6d70 6c65 2e0a 0a20       example... 
+00000420: 2020 2020 2020 2020 2020 2050 6172 616d             Param
+00000430: 6574 6572 730a 2020 2020 2020 2020 2020  eters.          
+00000440: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00000450: 2020 2020 2020 2020 2062 636d 3a20 4261           bcm: Ba
+00000460: 7965 7369 616e 436f 6d70 6172 746d 656e  yesianCompartmen
+00000470: 7461 6c4d 6f64 656c 0a20 2020 2020 2020  talModel.       
+00000480: 2020 2020 204e a901 7203 0000 0029 01da       N..r....)..
+00000490: 0473 656c 6672 0500 0000 a900 fa2e 433a  .selfr........C:
+000004a0: 5c64 6576 5c45 4d55 5c65 7374 6976 616c  \dev\EMU\estival
+000004b0: 5c65 7374 6976 616c 5c63 616c 6962 7261  \estival\calibra
+000004c0: 7469 6f6e 5c70 796d 632e 7079 da08 5f5f  tion\pymc.py..__
+000004d0: 696e 6974 5f5f 2b00 0000 7302 0000 000a  init__+...s.....
+000004e0: 0c7a 2b67 6574 5f77 7261 7070 6564 5f6c  .z+get_wrapped_l
+000004f0: 6c2e 3c6c 6f63 616c 733e 2e42 434d 4c6f  l.<locals>.BCMLo
+00000500: 674c 696b 652e 5f5f 696e 6974 5f5f 6304  gLike.__init__c.
+00000510: 0000 0000 0000 0000 0000 0006 0000 0004  ................
+00000520: 0000 0013 0000 0073 4600 0000 7c02 8900  .......sF...|...
+00000530: 8700 6601 6401 6402 8408 7400 7c00 6a01  ..f.d.d...t.|.j.
+00000540: 6a02 8301 4400 8301 7d04 7c00 6a01 6a03  j...D...}.|.j.j.
+00000550: 6404 6900 7c04 a401 8e01 7d05 7404 a005  d.i.|.....}.t...
+00000560: 7c05 a101 7c03 6403 1900 6403 3c00 6400  |...|.d...d.<.d.
+00000570: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000580: 0000 0300 0000 0500 0000 1300 0000 731a  ..............s.
+00000590: 0000 0069 007c 005d 095c 027d 017d 027c  ...i.|.].\.}.}.|
+000005a0: 0288 007c 0119 0093 0271 0253 0072 0700  ...|.....q.S.r..
+000005b0: 0000 7207 0000 0029 03da 022e 30da 0169  ..r....)....0..i
+000005c0: da01 6ba9 01da 0670 6172 616d 7372 0700  ..k....paramsr..
+000005d0: 0000 7208 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
+000005e0: 6d70 3e3b 0000 0073 0200 0000 1a00 7a3e  mp>;...s......z>
+000005f0: 6765 745f 7772 6170 7065 645f 6c6c 2e3c  get_wrapped_ll.<
+00000600: 6c6f 6361 6c73 3e2e 4243 4d4c 6f67 4c69  locals>.BCMLogLi
+00000610: 6b65 2e70 6572 666f 726d 2e3c 6c6f 6361  ke.perform.<loca
+00000620: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7201  ls>.<dictcomp>r.
+00000630: 0000 0072 0700 0000 2906 da09 656e 756d  ...r....)...enum
+00000640: 6572 6174 6572 0300 0000 da06 7072 696f  erater......prio
+00000650: 7273 da0d 6c6f 676c 696b 656c 6968 6f6f  rs..loglikelihoo
+00000660: 64da 026e 70da 0561 7272 6179 2906 7206  d..np..array).r.
+00000670: 0000 00da 046e 6f64 65da 0669 6e70 7574  .....node..input
+00000680: 73da 076f 7574 7075 7473 da06 6b77 6172  s..outputs..kwar
+00000690: 6773 da04 6c6f 676c 7207 0000 0072 0d00  gs..loglr....r..
+000006a0: 0000 7208 0000 00da 0770 6572 666f 726d  ..r......perform
+000006b0: 3900 0000 7308 0000 0004 011a 0112 0316  9...s...........
+000006c0: 027a 2a67 6574 5f77 7261 7070 6564 5f6c  .z*get_wrapped_l
+000006d0: 6c2e 3c6c 6f63 616c 733e 2e42 434d 4c6f  l.<locals>.BCMLo
+000006e0: 674c 696b 652e 7065 7266 6f72 6d4e 290a  gLike.performN).
+000006f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000700: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000710: 6d65 5f5f da07 5f5f 646f 635f 5fda 0669  me__..__doc__..i
+00000720: 7479 7065 73da 0270 74da 0764 7363 616c  types..pt..dscal
+00000730: 6172 da06 6f74 7970 6573 7209 0000 0072  ar..otypesr....r
+00000740: 1a00 0000 7207 0000 00a9 0272 0300 0000  ....r......r....
+00000750: 5a0b 7072 696f 725f 7479 7065 7372 0700  Z.prior_typesr..
+00000760: 0000 7208 0000 00da 0a42 434d 4c6f 674c  ..r......BCMLogL
+00000770: 696b 651c 0000 0073 0c00 0000 0800 0401  ike....s........
+00000780: 0407 0805 0c02 0c0e 7224 0000 0029 0872  ........r$...).r
+00000790: 1100 0000 da05 6974 656d 73da 0473 697a  ......items..siz
+000007a0: 65da 0661 7070 656e 6472 2000 0000 da07  e..appendr .....
+000007b0: 6476 6563 746f 7272 2100 0000 da02 4f70  dvectorr!.....Op
+000007c0: 2904 7203 0000 0072 0c00 0000 da05 7072  ).r....r......pr
+000007d0: 696f 7272 2400 0000 7207 0000 0072 2300  iorr$...r....r#.
+000007e0: 0000 7208 0000 00da 0e67 6574 5f77 7261  ..r......get_wra
+000007f0: 7070 6564 5f6c 6c0a 0000 0073 0e00 0000  pped_ll....s....
+00000800: 040a 1201 0a01 0e01 0e02 1803 0426 722b  .............&r+
+00000810: 0000 0046 da06 7265 7475 726e 6302 0000  ...F..returnc...
+00000820: 0000 0000 0000 0000 0008 0000 0005 0000  ................
+00000830: 0043 0000 0073 6200 0000 7400 7c00 8301  .C...sb...t.|...
+00000840: 8300 7d02 6700 7d03 7c00 6a01 a002 a100  ..}.g.}.|.j.....
+00000850: 4400 5d0b 5c02 7d04 7d05 7c03 a003 7c05  D.].\.}.}.|...|.
+00000860: a004 a100 a101 0100 710c 6401 6402 8400  ........q.d.d...
+00000870: 7c03 4400 8301 7d06 7405 a006 6403 7c02  |.D...}.t...d.|.
+00000880: 7c06 8e00 a102 7d07 7c01 722f 7405 a007  |.....}.|.r/t...
+00000890: 6404 7c07 a102 0100 7c03 5300 2905 61a3  d.|.....|.S.).a.
+000008a0: 0100 0055 7365 2061 2067 6976 656e 2042  ...Use a given B
+000008b0: 6179 6573 6961 6e43 6f6d 7061 7274 6d65  ayesianCompartme
+000008c0: 6e74 616c 4d6f 6465 6c20 666f 7220 7079  ntalModel for py
+000008d0: 6d63 2073 616d 706c 696e 670a 2020 2020  mc sampling.    
+000008e0: 5468 6973 2073 686f 756c 6420 6265 2063  This should be c
+000008f0: 616c 6c65 6420 696e 7369 6465 2061 206d  alled inside a m
+00000900: 6f64 656c 2063 6f6e 7465 7874 206c 696b  odel context lik
+00000910: 6520 736f 0a0a 2020 2020 7769 7468 2070  e so..    with p
+00000920: 6d2e 4d6f 6465 6c28 293a 0a20 2020 2020  m.Model():.     
+00000930: 2020 2076 6172 6961 626c 6573 203d 2075     variables = u
+00000940: 7365 5f6d 6f64 656c 2862 636d 290a 2020  se_model(bcm).  
+00000950: 2020 2020 2020 706d 2e73 616d 706c 6528        pm.sample(
+00000960: 7374 6570 3d5b 706d 2e44 454d 6574 726f  step=[pm.DEMetro
+00000970: 706f 6c69 7328 7661 7269 6162 6c65 7329  polis(variables)
+00000980: 5d29 0a0a 2020 2020 4172 6773 3a0a 2020  ])..    Args:.  
+00000990: 2020 2020 2020 6263 6d3a 2054 6865 2042        bcm: The B
+000009a0: 434d 2074 6f20 7573 6520 666f 7220 7361  CM to use for sa
+000009b0: 6d70 6c69 6e67 0a20 2020 2020 2020 2069  mpling.        i
+000009c0: 6e63 6c75 6465 5f6c 6c3a 2049 6e63 6c75  nclude_ll: Inclu
+000009d0: 6465 206c 6f67 6c69 6b65 6c69 686f 6f64  de loglikelihood
+000009e0: 2069 6e20 7468 6520 7361 6d70 6c65 206f   in the sample o
+000009f0: 7574 7075 7473 0a0a 2020 2020 5265 7475  utputs..    Retu
+00000a00: 726e 733a 0a20 2020 2020 2020 2054 6865  rns:.        The
+00000a10: 206c 6973 7420 6f66 2076 6172 6961 626c   list of variabl
+00000a20: 6573 2074 6f20 6265 2070 6173 7365 6420  es to be passed 
+00000a30: 746f 2061 2073 616d 706c 6572 2073 7465  to a sampler ste
+00000a40: 700a 2020 2020 6301 0000 0000 0000 0000  p.    c.........
+00000a50: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
+00000a60: 1600 0000 6700 7c00 5d07 7d01 7400 a001  ....g.|.].}.t...
+00000a70: 7c01 a101 9102 7102 5300 7207 0000 0029  |.....q.S.r....)
+00000a80: 0272 2000 0000 da12 6173 5f74 656e 736f  .r .....as_tenso
+00000a90: 725f 7661 7269 6162 6c65 2902 720a 0000  r_variable).r...
+00000aa0: 00da 0176 7207 0000 0072 0700 0000 7208  ...vr....r....r.
+00000ab0: 0000 00da 0a3c 6c69 7374 636f 6d70 3e5b  .....<listcomp>[
+00000ac0: 0000 0073 0200 0000 1600 7a1d 7573 655f  ...s......z.use_
+00000ad0: 6d6f 6465 6c2e 3c6c 6f63 616c 733e 2e3c  model.<locals>.<
+00000ae0: 6c69 7374 636f 6d70 3e72 1200 0000 da07  listcomp>r......
+00000af0: 6c6f 676c 696b 6529 0872 2b00 0000 7211  loglike).r+...r.
+00000b00: 0000 0072 2500 0000 7227 0000 00da 0774  ...r%...r'.....t
+00000b10: 6f5f 7079 6d63 da02 706d da09 506f 7465  o_pymc..pm..Pote
+00000b20: 6e74 6961 6cda 0d44 6574 6572 6d69 6e69  ntial..Determini
+00000b30: 7374 6963 2908 7203 0000 00da 0a69 6e63  stic).r......inc
+00000b40: 6c75 6465 5f6c 6c72 1900 0000 5a0b 7079  lude_llr....Z.py
+00000b50: 6d63 5f70 7269 6f72 7372 0c00 0000 722a  mc_priorsr....r*
+00000b60: 0000 00da 0669 6e76 6172 73da 0370 6f74  .....invars..pot
+00000b70: 7207 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+00000b80: 0975 7365 5f6d 6f64 656c 4500 0000 7312  .use_modelE...s.
+00000b90: 0000 000a 0f04 0212 0210 010e 0210 0304  ................
+00000ba0: 020c 0104 0272 3800 0000 6302 0000 0000  .....r8...c.....
+00000bb0: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00000bc0: 0000 0073 5400 0000 7400 a001 7c00 a101  ...sT...t...|...
+00000bd0: 7d02 7402 a003 a100 8f17 7d03 7404 7c02  }.t.......}.t.|.
+00000be0: 6401 6402 8d02 7d04 7402 6a05 7c01 6401  d.d...}.t.j.|.d.
+00000bf0: 6401 6403 8d03 7d05 5700 6400 0400 0400  d.d...}.W.d.....
+00000c00: 8303 0100 7c05 5300 3100 7323 7701 0100  ....|.S.1.s#w...
+00000c10: 0100 0100 5900 0100 7c05 5300 2904 4e46  ....Y...|.S.).NF
+00000c20: 2901 7235 0000 0029 02da 1369 6e63 6c75  ).r5...)...inclu
+00000c30: 6465 5f74 7261 6e73 666f 726d 6564 da0b  de_transformed..
+00000c40: 7072 6f67 7265 7373 6261 7229 06da 0b63  progressbar)...c
+00000c50: 6c6f 7564 7069 636b 6c65 da05 6c6f 6164  loudpickle..load
+00000c60: 7372 3200 0000 da05 4d6f 6465 6c72 3800  sr2.....Modelr8.
+00000c70: 0000 da08 6669 6e64 5f4d 4150 2906 5a07  ....find_MAP).Z.
+00000c80: 6263 6d5f 706b 6cda 0469 7661 6c72 0300  bcm_pkl..ivalr..
+00000c90: 0000 da05 6d6f 6465 6cda 0976 6172 6961  ....model..varia
+00000ca0: 626c 6573 5a07 6d61 705f 6573 7472 0700  blesZ.map_estr..
+00000cb0: 0000 7207 0000 0072 0800 0000 da07 7275  ..r....r......ru
+00000cc0: 6e5f 6d61 7066 0000 0073 1000 0000 0a01  n_mapf...s......
+00000cd0: 0a01 0c01 1201 0afe 0403 10fd 0403 7242  ..............rB
+00000ce0: 0000 0029 0146 290e da05 6e75 6d70 7972  ...).F)...numpyr
+00000cf0: 1300 0000 da04 7079 6d63 7232 0000 00da  ......pymcr2....
+00000d00: 0f70 7974 656e 736f 722e 7465 6e73 6f72  .pytensor.tensor
+00000d10: da06 7465 6e73 6f72 7220 0000 00da 0d65  ..tensorr .....e
+00000d20: 7374 6976 616c 2e6d 6f64 656c 7202 0000  stival.modelr...
+00000d30: 0072 3b00 0000 722b 0000 00da 046c 6973  .r;...r+.....lis
+00000d40: 7472 3800 0000 7242 0000 0072 0700 0000  tr8...rB...r....
+00000d50: 7207 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+00000d60: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
+00000d70: 0000 0800 0801 0c01 0c02 0802 0e03 143b  ...............;
+00000d80: 0c21                                     .!
```

### Comparing `estival-0.2.3/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc` & `estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc` & `estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc` & `estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/calibration/mcmc/adaptive.py` & `estival-0.2.4/estival/calibration/mcmc/adaptive.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/calibration/mcmc/covariance.py` & `estival-0.2.4/estival/calibration/mcmc/covariance.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/calibration/mcmc/transformations.py` & `estival-0.2.4/estival/calibration/mcmc/transformations.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/calibration/pymc.py` & `estival-0.2.4/estival/calibration/pymc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,107 @@
-import numpy as np
-import pymc as pm
-import pytensor.tensor as pt
-
-from estival.model import BayesianCompartmentalModel
-
-def get_wrapped_ll(bcm: BayesianCompartmentalModel):
-    """_summary_
-
-    Args:
-        bcm: The model to wrap
-
-    Returns:
-        A wrapped pytensor op for use in pymc
-    """
-    # define a pytensor Op for our likelihood function
-    class BCMLogLike(pt.Op):
-        """
-        Specify what type of object will be passed and returned to the Op when it is
-        called. In our case we will be passing it a vector of values (the parameters
-        that define our model) and returning a single "scalar" value (the
-        log-likelihood)
-        """
-
-        itypes = [pt.dscalar] * len(bcm.priors)#[pt.dvector]  # expects a vector of parameter values when called
-        otypes = [pt.dscalar]  # outputs a single scalar value (the log likelihood)
-
-        def __init__(self):
-            """
-            Initialise the Op with various things that our log-likelihood function
-            requires. Below are the things that are needed in this particular
-            example.
-
-            Parameters
-            ----------
-            bcm: BayesianCompartmentalModel
-            """
-
-            # Capture the BayesianCompartmentalModel
-            self.bcm = bcm
-
-        def perform(self, node, inputs, outputs):
-            params = inputs
-            kwargs = {k:params[i] for i,k in enumerate(self.bcm.priors)}
-
-            # call the log-likelihood function
-            logl = self.bcm.loglikelihood(**kwargs)
-
-            outputs[0][0] = np.array(logl)  # output the log-likelihood
-            
-    return BCMLogLike
-
-def use_model(bcm: BayesianCompartmentalModel, include_ll=False) -> list:
-    """Use a given BayesianCompartmentalModel for pymc sampling
-    This should be called inside a model context like so
-    
-    with pm.Model():
-        variables = use_model(bcm)
-        pm.sample(step=[pm.DEMetropolis(variables)])
-
-    Args:
-        bcm: The BCM to use for sampling
-        include_ll: Include loglikelihood in the sample outputs
-
-    Returns:
-        The list of variables to be passed to a sampler step
-    """
-    logl = get_wrapped_ll(bcm)()
-
-    pymc_priors = []
-
-    for k, prior in bcm.priors.items():
-        pymc_priors.append(prior.to_pymc())
-
-    invars = [pt.as_tensor_variable(v) for v in pymc_priors]
-
-    # use a Potential to "call" the Op and include it in the logp computation
-    pot = pm.Potential("loglikelihood", logl(*invars))
-
-    if include_ll:
-        pm.Deterministic("loglike", pot)
-    
-    return pymc_priors
+import numpy as np
+import pymc as pm
+import pytensor.tensor as pt
+
+from estival.model import BayesianCompartmentalModel
+
+import cloudpickle
+
+
+def get_wrapped_ll(bcm: BayesianCompartmentalModel):
+    """_summary_
+
+    Args:
+        bcm: The model to wrap
+
+    Returns:
+        A wrapped pytensor op for use in pymc
+    """
+
+    prior_types = []
+    for k, prior in bcm.priors.items():
+        if prior.size > 1:
+            prior_types.append(pt.dvector)
+        else:
+            prior_types.append(pt.dscalar)
+
+    # define a pytensor Op for our likelihood function
+    class BCMLogLike(pt.Op):
+        """
+        Specify what type of object will be passed and returned to the Op when it is
+        called. In our case we will be passing it a vector of values (the parameters
+        that define our model) and returning a single "scalar" value (the
+        log-likelihood)
+        """
+
+        itypes = prior_types
+
+        # [pt.dscalar] * len(
+        #    bcm.priors
+        # )  # [pt.dvector]  # expects a vector of parameter values when called
+        otypes = [pt.dscalar]  # outputs a single scalar value (the log likelihood)
+
+        def __init__(self):
+            """
+            Initialise the Op with various things that our log-likelihood function
+            requires. Below are the things that are needed in this particular
+            example.
+
+            Parameters
+            ----------
+            bcm: BayesianCompartmentalModel
+            """
+
+            # Capture the BayesianCompartmentalModel
+            self.bcm = bcm
+
+        def perform(self, node, inputs, outputs):
+            params = inputs
+            kwargs = {k: params[i] for i, k in enumerate(self.bcm.priors)}
+
+            # call the log-likelihood function
+            logl = self.bcm.loglikelihood(**kwargs)
+
+            outputs[0][0] = np.array(logl)  # output the log-likelihood
+
+    return BCMLogLike
+
+
+def use_model(bcm: BayesianCompartmentalModel, include_ll=False) -> list:
+    """Use a given BayesianCompartmentalModel for pymc sampling
+    This should be called inside a model context like so
+
+    with pm.Model():
+        variables = use_model(bcm)
+        pm.sample(step=[pm.DEMetropolis(variables)])
+
+    Args:
+        bcm: The BCM to use for sampling
+        include_ll: Include loglikelihood in the sample outputs
+
+    Returns:
+        The list of variables to be passed to a sampler step
+    """
+    logl = get_wrapped_ll(bcm)()
+
+    pymc_priors = []
+
+    for k, prior in bcm.priors.items():
+        pymc_priors.append(prior.to_pymc())
+
+    invars = [pt.as_tensor_variable(v) for v in pymc_priors]
+
+    # use a Potential to "call" the Op and include it in the logp computation
+    pot = pm.Potential("loglikelihood", logl(*invars))
+
+    if include_ll:
+        pm.Deterministic("loglike", pot)
+
+    return pymc_priors
+
+
+def run_map(bcm_pkl, ival):
+    bcm = cloudpickle.loads(bcm_pkl)
+    with pm.Model() as model:
+        variables = use_model(bcm, include_ll=False)
+        map_est = pm.find_MAP(ival, include_transformed=False, progressbar=False)
+    return map_est
```

### Comparing `estival-0.2.3/estival/model.py` & `estival-0.2.4/estival/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,33 +21,34 @@
         self.parameters = parameters
         self.targets = {t.name: t for t in targets}
 
         for t in targets:
             priors = priors + t.get_priors()
         self.priors = {p.name: p for p in priors}
 
+        self._ref_idx = self.model._get_ref_idx()
+        self.epoch = self.model.get_epoch()
+
         self.loglikelihood = self._build_logll_func(extra_ll)
 
-        self._ref_idx = self.model._get_ref_idx()
+
 
     def _build_logll_func(self, extra_ll=None):
         model_params = self.model.get_input_parameters()
         dyn_params = list(model_params.intersection(set(self.priors)))
         self.model.set_derived_outputs_whitelist(list(self.targets))
 
         self._ll_runner = self.model.get_runner(self.parameters, dyn_params)
 
         self.model.set_derived_outputs_whitelist([])
         self._full_runner = self.model.get_runner(self.parameters, dyn_params)
 
-        tidx = pd.Index(self.model.times)
-
         self._evaluators = {}
         for k, t in self.targets.items():
-            tev = t.get_evaluator(tidx)
+            tev = t.get_evaluator(self._ref_idx, self.epoch)
             self._evaluators[k] = tev.evaluate
 
         @jit
         def logll(**kwargs):
             dict_args = capture_model_kwargs(self.model, **kwargs)
             res = self._ll_runner._run_func(dict_args)["derived_outputs"]
```

### Comparing `estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-310.pyc` & `estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-311.pyc` & `estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0xb1d25164 (Wed May  3 03:19:13 2023 UTC)
-files sz: 2716
+moddate:  0x63cb5264 (Wed May  3 21:00:19 2023 UTC)
+files sz: 2635
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 11
+   stacksize : 13
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c065a07640064056c086d095a09010064
       0064066c0a6d0b5a0b01000900640064046c0c5a0d6e072300010059006e
-      037803590077016413640884015a0e0200470064098400640aa6020000ab
+      037803590077016414640884015a0e0200470064098400640aa6020000ab
       0200000000000000005a0f640b650d6a1000000000000000006a11000000
-      00000000006404640464076501640c6607640d6509640e6512640f651264
-      10651364116514660a641284055a1564045300
+      00000000006404640464076404640c6607640d6509640e6512640f651264
+      1065136411651464126501660c641384055a1564045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Callable',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Callable)
                 10 STORE_NAME               1 (Callable)
@@ -69,15 +69,15 @@
    
     15          86 POP_EXCEPT
                 88 JUMP_FORWARD             3 (to 96)
            >>   90 COPY                     3
                 92 POP_EXCEPT
                 94 RERAISE                  1
    
-    18     >>   96 LOAD_CONST              19 ((None, 'midpoint'))
+    18     >>   96 LOAD_CONST              20 ((None, 'midpoint'))
                 98 LOAD_CONST               8 (<code object get_instrumentation, file "/mnt/c/dev/EMU/estival/estival/optimization/nevergrad.py", line 18>)
                100 MAKE_FUNCTION            1 (defaults)
                102 STORE_NAME              14 (get_instrumentation)
    
     45         104 PUSH_NULL
                106 LOAD_BUILD_CLASS
                108 LOAD_CONST               9 (<code object OptRunner, file "/mnt/c/dev/EMU/estival/estival/optimization/nevergrad.py", line 45>)
@@ -95,15 +95,15 @@
    
     63         154 LOAD_CONST               4 (None)
    
     64         156 LOAD_CONST               4 (None)
    
     65         158 LOAD_CONST               7 ('midpoint')
    
-    66         160 LOAD_NAME                1 (Callable)
+    66         160 LOAD_CONST               4 (None)
    
     67         162 LOAD_CONST              12 (True)
    
     59         164 BUILD_TUPLE              7
                166 LOAD_CONST              13 ('bcm')
    
     60         168 LOAD_NAME                9 (BayesianCompartmentalModel)
@@ -120,20 +120,24 @@
    
     64         180 LOAD_NAME               19 (dict)
    
     59         182 LOAD_CONST              17 ('init_method')
    
     65         184 LOAD_NAME               20 (str)
    
-    59         186 BUILD_TUPLE             10
-               188 LOAD_CONST              18 (<code object optimize_model, file "/mnt/c/dev/EMU/estival/estival/optimization/nevergrad.py", line 59>)
-               190 MAKE_FUNCTION            5 (defaults, annotations)
-               192 STORE_NAME              21 (optimize_model)
-               194 LOAD_CONST               4 (None)
-               196 RETURN_VALUE
+    59         186 LOAD_CONST              18 ('obj_function')
+   
+    66         188 LOAD_NAME                1 (Callable)
+   
+    59         190 BUILD_TUPLE             12
+               192 LOAD_CONST              19 (<code object optimize_model, file "/mnt/c/dev/EMU/estival/estival/optimization/nevergrad.py", line 59>)
+               194 MAKE_FUNCTION            5 (defaults, annotations)
+               196 STORE_NAME              21 (optimize_model)
+               198 LOAD_CONST               4 (None)
+               200 RETURN_VALUE
    ExceptionTable:
      72 to 78 -> 82 [0]
      82 to 84 -> 90 [1] lasti
    consts
       0
       ('Callable',)
       ('futures',)
@@ -498,14 +502,15 @@
       1000
       True
       'bcm'
       'budget'
       'num_workers'
       'suggested'
       'init_method'
+      'obj_function'
       code
          argcount  : 8
          nlocals   : 12
          stacksize : 5
          flags     : 3
          code
             0x97007c03730e740100000000000000000000a6000000ab000000000000
@@ -663,8 +668,8 @@
    cellvars   ()
    filename   '/mnt/c/dev/EMU/estival/estival/optimization/nevergrad.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c020c010c0108020c010c0402010c0102010a03081b1a1002
       011601020102010201020102f8040102ff020202fe020402fc020502fb02
-      0602fa
+      0602fa020702f9
```

### Comparing `estival-0.2.3/estival/optimization/nevergrad.py` & `estival-0.2.4/estival/optimization/nevergrad.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/estival/priors.py` & `estival-0.2.4/estival/priors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Tuple, Union
 from abc import ABC
 
+import numpy as np
 from scipy import stats
 from scipy.optimize import minimize
 
 # pymc is optional - just be silent on failed import
 try:
     import pymc as pm
 except:
@@ -102,15 +103,21 @@
         super().__init__(name)
         self.start, self.end = domain
         self.distri_params = {"loc": self.start, "scale": self.end - self.start}
         self.rv = stats.uniform(**self.distri_params)
         self.size = size
 
     def to_pymc(self):
-        return pm.Uniform(self.name, lower=self.start, upper=self.end)
+        if self.size > 1:
+            lower = np.repeat(self.start, self.size)
+            upper = np.repeat(self.end, self.size)
+        else:
+            lower, upper = self.start, self.end
+        return pm.Uniform(self.name, lower=lower, upper=upper)
+
 
 class TruncNormalPrior(BasePrior):
     """
     A prior with a truncated normal distribution.
     """
 
     def __init__(self, name: str, mean: float, stdev: float, trunc_range: Tuple[float, float]):
@@ -123,8 +130,15 @@
             "a": (trunc_range[0] - mean) / stdev,
             "b": (trunc_range[1] - mean) / stdev,
         }
         self.rv = stats.truncnorm(**self.distri_params)
 
     def to_pymc(self):
         lower, upper = self.trunc_range
-        return pm.TruncatedNormal(self.name, mu=self.mean, sigma=self.stdev, lower=lower, upper=upper)
+        if self.size > 1:
+            lower = np.repeat(self.start, self.size)
+            upper = np.repeat(self.start, self.size)
+        else:
+            lower, upper = self.start, self.end
+        return pm.TruncatedNormal(
+            self.name, mu=self.mean, sigma=self.stdev, lower=lower, upper=upper
+        )
```

### Comparing `estival-0.2.3/estival/targets.py` & `estival-0.2.4/estival/targets.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from copy import copy
 
 import pandas as pd
 import numpy as np
 
 from jax import jit, scipy as jsp, numpy as jnp
 
+from summer2.utils import Epoch
+
 from .priors import DistriParam, BasePrior
 
 
 class BaseTarget(ABC):
     name: str
     data: pd.Series
     _data_attrs: List = []
@@ -45,20 +47,28 @@
 
         if self.time_weights is not None:
             new_time_weights = out_target.time_weights[valid_idx]
             out_target.time_weights = new_time_weights / new_time_weights.sum()
         return out_target
 
     @abstractmethod
-    def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
+    def get_evaluator(self, model_times: pd.Index, epoch: Epoch) -> TargetEvaluator:
         raise NotImplementedError()
 
 
 class TargetEvaluator(ABC):
-    def __init__(self, target: BaseTarget, model_times: pd.Index):
+    def __init__(self, target: BaseTarget, model_times: pd.Index, epoch: Epoch=None):
+
+        if not isinstance(target.data.index, pd.DatetimeIndex):
+            if epoch is not None:
+                model_times = epoch.dti_to_index(model_times)
+        else:
+            if epoch is None:
+                raise Exception("Target data expressed as datetime but no ref_date set for model")
+
         self.target = target.filtered(model_times)
         self.data = self.target.data.to_numpy()
         for da in target._data_attrs:
             data = getattr(self.target, da)
             setattr(self, da, data.to_numpy())
         self.index = np.array([model_times.get_loc(t) for t in self.target.data.index])
         if self.target.time_weights is not None:
@@ -68,16 +78,16 @@
 
     @abstractmethod
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         raise NotImplementedError()
 
 
 class NegativeBinomialEvaluator(TargetEvaluator):
-    def __init__(self, target: BaseTarget, model_times: pd.Index):
-        super().__init__(target, model_times)
+    def __init__(self, target: BaseTarget, model_times: pd.Index, epoch: Epoch):
+        super().__init__(target, model_times, epoch)
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         if isinstance(self.target.dispersion_param, BasePrior):
             n = parameters[self.target.dispersion_param.name]
         else:
             n = self.target.dispersion_param
 
@@ -115,16 +125,16 @@
 
     def get_priors(self):
         if isinstance(self.dispersion_param, BasePrior):
             return [self.dispersion_param]
         else:
             return []
 
-    def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
-        return NegativeBinomialEvaluator(self, model_times)
+    def get_evaluator(self, model_times: pd.Index, epoch: Epoch) -> TargetEvaluator:
+        return NegativeBinomialEvaluator(self, model_times, epoch)
 
 
 class BinomialTarget(BaseTarget):
     """
     A calibration target sampled from a binomial distribution
     """
 
@@ -136,21 +146,21 @@
         weight: float = 1.0,
         time_weights: pd.Series = None,
     ):
         super().__init__(name, data, weight, time_weights)
         self._data_attrs = ["sample_sizes"]
         self.sample_sizes = sample_sizes
 
-    def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
-        return BinomialEvaluator(self, model_times)
+    def get_evaluator(self, model_times: pd.Index, epoch: Epoch) -> TargetEvaluator:
+        return BinomialEvaluator(self, model_times, epoch)
 
 
 class BinomialEvaluator(TargetEvaluator):
-    def __init__(self, target: BaseTarget, model_times: pd.Index):
-        super().__init__(target, model_times)
+    def __init__(self, target: BaseTarget, model_times: pd.Index, epoch: Epoch):
+        super().__init__(target, model_times, epoch)
         # Enforce this here so TFP-jax picks the right output types
         self.sample_sizes = self.sample_sizes.astype(float)
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         from tensorflow_probability.substrates import jax as tfp
 
         # use a binomial (n, p) where n is the sample size observed in the data and p the modelled proportion
@@ -189,21 +199,21 @@
 
     def get_priors(self):
         if isinstance(self.stdev, BasePrior):
             return [self.stdev]
         else:
             return []
 
-    def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
-        return TruncatedNormalTargetEvaluator(self, model_times)
+    def get_evaluator(self, model_times: pd.Index, epoch: Epoch) -> TargetEvaluator:
+        return TruncatedNormalTargetEvaluator(self, model_times, epoch)
 
 
 class TruncatedNormalTargetEvaluator(TargetEvaluator):
-    def __init__(self, target: TruncatedNormalTarget, model_times: pd.Index):
-        super().__init__(target, model_times)
+    def __init__(self, target: TruncatedNormalTarget, model_times: pd.Index, epoch: Epoch):
+        super().__init__(target, model_times, epoch)
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         if isinstance(self.target.stdev, BasePrior):
             sd = parameters[self.target.stdev.name]
         else:
             sd = self.target.stdev
 
@@ -248,21 +258,21 @@
 
     def get_priors(self):
         if isinstance(self.stdev, BasePrior):
             return [self.stdev]
         else:
             return []
 
-    def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
-        return NormalTargetEvaluator(self, model_times)
+    def get_evaluator(self, model_times: pd.Index, epoch: Epoch) -> TargetEvaluator:
+        return NormalTargetEvaluator(self, model_times, epoch)
 
 
 class NormalTargetEvaluator(TargetEvaluator):
-    def __init__(self, target: BaseTarget, model_times: pd.Index):
-        super().__init__(target, model_times)
+    def __init__(self, target: BaseTarget, model_times: pd.Index, epoch: Epoch):
+        super().__init__(target, model_times, epoch)
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         if isinstance(self.target.stdev, BasePrior):
             sd = parameters[self.target.stdev.name]
         else:
             sd = self.target.stdev
 
@@ -272,16 +282,16 @@
             ll = ll * self.time_weights
             return jnp.sum(ll) * self.target.weight
         else:
             return jnp.mean(ll) * self.target.weight
 
 
 class CustomTargetEvaluator(TargetEvaluator):
-    def __init__(self, target, model_times, eval_func):
-        super().__init__(target, model_times)
+    def __init__(self, target, model_times, eval_func, epoch):
+        super().__init__(target, model_times, epoch)
         self._eval_func = eval_func
 
     def evaluate(self, modelled, parameters):
         return (
             self._eval_func(modelled[self.index], self.data, parameters, self.time_weights)
             * self.target.weight
         )
@@ -306,16 +316,16 @@
             eval_func: Callable as described above
             weight (optional): Scales resulting output
             time_weights (optional): Passed to eval_func - Series with index matching data
         """
         super().__init__(name, data, weight, time_weights)
         self.eval_func = eval_func
 
-    def get_evaluator(self, model_times):
-        return CustomTargetEvaluator(self, model_times, self.eval_func)
+    def get_evaluator(self, model_times, epoch: Epoch):
+        return CustomTargetEvaluator(self, model_times, self.eval_func, epoch)
 
 
 def get_target_sd(data: pd.Series) -> float:
     """Return a value such that the 95% CI of the associated normal distribution covers a width
        equivalent to 25% of the maximum value of the target.
 
     Args:
```

### Comparing `estival-0.2.3/estival/utils.py` & `estival-0.2.4/estival/utils.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/LICENSE` & `estival-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `estival-0.2.3/pyproject.toml` & `estival-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "estival"
-version = "0.2.3"
+version = "0.2.4"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/estival"
 repository = "https://github.com/monash-emu/estival"
 documentation = "https://github.com/monash-emu/estival"
 keywords = [
     "calibration",
@@ -16,22 +16,23 @@
 description = "A set of calibration and probabilistic programming tools for use with summerepi2"
 authors = ["David Shipman <dshipman@gmail.com>"]
 packages = [
     {include = "estival"}
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.0"
+python = ">=3.8.0, <4.0.0"
 numpy = ">=1.20.3"
 scipy = ">=1.7.3"
 arviz = ">=0.12.1"
 nevergrad = ">=0.6.0"
 pymc = ">=5.2.0"
-summerepi2 = ">=1.2.1"
+summerepi2 = ">=1.2.3"
 tensorflow-probability = ">=0.9.0"
+cloudpickle = ">=2.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 black = "^20.8b0"
 pytest-parallel = "^0.1.0"
 pre-commit = "^2.19.0"
```

### Comparing `estival-0.2.3/PKG-INFO` & `estival-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: estival
-Version: 0.2.3
+Version: 0.2.4
 Summary: A set of calibration and probabilistic programming tools for use with summerepi2
 Home-page: https://github.com/monash-emu/estival
 License: BSD-2-Clause
 Keywords: calibration,optimization,bayesian,compartmental modelling,summerepi
 Author: David Shipman
 Author-email: dshipman@gmail.com
-Requires-Python: >=3.8.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arviz (>=0.12.1)
+Requires-Dist: cloudpickle (>=2.2.1)
 Requires-Dist: nevergrad (>=0.6.0)
 Requires-Dist: numpy (>=1.20.3)
 Requires-Dist: pymc (>=5.2.0)
 Requires-Dist: scipy (>=1.7.3)
-Requires-Dist: summerepi2 (>=1.2.1)
+Requires-Dist: summerepi2 (>=1.2.3)
 Requires-Dist: tensorflow-probability (>=0.9.0)
 Project-URL: Documentation, https://github.com/monash-emu/estival
 Project-URL: Repository, https://github.com/monash-emu/estival
 Description-Content-Type: text/markdown
 
 # estival
 Calibration and optimization tools for summer2
@@ -35,7 +36,10 @@
 
 ### CHANGELOG
 
 - 0.2.2  
 Add logprior/logposterior to BayesianCompartmentalModel
 - 0.2.3  
 Include tensorflow-probability(jax) for more (and better tested) stats modules
+- 0.2.4
+Bugfix (vector priors were not exported to pymc correctly)
+Add Epoch support to allow DatetimeIndex targets
```


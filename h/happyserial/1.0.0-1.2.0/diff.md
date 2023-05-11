# Comparing `tmp/happyserial-1.0.0.tar.gz` & `tmp/happyserial-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyserial-1.0.0.tar", last modified: Thu Nov 10 10:09:53 2022, max compression
+gzip compressed data, was "happyserial-1.2.0.tar", last modified: Thu May 11 09:44:40 2023, max compression
```

## Comparing `happyserial-1.0.0.tar` & `happyserial-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 10:09:53.107760 happyserial-1.0.0/
--rw-rw-rw-   0        0        0     1231 2022-11-10 10:09:53.108244 happyserial-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      695 2022-11-10 10:07:21.000000 happyserial-1.0.0/README.md
--rw-rw-rw-   0        0        0      213 2022-11-10 10:07:21.000000 happyserial-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      791 2022-11-10 10:09:53.109241 happyserial-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-11-10 10:07:21.000000 happyserial-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-10 10:09:53.079285 happyserial-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-10 10:09:53.093878 happyserial-1.0.0/src/happyserial/
--rw-rw-rw-   0        0        0      876 2022-11-10 10:07:21.000000 happyserial-1.0.0/src/happyserial/BreakfastSerial.py
--rw-rw-rw-   0        0        0     2567 2022-11-10 10:07:21.000000 happyserial-1.0.0/src/happyserial/Crc.py
--rw-rw-rw-   0        0        0      768 2022-11-10 10:07:21.000000 happyserial-1.0.0/src/happyserial/HappySerial.py
--rw-rw-rw-   0        0        0       17 2022-11-10 10:07:21.000000 happyserial-1.0.0/src/happyserial/HappyVersion.py
--rw-rw-rw-   0        0        0     4080 2022-11-10 10:07:21.000000 happyserial-1.0.0/src/happyserial/Hdlc.py
--rw-rw-rw-   0        0        0       53 2022-11-10 10:07:21.000000 happyserial-1.0.0/src/happyserial/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-10 10:09:53.106763 happyserial-1.0.0/src/happyserial.egg-info/
--rw-rw-rw-   0        0        0     1231 2022-11-10 10:09:53.000000 happyserial-1.0.0/src/happyserial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2022-11-10 10:09:53.000000 happyserial-1.0.0/src/happyserial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 10:09:53.000000 happyserial-1.0.0/src/happyserial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-11-10 10:09:53.000000 happyserial-1.0.0/src/happyserial.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-10 10:09:53.000000 happyserial-1.0.0/src/happyserial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 09:44:40.815164 happyserial-1.2.0/
+-rw-rw-rw-   0        0        0     1373 2023-05-11 09:44:40.815164 happyserial-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      837 2023-05-11 09:42:25.000000 happyserial-1.2.0/README.md
+-rw-rw-rw-   0        0        0      249 2023-05-11 09:42:25.000000 happyserial-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      796 2023-05-11 09:44:40.816191 happyserial-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-05-10 16:01:46.000000 happyserial-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:44:40.764232 happyserial-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 09:44:40.793455 happyserial-1.2.0/src/happyserial/
+-rw-rw-rw-   0        0        0      876 2023-05-10 16:01:46.000000 happyserial-1.2.0/src/happyserial/BreakfastSerial.py
+-rw-rw-rw-   0        0        0     2567 2023-05-10 16:01:46.000000 happyserial-1.2.0/src/happyserial/Crc.py
+-rw-rw-rw-   0        0        0     1788 2023-05-11 09:42:25.000000 happyserial-1.2.0/src/happyserial/HappySerial.py
+-rw-rw-rw-   0        0        0       22 2023-05-11 09:42:25.000000 happyserial-1.2.0/src/happyserial/HappyVersion.py
+-rw-rw-rw-   0        0        0     4080 2023-05-10 16:01:46.000000 happyserial-1.2.0/src/happyserial/Hdlc.py
+-rw-rw-rw-   0        0        0       53 2023-05-10 16:01:46.000000 happyserial-1.2.0/src/happyserial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:44:40.805528 happyserial-1.2.0/src/happyserial.egg-info/
+-rw-rw-rw-   0        0        0     1373 2023-05-11 09:44:40.000000 happyserial-1.2.0/src/happyserial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-05-11 09:44:40.000000 happyserial-1.2.0/src/happyserial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:44:40.000000 happyserial-1.2.0/src/happyserial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 09:44:40.000000 happyserial-1.2.0/src/happyserial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 09:44:40.000000 happyserial-1.2.0/src/happyserial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 09:44:40.813170 happyserial-1.2.0/tests/
+-rw-rw-rw-   0        0        0       44 2023-05-10 16:01:46.000000 happyserial-1.2.0/tests/test_dummy.py
+-rw-rw-rw-   0        0        0     1347 2023-05-11 09:42:25.000000 happyserial-1.2.0/tests/test_echo.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 16:01:46.000000 happyserial-1.2.0/tests/test_import.py
+-rw-rw-rw-   0        0        0      740 2023-05-11 09:42:25.000000 happyserial-1.2.0/tests/test_version.py
```

### Comparing `happyserial-1.0.0/PKG-INFO` & `happyserial-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: happyserial
-Version: 1.0.0
+Version: 1.2.0
 Summary: DMA-based framing for serial interaction with an nRF chip
 Author: Thomas Watteyne
 Author-email: twatteyne@gmail.com
 Project-URL: Source Code, https://github.com/openwsn-berkeley/happyserial/
 Project-URL: Bug Tracker, https://github.com/openwsn-berkeley/happyserial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
+# running tests
+- `cd src_python`
+- `pytest` to run all tests, including functional
+- `pytest -m "not functional"` to run only unitests
+
 # run from source
 
 - `cd src_python`
 - `pip install -r requirements.txt`
 - `cd src`
 - `python -m happyserial`
```

### Comparing `happyserial-1.0.0/README.md` & `happyserial-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# running tests
+- `cd src_python`
+- `pytest` to run all tests, including functional
+- `pytest -m "not functional"` to run only unitests
+
 # run from source
 
 - `cd src_python`
 - `pip install -r requirements.txt`
 - `cd src`
 - `python -m happyserial`
```

### Comparing `happyserial-1.0.0/setup.cfg` & `happyserial-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 6170 7079 7365 7269 616c 0d0a   = happyserial..
 00000020: 7665 7273 696f 6e20 3d20 6174 7472 3a20  version = attr: 
 00000030: 6861 7070 7973 6572 6961 6c2e 4861 7070  happyserial.Happ
-00000040: 7956 6572 7369 6f6e 2e56 4552 5349 4f4e  yVersion.VERSION
-00000050: 0d0a 6175 7468 6f72 203d 2054 686f 6d61  ..author = Thoma
-00000060: 7320 5761 7474 6579 6e65 0d0a 6175 7468  s Watteyne..auth
-00000070: 6f72 5f65 6d61 696c 203d 2074 7761 7474  or_email = twatt
-00000080: 6579 6e65 4067 6d61 696c 2e63 6f6d 0d0a  eyne@gmail.com..
-00000090: 6465 7363 7269 7074 696f 6e20 3d20 444d  description = DM
-000000a0: 412d 6261 7365 6420 6672 616d 696e 6720  A-based framing 
-000000b0: 666f 7220 7365 7269 616c 2069 6e74 6572  for serial inter
-000000c0: 6163 7469 6f6e 2077 6974 6820 616e 206e  action with an n
-000000d0: 5246 2063 6869 700d 0a6c 6f6e 675f 6465  RF chip..long_de
-000000e0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-000000f0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-00000100: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-00000110: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-00000120: 742f 6d61 726b 646f 776e 0d0a 7072 6f6a  t/markdown..proj
-00000130: 6563 745f 7572 6c73 203d 200d 0a09 536f  ect_urls = ...So
-00000140: 7572 6365 2043 6f64 6520 2020 2020 2020  urce Code       
-00000150: 2020 2020 2020 2020 2020 2020 3d20 6874              = ht
-00000160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000170: 2f6f 7065 6e77 736e 2d62 6572 6b65 6c65  /openwsn-berkele
-00000180: 792f 6861 7070 7973 6572 6961 6c2f 0d0a  y/happyserial/..
-00000190: 0942 7567 2054 7261 636b 6572 2020 2020  .Bug Tracker    
-000001a0: 2020 2020 2020 2020 2020 2020 2020 203d                 =
-000001b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001c0: 636f 6d2f 6f70 656e 7773 6e2d 6265 726b  com/openwsn-berk
-000001d0: 656c 6579 2f68 6170 7079 7365 7269 616c  eley/happyserial
-000001e0: 2f69 7373 7565 730d 0a63 6c61 7373 6966  /issues..classif
-000001f0: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-00000200: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000210: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-00000220: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000230: 7070 726f 7665 6420 3a3a 2042 5344 204c  pproved :: BSD L
-00000240: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-00000250: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000260: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
-00000270: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000280: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
-00000290: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-000002a0: 3a0d 0a69 6e73 7461 6c6c 5f72 6571 7569  :..install_requi
-000002b0: 7265 7320 3d20 0d0a 0970 7973 6572 6961  res = ...pyseria
-000002c0: 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  l....[options.pa
-000002d0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-000002e0: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
-000002f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000300: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000310: 3d20 300d 0a0d 0a                        = 0....
+00000040: 7956 6572 7369 6f6e 2e48 4150 5059 5645  yVersion.HAPPYVE
+00000050: 5253 494f 4e0d 0a61 7574 686f 7220 3d20  RSION..author = 
+00000060: 5468 6f6d 6173 2057 6174 7465 796e 650d  Thomas Watteyne.
+00000070: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000080: 7477 6174 7465 796e 6540 676d 6169 6c2e  twatteyne@gmail.
+00000090: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
+000000a0: 203d 2044 4d41 2d62 6173 6564 2066 7261   = DMA-based fra
+000000b0: 6d69 6e67 2066 6f72 2073 6572 6961 6c20  ming for serial 
+000000c0: 696e 7465 7261 6374 696f 6e20 7769 7468  interaction with
+000000d0: 2061 6e20 6e52 4620 6368 6970 0d0a 6c6f   an nRF chip..lo
+000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+000000f0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+00000100: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000110: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000120: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+00000130: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
+00000140: 0d0a 0953 6f75 7263 6520 436f 6465 2020  ...Source Code  
+00000150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000160: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000170: 622e 636f 6d2f 6f70 656e 7773 6e2d 6265  b.com/openwsn-be
+00000180: 726b 656c 6579 2f68 6170 7079 7365 7269  rkeley/happyseri
+00000190: 616c 2f0d 0a09 4275 6720 5472 6163 6b65  al/...Bug Tracke
+000001a0: 7220 2020 2020 2020 2020 2020 2020 2020  r               
+000001b0: 2020 2020 3d20 6874 7470 733a 2f2f 6769      = https://gi
+000001c0: 7468 7562 2e63 6f6d 2f6f 7065 6e77 736e  thub.com/openwsn
+000001d0: 2d62 6572 6b65 6c65 792f 6861 7070 7973  -berkeley/happys
+000001e0: 6572 6961 6c2f 6973 7375 6573 0d0a 636c  erial/issues..cl
+000001f0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+00000200: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000210: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000220: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+00000230: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000240: 4253 4420 4c69 6365 6e73 650d 0a09 4f70  BSD License...Op
+00000250: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000260: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000270: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000280: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000290: 3d73 7263 0d0a 7061 636b 6167 6573 203d  =src..packages =
+000002a0: 2066 696e 643a 0d0a 696e 7374 616c 6c5f   find:..install_
+000002b0: 7265 7175 6972 6573 203d 200d 0a09 7079  requires = ...py
+000002c0: 7365 7269 616c 0d0a 0d0a 5b6f 7074 696f  serial....[optio
+000002d0: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+000002e0: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+000002f0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000300: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000310: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `happyserial-1.0.0/src/happyserial/BreakfastSerial.py` & `happyserial-1.2.0/src/happyserial/BreakfastSerial.py`

 * *Files identical despite different names*

### Comparing `happyserial-1.0.0/src/happyserial/Crc.py` & `happyserial-1.2.0/src/happyserial/Crc.py`

 * *Files identical despite different names*

### Comparing `happyserial-1.0.0/src/happyserial/Hdlc.py` & `happyserial-1.2.0/src/happyserial/Hdlc.py`

 * *Files identical despite different names*

### Comparing `happyserial-1.0.0/src/happyserial.egg-info/PKG-INFO` & `happyserial-1.2.0/src/happyserial.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: happyserial
-Version: 1.0.0
+Version: 1.2.0
 Summary: DMA-based framing for serial interaction with an nRF chip
 Author: Thomas Watteyne
 Author-email: twatteyne@gmail.com
 Project-URL: Source Code, https://github.com/openwsn-berkeley/happyserial/
 Project-URL: Bug Tracker, https://github.com/openwsn-berkeley/happyserial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
+# running tests
+- `cd src_python`
+- `pytest` to run all tests, including functional
+- `pytest -m "not functional"` to run only unitests
+
 # run from source
 
 - `cd src_python`
 - `pip install -r requirements.txt`
 - `cd src`
 - `python -m happyserial`
```


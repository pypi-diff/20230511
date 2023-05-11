# Comparing `tmp/PyroLab-0.2.1.tar.gz` & `tmp/PyroLab-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroLab-0.2.1.tar", last modified: Sun Feb 13 03:43:00 2022, max compression
+gzip compressed data, was "PyroLab-0.3.0.tar", last modified: Wed Mar  1 00:41:43 2023, max compression
```

## Comparing `PyroLab-0.2.1.tar` & `PyroLab-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-02-13 03:42:33.000000 PyroLab-0.2.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-02-13 03:42:33.000000 PyroLab-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-02-13 03:42:33.000000 PyroLab-0.2.1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8779 2022-02-13 03:43:00.557609 PyroLab-0.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.553609 PyroLab-0.2.1/PyroLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8779 2022-02-13 03:43:00.000000 PyroLab-0.2.1/PyroLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-02-13 03:43:00.000000 PyroLab-0.2.1/PyroLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 03:43:00.000000 PyroLab-0.2.1/PyroLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-02-13 03:43:00.000000 PyroLab-0.2.1/PyroLab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-02-13 03:43:00.000000 PyroLab-0.2.1/PyroLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-13 03:43:00.000000 PyroLab-0.2.1/PyroLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6768 2022-02-13 03:42:33.000000 PyroLab-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13777 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    28806 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)     5860 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/drivers/arduino/
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/arduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/arduino/arduino.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/drivers/cameras/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6845 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/cameras/sciTSI.py
--rw-r--r--   0 runner    (1001) docker     (121)    17590 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/cameras/thorcam.py
--rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/cameras/uc480.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/drivers/lasers/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/lasers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18024 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/lasers/ppcl55x.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/lasers/sachertec.py
--rw-r--r--   0 runner    (1001) docker     (121)    50568 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/lasers/tsl550.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/drivers/motion/
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/drivers/motion/kinesis/
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14278 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/kinesis/bpc303.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/kinesis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    27433 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/kinesis/kdc101.py
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/max31x.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/prm1z8.py
--rw-r--r--   0 runner    (1001) docker     (121)     4478 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/motion/z8xx.py
--rw-r--r--   0 runner    (1001) docker     (121)     7550 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 03:43:00.557609 PyroLab-0.2.1/pyrolab/drivers/scopes/
--rw-r--r--   0 runner    (1001) docker     (121)     8348 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/scopes/VISAResourceExtentions.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/scopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19219 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/drivers/scopes/rohdeschwarz.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    21649 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/nameserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     8127 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/pyrolabd.py
--rw-r--r--   0 runner    (1001) docker     (121)    13827 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-02-13 03:42:34.000000 PyroLab-0.2.1/pyrolab/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-02-13 03:43:00.557609 PyroLab-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-01 00:41:14.000000 PyroLab-0.3.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-01 00:41:14.000000 PyroLab-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-01 00:41:14.000000 PyroLab-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-01 00:41:14.000000 PyroLab-0.3.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    49794 2023-03-01 00:41:43.448003 PyroLab-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-03-01 00:41:14.000000 PyroLab-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-01 00:41:14.000000 PyroLab-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 00:41:43.448003 PyroLab-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/PyroLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49794 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-01 00:41:43.000000 PyroLab-0.3.0/src/PyroLab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/pyrolab/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/pyrolabd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyrolab/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:41:43.448003 PyroLab-0.3.0/src/pyromonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-01 00:41:14.000000 PyroLab-0.3.0/src/pyromonitor/lister.py
```

### Comparing `PyroLab-0.2.1/AUTHORS.txt` & `PyroLab-0.3.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `PyroLab-0.2.1/LICENSE` & `PyroLab-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyroLab-0.2.1/NOTICE.txt` & `PyroLab-0.3.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `PyroLab-0.2.1/PKG-INFO` & `PyroLab-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,549 +1,461 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 5079 726f  : 2.1.Name: Pyro
-00000020: 4c61 620a 5665 7273 696f 6e3a 2030 2e32  Lab.Version: 0.2
-00000030: 2e31 0a53 756d 6d61 7279 3a20 4120 6672  .1.Summary: A fr
-00000040: 616d 6577 6f72 6b20 666f 7220 7573 696e  amework for usin
-00000050: 6720 7265 6d6f 7465 206c 6162 2069 6e73  g remote lab ins
-00000060: 7472 756d 656e 7473 2061 7320 6c6f 6361  truments as loca
-00000070: 6c20 7265 736f 7572 6365 7320 6275 696c  l resources buil
-00000080: 7420 6f6e 2050 7972 6f35 0a48 6f6d 652d  t on Pyro5.Home-
-00000090: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
-000000a0: 7468 7562 2e63 6f6d 2f42 5955 4361 6d61  thub.com/BYUCama
-000000b0: 6368 6f4c 6162 2f70 7972 6f6c 6162 0a41  choLab/pyrolab.A
-000000c0: 7574 686f 723a 2053 6571 756f 6961 2050  uthor: Sequoia P
-000000d0: 6c6f 6567 0a41 7574 686f 722d 656d 6169  loeg.Author-emai
-000000e0: 6c3a 2073 6571 756f 6961 2e70 6c6f 6567  l: sequoia.ploeg
-000000f0: 4062 7975 2e65 6475 0a4c 6963 656e 7365  @byu.edu.License
-00000100: 3a20 4750 4c76 332b 0a50 726f 6a65 6374  : GPLv3+.Project
-00000110: 2d55 524c 3a20 536f 7572 6365 2c20 6874  -URL: Source, ht
-00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000130: 2f42 5955 4361 6d61 6368 6f4c 6162 2f70  /BYUCamachoLab/p
-00000140: 7972 6f6c 6162 0a50 726f 6a65 6374 2d55  yrolab.Project-U
-00000150: 524c 3a20 446f 6375 6d65 6e74 6174 696f  RL: Documentatio
-00000160: 6e2c 2068 7474 7073 3a2f 2f70 7972 6f6c  n, https://pyrol
-00000170: 6162 2e72 6561 6474 6865 646f 6373 2e69  ab.readthedocs.i
-00000180: 6f2f 656e 2f6c 6174 6573 742f 0a50 726f  o/en/latest/.Pro
-00000190: 6a65 6374 2d55 524c 3a20 5472 6163 6b65  ject-URL: Tracke
-000001a0: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
-000001b0: 622e 636f 6d2f 4259 5543 616d 6163 686f  b.com/BYUCamacho
-000001c0: 4c61 622f 7079 726f 6c61 622f 6973 7375  Lab/pyrolab/issu
-000001d0: 6573 0a50 726f 6a65 6374 2d55 524c 3a20  es.Project-URL: 
-000001e0: 5265 7365 6172 6368 2047 726f 7570 2c20  Research Group, 
-000001f0: 6874 7470 733a 2f2f 6361 6d61 6368 6f6c  https://camachol
-00000200: 6162 2e62 7975 2e65 6475 2f0a 4b65 7977  ab.byu.edu/.Keyw
-00000210: 6f72 6473 3a20 5079 726f 4c61 622c 5079  ords: PyroLab,Py
-00000220: 726f 352c 5079 726f 2c6c 6162 2c69 6e73  ro5,Pyro,lab,ins
-00000230: 7472 756d 656e 742c 7265 6d6f 7465 2c72  trument,remote,r
-00000240: 6573 6f75 7263 6573 2c66 7261 6d65 776f  esources,framewo
-00000250: 726b 2c6c 6162 6f72 6174 6f72 792c 696e  rk,laboratory,in
-00000260: 7374 7275 6d65 6e74 6174 696f 6e2c 6861  strumentation,ha
-00000270: 7264 7761 7265 2c73 6369 656e 6365 2c72  rdware,science,r
-00000280: 656d 6f74 652c 6e65 7477 6f72 6b2c 696e  emote,network,in
-00000290: 7465 6772 6174 696f 6e0a 506c 6174 666f  tegration.Platfo
-000002a0: 726d 3a20 5769 6e64 6f77 730a 506c 6174  rm: Windows.Plat
-000002b0: 666f 726d 3a20 4c69 6e75 780a 506c 6174  form: Linux.Plat
-000002c0: 666f 726d 3a20 4d61 6320 4f53 2d58 0a43  form: Mac OS-X.C
-000002d0: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-000002e0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-000002f0: 2034 202d 2042 6574 610a 436c 6173 7369   4 - Beta.Classi
-00000300: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000310: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
-00000320: 6365 2f52 6573 6561 7263 680a 436c 6173  ce/Research.Clas
-00000330: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-00000340: 2041 7564 6965 6e63 6520 3a3a 2045 6475   Audience :: Edu
-00000350: 6361 7469 6f6e 0a43 6c61 7373 6966 6965  cation.Classifie
-00000360: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000370: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000380: 7273 0a43 6c61 7373 6966 6965 723a 204c  rs.Classifier: L
-00000390: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000003a0: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
-000003b0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-000003c0: 656e 7365 2076 3320 6f72 206c 6174 6572  ense v3 or later
-000003d0: 2028 4750 4c76 332b 290a 436c 6173 7369   (GPLv3+).Classi
-000003e0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-000003f0: 5379 7374 656d 203a 3a20 4d69 6372 6f73  System :: Micros
-00000400: 6f66 7420 3a3a 2057 696e 646f 7773 0a43  oft :: Windows.C
-00000410: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00000420: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
-00000430: 6163 4f53 0a43 6c61 7373 6966 6965 723a  acOS.Classifier:
-00000440: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-00000450: 6d20 3a3a 2050 4f53 4958 203a 3a20 4c69  m :: POSIX :: Li
-00000460: 6e75 780a 436c 6173 7369 6669 6572 3a20  nux.Classifier: 
-00000470: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000480: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000490: 6e74 0a43 6c61 7373 6966 6965 723a 2050  nt.Classifier: P
-000004a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000004b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000004c0: 2033 0a43 6c61 7373 6966 6965 723a 2050   3.Classifier: P
-000004d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000004e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000004f0: 2033 2e37 0a43 6c61 7373 6966 6965 723a   3.7.Classifier:
-00000500: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000510: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000520: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
-00000530: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000540: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000550: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
-00000560: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000570: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000580: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
-00000590: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000005a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000005b0: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-000005c0: 6e6c 790a 436c 6173 7369 6669 6572 3a20  nly.Classifier: 
-000005d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000005e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000005f0: 3a20 496d 706c 656d 656e 7461 7469 6f6e  : Implementation
-00000600: 203a 3a20 4350 7974 686f 6e0a 436c 6173   :: CPython.Clas
-00000610: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000620: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-00000630: 6e65 6572 696e 670a 436c 6173 7369 6669  neering.Classifi
-00000640: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
-00000650: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-00000660: 696e 6720 3a3a 2050 6879 7369 6373 0a43  ing :: Physics.C
-00000670: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000680: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-00000690: 6e67 696e 6565 7269 6e67 203a 3a20 5669  ngineering :: Vi
-000006a0: 7375 616c 697a 6174 696f 6e0a 436c 6173  sualization.Clas
-000006b0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-000006c0: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
-000006d0: 706d 656e 7420 3a3a 204c 6962 7261 7269  pment :: Librari
-000006e0: 6573 203a 3a20 5079 7468 6f6e 204d 6f64  es :: Python Mod
-000006f0: 756c 6573 0a52 6571 7569 7265 732d 5079  ules.Requires-Py
-00000700: 7468 6f6e 3a20 3e3d 332e 370a 4465 7363  thon: >=3.7.Desc
-00000710: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000720: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000730: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-00000740: 7261 3a20 7473 6c35 3530 0a50 726f 7669  ra: tsl550.Provi
-00000750: 6465 732d 4578 7472 613a 2070 7063 6c35  des-Extra: ppcl5
-00000760: 3578 0a50 726f 7669 6465 732d 4578 7472  5x.Provides-Extr
-00000770: 613a 2072 746f 0a50 726f 7669 6465 732d  a: rto.Provides-
-00000780: 4578 7472 613a 2061 7264 7569 6e6f 0a4c  Extra: arduino.L
-00000790: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-000007a0: 454e 5345 0a4c 6963 656e 7365 2d46 696c  ENSE.License-Fil
-000007b0: 653a 204e 4f54 4943 452e 7478 740a 4c69  e: NOTICE.txt.Li
-000007c0: 6365 6e73 652d 4669 6c65 3a20 4155 5448  cense-File: AUTH
-000007d0: 4f52 532e 7478 740a 0a3c 7020 616c 6967  ORS.txt..<p alig
-000007e0: 6e3d 2263 656e 7465 7222 3e0a 3c69 6d67  n="center">.<img
-000007f0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000800: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000810: 656e 742e 636f 6d2f 4259 5543 616d 6163  ent.com/BYUCamac
-00000820: 686f 4c61 622f 7079 726f 6c61 622f 6d61  hoLab/pyrolab/ma
-00000830: 7374 6572 2f64 6f63 732f 5f73 7461 7469  ster/docs/_stati
-00000840: 632f 696d 6167 6573 2f70 7972 6f6c 6162  c/images/pyrolab
-00000850: 5f6c 6f67 6f2e 7376 6722 2077 6964 7468  _logo.svg" width
-00000860: 3d22 3430 2522 2061 6c74 3d22 5079 726f  ="40%" alt="Pyro
-00000870: 4c61 6222 3e0a 3c2f 703e 0a0a 2d2d 2d0a  Lab">.</p>..---.
-00000880: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00000890: 7222 3e0a 3c69 6d67 2061 6c74 3d22 4465  r">.<img alt="De
-000008a0: 7665 6c6f 706d 656e 7420 7665 7273 696f  velopment versio
-000008b0: 6e22 2073 7263 3d22 6874 7470 733a 2f2f  n" src="https://
-000008c0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000008d0: 6164 6765 2f6d 6173 7465 722d 7630 2e32  adge/master-v0.2
-000008e0: 2e31 2d69 6e66 6f72 6d61 7469 6f6e 616c  .1-informational
-000008f0: 223e 0a3c 6120 6872 6566 3d22 6874 7470  ">.<a href="http
-00000900: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
-00000910: 6f72 672f 7079 7069 2f70 7972 6f6c 6162  org/pypi/pyrolab
-00000920: 223e 3c69 6d67 2061 6c74 3d22 5079 5049  "><img alt="PyPI
-00000930: 2056 6572 7369 6f6e 2220 7372 633d 2268   Version" src="h
-00000940: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000950: 6473 2e69 6f2f 7079 7069 2f76 2f70 7972  ds.io/pypi/v/pyr
-00000960: 6f6c 6162 2e73 7667 223e 3c2f 613e 0a3c  olab.svg"></a>.<
-00000970: 696d 6720 616c 743d 2250 7950 4920 2d20  img alt="PyPI - 
-00000980: 5079 7468 6f6e 2056 6572 7369 6f6e 2220  Python Version" 
-00000990: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000009a0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000009b0: 2f70 7976 6572 7369 6f6e 732f 7079 726f  /pyversions/pyro
-000009c0: 6c61 6222 3e0a 3c21 2d2d 203c 6120 6872  lab">.<!-- <a hr
-000009d0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000009e0: 7562 2e63 6f6d 2f42 5955 4361 6d61 6368  ub.com/BYUCamach
-000009f0: 6f4c 6162 2f73 696d 7068 6f6e 792f 6163  oLab/simphony/ac
-00000a00: 7469 6f6e 733f 7175 6572 793d 776f 726b  tions?query=work
-00000a10: 666c 6f77 2533 4125 3232 6275 696c 642b  flow%3A%22build+
-00000a20: 2532 3870 6970 2532 3925 3232 223e 3c69  %28pip%29%22"><i
-00000a30: 6d67 2061 6c74 3d22 4275 696c 6420 5374  mg alt="Build St
-00000a40: 6174 7573 2220 7372 633d 2268 7474 7073  atus" src="https
-00000a50: 3a2f 2f67 6974 6875 622e 636f 6d2f 4259  ://github.com/BY
-00000a60: 5543 616d 6163 686f 4c61 622f 7369 6d70  UCamachoLab/simp
-00000a70: 686f 6e79 2f77 6f72 6b66 6c6f 7773 2f62  hony/workflows/b
-00000a80: 7569 6c64 2532 3028 7069 7029 2f62 6164  uild%20(pip)/bad
-00000a90: 6765 2e73 7667 223e 3c2f 613e 202d 2d3e  ge.svg"></a> -->
-00000aa0: 0a3c 212d 2d20 3c61 2068 7265 663d 2268  .<!-- <a href="h
-00000ab0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000ac0: 6d2f 7072 652d 636f 6d6d 6974 2f70 7265  m/pre-commit/pre
-00000ad0: 2d63 6f6d 6d69 7422 3e3c 696d 6720 7372  -commit"><img sr
-00000ae0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000af0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000b00: 7072 652d 2d63 6f6d 6d69 742d 656e 6162  pre--commit-enab
-00000b10: 6c65 642d 6272 6967 6874 6772 6565 6e3f  led-brightgreen?
-00000b20: 6c6f 676f 3d70 7265 2d63 6f6d 6d69 7426  logo=pre-commit&
-00000b30: 6c6f 676f 436f 6c6f 723d 7768 6974 6522  logoColor=white"
-00000b40: 2061 6c74 3d22 7072 652d 636f 6d6d 6974   alt="pre-commit
-00000b50: 2220 7374 796c 653d 226d 6178 2d77 6964  " style="max-wid
-00000b60: 7468 3a31 3030 253b 223e 3c2f 613e 202d  th:100%;"></a> -
-00000b70: 2d3e 0a3c 6120 6872 6566 3d22 6874 7470  ->.<a href="http
-00000b80: 733a 2f2f 7079 726f 6c61 622e 7265 6164  s://pyrolab.read
-00000b90: 7468 6564 6f63 732e 696f 2f22 3e3c 696d  thedocs.io/"><im
-00000ba0: 6720 616c 743d 2244 6f63 756d 656e 7461  g alt="Documenta
-00000bb0: 7469 6f6e 2053 7461 7475 7322 2073 7263  tion Status" src
-00000bc0: 3d22 6874 7470 733a 2f2f 7265 6164 7468  ="https://readth
-00000bd0: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
-00000be0: 7473 2f70 7972 6f6c 6162 2f62 6164 6765  ts/pyrolab/badge
-00000bf0: 2f3f 7665 7273 696f 6e3d 6c61 7465 7374  /?version=latest
-00000c00: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-00000c10: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
-00000c20: 686f 6e2e 6f72 672f 7079 7069 2f70 7972  hon.org/pypi/pyr
-00000c30: 6f6c 6162 2f22 3e3c 696d 6720 616c 743d  olab/"><img alt=
-00000c40: 224c 6963 656e 7365 2220 7372 633d 2268  "License" src="h
-00000c50: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000c60: 6473 2e69 6f2f 7079 7069 2f6c 2f70 7972  ds.io/pypi/l/pyr
-00000c70: 6f6c 6162 2e73 7667 223e 3c2f 613e 0a3c  olab.svg"></a>.<
-00000c80: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000c90: 6769 7468 7562 2e63 6f6d 2f73 6571 756f  github.com/sequo
-00000ca0: 6961 702f 7079 726f 6c61 622f 636f 6d6d  iap/pyrolab/comm
-00000cb0: 6974 732f 6d61 7374 6572 223e 3c69 6d67  its/master"><img
-00000cc0: 2061 6c74 3d22 4c61 7465 7374 2043 6f6d   alt="Latest Com
-00000cd0: 6d69 7422 2073 7263 3d22 6874 7470 733a  mit" src="https:
-00000ce0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000cf0: 2f67 6974 6875 622f 6c61 7374 2d63 6f6d  /github/last-com
-00000d00: 6d69 742f 7365 7175 6f69 6170 2f70 7972  mit/sequoiap/pyr
-00000d10: 6f6c 6162 2e73 7667 223e 3c2f 613e 0a3c  olab.svg"></a>.<
-00000d20: 2f70 3e0a 0a41 2066 7261 6d65 776f 726b  /p>..A framework
-00000d30: 2066 6f72 2075 7369 6e67 2072 656d 6f74   for using remot
-00000d40: 6520 6c61 6220 696e 7374 7275 6d65 6e74  e lab instrument
-00000d50: 7320 6173 206c 6f63 616c 2072 6573 6f75  s as local resou
-00000d60: 7263 6573 2c20 6275 696c 7420 6f6e 2050  rces, built on P
-00000d70: 7972 6f35 2e0a 0a44 6576 656c 6f70 6564  yro5...Developed
-00000d80: 2062 7920 5365 7175 6f69 6120 506c 6f65   by Sequoia Ploe
-00000d90: 6720 2866 6f72 205b 4361 6d61 6368 6f4c  g (for [CamachoL
-00000da0: 6162 5d28 6874 7470 733a 2f2f 6361 6d61  ab](https://cama
-00000db0: 6368 6f6c 6162 2e62 7975 2e65 6475 2f29  cholab.byu.edu/)
-00000dc0: 2c20 0a42 7269 6768 616d 2059 6f75 6e67  , .Brigham Young
-00000dd0: 2055 6e69 7665 7273 6974 7929 2e0a 0a23   University)...#
-00000de0: 2320 4162 6f75 740a 5468 6973 2070 726f  # About.This pro
-00000df0: 6a65 6374 2061 696d 7320 746f 2061 6c6c  ject aims to all
-00000e00: 6f77 2061 6c6c 206c 6162 6f72 6174 6f72  ow all laborator
-00000e10: 7920 696e 7374 7275 6d65 6e74 7320 746f  y instruments to
-00000e20: 2062 6520 6163 6365 7373 6564 2061 730a   be accessed as.
-00000e30: 6c6f 6361 6c20 6f62 6a65 6374 7320 6672  local objects fr
-00000e40: 6f6d 2061 2072 656d 6f74 6520 6d61 6368  om a remote mach
-00000e50: 696e 652e 2049 6e73 7472 756d 656e 7473  ine. Instruments
-00000e60: 2074 6861 7420 646f 6e27 7420 6e61 7469   that don't nati
-00000e70: 7665 6c79 0a73 7570 706f 7274 2073 7563  vely.support suc
-00000e80: 6820 6163 6365 7373 2c20 7375 6368 2061  h access, such a
-00000e90: 7320 7468 6f73 6520 7265 7175 6972 6564  s those required
-00000ea0: 2074 6f20 6265 2063 6f6e 6e65 6374 6564   to be connected
-00000eb0: 2062 7920 6120 5553 4220 6361 626c 650a   by a USB cable.
-00000ec0: 286f 7220 7369 6d69 6c61 7229 2c20 6172  (or similar), ar
-00000ed0: 6520 7772 6170 7065 6420 7769 7468 2061  e wrapped with a
-00000ee0: 2050 7972 6f35 2069 6e74 6572 6661 6365   Pyro5 interface
-00000ef0: 2e20 486f 7765 7665 722c 2074 6869 7320  . However, this 
-00000f00: 6c69 6272 6172 7920 6d61 790a 636f 6e74  library may.cont
-00000f10: 6169 6e20 6f74 6865 7220 696e 7374 7275  ain other instru
-00000f20: 6d65 6e74 7320 7468 6174 2061 7265 2061  ments that are a
-00000f30: 6c72 6561 6479 2069 6e74 6572 6e65 742d  lready internet-
-00000f40: 6361 7061 626c 6520 616e 6420 646f 6e27  capable and don'
-00000f50: 7420 7265 6c79 0a6f 6e20 5079 726f 352e  t rely.on Pyro5.
-00000f60: 2054 6861 7427 7320 616c 7269 6768 743b   That's alright;
-00000f70: 2077 6527 7265 206a 7573 7420 7472 7969   we're just tryi
-00000f80: 6e67 2074 6f20 6372 6561 7465 2061 206d  ng to create a m
-00000f90: 696e 696d 616c 2d64 6570 656e 6465 6e63  inimal-dependenc
-00000fa0: 792c 0a6f 6e65 2d73 746f 702d 7368 6f70  y,.one-stop-shop
-00000fb0: 2066 6f72 206c 6162 6f72 6174 6f72 7920   for laboratory 
-00000fc0: 696e 7374 7275 6d65 6e74 7321 0a0a 2a2a  instruments!..**
-00000fd0: 4e6f 7465 3a2a 2a20 7768 696c 6520 7468  Note:** while th
-00000fe0: 6520 736f 6674 7761 7265 2073 6179 7320  e software says 
-00000ff0: 224f 5320 496e 6465 7065 6e64 656e 7422  "OS Independent"
-00001000: 2c20 736f 6d65 206f 6620 7468 6520 7365  , some of the se
-00001010: 7276 6572 7320 2a61 7265 2a0a 4f53 2d73  rvers *are*.OS-s
-00001020: 7065 6369 6669 632e 2046 6f72 2065 7861  pecific. For exa
-00001030: 6d70 6c65 2c20 5468 6f72 4c61 6273 2044  mple, ThorLabs D
-00001040: 4c4c 2773 206f 6e6c 7920 776f 726b 206f  LL's only work o
-00001050: 6e20 5769 6e64 6f77 732e 2048 6f77 6576  n Windows. Howev
-00001060: 6572 2c20 796f 7520 636f 756c 640a 7573  er, you could.us
-00001070: 6520 5079 726f 4c61 6220 746f 2063 6f6e  e PyroLab to con
-00001080: 6e65 6374 2074 6f20 7468 6f73 6520 6465  nect to those de
-00001090: 7669 6365 7320 6672 6f6d 2061 6e79 206f  vices from any o
-000010a0: 7065 7261 7469 6e67 2073 7973 7465 6d2e  perating system.
-000010b0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000010c0: 6e0a 0a50 7972 6f4c 6162 2069 7320 7069  n..PyroLab is pi
-000010d0: 7020 696e 7374 616c 6c61 626c 653a 0a0a  p installable:..
-000010e0: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
-000010f0: 7079 726f 6c61 620a 6060 600a 0a50 7972  pyrolab.```..Pyr
-00001100: 6f4c 6162 2064 6563 6c61 7265 7320 7365  oLab declares se
-00001110: 7665 7261 6c20 2265 7874 7261 7322 2c20  veral "extras", 
-00001120: 6465 7065 6e64 696e 6720 6f6e 2077 6869  depending on whi
-00001130: 6368 2069 6e73 7472 756d 656e 7473 2079  ch instruments y
-00001140: 6f75 206e 6565 640a 746f 2073 7570 706f  ou need.to suppo
-00001150: 7274 3a0a 0a60 6060 0a70 6970 2069 6e73  rt:..```.pip ins
-00001160: 7461 6c6c 2070 7972 6f6c 6162 5b74 736c  tall pyrolab[tsl
-00001170: 3535 302c 206f 7363 6f70 655d 0a60 6060  550, oscope].```
-00001180: 0a0a 5468 6520 6675 6c6c 206c 6973 7420  ..The full list 
-00001190: 6f66 2073 7570 706f 7274 6564 2065 7874  of supported ext
-000011a0: 7261 7320 6973 3a0a 2d20 7473 6c35 3530  ras is:.- tsl550
-000011b0: 0a2d 206f 7363 6f70 650a 2d20 6172 6475  .- oscope.- ardu
-000011c0: 696e 6f0a 0a59 6f75 2063 616e 2061 6c73  ino..You can als
-000011d0: 6f20 636c 6f6e 6520 7468 6520 7265 706f  o clone the repo
-000011e0: 7369 746f 7279 2c20 6e61 7669 6761 7465  sitory, navigate
-000011f0: 2074 6f20 7468 6520 746f 706c 6576 656c   to the toplevel
-00001200: 2c20 616e 6420 696e 7374 616c 6c20 696e  , and install in
-00001210: 200a 6564 6974 6162 6c65 206d 6f64 6520   .editable mode 
-00001220: 286d 616b 6520 7375 7265 2079 6f75 2068  (make sure you h
-00001230: 6176 6520 7069 7020 3e3d 2032 312e 3129  ave pip >= 21.1)
-00001240: 3a0a 0a60 6060 0a70 6970 2069 6e73 7461  :..```.pip insta
-00001250: 6c6c 202d 6520 2e0a 6060 600a 0a23 2320  ll -e ..```..## 
-00001260: 556e 696e 7374 616c 6c61 7469 6f6e 0a0a  Uninstallation..
-00001270: 5079 726f 4c61 6220 6372 6561 7465 7320  PyroLab creates 
-00001280: 6461 7461 2061 6e64 2063 6f6e 6669 6775  data and configu
-00001290: 7261 7469 6f6e 2064 6972 6563 746f 7269  ration directori
-000012a0: 6573 2074 6861 7420 6172 656e 2774 2064  es that aren't d
-000012b0: 656c 6574 6564 2077 6865 6e0a 7069 7020  eleted when.pip 
-000012c0: 756e 696e 7374 616c 6c65 642e 2059 6f75  uninstalled. You
-000012d0: 2063 616e 2066 696e 6420 7468 6569 7220   can find their 
-000012e0: 6c6f 6361 7469 6f6e 7320 6279 2072 756e  locations by run
-000012f0: 6e69 6e67 2028 6265 666f 7265 200a 756e  ning (before .un
-00001300: 696e 7374 616c 6c61 7469 6f6e 293a 0a0a  installation):..
-00001310: 6060 600a 696d 706f 7274 2070 7972 6f6c  ```.import pyrol
-00001320: 6162 0a70 7269 6e74 2870 7972 6f6c 6162  ab.print(pyrolab
-00001330: 2e50 5952 4f4c 4142 5f44 4154 415f 4449  .PYROLAB_DATA_DI
-00001340: 5229 0a70 7269 6e74 2870 7972 6f6c 6162  R).print(pyrolab
-00001350: 2e50 5952 4f4c 4142 5f43 4f4e 4649 475f  .PYROLAB_CONFIG_
-00001360: 4449 5229 0a60 6060 0a0a 5468 6573 6520  DIR).```..These 
-00001370: 666f 6c64 6572 7320 6361 6e20 6265 2073  folders can be s
-00001380: 6166 656c 7920 6465 6c65 7465 6420 6166  afely deleted af
-00001390: 7465 7220 756e 696e 7374 616c 6c61 7469  ter uninstallati
-000013a0: 6f6e 2e0a 0a23 2320 4578 616d 706c 650a  on...## Example.
-000013b0: 0a23 2323 204c 6f63 616c 2049 6e73 7472  .### Local Instr
-000013c0: 756d 656e 7473 0a0a 4c6f 6361 6c6c 7920  uments..Locally 
-000013d0: 6176 6169 6c61 626c 6520 696e 7374 7275  available instru
-000013e0: 6d65 6e74 7320 6a75 7374 2069 6d70 6f72  ments just impor
-000013f0: 7420 6472 6976 6572 7320 7769 7468 6f75  t drivers withou
-00001400: 7420 7573 696e 6720 616e 7920 6f66 2074  t using any of t
-00001410: 6865 200a 6f74 6865 7220 6665 6174 7572  he .other featur
-00001420: 6573 206f 6620 5079 726f 4c61 622e 0a0a  es of PyroLab...
-00001430: 6060 600a 6672 6f6d 2070 7972 6f6c 6162  ```.from pyrolab
-00001440: 2e64 7269 7665 7273 2e6c 6173 6572 732e  .drivers.lasers.
-00001450: 7473 6c35 3530 2069 6d70 6f72 7420 5453  tsl550 import TS
-00001460: 4c35 3530 0a0a 6c61 7365 7220 3d20 5453  L550..laser = TS
-00001470: 4c35 3530 2822 434f 4d34 2229 0a6c 6173  L550("COM4").las
-00001480: 6572 2e6f 6e28 290a 6c61 7365 722e 706f  er.on().laser.po
-00001490: 7765 725f 6442 6d28 3132 290a 6c61 7365  wer_dBm(12).lase
-000014a0: 722e 6f70 656e 5f73 6875 7474 6572 2829  r.open_shutter()
-000014b0: 0a6c 6173 6572 2e73 7765 6570 5f73 6574  .laser.sweep_set
-000014c0: 5f6d 6f64 6528 636f 6e74 696e 756f 7573  _mode(continuous
-000014d0: 3d54 7275 652c 2074 776f 7761 793d 5472  =True, twoway=Tr
-000014e0: 7565 2c20 7472 6967 6765 723d 4661 6c73  ue, trigger=Fals
-000014f0: 652c 2063 6f6e 7374 5f66 7265 715f 7374  e, const_freq_st
-00001500: 6570 3d46 616c 7365 290a 6060 600a 0a23  ep=False).```..#
-00001510: 2323 2052 656d 6f74 6520 496e 7374 7275  ## Remote Instru
-00001520: 6d65 6e74 730a 0a46 6972 7374 2c20 6d61  ments..First, ma
-00001530: 6b65 2073 7572 6520 616c 6c20 636f 6e66  ke sure all conf
-00001540: 6967 7572 6174 696f 6e73 206f 6e20 7468  igurations on th
-00001550: 6520 6e61 6d65 7365 7276 6572 2063 6f6d  e nameserver com
-00001560: 7075 7465 722c 2069 6e73 7472 756d 656e  puter, instrumen
-00001570: 7420 0a73 6572 7665 7220 636f 6d70 7574  t .server comput
-00001580: 6572 2c20 616e 6420 636c 6965 6e74 2061  er, and client a
-00001590: 7265 2063 6f72 7265 6374 2028 7769 7468  re correct (with
-000015a0: 2074 6865 2070 726f 7065 7220 6b65 7973   the proper keys
-000015b0: 2c20 6966 2063 6f6e 6669 6775 7265 642c  , if configured,
-000015c0: 200a 6574 632e 292e 0a0a 5275 6e20 6120   .etc.)...Run a 
-000015d0: 6e61 6d65 7365 7276 6572 3a0a 0a60 6060  nameserver:..```
-000015e0: 7079 7468 6f6e 0a66 726f 6d20 7079 726f  python.from pyro
-000015f0: 6c61 622e 6170 6920 696d 706f 7274 2073  lab.api import s
-00001600: 7461 7274 5f6e 735f 6c6f 6f70 0a73 7461  tart_ns_loop.sta
-00001610: 7274 5f6e 735f 6c6f 6f70 2829 0a60 6060  rt_ns_loop().```
-00001620: 0a0a 5072 6f76 6964 6520 6120 7365 7276  ..Provide a serv
-00001630: 6963 653a 0a0a 6060 6070 7974 686f 6e0a  ice:..```python.
-00001640: 6672 6f6d 2070 7972 6f6c 6162 2e61 7069  from pyrolab.api
-00001650: 2069 6d70 6f72 7420 4461 656d 6f6e 2c20   import Daemon, 
-00001660: 6c6f 6361 7465 5f6e 730a 6672 6f6d 2070  locate_ns.from p
-00001670: 7972 6f6c 6162 2e64 7269 7665 7273 2e73  yrolab.drivers.s
-00001680: 616d 706c 6520 696d 706f 7274 2053 616d  ample import Sam
-00001690: 706c 6553 6572 7669 6365 0a0a 6461 656d  pleService..daem
-000016a0: 6f6e 203d 2044 6165 6d6f 6e28 290a 6e73  on = Daemon().ns
-000016b0: 203d 206c 6f63 6174 655f 6e73 2868 6f73   = locate_ns(hos
-000016c0: 743d 226c 6f63 616c 686f 7374 2229 0a75  t="localhost").u
-000016d0: 7269 203d 2064 6165 6d6f 6e2e 7265 6769  ri = daemon.regi
-000016e0: 7374 6572 2853 616d 706c 6553 6572 7669  ster(SampleServi
-000016f0: 6365 290a 6e73 2e72 6567 6973 7465 7228  ce).ns.register(
-00001700: 2274 6573 742e 5361 6d70 6c65 5365 7276  "test.SampleServ
-00001710: 6963 6522 2c20 7572 6929 0a0a 7472 793a  ice", uri)..try:
-00001720: 0a20 2020 2064 6165 6d6f 6e2e 7265 7175  .    daemon.requ
-00001730: 6573 744c 6f6f 7028 290a 6669 6e61 6c6c  estLoop().finall
-00001740: 793a 0a20 2020 206e 732e 7265 6d6f 7665  y:.    ns.remove
-00001750: 2822 7465 7374 2e53 616d 706c 6553 6572  ("test.SampleSer
-00001760: 7669 6365 2229 0a60 6060 0a0a 436f 6e6e  vice").```..Conn
-00001770: 6563 7420 7573 696e 6720 6120 7265 6d6f  ect using a remo
-00001780: 7465 2063 6c69 656e 743a 0a0a 6060 6070  te client:..```p
-00001790: 7974 686f 6e0a 6672 6f6d 2070 7972 6f6c  ython.from pyrol
-000017a0: 6162 2e61 7069 2069 6d70 6f72 7420 6c6f  ab.api import lo
-000017b0: 6361 7465 5f6e 732c 2050 726f 7879 0a0a  cate_ns, Proxy..
-000017c0: 6e73 203d 206c 6f63 6174 655f 6e73 2868  ns = locate_ns(h
-000017d0: 6f73 743d 226c 6f63 616c 686f 7374 2229  ost="localhost")
-000017e0: 0a75 7269 203d 206e 732e 6c6f 6f6b 7570  .uri = ns.lookup
-000017f0: 2822 7465 7374 2e53 616d 706c 6553 6572  ("test.SampleSer
-00001800: 7669 6365 2229 0a0a 7769 7468 2050 726f  vice")..with Pro
-00001810: 7879 2875 7269 2920 6173 2073 6572 7669  xy(uri) as servi
-00001820: 6365 3a0a 2020 2020 7265 7370 203d 2073  ce:.    resp = s
-00001830: 6572 7669 6365 2e65 6368 6f28 2248 656c  ervice.echo("Hel
-00001840: 6c6f 2c20 7365 7276 6572 2122 290a 2020  lo, server!").  
-00001850: 2020 7072 696e 7428 7479 7065 2872 6573    print(type(res
-00001860: 7029 2c20 7265 7370 290a 6060 600a 0a23  p), resp).```..#
-00001870: 2320 496e 7374 7275 6d65 6e74 2053 6572  # Instrument Ser
-00001880: 7665 7220 436f 6e66 6967 7572 6174 696f  ver Configuratio
-00001890: 6e0a 0a50 7972 6f4c 6162 2073 746f 7265  n..PyroLab store
-000018a0: 7320 696e 666f 726d 6174 696f 6e20 6162  s information ab
-000018b0: 6f75 7420 696e 7374 7275 6d65 6e74 7320  out instruments 
-000018c0: 616e 6420 7365 7276 6572 7320 7768 656e  and servers when
-000018d0: 2069 7420 636c 6f73 6573 2e20 5468 6973   it closes. This
-000018e0: 0a6d 6561 6e73 2074 6861 7420 6f6e 6365  .means that once
-000018f0: 2050 7972 6f4c 6162 2068 6173 2062 6565   PyroLab has bee
-00001900: 6e20 636f 6e66 6967 7572 6564 206f 6e63  n configured onc
-00001910: 652c 2065 6163 6820 7469 6d65 2069 7420  e, each time it 
-00001920: 6973 2072 6573 7461 7274 6564 2c0a 6974  is restarted,.it
-00001930: 2077 696c 6c20 7265 6d65 6d62 6572 2061   will remember a
-00001940: 6e64 2072 656c 6f61 6420 7468 6520 7072  nd reload the pr
-00001950: 6576 696f 7573 2063 6f6e 6669 6775 7261  evious configura
-00001960: 7469 6f6e 2e20 4865 6e63 652c 206f 6e63  tion. Hence, onc
-00001970: 6520 6120 7365 7276 6572 0a69 7320 7365  e a server.is se
-00001980: 7420 7570 2c20 756e 6c65 7373 2074 6865  t up, unless the
-00001990: 2061 7661 696c 6162 6c65 2069 6e73 7472   available instr
-000019a0: 756d 656e 7473 2c20 6e61 6d65 7365 7276  uments, nameserv
-000019b0: 6572 2c20 6f72 206f 7468 6572 200a 636f  er, or other .co
-000019c0: 6e66 6967 7572 6174 696f 6e73 2063 6861  nfigurations cha
-000019d0: 6e67 652c 2050 7972 6f4c 6162 2077 696c  nge, PyroLab wil
-000019e0: 6c20 6175 746f 6d61 7469 6361 6c6c 7920  l automatically 
-000019f0: 776f 726b 2077 6865 6e20 7374 6172 7465  work when starte
-00001a00: 642c 2065 7665 7279 200a 7469 6d65 210a  d, every .time!.
-00001a10: 0a46 6f72 2061 6e20 6578 616d 706c 6520  .For an example 
-00001a20: 6f66 2068 6f77 2061 206e 6577 2050 7972  of how a new Pyr
-00001a30: 6f4c 6162 2069 6e73 7472 756d 656e 7420  oLab instrument 
-00001a40: 7365 7276 6572 2073 686f 756c 6420 6265  server should be
-00001a50: 2063 6f6e 6669 6775 7265 6420 7468 650a   configured the.
-00001a60: 6669 7273 7420 7469 6d65 2069 7427 7320  first time it's 
-00001a70: 7275 6e2c 2073 6565 2060 6065 7861 6d70  run, see ``examp
-00001a80: 6c65 732f 3330 322e 7265 736f 7572 6365  les/302.resource
-00001a90: 2d6d 616e 6167 6572 2f70 7265 702e 7079  -manager/prep.py
-00001aa0: 6060 2e0a 0a23 2320 4641 5127 730a 312e  ``...## FAQ's.1.
-00001ab0: 202a 2a41 6e6f 7468 6572 2069 6e73 7472   **Another instr
-00001ac0: 756d 656e 7420 6c69 6272 6172 793f 2057  ument library? W
-00001ad0: 6861 7420 6162 6f75 7420 616c 6c20 7468  hat about all th
-00001ae0: 6520 6f74 6865 7273 3f2a 2a20 200a 2020  e others?**  .  
-00001af0: 2020 496e 206f 7572 2065 7870 6572 6965    In our experie
-00001b00: 6e63 652c 206d 616e 7920 6f66 2074 6865  nce, many of the
-00001b10: 206f 7468 6572 206c 6962 7261 7269 6573   other libraries
-00001b20: 2061 7265 2062 7567 6779 206f 7220 6861   are buggy or ha
-00001b30: 7665 2064 6966 6669 6375 6c74 790a 2020  ve difficulty.  
-00001b40: 2020 7769 7468 206e 6574 776f 726b 2063    with network c
-00001b50: 6f6e 6e65 6374 696f 6e73 2e20 536f 2c20  onnections. So, 
-00001b60: 6f75 7220 6170 7072 6f61 6368 2077 6173  our approach was
-00001b70: 2074 6f20 7265 6c79 206f 6e20 6120 7765   to rely on a we
-00001b80: 6c6c 2064 6576 656c 6f70 6564 0a20 2020  ll developed.   
-00001b90: 2061 6e64 2074 696d 652d 7465 7374 6564   and time-tested
-00001ba0: 2066 7261 6d65 776f 726b 2028 5079 726f   framework (Pyro
-00001bb0: 2920 696e 7374 6561 6420 6f66 2077 6f72  ) instead of wor
-00001bc0: 7279 696e 6720 6162 6f75 7420 6465 7665  rying about deve
-00001bd0: 6c6f 7069 6e67 2061 6e64 0a20 2020 2073  loping and.    s
-00001be0: 7570 706f 7274 696e 6720 6f75 7220 6f77  upporting our ow
-00001bf0: 6e20 6375 7374 6f6d 2073 6574 206f 6620  n custom set of 
-00001c00: 7365 7276 6572 732e 0a0a 322e 202a 2a49  servers...2. **I
-00001c10: 7320 7468 6973 2061 2073 7461 6e64 616c  s this a standal
-00001c20: 6f6e 6520 736f 6674 7761 7265 2074 6861  one software tha
-00001c30: 7420 6175 746f 6d61 7469 6361 6c6c 7920  t automatically 
-00001c40: 7375 7070 6f72 7473 2061 6c6c 2074 6865  supports all the
-00001c50: 2061 6476 6572 7469 7365 6420 0a69 6e73   advertised .ins
-00001c60: 7472 756d 656e 7473 3f2a 2a20 200a 2020  truments?**  .  
-00001c70: 2020 4e6f 3b20 6d61 6e79 206f 6620 7468    No; many of th
-00001c80: 6573 6520 696e 7374 7275 6d65 6e74 7320  ese instruments 
-00001c90: 6465 7065 6e64 206f 6e20 6f74 6865 7220  depend on other 
-00001ca0: 736f 6674 7761 7265 2061 6c72 6561 6479  software already
-00001cb0: 2062 6569 6e67 0a20 2020 2069 6e73 7461   being.    insta
-00001cc0: 6c6c 6564 2e20 496e 2070 6172 7469 6375  lled. In particu
-00001cd0: 6c61 722c 2054 686f 724c 6162 7320 6571  lar, ThorLabs eq
-00001ce0: 7569 706d 656e 7420 6465 7065 6e64 7320  uipment depends 
-00001cf0: 6f6e 2054 686f 724c 6162 7320 736f 6674  on ThorLabs soft
-00001d00: 7761 7265 0a20 2020 2061 6c72 6561 6479  ware.    already
-00001d10: 2062 6569 6e67 2069 6e73 7461 6c6c 6564   being installed
-00001d20: 206f 6e20 7468 6520 636f 6d70 7574 6572   on the computer
-00001d30: 2063 6f6e 6e65 6374 6564 2074 6f20 7468   connected to th
-00001d40: 6520 7068 7973 6963 616c 2068 6172 6477  e physical hardw
-00001d50: 6172 650a 2020 2020 2862 7574 206e 6f74  are.    (but not
-00001d60: 206f 6e20 7468 6520 7265 6d6f 7465 2063   on the remote c
-00001d70: 6f6d 7075 7465 7221 292e 2041 7320 6d75  omputer!). As mu
-00001d80: 6368 2061 7320 706f 7373 6962 6c65 2c20  ch as possible, 
-00001d90: 7468 6f75 6768 2c20 7765 2074 7279 2074  though, we try t
-00001da0: 6f0a 2020 2020 6d61 6b65 2074 6865 2064  o.    make the d
-00001db0: 7269 7665 7273 2073 7461 6e64 616c 6f6e  rivers standalon
-00001dc0: 6520 6361 7061 626c 652e 0a0a 2323 2046  e capable...## F
-00001dd0: 6f72 2044 6576 656c 6f70 6572 730a 0a53  or Developers..S
-00001de0: 696e 6365 2074 6865 2070 6173 7369 6e67  ince the passing
-00001df0: 206f 6620 6461 7461 2069 732c 2062 7920   of data is, by 
-00001e00: 6465 6669 6e69 7469 6f6e 2c20 6265 7477  definition, betw
-00001e10: 6565 6e20 686f 7374 7320 616e 6420 6f76  een hosts and ov
-00001e20: 6572 2049 502c 2050 7972 6f4c 6162 0a61  er IP, PyroLab.a
-00001e30: 766f 6964 7320 7468 6520 7573 6520 6f66  voids the use of
-00001e40: 2063 6f6d 706c 6578 2050 7974 686f 6e20   complex Python 
-00001e50: 6f62 6a65 6374 7320 666f 7220 7265 7475  objects for retu
-00001e60: 726e 2076 616c 7565 7320 7468 6174 2077  rn values that w
-00001e70: 696c 6c20 6265 200a 7472 616e 736d 6974  ill be .transmit
-00001e80: 7465 6420 746f 2072 656d 6f74 6520 6d61  ted to remote ma
-00001e90: 6368 696e 6573 2e20 5369 6e63 6520 7365  chines. Since se
-00001ea0: 7269 616c 697a 6174 696f 6e20 6973 2063  rialization is c
-00001eb0: 6f6d 706c 6963 6174 6564 2c20 616e 640a  omplicated, and.
-00001ec0: 7365 6375 7269 7479 2069 7320 6576 656e  security is even
-00001ed0: 2068 6172 6465 722c 2077 6520 7265 736f   harder, we reso
-00001ee0: 7274 2074 6f20 7573 696e 6720 6f6e 6c79  rt to using only
-00001ef0: 2062 6173 6963 2050 7974 686f 6e20 7479   basic Python ty
-00001f00: 7065 7320 7768 656e 0a69 6e74 6572 6661  pes when.interfa
-00001f10: 6369 6e67 2077 6974 6820 6861 7264 7761  cing with hardwa
-00001f20: 7265 2028 692e 652e 2c20 5079 7468 6f6e  re (i.e., Python
-00001f30: 206c 6973 7473 2c20 696e 7473 2c20 7475   lists, ints, tu
-00001f40: 706c 6573 2c20 616e 6420 6e6f 7420 4e75  ples, and not Nu
-00001f50: 6d50 7920 0a61 7272 6179 732c 206d 6174  mPy .arrays, mat
-00001f60: 706c 6f74 6c69 6220 706c 6f74 206f 626a  plotlib plot obj
-00001f70: 6563 7473 2c20 6375 7374 6f6d 206f 626a  ects, custom obj
-00001f80: 6563 7473 2c20 6574 632e 292e 0a0a 546f  ects, etc.)...To
-00001f90: 2062 756d 7020 7665 7273 696f 6e20 7072   bump version pr
-00001fa0: 696f 7220 746f 2061 2072 656c 6561 7365  ior to a release
-00001fb0: 2c20 7275 6e20 6f6e 6520 6f66 2074 6865  , run one of the
-00001fc0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00001fd0: 6e64 733a 0a0a 6060 6062 6173 680a 6275  nds:..```bash.bu
-00001fe0: 6d70 7665 7273 696f 6e20 6d61 6a6f 720a  mpversion major.
-00001ff0: 6275 6d70 7665 7273 696f 6e20 6d69 6e6f  bumpversion mino
-00002000: 720a 6275 6d70 7665 7273 696f 6e20 7061  r.bumpversion pa
-00002010: 7463 680a 6060 600a 0a46 6f72 2063 6f64  tch.```..For cod
-00002020: 6520 7175 616c 6974 792c 2070 6c65 6173  e quality, pleas
-00002030: 6520 7275 6e20 6973 6f72 7420 616e 6420  e run isort and 
-00002040: 626c 6163 6b20 6265 666f 7265 2063 6f6d  black before com
-00002050: 6d69 7474 696e 6720 286e 6f74 6520 7468  mitting (note th
-00002060: 6174 2074 6865 0a6c 6174 6573 7420 7265  at the.latest re
-00002070: 6c65 6173 6520 6f66 2069 736f 7274 206d  lease of isort m
-00002080: 6179 206e 6f74 2077 6f72 6b20 7468 726f  ay not work thro
-00002090: 7567 6820 5653 436f 6465 2773 2069 6e74  ugh VSCode's int
-000020a0: 6567 7261 7465 6420 7465 726d 696e 616c  egrated terminal
-000020b0: 2c20 616e 640a 6974 2773 2073 6166 6573  , and.it's safes
-000020c0: 7420 746f 2072 756e 2069 7420 7365 7061  t to run it sepa
-000020d0: 7261 7465 6c79 2074 6872 6f75 6768 2061  rately through a
-000020e0: 6e6f 7468 6572 2074 6572 6d69 6e61 6c29  nother terminal)
-000020f0: 2e0a 0a52 656c 6561 7365 7320 6172 6520  ...Releases are 
-00002100: 6175 746f 6d61 7469 6361 6c6c 7920 6372  automatically cr
-00002110: 6561 7465 6420 7768 656e 2067 6974 2074  eated when git t
-00002120: 6167 7320 6d61 7463 6869 6e67 2074 6865  ags matching the
-00002130: 2022 762a 2220 7061 7474 6572 6e0a 6172   "v*" pattern.ar
-00002140: 6520 6372 6561 7465 642e 0a0a 2323 2042  e created...## B
-00002150: 7569 6c64 696e 6720 7468 6520 446f 6373  uilding the Docs
-00002160: 0a0a 4d75 6368 206f 6620 7468 6520 4150  ..Much of the AP
-00002170: 4920 646f 6375 6d65 6e74 6174 696f 6e20  I documentation 
-00002180: 6973 2061 7574 6f67 656e 6572 6174 6564  is autogenerated
-00002190: 2066 726f 6d20 7468 6520 736f 7572 6365   from the source
-000021a0: 2063 6f64 652e 2044 7565 2074 6f0a 7468   code. Due to.th
-000021b0: 6973 2c20 746f 206d 6169 6e74 6169 6e20  is, to maintain 
-000021c0: 6120 636c 6561 6e20 7265 706f 7369 746f  a clean reposito
-000021d0: 7279 2c20 6d61 6b65 2073 7572 6520 746f  ry, make sure to
-000021e0: 206e 6576 6572 2063 6f6d 6d69 7420 7468   never commit th
-000021f0: 6520 6469 7265 6374 6f72 790a 6060 2f64  e directory.``/d
-00002200: 6f63 732f 7265 6665 7265 6e63 652f 6170  ocs/reference/ap
-00002210: 6960 6020 746f 2047 6974 2e20 416c 7761  i`` to Git. Alwa
-00002220: 7973 2064 656c 6574 6520 7468 6973 2066  ys delete this f
-00002230: 6f6c 6465 7220 6265 666f 7265 2063 6f6d  older before com
-00002240: 6d69 7474 696e 672e 0a0a 0a              mitting....
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
+00000020: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000030: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f42  sercontent.com/B
+00000040: 5955 4361 6d61 6368 6f4c 6162 2f70 7972  YUCamachoLab/pyr
+00000050: 6f6c 6162 2f6d 6173 7465 722f 646f 6373  olab/master/docs
+00000060: 2f5f 7374 6174 6963 2f69 6d61 6765 732f  /_static/images/
+00000070: 7079 726f 6c61 625f 6c6f 676f 2e73 7667  pyrolab_logo.svg
+00000080: 2220 7769 6474 683d 2234 3025 2220 616c  " width="40%" al
+00000090: 743d 2250 7972 6f4c 6162 223e 0a3c 2f70  t="PyroLab">.</p
+000000a0: 3e0a 0a2d 2d2d 0a0a 3c70 2061 6c69 676e  >..---..<p align
+000000b0: 3d22 6365 6e74 6572 223e 0a3c 696d 6720  ="center">.<img 
+000000c0: 616c 743d 2244 6576 656c 6f70 6d65 6e74  alt="Development
+000000d0: 2076 6572 7369 6f6e 2220 7372 633d 2268   version" src="h
+000000e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000000f0: 6473 2e69 6f2f 6261 6467 652f 6d61 7374  ds.io/badge/mast
+00000100: 6572 2d76 302e 332e 302d 696e 666f 726d  er-v0.3.0-inform
+00000110: 6174 696f 6e61 6c22 3e0a 3c61 2068 7265  ational">.<a hre
+00000120: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00000130: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
+00000140: 7079 726f 6c61 6222 3e3c 696d 6720 616c  pyrolab"><img al
+00000150: 743d 2250 7950 4920 5665 7273 696f 6e22  t="PyPI Version"
+00000160: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000170: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000180: 692f 762f 7079 726f 6c61 622e 7376 6722  i/v/pyrolab.svg"
+00000190: 3e3c 2f61 3e0a 3c69 6d67 2061 6c74 3d22  ></a>.<img alt="
+000001a0: 5079 5049 202d 2050 7974 686f 6e20 5665  PyPI - Python Ve
+000001b0: 7273 696f 6e22 2073 7263 3d22 6874 7470  rsion" src="http
+000001c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000001d0: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+000001e0: 6e73 2f70 7972 6f6c 6162 223e 0a3c 6120  ns/pyrolab">.<a 
+000001f0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000200: 726f 6c61 622e 7265 6164 7468 6564 6f63  rolab.readthedoc
+00000210: 732e 696f 2f22 3e3c 696d 6720 616c 743d  s.io/"><img alt=
+00000220: 2244 6f63 756d 656e 7461 7469 6f6e 2053  "Documentation S
+00000230: 7461 7475 7322 2073 7263 3d22 6874 7470  tatus" src="http
+00000240: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
+00000250: 6f72 672f 7072 6f6a 6563 7473 2f70 7972  org/projects/pyr
+00000260: 6f6c 6162 2f62 6164 6765 2f3f 7665 7273  olab/badge/?vers
+00000270: 696f 6e3d 6c61 7465 7374 223e 3c2f 613e  ion=latest"></a>
+00000280: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000290: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+000002a0: 672f 7079 7069 2f70 7972 6f6c 6162 2f22  g/pypi/pyrolab/"
+000002b0: 3e3c 696d 6720 616c 743d 224c 6963 656e  ><img alt="Licen
+000002c0: 7365 2220 7372 633d 2268 7474 7073 3a2f  se" src="https:/
+000002d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000002e0: 7079 7069 2f6c 2f70 7972 6f6c 6162 2e73  pypi/l/pyrolab.s
+000002f0: 7667 223e 3c2f 613e 0a3c 6120 6872 6566  vg"></a>.<a href
+00000300: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000310: 2e63 6f6d 2f42 5955 4361 6d61 6368 6f4c  .com/BYUCamachoL
+00000320: 6162 2f70 7972 6f6c 6162 2f63 6f6d 6d69  ab/pyrolab/commi
+00000330: 7473 2f6d 6173 7465 7222 3e3c 696d 6720  ts/master"><img 
+00000340: 616c 743d 224c 6174 6573 7420 436f 6d6d  alt="Latest Comm
+00000350: 6974 2220 7372 633d 2268 7474 7073 3a2f  it" src="https:/
+00000360: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000370: 6769 7468 7562 2f6c 6173 742d 636f 6d6d  github/last-comm
+00000380: 6974 2f42 5955 4361 6d61 6368 6f4c 6162  it/BYUCamachoLab
+00000390: 2f70 7972 6f6c 6162 2e73 7667 223e 3c2f  /pyrolab.svg"></
+000003a0: 613e 0a3c 2f70 3e0a 0a41 2066 7261 6d65  a>.</p>..A frame
+000003b0: 776f 726b 2066 6f72 2075 7369 6e67 2072  work for using r
+000003c0: 656d 6f74 6520 6c61 6220 696e 7374 7275  emote lab instru
+000003d0: 6d65 6e74 7320 6173 206c 6f63 616c 2072  ments as local r
+000003e0: 6573 6f75 7263 6573 2c20 6275 696c 7420  esources, built 
+000003f0: 6f6e 2050 7972 6f35 2e0a 0a44 6576 656c  on Pyro5...Devel
+00000400: 6f70 6564 2062 7920 5365 7175 6f69 6120  oped by Sequoia 
+00000410: 506c 6f65 6720 2866 6f72 205b 4361 6d61  Ploeg (for [Cama
+00000420: 6368 6f4c 6162 5d28 6874 7470 733a 2f2f  choLab](https://
+00000430: 6361 6d61 6368 6f6c 6162 2e62 7975 2e65  camacholab.byu.e
+00000440: 6475 2f29 2c20 0a42 7269 6768 616d 2059  du/), .Brigham Y
+00000450: 6f75 6e67 2055 6e69 7665 7273 6974 7929  oung University)
+00000460: 2e0a 0a23 2320 4162 6f75 740a 5468 6973  ...## About.This
+00000470: 2070 726f 6a65 6374 2061 696d 7320 746f   project aims to
+00000480: 2061 6c6c 6f77 2061 6c6c 206c 6162 6f72   allow all labor
+00000490: 6174 6f72 7920 696e 7374 7275 6d65 6e74  atory instrument
+000004a0: 7320 746f 2062 6520 6163 6365 7373 6564  s to be accessed
+000004b0: 2061 730a 6c6f 6361 6c20 6f62 6a65 6374   as.local object
+000004c0: 7320 6672 6f6d 2061 2072 656d 6f74 6520  s from a remote 
+000004d0: 6d61 6368 696e 652e 2049 6e73 7472 756d  machine. Instrum
+000004e0: 656e 7473 2074 6861 7420 646f 6e27 7420  ents that don't 
+000004f0: 6e61 7469 7665 6c79 0a73 7570 706f 7274  natively.support
+00000500: 2073 7563 6820 6163 6365 7373 2c20 7375   such access, su
+00000510: 6368 2061 7320 7468 6f73 6520 7265 7175  ch as those requ
+00000520: 6972 6564 2074 6f20 6265 2063 6f6e 6e65  ired to be conne
+00000530: 6374 6564 2062 7920 6120 5553 4220 6361  cted by a USB ca
+00000540: 626c 650a 286f 7220 7369 6d69 6c61 7229  ble.(or similar)
+00000550: 2c20 6172 6520 7772 6170 7065 6420 7769  , are wrapped wi
+00000560: 7468 2061 2050 7972 6f35 2069 6e74 6572  th a Pyro5 inter
+00000570: 6661 6365 2e20 486f 7765 7665 722c 2074  face. However, t
+00000580: 6869 7320 6c69 6272 6172 7920 6d61 790a  his library may.
+00000590: 636f 6e74 6169 6e20 6f74 6865 7220 696e  contain other in
+000005a0: 7374 7275 6d65 6e74 7320 7468 6174 2061  struments that a
+000005b0: 7265 2061 6c72 6561 6479 2069 6e74 6572  re already inter
+000005c0: 6e65 742d 6361 7061 626c 6520 616e 6420  net-capable and 
+000005d0: 646f 6e27 7420 7265 6c79 0a6f 6e20 5079  don't rely.on Py
+000005e0: 726f 352e 2054 6861 7427 7320 616c 7269  ro5. That's alri
+000005f0: 6768 743b 2077 6527 7265 206a 7573 7420  ght; we're just 
+00000600: 7472 7969 6e67 2074 6f20 6372 6561 7465  trying to create
+00000610: 2061 206d 696e 696d 616c 2d64 6570 656e   a minimal-depen
+00000620: 6465 6e63 792c 0a6f 6e65 2d73 746f 702d  dency,.one-stop-
+00000630: 7368 6f70 2066 6f72 206c 6162 6f72 6174  shop for laborat
+00000640: 6f72 7920 696e 7374 7275 6d65 6e74 7321  ory instruments!
+00000650: 0a0a 2a2a 4e6f 7465 3a2a 2a20 7768 696c  ..**Note:** whil
+00000660: 6520 7468 6520 736f 6674 7761 7265 2073  e the software s
+00000670: 6179 7320 224f 5320 496e 6465 7065 6e64  ays "OS Independ
+00000680: 656e 7422 2c20 736f 6d65 206f 6620 7468  ent", some of th
+00000690: 6520 7365 7276 6572 7320 2a61 7265 2a0a  e servers *are*.
+000006a0: 4f53 2d73 7065 6369 6669 632e 2046 6f72  OS-specific. For
+000006b0: 2065 7861 6d70 6c65 2c20 5468 6f72 4c61   example, ThorLa
+000006c0: 6273 2044 4c4c 2773 206f 6e6c 7920 776f  bs DLL's only wo
+000006d0: 726b 206f 6e20 5769 6e64 6f77 732e 2048  rk on Windows. H
+000006e0: 6f77 6576 6572 2c20 796f 7520 636f 756c  owever, you coul
+000006f0: 640a 7573 6520 5079 726f 4c61 6220 746f  d.use PyroLab to
+00000700: 2063 6f6e 6e65 6374 2074 6f20 7468 6f73   connect to thos
+00000710: 6520 6465 7669 6365 7320 6672 6f6d 2061  e devices from a
+00000720: 6e79 206f 7065 7261 7469 6e67 2073 7973  ny operating sys
+00000730: 7465 6d2e 0a0a 2323 2049 6e73 7461 6c6c  tem...## Install
+00000740: 6174 696f 6e0a 0a50 7972 6f4c 6162 2069  ation..PyroLab i
+00000750: 7320 7069 7020 696e 7374 616c 6c61 626c  s pip installabl
+00000760: 653a 0a0a 6060 600a 7069 7020 696e 7374  e:..```.pip inst
+00000770: 616c 6c20 7079 726f 6c61 620a 6060 600a  all pyrolab.```.
+00000780: 0a50 7972 6f4c 6162 2064 6563 6c61 7265  .PyroLab declare
+00000790: 7320 7365 7665 7261 6c20 2265 7874 7261  s several "extra
+000007a0: 7322 2c20 6465 7065 6e64 696e 6720 6f6e  s", depending on
+000007b0: 2077 6869 6368 2069 6e73 7472 756d 656e   which instrumen
+000007c0: 7473 2079 6f75 206e 6565 640a 746f 2073  ts you need.to s
+000007d0: 7570 706f 7274 3a0a 0a60 6060 0a70 6970  upport:..```.pip
+000007e0: 2069 6e73 7461 6c6c 2070 7972 6f6c 6162   install pyrolab
+000007f0: 5b74 736c 3535 302c 206f 7363 6f70 655d  [tsl550, oscope]
+00000800: 0a60 6060 0a0a 5468 6520 6675 6c6c 206c  .```..The full l
+00000810: 6973 7420 6f66 2073 7570 706f 7274 6564  ist of supported
+00000820: 2065 7874 7261 7320 6973 3a0a 2d20 7473   extras is:.- ts
+00000830: 6c35 3530 0a2d 206f 7363 6f70 650a 2d20  l550.- oscope.- 
+00000840: 6172 6475 696e 6f0a 2d20 6d6f 6e69 746f  arduino.- monito
+00000850: 720a 0a59 6f75 2063 616e 2061 6c73 6f20  r..You can also 
+00000860: 636c 6f6e 6520 7468 6520 7265 706f 7369  clone the reposi
+00000870: 746f 7279 2c20 6e61 7669 6761 7465 2074  tory, navigate t
+00000880: 6f20 7468 6520 746f 706c 6576 656c 2c20  o the toplevel, 
+00000890: 616e 6420 696e 7374 616c 6c20 696e 200a  and install in .
+000008a0: 6564 6974 6162 6c65 206d 6f64 6520 286d  editable mode (m
+000008b0: 616b 6520 7375 7265 2079 6f75 2068 6176  ake sure you hav
+000008c0: 6520 7069 7020 3e3d 2032 312e 3129 3a0a  e pip >= 21.1):.
+000008d0: 0a60 6060 0a70 6970 2069 6e73 7461 6c6c  .```.pip install
+000008e0: 202d 6520 2e0a 6060 600a 0a23 2320 5765   -e ..```..## We
+000008f0: 6220 4d6f 6e69 746f 720a 0a50 7972 6f4c  b Monitor..PyroL
+00000900: 6162 2063 6f6d 6573 2077 6974 6820 6120  ab comes with a 
+00000910: 7765 6220 6170 706c 6963 6174 696f 6e20  web application 
+00000920: 7468 6174 2063 616e 206d 6f6e 6974 6f72  that can monitor
+00000930: 2079 6f75 7220 6e61 6d65 7365 7276 6572   your nameserver
+00000940: 2061 6e64 200a 7072 6f76 6964 6520 616e   and .provide an
+00000950: 2065 6173 792d 746f 2d61 6363 6573 7320   easy-to-access 
+00000960: 7374 6174 7573 2062 6f61 7264 2e20 4974  status board. It
+00000970: 2773 2061 2046 6c61 736b 2061 7070 2074  's a Flask app t
+00000980: 6861 7420 6361 6e20 6265 2073 6572 7665  hat can be serve
+00000990: 640a 7573 696e 6720 6120 7072 6f64 7563  d.using a produc
+000009a0: 7469 6f6e 2067 7261 6465 2073 6572 7665  tion grade serve
+000009b0: 722e 2054 6f20 7275 6e3a 0a0a 6060 600a  r. To run:..```.
+000009c0: 7079 726f 6d6f 6e69 746f 7220 7570 0a60  pyromonitor up.`
+000009d0: 6060 0a0a 2323 2045 7861 6d70 6c65 0a0a  ``..## Example..
+000009e0: 2323 2320 4c6f 6361 6c20 496e 7374 7275  ### Local Instru
+000009f0: 6d65 6e74 730a 0a4c 6f63 616c 6c79 2061  ments..Locally a
+00000a00: 7661 696c 6162 6c65 2069 6e73 7472 756d  vailable instrum
+00000a10: 656e 7473 206a 7573 7420 696d 706f 7274  ents just import
+00000a20: 2064 7269 7665 7273 2077 6974 686f 7574   drivers without
+00000a30: 2075 7369 6e67 2061 6e79 206f 6620 7468   using any of th
+00000a40: 6520 0a6f 7468 6572 2066 6561 7475 7265  e .other feature
+00000a50: 7320 6f66 2050 7972 6f4c 6162 2e0a 0a60  s of PyroLab...`
+00000a60: 6060 0a66 726f 6d20 7079 726f 6c61 622e  ``.from pyrolab.
+00000a70: 6472 6976 6572 732e 6c61 7365 7273 2e74  drivers.lasers.t
+00000a80: 736c 3535 3020 696d 706f 7274 2054 534c  sl550 import TSL
+00000a90: 3535 300a 0a6c 6173 6572 203d 2054 534c  550..laser = TSL
+00000aa0: 3535 3028 2243 4f4d 3422 290a 6c61 7365  550("COM4").lase
+00000ab0: 722e 6f6e 2829 0a6c 6173 6572 2e70 6f77  r.on().laser.pow
+00000ac0: 6572 5f64 426d 2831 3229 0a6c 6173 6572  er_dBm(12).laser
+00000ad0: 2e6f 7065 6e5f 7368 7574 7465 7228 290a  .open_shutter().
+00000ae0: 6c61 7365 722e 7377 6565 705f 7365 745f  laser.sweep_set_
+00000af0: 6d6f 6465 2863 6f6e 7469 6e75 6f75 733d  mode(continuous=
+00000b00: 5472 7565 2c20 7477 6f77 6179 3d54 7275  True, twoway=Tru
+00000b10: 652c 2074 7269 6767 6572 3d46 616c 7365  e, trigger=False
+00000b20: 2c20 636f 6e73 745f 6672 6571 5f73 7465  , const_freq_ste
+00000b30: 703d 4661 6c73 6529 0a60 6060 0a0a 2323  p=False).```..##
+00000b40: 2320 5265 6d6f 7465 2049 6e73 7472 756d  # Remote Instrum
+00000b50: 656e 7473 0a0a 4669 7273 742c 206d 616b  ents..First, mak
+00000b60: 6520 7375 7265 2061 6c6c 2063 6f6e 6669  e sure all confi
+00000b70: 6775 7261 7469 6f6e 7320 6f6e 2074 6865  gurations on the
+00000b80: 206e 616d 6573 6572 7665 7220 636f 6d70   nameserver comp
+00000b90: 7574 6572 2c20 696e 7374 7275 6d65 6e74  uter, instrument
+00000ba0: 200a 7365 7276 6572 2063 6f6d 7075 7465   .server compute
+00000bb0: 722c 2061 6e64 2063 6c69 656e 7420 6172  r, and client ar
+00000bc0: 6520 636f 7272 6563 7420 2877 6974 6820  e correct (with 
+00000bd0: 7468 6520 7072 6f70 6572 206b 6579 732c  the proper keys,
+00000be0: 2069 6620 636f 6e66 6967 7572 6564 2c20   if configured, 
+00000bf0: 0a65 7463 2e29 2e0a 0a52 756e 2061 206e  .etc.)...Run a n
+00000c00: 616d 6573 6572 7665 723a 0a0a 6060 6070  ameserver:..```p
+00000c10: 7974 686f 6e0a 6672 6f6d 2070 7972 6f6c  ython.from pyrol
+00000c20: 6162 2e61 7069 2069 6d70 6f72 7420 7374  ab.api import st
+00000c30: 6172 745f 6e73 5f6c 6f6f 700a 7374 6172  art_ns_loop.star
+00000c40: 745f 6e73 5f6c 6f6f 7028 290a 6060 600a  t_ns_loop().```.
+00000c50: 0a50 726f 7669 6465 2061 2073 6572 7669  .Provide a servi
+00000c60: 6365 3a0a 0a60 6060 7079 7468 6f6e 0a66  ce:..```python.f
+00000c70: 726f 6d20 7079 726f 6c61 622e 6170 6920  rom pyrolab.api 
+00000c80: 696d 706f 7274 2044 6165 6d6f 6e2c 206c  import Daemon, l
+00000c90: 6f63 6174 655f 6e73 0a66 726f 6d20 7079  ocate_ns.from py
+00000ca0: 726f 6c61 622e 6472 6976 6572 732e 7361  rolab.drivers.sa
+00000cb0: 6d70 6c65 2069 6d70 6f72 7420 5361 6d70  mple import Samp
+00000cc0: 6c65 5365 7276 6963 650a 0a64 6165 6d6f  leService..daemo
+00000cd0: 6e20 3d20 4461 656d 6f6e 2829 0a6e 7320  n = Daemon().ns 
+00000ce0: 3d20 6c6f 6361 7465 5f6e 7328 686f 7374  = locate_ns(host
+00000cf0: 3d22 6c6f 6361 6c68 6f73 7422 290a 7572  ="localhost").ur
+00000d00: 6920 3d20 6461 656d 6f6e 2e72 6567 6973  i = daemon.regis
+00000d10: 7465 7228 5361 6d70 6c65 5365 7276 6963  ter(SampleServic
+00000d20: 6529 0a6e 732e 7265 6769 7374 6572 2822  e).ns.register("
+00000d30: 7465 7374 2e53 616d 706c 6553 6572 7669  test.SampleServi
+00000d40: 6365 222c 2075 7269 290a 0a74 7279 3a0a  ce", uri)..try:.
+00000d50: 2020 2020 6461 656d 6f6e 2e72 6571 7565      daemon.reque
+00000d60: 7374 4c6f 6f70 2829 0a66 696e 616c 6c79  stLoop().finally
+00000d70: 3a0a 2020 2020 6e73 2e72 656d 6f76 6528  :.    ns.remove(
+00000d80: 2274 6573 742e 5361 6d70 6c65 5365 7276  "test.SampleServ
+00000d90: 6963 6522 290a 6060 600a 0a43 6f6e 6e65  ice").```..Conne
+00000da0: 6374 2075 7369 6e67 2061 2072 656d 6f74  ct using a remot
+00000db0: 6520 636c 6965 6e74 3a0a 0a60 6060 7079  e client:..```py
+00000dc0: 7468 6f6e 0a66 726f 6d20 7079 726f 6c61  thon.from pyrola
+00000dd0: 622e 6170 6920 696d 706f 7274 206c 6f63  b.api import loc
+00000de0: 6174 655f 6e73 2c20 5072 6f78 790a 0a6e  ate_ns, Proxy..n
+00000df0: 7320 3d20 6c6f 6361 7465 5f6e 7328 686f  s = locate_ns(ho
+00000e00: 7374 3d22 6c6f 6361 6c68 6f73 7422 290a  st="localhost").
+00000e10: 7572 6920 3d20 6e73 2e6c 6f6f 6b75 7028  uri = ns.lookup(
+00000e20: 2274 6573 742e 5361 6d70 6c65 5365 7276  "test.SampleServ
+00000e30: 6963 6522 290a 0a77 6974 6820 5072 6f78  ice")..with Prox
+00000e40: 7928 7572 6929 2061 7320 7365 7276 6963  y(uri) as servic
+00000e50: 653a 0a20 2020 2072 6573 7020 3d20 7365  e:.    resp = se
+00000e60: 7276 6963 652e 6563 686f 2822 4865 6c6c  rvice.echo("Hell
+00000e70: 6f2c 2073 6572 7665 7221 2229 0a20 2020  o, server!").   
+00000e80: 2070 7269 6e74 2874 7970 6528 7265 7370   print(type(resp
+00000e90: 292c 2072 6573 7029 0a60 6060 0a0a 2323  ), resp).```..##
+00000ea0: 2049 6e73 7472 756d 656e 7420 5365 7276   Instrument Serv
+00000eb0: 6572 2043 6f6e 6669 6775 7261 7469 6f6e  er Configuration
+00000ec0: 0a0a 5079 726f 4c61 6220 7374 6f72 6573  ..PyroLab stores
+00000ed0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
+00000ee0: 7574 2069 6e73 7472 756d 656e 7473 2061  ut instruments a
+00000ef0: 6e64 2073 6572 7665 7273 2077 6865 6e20  nd servers when 
+00000f00: 6974 2063 6c6f 7365 732e 2054 6869 730a  it closes. This.
+00000f10: 6d65 616e 7320 7468 6174 206f 6e63 6520  means that once 
+00000f20: 5079 726f 4c61 6220 6861 7320 6265 656e  PyroLab has been
+00000f30: 2063 6f6e 6669 6775 7265 6420 6f6e 6365   configured once
+00000f40: 2c20 6561 6368 2074 696d 6520 6974 2069  , each time it i
+00000f50: 7320 7265 7374 6172 7465 642c 0a69 7420  s restarted,.it 
+00000f60: 7769 6c6c 2072 656d 656d 6265 7220 616e  will remember an
+00000f70: 6420 7265 6c6f 6164 2074 6865 2070 7265  d reload the pre
+00000f80: 7669 6f75 7320 636f 6e66 6967 7572 6174  vious configurat
+00000f90: 696f 6e2e 2048 656e 6365 2c20 6f6e 6365  ion. Hence, once
+00000fa0: 2061 2073 6572 7665 720a 6973 2073 6574   a server.is set
+00000fb0: 2075 702c 2075 6e6c 6573 7320 7468 6520   up, unless the 
+00000fc0: 6176 6169 6c61 626c 6520 696e 7374 7275  available instru
+00000fd0: 6d65 6e74 732c 206e 616d 6573 6572 7665  ments, nameserve
+00000fe0: 722c 206f 7220 6f74 6865 7220 0a63 6f6e  r, or other .con
+00000ff0: 6669 6775 7261 7469 6f6e 7320 6368 616e  figurations chan
+00001000: 6765 2c20 5079 726f 4c61 6220 7769 6c6c  ge, PyroLab will
+00001010: 2061 7574 6f6d 6174 6963 616c 6c79 2077   automatically w
+00001020: 6f72 6b20 7768 656e 2073 7461 7274 6564  ork when started
+00001030: 2c20 6576 6572 7920 0a74 696d 6521 0a0a  , every .time!..
+00001040: 466f 7220 616e 2065 7861 6d70 6c65 206f  For an example o
+00001050: 6620 686f 7720 6120 6e65 7720 5079 726f  f how a new Pyro
+00001060: 4c61 6220 696e 7374 7275 6d65 6e74 2073  Lab instrument s
+00001070: 6572 7665 7220 7368 6f75 6c64 2062 6520  erver should be 
+00001080: 636f 6e66 6967 7572 6564 2074 6865 0a66  configured the.f
+00001090: 6972 7374 2074 696d 6520 6974 2773 2072  irst time it's r
+000010a0: 756e 2c20 7365 6520 6060 6578 616d 706c  un, see ``exampl
+000010b0: 6573 2f6c 6962 7261 7279 2d63 6174 616c  es/library-catal
+000010c0: 6f67 2f63 6f6e 6669 672e 7961 6d6c 6060  og/config.yaml``
+000010d0: 2e0a 0a23 2320 4641 5127 730a 312e 202a  ...## FAQ's.1. *
+000010e0: 2a41 6e6f 7468 6572 2069 6e73 7472 756d  *Another instrum
+000010f0: 656e 7420 6c69 6272 6172 793f 2057 6861  ent library? Wha
+00001100: 7420 6162 6f75 7420 616c 6c20 7468 6520  t about all the 
+00001110: 6f74 6865 7273 3f2a 2a20 200a 2020 2020  others?**  .    
+00001120: 496e 206f 7572 2065 7870 6572 6965 6e63  In our experienc
+00001130: 652c 206d 616e 7920 6f66 2074 6865 206f  e, many of the o
+00001140: 7468 6572 206c 6962 7261 7269 6573 2061  ther libraries a
+00001150: 7265 2062 7567 6779 206f 7220 6861 7665  re buggy or have
+00001160: 2064 6966 6669 6375 6c74 790a 2020 2020   difficulty.    
+00001170: 7769 7468 206e 6574 776f 726b 2063 6f6e  with network con
+00001180: 6e65 6374 696f 6e73 2e20 536f 2c20 6f75  nections. So, ou
+00001190: 7220 6170 7072 6f61 6368 2077 6173 2074  r approach was t
+000011a0: 6f20 7265 6c79 206f 6e20 6120 7765 6c6c  o rely on a well
+000011b0: 2064 6576 656c 6f70 6564 0a20 2020 2061   developed.    a
+000011c0: 6e64 2074 696d 652d 7465 7374 6564 2066  nd time-tested f
+000011d0: 7261 6d65 776f 726b 2028 5079 726f 2920  ramework (Pyro) 
+000011e0: 696e 7374 6561 6420 6f66 2077 6f72 7279  instead of worry
+000011f0: 696e 6720 6162 6f75 7420 6465 7665 6c6f  ing about develo
+00001200: 7069 6e67 2061 6e64 0a20 2020 2073 7570  ping and.    sup
+00001210: 706f 7274 696e 6720 6f75 7220 6f77 6e20  porting our own 
+00001220: 6375 7374 6f6d 2073 6574 206f 6620 7365  custom set of se
+00001230: 7276 6572 732e 0a0a 322e 202a 2a49 7320  rvers...2. **Is 
+00001240: 7468 6973 2061 2073 7461 6e64 616c 6f6e  this a standalon
+00001250: 6520 736f 6674 7761 7265 2074 6861 7420  e software that 
+00001260: 6175 746f 6d61 7469 6361 6c6c 7920 7375  automatically su
+00001270: 7070 6f72 7473 2061 6c6c 2074 6865 2061  pports all the a
+00001280: 6476 6572 7469 7365 6420 0a69 6e73 7472  dvertised .instr
+00001290: 756d 656e 7473 3f2a 2a20 200a 2020 2020  uments?**  .    
+000012a0: 4e6f 3b20 6d61 6e79 206f 6620 7468 6573  No; many of thes
+000012b0: 6520 696e 7374 7275 6d65 6e74 7320 6465  e instruments de
+000012c0: 7065 6e64 206f 6e20 6f74 6865 7220 736f  pend on other so
+000012d0: 6674 7761 7265 2061 6c72 6561 6479 2062  ftware already b
+000012e0: 6569 6e67 0a20 2020 2069 6e73 7461 6c6c  eing.    install
+000012f0: 6564 2e20 496e 2070 6172 7469 6375 6c61  ed. In particula
+00001300: 722c 2054 686f 724c 6162 7320 6571 7569  r, ThorLabs equi
+00001310: 706d 656e 7420 6465 7065 6e64 7320 6f6e  pment depends on
+00001320: 2054 686f 724c 6162 7320 736f 6674 7761   ThorLabs softwa
+00001330: 7265 0a20 2020 2061 6c72 6561 6479 2062  re.    already b
+00001340: 6569 6e67 2069 6e73 7461 6c6c 6564 206f  eing installed o
+00001350: 6e20 7468 6520 636f 6d70 7574 6572 2063  n the computer c
+00001360: 6f6e 6e65 6374 6564 2074 6f20 7468 6520  onnected to the 
+00001370: 7068 7973 6963 616c 2068 6172 6477 6172  physical hardwar
+00001380: 650a 2020 2020 2862 7574 206e 6f74 206f  e.    (but not o
+00001390: 6e20 7468 6520 7265 6d6f 7465 2063 6f6d  n the remote com
+000013a0: 7075 7465 7221 292e 2041 7320 6d75 6368  puter!). As much
+000013b0: 2061 7320 706f 7373 6962 6c65 2c20 7468   as possible, th
+000013c0: 6f75 6768 2c20 7765 2074 7279 2074 6f0a  ough, we try to.
+000013d0: 2020 2020 6d61 6b65 2074 6865 2064 7269      make the dri
+000013e0: 7665 7273 2073 7461 6e64 616c 6f6e 6520  vers standalone 
+000013f0: 6361 7061 626c 652e 0a0a 2323 2046 6f72  capable...## For
+00001400: 2044 6576 656c 6f70 6572 730a 0a53 696e   Developers..Sin
+00001410: 6365 2074 6865 2070 6173 7369 6e67 206f  ce the passing o
+00001420: 6620 6461 7461 2069 732c 2062 7920 6465  f data is, by de
+00001430: 6669 6e69 7469 6f6e 2c20 6265 7477 6565  finition, betwee
+00001440: 6e20 686f 7374 7320 616e 6420 6f76 6572  n hosts and over
+00001450: 2049 502c 2050 7972 6f4c 6162 0a61 766f   IP, PyroLab.avo
+00001460: 6964 7320 7468 6520 7573 6520 6f66 2063  ids the use of c
+00001470: 6f6d 706c 6578 2050 7974 686f 6e20 6f62  omplex Python ob
+00001480: 6a65 6374 7320 666f 7220 7265 7475 726e  jects for return
+00001490: 2076 616c 7565 7320 7468 6174 2077 696c   values that wil
+000014a0: 6c20 6265 200a 7472 616e 736d 6974 7465  l be .transmitte
+000014b0: 6420 746f 2072 656d 6f74 6520 6d61 6368  d to remote mach
+000014c0: 696e 6573 2e20 5369 6e63 6520 7365 7269  ines. Since seri
+000014d0: 616c 697a 6174 696f 6e20 6973 2063 6f6d  alization is com
+000014e0: 706c 6963 6174 6564 2c20 616e 640a 7365  plicated, and.se
+000014f0: 6375 7269 7479 2069 7320 6576 656e 2068  curity is even h
+00001500: 6172 6465 722c 2077 6520 7265 736f 7274  arder, we resort
+00001510: 2074 6f20 7573 696e 6720 6f6e 6c79 2062   to using only b
+00001520: 6173 6963 2050 7974 686f 6e20 7479 7065  asic Python type
+00001530: 7320 7768 656e 0a69 6e74 6572 6661 6369  s when.interfaci
+00001540: 6e67 2077 6974 6820 6861 7264 7761 7265  ng with hardware
+00001550: 2028 692e 652e 2c20 5079 7468 6f6e 206c   (i.e., Python l
+00001560: 6973 7473 2c20 696e 7473 2c20 7475 706c  ists, ints, tupl
+00001570: 6573 2c20 616e 6420 6e6f 7420 4e75 6d50  es, and not NumP
+00001580: 7920 0a61 7272 6179 732c 206d 6174 706c  y .arrays, matpl
+00001590: 6f74 6c69 6220 706c 6f74 206f 626a 6563  otlib plot objec
+000015a0: 7473 2c20 6375 7374 6f6d 206f 626a 6563  ts, custom objec
+000015b0: 7473 2c20 6574 632e 292e 0a0a 2323 2052  ts, etc.)...## R
+000015c0: 656c 6561 7369 6e67 0a0a 4d61 6b65 2073  eleasing..Make s
+000015d0: 7572 6520 796f 7520 6861 7665 2063 6f6d  ure you have com
+000015e0: 6d69 7474 6564 2061 2063 6861 6e67 656c  mitted a changel
+000015f0: 6f67 2066 696c 6520 756e 6465 7220 6060  og file under ``
+00001600: 646f 6373 2f63 6861 6e67 656c 6f67 6060  docs/changelog``
+00001610: 2074 6974 6c65 6420 0a60 603c 6d61 6a6f   titled .``<majo
+00001620: 723e 2e3c 6d69 6e6f 723e 2e3c 7061 7463  r>.<minor>.<patc
+00001630: 683e 2d63 6861 6e67 656c 6f67 2e6d 6460  h>-changelog.md`
+00001640: 6020 6265 666f 7265 2062 756d 7069 6e67  ` before bumping
+00001650: 2076 6572 7369 6f6e 2e20 416c 736f 2c20   version. Also, 
+00001660: 7468 6520 6769 740a 6469 7265 6374 6f72  the git.director
+00001670: 7920 7368 6f75 6c64 2062 6520 636c 6561  y should be clea
+00001680: 6e20 286e 6f20 756e 636f 6d6d 6974 7465  n (no uncommitte
+00001690: 6420 6368 616e 6765 7329 2e0a 0a54 6f20  d changes)...To 
+000016a0: 6275 6d70 2076 6572 7369 6f6e 2070 7269  bump version pri
+000016b0: 6f72 2074 6f20 6120 7265 6c65 6173 652c  or to a release,
+000016c0: 2072 756e 206f 6e65 206f 6620 7468 6520   run one of the 
+000016d0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+000016e0: 6473 3a0a 0a60 6060 0a62 756d 7076 6572  ds:..```.bumpver
+000016f0: 7369 6f6e 206d 616a 6f72 0a62 756d 7076  sion major.bumpv
+00001700: 6572 7369 6f6e 206d 696e 6f72 0a62 756d  ersion minor.bum
+00001710: 7076 6572 7369 6f6e 2070 6174 6368 0a60  pversion patch.`
+00001720: 6060 0a0a 5468 6973 2077 696c 6c20 6175  ``..This will au
+00001730: 746f 6d61 7469 6361 6c6c 7920 6372 6561  tomatically crea
+00001740: 7465 2061 2067 6974 2074 6167 2069 6e20  te a git tag in 
+00001750: 7468 6520 7265 706f 7369 746f 7279 2077  the repository w
+00001760: 6974 6820 7468 6520 0a63 6f72 7272 6573  ith the .corrres
+00001770: 706f 6e64 696e 6720 7665 7273 696f 6e20  ponding version 
+00001780: 6e75 6d62 6572 2061 6e64 2063 6f6d 6d69  number and commi
+00001790: 7420 7468 6520 6d6f 6469 6669 6564 2066  t the modified f
+000017a0: 696c 6573 2028 7768 6572 6520 7665 7273  iles (where vers
+000017b0: 696f 6e0a 6e75 6d62 6572 7320 7765 7265  ion.numbers were
+000017c0: 2075 7064 6174 6564 292e 2050 7573 6869   updated). Pushi
+000017d0: 6e67 2074 6865 2074 6167 7320 2861 206d  ng the tags (a m
+000017e0: 616e 7561 6c20 7072 6f63 6573 7329 2074  anual process) t
+000017f0: 6f20 7468 6520 7265 6d6f 7465 2077 696c  o the remote wil
+00001800: 6c20 0a61 7574 6f6d 6174 6963 616c 6c79  l .automatically
+00001810: 2063 7265 6174 6520 6120 6e65 7720 7265   create a new re
+00001820: 6c65 6173 652e 2052 656c 6561 7365 7320  lease. Releases 
+00001830: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
+00001840: 7920 7075 626c 6973 6865 6420 746f 200a  y published to .
+00001850: 5079 5049 2061 6e64 2047 6974 4875 6220  PyPI and GitHub 
+00001860: 7768 656e 2067 6974 2074 6167 7320 6d61  when git tags ma
+00001870: 7463 6869 6e67 2074 6865 2022 762a 2220  tching the "v*" 
+00001880: 7061 7474 6572 6e20 6172 6520 6372 6561  pattern are crea
+00001890: 7465 6420 0a28 652e 672e 2022 7630 2e33  ted .(e.g. "v0.3
+000018a0: 2e30 2229 2c20 6173 2062 756d 7076 6572  .0"), as bumpver
+000018b0: 7369 6f6e 2064 6f65 732e 0a0a 4166 7465  sion does...Afte
+000018c0: 7220 6275 6d70 696e 6720 7665 7273 696f  r bumping versio
+000018d0: 6e2c 2079 6f75 2063 616e 2076 6965 7720  n, you can view 
+000018e0: 7468 6520 7461 6773 206f 6e20 7468 6520  the tags on the 
+000018f0: 6c6f 6361 6c20 6d61 6368 696e 6520 6279  local machine by
+00001900: 2072 756e 6e69 6e67 200a 6060 6769 7420   running .``git 
+00001910: 7461 6760 602e 2054 6f20 7075 7368 2074  tag``. To push t
+00001920: 6865 2074 6167 7320 746f 2074 6865 2072  he tags to the r
+00001930: 656d 6f74 6520 7365 7276 6572 2061 6e64  emote server and
+00001940: 2074 7269 6767 6572 2074 6865 2072 656c   trigger the rel
+00001950: 6561 7365 0a77 6f72 6b66 6c6f 772c 2079  ease.workflow, y
+00001960: 6f75 2063 616e 2072 756e 2060 6067 6974  ou can run ``git
+00001970: 2070 7573 6820 6f72 6967 696e 203c 7461   push origin <ta
+00001980: 676e 616d 653e 6060 2e0a 0a46 6f72 2063  gname>``...For c
+00001990: 6f64 6520 7175 616c 6974 792c 2070 6c65  ode quality, ple
+000019a0: 6173 6520 7275 6e20 6973 6f72 7420 616e  ase run isort an
+000019b0: 6420 626c 6163 6b20 6265 666f 7265 2063  d black before c
+000019c0: 6f6d 6d69 7474 696e 6720 286e 6f74 6520  ommitting (note 
+000019d0: 7468 6174 2074 6865 0a6c 6174 6573 7420  that the.latest 
+000019e0: 7265 6c65 6173 6520 6f66 2069 736f 7274  release of isort
+000019f0: 206d 6179 206e 6f74 2077 6f72 6b20 7468   may not work th
+00001a00: 726f 7567 6820 5653 436f 6465 2773 2069  rough VSCode's i
+00001a10: 6e74 6567 7261 7465 6420 7465 726d 696e  ntegrated termin
+00001a20: 616c 2c20 616e 640a 6974 2773 2073 6166  al, and.it's saf
+00001a30: 6573 7420 746f 2072 756e 2069 7420 7365  est to run it se
+00001a40: 7061 7261 7465 6c79 2074 6872 6f75 6768  parately through
+00001a50: 2061 6e6f 7468 6572 2074 6572 6d69 6e61   another termina
+00001a60: 6c29 2e0a 0a23 2320 4275 696c 6469 6e67  l)...## Building
+00001a70: 2074 6865 2044 6f63 730a 0a4d 7563 6820   the Docs..Much 
+00001a80: 6f66 2074 6865 2041 5049 2064 6f63 756d  of the API docum
+00001a90: 656e 7461 7469 6f6e 2069 7320 6175 746f  entation is auto
+00001aa0: 6765 6e65 7261 7465 6420 6672 6f6d 2074  generated from t
+00001ab0: 6865 2073 6f75 7263 6520 636f 6465 2e20  he source code. 
+00001ac0: 4769 7469 676e 6f72 6573 0a61 7265 2069  Gitignores.are i
+00001ad0: 6e20 706c 6163 6520 746f 2070 7265 7665  n place to preve
+00001ae0: 6e74 2079 6f75 2066 726f 6d20 636f 6d6d  nt you from comm
+00001af0: 6974 7469 6e67 2061 7574 6f67 656e 6572  itting autogener
+00001b00: 6174 6564 2070 6167 6573 2e0a 0a54 6f20  ated pages...To 
+00001b10: 6275 696c 6420 7468 6520 646f 6373 2c20  build the docs, 
+00001b20: 6e61 7669 6761 7465 2074 6f20 7468 6520  navigate to the 
+00001b30: 6060 646f 6373 2f60 6020 6469 7265 6374  ``docs/`` direct
+00001b40: 6f72 7920 616e 6420 7275 6e3a 0a0a 6060  ory and run:..``
+00001b50: 600a 7069 7020 696e 7374 616c 6c20 2d72  `.pip install -r
+00001b60: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
+00001b70: 740a 6d61 6b65 2068 746d 6c0a 6060 600a  t.make html.```.
+00001b80: 0a23 2320 4275 696c 6469 6e67 2074 6865  .## Building the
+00001b90: 2050 6163 6b61 6765 0a0a 596f 7520 6361   Package..You ca
+00001ba0: 6e20 7465 7374 2074 6865 2062 7569 6c64  n test the build
+00001bb0: 2061 6e64 2076 6965 7720 7468 6520 6275   and view the bu
+00001bc0: 6e64 6c65 6420 6172 7469 6661 6374 7320  ndled artifacts 
+00001bd0: 7573 696e 6720 0a5b 6275 696c 645d 2868  using .[build](h
+00001be0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00001bf0: 7072 6f6a 6563 742f 6275 696c 642f 292e  project/build/).
+00001c00: 2049 7427 7320 7265 636f 6d6d 656e 6465   It's recommende
+00001c10: 6420 796f 7520 6275 696c 6420 6c6f 6361  d you build loca
+00001c20: 6c6c 790a 6265 666f 7265 2070 7573 6869  lly.before pushi
+00001c30: 6e67 2074 6f20 5079 5049 2e20 496e 2070  ng to PyPI. In p
+00001c40: 6172 7469 6375 6c61 722c 2064 6f75 626c  articular, doubl
+00001c50: 6520 6368 6563 6b20 7468 6520 696e 636c  e check the incl
+00001c60: 7564 6564 2066 696c 6573 2061 6e64 206d  uded files and m
+00001c70: 616b 650a 7375 7265 206f 6e6c 7920 7468  ake.sure only th
+00001c80: 6520 7265 7175 6972 6564 2066 696c 6573  e required files
+00001c90: 2061 7265 2074 6865 7265 2062 7920 6d6f   are there by mo
+00001ca0: 6469 6679 696e 6720 4d41 4e49 4645 5354  difying MANIFEST
+00001cb0: 2e69 6e20 6173 206e 6563 6573 7361 7279  .in as necessary
+00001cc0: 2e0a                                     ..
```

### Comparing `PyroLab-0.2.1/pyrolab/__init__.py` & `PyroLab-0.3.0/src/pyrolab/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright © 2020- PyroLab Project Contributors and others (see AUTHORS.txt).
 # The resources, libraries, and some source files under other terms (see NOTICE.txt).
 #
 # This file is part of PyroLab.
 #
 # PyroLab is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -25,101 +24,118 @@
 """
 
 import os
 import pathlib
 import platform
 import sys
 
-if sys.version_info < (3, 7, 0):
+# Check if Python version is supported
+pyversion = sys.version_info
+if pyversion < (3, 7, 0):
     raise Exception(
         "PyroLab requires Python 3.7+ (version "
         + platform.python_version()
         + " detected)."
     )
 
+
+# Metadata
 __name__ = "PyroLab"
 __author__ = "CamachoLab"
 __copyright__ = "Copyright 2020, The PyroLab Project"
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 __license__ = "GPLv3+"
 __maintainer__ = "Sequoia Ploeg"
 __maintainer_email__ = "sequoia.ploeg@byu.edu"
 __status__ = "Development" # "Production"
 __project_url__ = "https://github.com/sequoiap/pyrolab"
 __forum_url__ = "https://github.com/sequoiap/pyrolab/issues"
 __website_url__ = "https://camacholab.byu.edu/"
 
 
+# Filter warnings
 import warnings
 
 warnings.filterwarnings("default", category=DeprecationWarning)
 if "PYROLAB_HUSH_DEPRECATION" in os.environ:
     warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 
-# Hide a very annoying warnings from appnope about Python 3.12
-with warnings.catch_warnings():
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-    import appnope
-    appnope.nope()
-
-
-from appdirs import AppDirs
-
-_dirs = AppDirs(__name__, __author__)
+# Configuration directories
+# Old api deprecated in 3.11, new api added in 3.9
+if pyversion < (3, 9, 0):
+    base_path = pathlib.Path(__file__).resolve().parent
+else:
+    from importlib.resources import files
+    base_path = files("pyrolab")
+base_path = base_path / "data" / "local"
 
-# Data Directories
-PYROLAB_DATA_DIR = pathlib.Path(_dirs.user_data_dir)
+# Data directories
+PYROLAB_DATA_DIR = pathlib.Path(base_path)
 PYROLAB_DATA_DIR.mkdir(parents=True, exist_ok=True)
 
-# Configuration Directories
-PYROLAB_CONFIG_DIR = PYROLAB_DATA_DIR / "config"
-PYROLAB_CONFIG_DIR.mkdir(parents=True, exist_ok=True)
-
-# User config file directory
-CONFIG_DIR = PYROLAB_CONFIG_DIR / "user"
-CONFIG_DIR.mkdir(parents=True, exist_ok=True)
-
-# Background daemon data directory
-PYROLABD_DATA = PYROLAB_DATA_DIR / "pyrolabd"
-PYROLABD_DATA.mkdir(parents=True, exist_ok=True)
-
-NAMESERVER_STORAGE = PYROLAB_DATA_DIR / "nameservers"
+NAMESERVER_STORAGE = PYROLAB_DATA_DIR / "nameserver"
 NAMESERVER_STORAGE.mkdir(parents=True, exist_ok=True)
 
-LOCKFILE = PYROLABD_DATA / "pyrolabd.lock"
-USER_CONFIG_FILE = CONFIG_DIR / "user_configuration.yaml"
-RUNTIME_CONFIG = PYROLABD_DATA / "runtime_config.yaml"
-PYROLAB_LOGFILE = PYROLAB_DATA_DIR / "pyrolab.log"
+PYROLAB_LOGDIR = PYROLAB_DATA_DIR / "logs"
+PYROLAB_LOGDIR.mkdir(parents=True, exist_ok=True)
+
+LOCKFILE = PYROLAB_DATA_DIR / "pyrolabd.lock"
+USER_CONFIG_FILE = PYROLAB_DATA_DIR / "user_configuration.yaml"
+RUNTIME_CONFIG = PYROLAB_DATA_DIR / "runtime_config.yaml"
 
 
 # Set up logging to file
 import logging
 import logging.handlers
 
 
 def get_loglevel() -> int:
     loglevel = os.getenv("PYROLAB_LOGLEVEL", "INFO")
     try:
         loglevel = getattr(logging, loglevel.upper())
     except AttributeError:
         loglevel = logging.INFO
-    loglevel = logging.DEBUG
     return loglevel
 
-if len(logging.root.handlers) == 0:    
-    # This is not multiprocess safe, but it's not critical right now
-    logfile = os.getenv("PYROLAB_LOGFILE", PYROLAB_LOGFILE)
 
+if len(logging.root.handlers) == 0:    
+    logfile = PYROLAB_LOGDIR / f"pyrolab_{os.getpid()}.log"
     root = logging.getLogger()
     h = logging.handlers.RotatingFileHandler(logfile, 'a', 30000, 10)
-    f = logging.Formatter('%(asctime)s.%(msecs)03d %(process)-5s %(processName)-10s %(name)-12s %(levelname)-8s %(message)s', datefmt="%Y-%m-%d %H:%M:%S")
+    f = logging.Formatter('[%(asctime)s.%(msecs)03d] %(process)-5s %(processName)-10s %(name)-12s %(levelname)-8s %(message)s', datefmt="%Y-%m-%d %H:%M:%S")
     h.setFormatter(f)
     root.addHandler(h)
     root.setLevel(get_loglevel())
     root.debug("PyroLab logging configured")
 
 
 # Include remote traceback in local tracebacks
 import Pyro5.errors
 
 sys.excepthook = Pyro5.errors.excepthook
+
+
+# Check for updates to PyroLab
+try:
+    import json
+    import requests
+    from requests.adapters import HTTPAdapter
+    from packaging.version import parse
+
+    url = "https://pypi.org/pypi/pyrolab/json"
+    with requests.Session() as s:
+        s.mount('https://pypi.org', HTTPAdapter(max_retries=3))
+        resp = s.get(url).text
+
+    v = json.loads(resp)['info']['version']
+    curver = parse(__version__)
+    latest = parse(v)
+
+    log = logging.getLogger(__name__)
+
+    if curver < latest:
+        message = f"A new version of PyroLab is available (latest is {latest}, but {curver} is installed)."
+        warnings.warn(message, stacklevel=2)
+        log.info(message)
+except:
+    pass
```

### Comparing `PyroLab-0.2.1/pyrolab/api.py` & `PyroLab-0.3.0/src/pyrolab/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,31 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 API
 ===
 
 A single module that centralizes the most frequently used objects from PyroLab.
 """
 
 from Pyro5.client import Proxy
 from Pyro5.core import locate_ns
+from Pyro5.server import behavior, expose, oneway, serve
 from pyrolab import USER_CONFIG_FILE
-
 from pyrolab.configure import (
     PyroLabConfiguration, 
     NameServerConfiguration, 
     DaemonConfiguration, 
     ServiceConfiguration, 
     reset_config, 
     update_config,
 )
-from pyrolab.server import (
-    Daemon,
-    LockableDaemon,
-    behavior,
-    expose,
-    oneway,
-    serve,
-)
+from pyrolab.server import Daemon, LockableDaemon
 from pyrolab.nameserver import start_ns, start_ns_loop
 from pyrolab.service import Service
 
 
 __all__ = [
     "locate_ns",
     "Proxy",
```

### Comparing `PyroLab-0.2.1/pyrolab/cli.py` & `PyroLab-0.3.0/src/pyrolab/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 Command Line Interface
 ======================
 
 Usage: pyrolab [OPTIONS] COMMAND [ARGS]...
 
-Try 'pyrolab --help' for help.
+Try ``pyrolab --help`` for help.
 """
 import platform
 import shutil
 import subprocess
 import sys
 import textwrap
-import time
-from datetime import date
+import fileinput
+import re
 from pathlib import Path
-from typing import Optional
+from typing import Callable, Iterable, Optional
+from time import sleep, strptime
 
 import pkg_resources
 import typer
 
-from pyrolab import LOCKFILE, PYROLAB_LOGFILE, RUNTIME_CONFIG, USER_CONFIG_FILE
+from pyrolab import LOCKFILE, PYROLAB_LOGDIR, RUNTIME_CONFIG, USER_CONFIG_FILE
 from pyrolab.api import Proxy
 from pyrolab.configure import (
     PyroLabConfiguration,
     export_config,
     reset_config,
     update_config,
 )
@@ -62,21 +61,15 @@
 # pyrolab up
 # pyrolab down
 # pyrolab reload
 # pyrolab ps
 # pyrolab --version
 ###############################################################################
 
-app = typer.Typer()
-
-print(f"PyroLab  Copyright © 2020-{date.today().year}  BYU CamachoLab, PyroLab Project Contributors")
-print("This program comes with ABSOLUTELY NO WARRANTY.")
-print("This is free software, and you are welcome to redistribute it under certain conditions.")
-print("See the documentation for more information (https://pyrolab.readthedocs.io).")
-print()
+app = typer.Typer(no_args_is_help=True)
 
 
 def _version_callback(value: bool=True) -> None:
     if value:
         from pyrolab import __version__
         typer.echo(f"PyroLab {__version__}")
         raise typer.Exit()
@@ -136,15 +129,15 @@
 def down():
     """
     Stop the background PyroLab daemon.
     """
     daemon = get_daemon(suppress_reload_message=True)
     daemon.shutdown()
     while LOCKFILE.exists():
-        time.sleep(0.1)
+        sleep(0.1)
     typer.secho("PyroLab daemon shutdown.", fg=typer.colors.GREEN)
 
 @app.command()
 def reload():
     """
     Reload the PyroLab daemon using the latest configuration file.
 
@@ -324,26 +317,41 @@
 app.add_typer(logs_app, name="logs")
 
 @logs_app.command("clean")
 def logs_clean():
     """
     Deletes all log files.
     """
-    PYROLAB_LOGFILE.unlink(missing_ok=True)
+    [f.unlink() for f in PYROLAB_LOGDIR.glob("*.*")]
+
+def try_itr(func: Callable, itr: Iterable, *exceptions, **kwargs):
+    """
+    Tests a function on an iterable, yields iterable if no exception is raised.
+    """
+    for elem in itr:
+        try:
+            func(elem, **kwargs)
+            yield elem
+        except exceptions:
+            pass
 
 @logs_app.command("export")
 def logs_export(filename: str):
     """
     Exports the log file to a file.
     """
-    if PYROLAB_LOGFILE.exists():
-        shutil.copy(PYROLAB_LOGFILE, filename)
-    else:
-        typer.secho("No log file found.", fg=typer.colors.RED)
-        raise typer.Abort()
+    f_names = PYROLAB_LOGDIR.glob('*.*')
+    lines = list(fileinput.input(f_names))
+    t_fmt = "%Y-%m-%d %H:%M:%S.%f" # format of time stamps
+    t_pat = re.compile(r'\[(.+?)\]') # pattern to extract timestamp
+    lines = list(try_itr(lambda l: strptime(t_pat.search(l).group(1), t_fmt), lines, AttributeError))
+    with Path(filename).open(mode='w') as f:
+        for l in sorted(lines, key=lambda l: strptime(t_pat.search(l).group(1), t_fmt)):
+            f.write(l)
+    typer.secho(f"Exported logs to {filename}", fg=typer.colors.GREEN)
 
 ###############################################################################
 # pyrolab rename
 ###############################################################################
 
 rename_app = typer.Typer()
 app.add_typer(rename_app, name="rename", help="Rename a nameserver, daemon or service.")
```

### Comparing `PyroLab-0.2.1/pyrolab/configure.py` & `PyroLab-0.3.0/src/pyrolab/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 Configuration Settings
 ======================
@@ -30,39 +28,39 @@
    method call is running at a time, so if it takes a while to complete, all 
    other calls are waiting for their turn (even when they are from different 
    proxies).
 
 """
 
 from __future__ import annotations
-import importlib
 
+import uuid
+import importlib
 import logging
 from pathlib import Path
 from typing import IO, Any, Dict, List, Optional, Type, Union
-import uuid
+
 
 import Pyro5
 from pydantic import BaseModel, BaseSettings, validator
 from pydantic.fields import PrivateAttr
 from yaml import dump, load
 from yaml.constructor import ConstructorError
 from yaml.nodes import MappingNode
-
-from pyrolab.server import Daemon
-from pyrolab.service import Service
-
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
 
+from pyrolab.server import Daemon
+from pyrolab.service import Service
 from pyrolab import NAMESERVER_STORAGE, USER_CONFIG_FILE
 from pyrolab.utils import generate_random_name, get_ip
 
+
 log = logging.getLogger(__name__)
 
 
 def uniquify_class(cls: Type[Service]) -> Type[Service]:
     """
     Returns a new class with a unique name that inherits from the original.
 
@@ -307,21 +305,25 @@
           automatically).
 
     Examples
     --------
     The following are examples of valid YAML configurations for nameservers.
     Keys not defined assume the default values.
 
+    Example 1. Basic configuration.
+
     .. code-block:: yaml
 
         host: localhost
         ns_port: 9090
         ns_autoclean: 0.0
         storage: memory
     
+    Example 2. Nameserver publicly accessible.
+
     .. code-block:: yaml
 
         host: public
         ns_port: 9100
         broadcast: false
         ns_bchost: null
         ns_bcport: 9091
@@ -405,34 +407,45 @@
     Parameters
     ----------
     module : str, optional
         The module that contains the Daemon class (default "pyrolab.server").
     classname : str, optional
         The name of the Daemon class to use (default is basic "Daemon").
     host : str, optional
-        The hostname of the local server, or the string "public", which 
-        is converted to the host's public IP address (default "localhost").
-    ns_host : str, optional
-        The hostname of the nameserver (default "localhost").
-    ns_port : int, optional
-        The port of the nameserver (default 9090).
-    ns_bcport : int, optional
-        The port of the broadcast server (default 9091).
-    ns_bchost : bool, optional
-        Whether to broadcast the nameserver (default None).
+        The hostname of the local server, or the string "public", which is
+        converted to the host's public IP address (default "localhost").
+    port : int, optional
+        Port to bind the server on (default 0, which means to pick a random
+        port).
+    unixsocket : str, optional
+        The name of a Unix domain socket to use instead of a TCP/IP socket
+        (default None, which means don't use).
+    nathost : str, optional
+        Hostname to use in published addresses (useful when running behind a
+        NAT firewall/router). Default is None which means to just use the
+        normal host. For more details about NAT, see the Pyro5 docs about using
+        Pyro5 behind a NAT router/firewall.
+    natport : int, optional
+        Port to use in published addresses (useful when running behind a NAT
+        firewall/router). If you use 0 here (default), Pyro will replace the
+        NAT-port by the internal port number to facilitate one-to-one NAT port
+        mappings.
     servertype : str, optional
         Either ``thread`` or ``multiplex`` (default "thread").
     nameservers : List[str], optional
-        Whether to register the daemon itself with known nameservers. Useful
+        Whether to register the *daemon itself* with known nameservers. Useful
         if the daemon provides functions for managing local instruments that
-        would be useful to remote clients.
+        would be useful to remote clients. Services declare their own
+        nameserver registrations; belonging to a daemon that registers itself
+        with a specific nameserver does not mean that its services will also be
+        registered with that nameserver.
 
     Examples
     --------
-    The following is an example of a valid configuration file "daemons" 
+    The following is an example of a valid configuration file "daemons"
     section. Keys not defined assume the default values.
 
     .. code-block:: yaml
 
         daemons:
             lockable:
                 classname: LockableDaemon
@@ -482,18 +495,14 @@
     
     Includes connection parameters for ``autoconnect()``. Services defined in
     other modules or libaries can also be included here, so long as the module
     can be found by the Python environment.
 
     Parameters
     ----------
-    name : str
-        A unique human-readable name for identifying the instrument. If you're
-        not creative, you can use :py:func:`pyrolab.utils.generate_random_name`
-        to generate a random name.
     module : str
         The PyroLab module the class belongs to, as a string.
     classname : str
         The classname of the object to be registered, as a string.
     parameters : Dict[str, Any]
         A dictionary of parameters passed to the object's ``connect()`` 
         function when ``autoconnect()`` is invoked.        
@@ -834,15 +843,16 @@
 def reset_config() -> None:
     """
     Resets the configuration to the default.
 
     This function deletes the user configuration file, reverting to the default
     configuration each time PyroLab is started.
     """
-    USER_CONFIG_FILE.unlink(missing_ok=True)
+    if USER_CONFIG_FILE.exists():
+        USER_CONFIG_FILE.unlink()
 
 def export_config(config: PyroLabConfiguration, filename: Union[str, Path]) -> None:
     """
     Exports the current configuration to a file.
 
     Parameters
     ----------
```

### Comparing `PyroLab-0.2.1/pyrolab/drivers/cameras/uc480.py` & `PyroLab-0.3.0/src/pyrolab/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,417 +1,429 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
-Thorlabs UC480 Scientific Camera
-================================
+Daemon
+======
 
-Driver for a Thorlabs Microscope.
+Wrapped daemon functions that references PyroLab configuration settings.
+"""
 
-.. attention::
+from __future__ import annotations
 
-   Presently Windows only. 
-   
-   Requires ThorCam software. Download it at `thorlabs.com`_.
+import inspect
+import logging
+from typing import TYPE_CHECKING, Callable, Optional, Type
 
-   .. _thorlabs.com: https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=ThorCam
+import Pyro5
+from Pyro5.core import URI
+from Pyro5.server import expose
 
-   Potential future Linux support, since ThorLabs does provide a Windows and 
-   Linux SDK.
+if TYPE_CHECKING:
+    from Pyro5.socketutil import SocketConnection
 
-.. admonition:: Dependencies
-   :class: note
+    from pyrolab.drivers import Instrument
+    from pyrolab.service import Service
 
-   thorlabs_kinesis (:ref:`installation instructions <Thorlabs Kinesis Package>`)
-"""
 
-# TODO: Investigate Linux support 
-# (https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=ThorCam)
+log = logging.getLogger(__name__)
 
-import logging
-from ctypes import *
-from typing import Tuple
 
-import numpy as np
-try:
-    from thorlabs_kinesis import thor_camera as tc
-except:
-    pass
-
-from pyrolab.api import expose
-from pyrolab.drivers.cameras.thorcam import ThorCamBase, ThorCamClient
-from pyrolab.errors import PyroLabError
+def change_behavior(cls: Type[Instrument], instance_mode: str="session", instance_creator: Optional[Callable]=None):
+    """
+    Dynamically add a behavior to a class.
 
+    Equivalent to using the ``behavior`` decorator on the class, but can 
+    be used dynamically during runtime. Services that specify some default 
+    behavior in the source code can be overridden using this function.
 
-log = logging.getLogger(__name__)
+    .. warning::
+       This function modifies the behavior of the class in place! It does 
+       not returning a new class object.
+
+    Parameters
+    ----------
+    cls : class
+        The class to be change the behavior of.
+    instance_mode : str
+        One of "session", "single", or "percall" (see manual for differences).
+    instance_creator : callable
+        A callable that creates a new instance of the class (see manual for
+        more details).
+
+    Raises
+    ------
+    ValueError
+        If the ``instance_mode`` is not one of "session", "single", or "percall".
+    SyntaxError
+        If ``instance_mode`` is not a string, or is missing.
+    TypeError
+        If the first argument is not a class, or ``instance_creator`` is not a callable.
+    """
+    if not isinstance(instance_mode, str):
+        raise SyntaxError("behavior decorator is missing argument(s)")
+    if not inspect.isclass(cls):
+        raise TypeError("add_behavior can only be used on a class")
+    if instance_mode not in ("single", "session", "percall"):
+        raise ValueError("invalid instance mode: " + instance_mode)
+    if instance_creator and not callable(instance_creator):
+        raise TypeError("instance_creator must be a callable")
+    cls._pyroInstancing = (instance_mode, instance_creator)
 
 
 @expose
-class UC480(ThorCamBase):
+class Lockable:
     """
-    The Thorlabs UC480 camera driver.
+    The Lockable instrument mixin. Only works with LockableDaemon.
+    
+    Rejects new connections at the Daemon level when locked. Daemon stores the 
+    user who locked the device for reference.
 
-    Attributes
-    ----------
-    HEADERSIZE : int
-    brightness : int
-    color : bool
-    roi_shape : (int, int)
-    roi_pos : (int, int)
-    pixelclock : int
-    exposure : int
-    framerate : int
+    This mixin only makes sense in the context of a Daemon. It is not intended
+    for use with local instruments. Additionally, any service registered with
+    a :py:class:`LockableDaemon` will automatically have this mixin added to 
+    it.
+
+    Examples
+    --------
+    .. code-block:: python
+
+        class MyCustomService(Service, Lockable):
+            def __init__(self, *args, **kwargs):
+                pass
     """
+    def lock(self, user: str="") -> bool:
+        """
+        Locks access to the object's attributes.
 
-    @property
-    @expose
-    def pixelclock(self) -> int:
-        """Sets the clockspeed of the camera, usually in the range of 24."""
-        return self._pixelclock
+        Parameters
+        ----------
+        user : str, optional
+            The user who has locked the device. Useful when a device is locked
+            and another user wants to know who is using it.
+        """
+        # TODO: Consider making "user" a required parameter so we never have
+        # to wonder who acquired the lock.
+        daemon = getattr(self, "_pyroDaemon", None)
+        if daemon:
+            return daemon._lock(self._pyroId, daemon._last_requestor, user)
+        return True
 
-    @pixelclock.setter
-    @expose
-    def pixelclock(self, clockspeed: int) -> None:
-        self._pixelclock = clockspeed
-        pixelclock = c_uint(clockspeed)
-        if hasattr(self, "handle"):
-            tc.PixelClock(self.handle, 6, byref(pixelclock), sizeof(pixelclock))
-        else:
-            raise PyroLabError("Cannot set pixelclock before connecting to device.")
+    def unlock(self) -> bool:
+        """
+        Releases the lock on the object.
+        """
+        daemon = getattr(self, "_pyroDaemon", None)
+        if daemon:
+            return daemon._release(self._pyroId)
+        return True
 
-    @property
-    @expose
-    def exposure(self) -> int:
-        """Sets the exposure of the camera, the time the shutter is open in
-        milliseconds (90 ms is a good default)."""
-        return self._exposure
+    def islocked(self) -> bool:
+        """
+        Returns the status of the lock.
 
-    @exposure.setter
-    @expose
-    def exposure(self, exposure: int) -> None:
-        self._exposure = exposure
-        exposure_c = c_double(exposure)
-        if hasattr(self, "handle"):
-            tc.SetExposure(self.handle, 12 , exposure_c, sizeof(exposure_c))
-        else:
-            raise PyroLabError("Cannot set exposure before connecting to device.")
+        Returns
+        -------
+        bool
+            True if the lock is engaged, False otherwise.
+        """
+        daemon = getattr(self, "_pyroDaemon", None)
+        if daemon:
+            return daemon._islocked(self._pyroId)
+        return False
 
-    @property
-    @expose
-    def framerate(self) -> int:
-        """The framerate of the camera (fps). You must reset the exposure
-        after setting the framerate."""
-        return self._framerate
 
-    @framerate.setter
-    @expose
-    def framerate(self, framerate: int) -> None:
-        self._framerate = framerate
-        s_framerate = c_double(0)
-        if hasattr(self, "handle"):
-            tc.SetFrameRate(self.handle, c_double(framerate), byref(s_framerate))
-        else:
-            raise PyroLabError("Cannot set framerate before connecting to device.")
+class Daemon(Pyro5.server.Daemon):
+    """
+    The PyroLab server daemon. This class is based on the Pyro5.server.Daemon.
 
-    def connect(self, 
-                serialno: str, 
-                local: bool = False, 
-                bit_depth: int = 8,
-                pixelclock: int = 24, 
-                color: bool = True, 
-                colormode: int = 11, 
-                roi_shape: Tuple[int, int] = (1024, 1280), 
-                roi_pos: Tuple[int, int] = (0,0), 
-                framerate: int = 15, 
-                exposure: int = 90, 
-                pixelbytes: int = 8, 
-                brightness: int = 5
-    ):
-        """
-        Opens the serial communication with the Thorlabs camera and sets defaults.
-        
-        Default low-level values that are set include the bit depth and camera 
-        name.
+    Parameters
+    ----------
+    host : str or None 
+        The hostname or IP address to bind the server on. Default is None which 
+        means it uses the configured default (which is localhost). It is 
+        necessary to set this argument to a visible hostname or ip address, if 
+        you want to access the daemon from other machines.
+    port : int, optional
+        Port to bind the server on. Defaults to 0, which means to pick a random 
+        port.
+    unixsocket : str, optional
+        The name of a Unix domain socket to use instead of a TCP/IP socket. 
+        Default is None (don't use).
+    nathost : str, optional
+        hostname to use in published addresses (useful when running behind a 
+        NAT firewall/router). Default is None which means to just use the 
+        normal host. For more details about NAT, see Pyro behind a NAT 
+        router/firewall.
+    natport : int, optional
+        Port to use in published addresses (useful when running behind a NAT 
+        firewall/router). If you use 0 here, Pyro will replace the NAT-port by 
+        the internal port number to facilitate one-to-one NAT port mappings.
+    interface : DaemonObject, optional
+        Optional alternative daemon object implementation (that provides the 
+        Pyro API of the daemon itself).
+    connected_socket : SocketConnection, optional
+        Pptional existing socket connection to use instead of creating a new 
+        server socket.
+    """
+    # TODO: Implement methods that allow a client to view and forcibly close 
+    # connections to this Daemon.
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    @staticmethod
+    def prepare_class(cls) -> Type[Service]:
+        """
+        Performs any actions on the class required for the given Daemon.
+
+        Some classes require mixins to be added in order for certain 
+        functionality to work. When the ProcessManager prepares to run a Daemon,
+        the child process will call this method on the class before registering
+        the class.
 
         Parameters
         ----------
-        serialno : int
-            The serial number of the camera that should be connected.
-        local : bool, optional
-            Whether the camera is being used as a local device; if True, will 
-            not configure sockets for streaming when starting capature (default 
-            False).
-        bit_depth : int, optional
-            The number of bits used for each pixel (default 8).
-        pixelclock: int, optional
-            Clock speed of the camera (default 24).
-        color : bool, optional
-            Whether the camera is in color mode or not (default True).
-        colormode: int, optional
-            Mode of color that the camera returns data in. ``11`` (default) 
-            returns raw format, see :py:func:`set_color_mode` for more 
-            information.
-        roi_shape : tuple(int, int), optional
-            Dimensions of the image that is taken by the camera (default 
-            ``(1024, 1280)``).
-        roi_pos : tuple(int, int), optional
-            Position of the top left corner of the roi (region of interest) in
-            relation to the sensor array (default ``(0,0)``).
-        framerate : int, optional
-            The framerate of the camera in frames per second (default 15).
-        exposure: int, optional
-            In milliseconds, the time the shutter is open on the camera 
-            (default 90).
-        pixelbytes: int, optional
-            The amount of memory space allocated per pixel in bytes (default 8).
-        brightness : int
-            Integer (range 1-10) defining the brightness, where 5 leaves the 
-            brightness unchanged.
-        """
-        self.local = local
-        self.color = color
-
-        log.debug(f"Attempting to connect to camera with serialno '{serialno}'")
-        num = c_int(0)
-        tc.GetNumberOfCameras(byref(num))
-        log.debug(f"Found {num.value} cameras")
-
-        uci_format = tc.UC480_CAMERA_INFO * 2
-        uci = uci_format(tc.UC480_CAMERA_INFO(), tc.UC480_CAMERA_INFO())
-        dwCount = c_int(num.value)
-        cam_list = tc.UC480_CAMERA_LIST(dwCount=dwCount, uci=uci)
-        tc.GetCameraList(byref(cam_list))
-
-        # Find the camera with the given serial number. Each camera has to be
-        # connected to and asked its serial number. We then check that they
-        # match.
-        for i in range(num.value):
-            handle = c_int(cam_list.uci[i].dwCameraID)
-            error = tc.InitCamera(byref(handle))
-            
-            # 0 means no error
-            if(error != 0):
-                continue
-
-            info = tc.CAMINFO()
-            error = tc.GetCameraInfo(handle, byref(info))
-
-            if(int(info.SerNo) == serialno):
-                self.handle = handle
-                break
-            elif(i == num.value - 1):
-                raise PyroLabError("Camera not found")
-            else:
-                error = tc.ExitCamera(handle)
-                if error != 0:
-                    log.error(f"Closing ThorCam failed with error code {error}")
-
-        self.bit_depth = bit_depth
-   
-        tc.SetDisplayMode(self.handle, c_int(32768))
-
-        self.meminfo = None
-
-        self.pixelclock = pixelclock
-        self.framerate = framerate
-        self.exposure = exposure
-        self.brightness = brightness
-        self.set_color_mode(colormode)
-        self._set_hardware_roi_shape(roi_shape)
-        self.roi_shape = [int(roi_shape[1]/2),int(roi_shape[0]/2)]
-        self._set_hardware_roi_pos(roi_pos)
-        self.roi_pos = [int(roi_pos[1]/2),int(roi_pos[0]/2)]
-        self._initialize_memory(pixelbytes)
+        cls : class
+            The class to prepare.
+        
+        Returns
+        -------
+        class
+            The prepared class.
+        """
+        return cls
     
     @expose
-    def set_color_mode(self, mode: int = 11) -> None:
+    def ping(self) -> bool:
         """
-        Sets the color mode of the image.
-
-        This sets the mode of image that is taken. Almost always
-        use ``11`` which will give you the raw photosensor data in the format:
-
-        .. table::
-
-           +----+----+----+
-           | R  | G0 |... |
-           +----+----+----+
-           | G1 | B  |... |
-           +----+----+----+
-           |... |... |    |
-           +----+----+----+
-        
-        This data is interpreted in the _get_image() function.
+        Returns a bool (True) to indicate that the Daemon is alive and can be
+        communicated with.
 
-        Parameters
-        ----------
-        mode : int, optional
-            The color mode of the pixel data. ``11``, the default, means raw 
-            8-bit. ``6`` means gray 8-bit.
-        """        
-        tc.SetColorMode(self.handle, mode)
+        Returns
+        -------
+        result : bool
+            True, meaning communication was established.
+        """
+        return True
     
-    def get_frame(self) -> np.array:
+    @expose
+    def pyrolab_version(self) -> str:
         """
-        Retrieves the last frame from the camera's memory buffer.
+        Return the version of PyroLab running the device.
+        """
+        from pyrolab import __version__
+        return __version__
 
-        Retrieves the last frame from the camera memory buffer and processes it
-        into a computer-readable image format.
 
-        .. warning:: 
+class LockableDaemon(Daemon):
+    """
+    A LockableDaemon supports lockable resources.
 
-           Not a Pyro exposed function, cannot be called from a Proxy. We 
-           recommend using the :py:class:`ThorCamClient` for streaming 
-           video/getting remote images.
+    Lockable resources are objects that can be locked by a client. This is
+    useful for preventing multiple clients from accessing the same resource
+    simultaneously. The lock can be released manually, or is automatically
+    released when the client disconnects.
 
-        For remote connections, the image is serialized using the pickle module
-        for remote connections. The header is then added to inform the client
-        how long the message is. This should not be called from the client. It
-        will be called from the function _video_loop() which is on a parallel
-        thread with Pyro5.
+    Only objects with instance behavior "single" can be locked.
 
-        Can only be called after :py:func:`start_capture`.
+    Parameters
+    ----------
+    host : str or None 
+        The hostname or IP address to bind the server on. Default is None which 
+        means it uses the configured default (which is localhost). It is 
+        necessary to set this argument to a visible hostname or ip address, if 
+        you want to access the daemon from other machines.
+    port : int, optional
+        Port to bind the server on. Defaults to 0, which means to pick a random 
+        port.
+    unixsocket : str, optional
+        The name of a Unix domain socket to use instead of a TCP/IP socket. 
+        Default is None (don’t use).
+    nathost : str, optional
+        hostname to use in published addresses (useful when running behind a 
+        NAT firewall/router). Default is None which means to just use the 
+        normal host. For more details about NAT, see Pyro behind a NAT 
+        router/firewall.
+    natport : int, optional
+        Port to use in published addresses (useful when running behind a NAT 
+        firewall/router). If you use 0 here, Pyro will replace the NAT-port by 
+        the internal port number to facilitate one-to-one NAT port mappings.
+    interface : DaemonObject, optional
+        Optional alternative daemon object implementation (that provides the 
+        Pyro API of the daemon itself).
+    connected_socket : SocketConnection, optional
+        Pptional existing socket connection to use instead of creating a new 
+        server socket.
+    """
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.locked_instances = {}
 
+    @staticmethod
+    def prepare_class(cls) -> Type[Service]:
+        """
+        Dynamically create a new class that is also based on Lockable.
+
+        Parameters
+        ----------
+        cls : class
+            The class to be used as a template while dynamically creating a new
+            class.
+        
         Returns
         -------
-        img : np.array
-            The last frame from the camera's memory buffer.
+        class
+            A subclass that inherits from the original class and ``Lockable``.
         """
-        log.debug("Retreiving frame from memory")
-        raw = np.frombuffer(self.meminfo[0], c_ubyte).reshape(self.hardware_roi_shape[1], self.hardware_roi_shape[0])
-        log.debug(f"Retreived (size {raw.shape})")
+        DynamicLockable = type(
+            cls.__name__ + "Lockable",
+            (cls, Lockable, ),
+            {}
+        )
+        return DynamicLockable
 
-        bayer =  self._bayer_convert(raw)
-        return self._obtain_roi(bayer)
-    
-    @expose
-    def start_capture(self) -> Tuple[str, str]:
+    def _lock(self, pyroId: str, conn: SocketConnection, user: str="") -> bool:
         """
-        Starts capture from the camera.
+        Logs a "lock" action on a Pyro object.
+        
+        LockableDaemon tracks which connection owns the lock over a given Pyro
+        object.
 
-        This starts the capture from the camera to the allocated memory
-        location as well as starts a new thread for the socket server to stream
-        video from camera memory to the client.
+        Parameters
+        ----------
+        pyroId : str
+            The pyroId of the Pyro object.
+        conn : SocketConnection
+            The socket connection with the client that owns the lock.
+        user : str, optional
+            The user who has locked the device. Useful when a device is locked
+            by a user and another user wants to know who is using it.
 
         Returns
         -------
-        address, port : tuple(str, str) 
-            The IP address and port of the socket serving the video stream.
+        bool
+            A success status flag.
         """
-        log.debug("Sending signal to camera to start capture")
-        tc.StartCapture(self.handle, tc.IS_DONT_WAIT)
-        log.debug("Signal sent")
+        if pyroId not in self.locked_instances:
+            self.locked_instances[pyroId] = (conn, user)
+        return True
 
-        if not self.local:
-            return self.start_streaming_thread()
-    
-    @expose
-    def stop_capture(self) -> None:
+    def _release(self, pyroId: str) -> bool:
         """
-        Stops the capture from the camera.
+        Logs a "lock release" action on a Pyro object.
 
-        This frees the memory used for storing the frames, then (for remote
-        connections) sets the stop_video flag which will close the daemon
-        socket thread (not necessarily immediately).
-        """
-        tc.FreeMemory(self.handle, self.meminfo[0], self.meminfo[1])
-        tc.StopCapture(self.handle, 1)
-        if not self.local:
-            self.stop_streaming_thread()
-    
-    def _initialize_memory(self, pixelbytes: int = 8) -> None:
-        """
-        Initializes the memory for holding the most recent frame from the camera.
+        LockableDaemon tracks which connection owns the lock over a given Pyro
+        object. In the case of a release action, it does not matter which
+        connection makes the release; only lock owners can even access the 
+        release attribute.
 
         Parameters
         ----------
-        pixelbytes: int, optional
-            The amount of memory space allocated per pixel in bytes (default 8).
+        pyroId : str
+            The object to be released.
+
+        Returns
+        -------
+        bool
+            A success status flag. False if the instance wasn't locked to begin
+            with.
         """
-        if self.meminfo is not None:
-            tc.FreeMemory(self.handle, self.meminfo[0], self.meminfo[1])
-        
-        xdim, ydim = self.hardware_roi_shape
-        log.debug(f"got dimenstions: {self.hardware_roi_shape}")
-        # ydim = self.roi_shape[1]
-        imgsize = xdim * ydim
-        log.debug(f"image size is {imgsize}")
-            
-        memid = c_int(0)
-        c_buf = (c_ubyte * imgsize)(0)
-        log.debug("allocating memory...")
-        tc.AllocateMemory(self.handle, xdim, ydim, c_int(pixelbytes), c_buf, byref(memid))
-        log.debug("setting image memory...")
-        tc.SetImageMemory(self.handle, c_buf, memid)
-        log.debug("setting infor...")
-        self.meminfo = [c_buf, memid]
-        log.debug("meminfo set")
+        removed = self.locked_instances.pop(pyroId, None)
+        return True if removed else False
 
-    def _set_hardware_roi_shape(self, roi_shape: Tuple[int, int]) -> None:
+    def _islocked(self, pyroId: str) -> bool:
         """
-        Sets the dimensions of the region of interest (roi).
+        Checks if a Pyro object is locked.
 
         Parameters
         ----------
-        roi_shape : tuple(int, int)
-            Dimensions of the image that is taken by the camera 
-            (usually 1024 x 1280).
+        pyroId : str
+            The pyroId of the object to check.
+
+        Returns
+        -------
+        bool
+            A success status flag.
         """
-        # Width and height
-        AOI_size = tc.IS_2D(roi_shape[0], roi_shape[1])
-        
-        # 5 for setting size, 3 for setting position
-        tc.AOI(self.handle, 5, byref(AOI_size), 8)
-        
-        # 6 for getting sizse, 4 for getting position
-        tc.AOI(self.handle, 6, byref(AOI_size), 8)
-        
-        self.hardware_roi_shape = [AOI_size.s32X, AOI_size.s32Y]
+        return True if (pyroId in self.locked_instances) else False
 
-    def _set_hardware_roi_pos(self, roi_pos: Tuple[int, int]) -> None:
+    @expose
+    def release(self, uri: str) -> str:
         """
-        Sets the origin position of the region of interest.
+        Provides a way to force unlock a resource via the Daemon itself.
+
+        The Daemon must itself be registered to a Daemon and be assigned a URI.
+        That Daemon can very well be itself.
 
         Parameters
         ----------
-        roi_pos : tuple(int, int)
-            Position of the top left corner of the roi (region of interest) in
-            relation to the sensor array (usually ``(0,0)``).
-        """
-        # Width and height
-        AOI_pos = tc.IS_2D(roi_pos[0], roi_pos[1])
-        
-        # 5 for setting size, 3 for setting position
-        tc.AOI(self.handle, 3, byref(AOI_pos), 8 )
+        uri : str
+            The Pyro URI of the object to be unlocked.
 
-        # 6 for getting size, 4 for getting position
-        tc.AOI(self.handle, 4, byref(AOI_pos), 8 )
-
-        self.hardware_roi_pos = [AOI_pos.s32X, AOI_pos.s32Y]
+        Returns
+        -------
+        result : bool
+            True if the resource was successfully released, False otherwise.
 
-    @expose
-    def close(self):
-        """
-        Closes communication with the camera and frees memory.
+        Raises
+        ------
+        Pyro5.errors.PyroError
+            If the URI is invalid.
+        """
+        objId = URI(uri).object
+        obj = self.objectsById[objId]
+
+        # Only matters when instance mode is "single".
+        instance = self._pyroInstances.get(obj)
+        if instance:
+            return instance.unlock()
+        else:
+            return True
 
-        Calls :py:func:`stop_capture` to free memory and end the socket server
-        and then closes serial communication with the camera.
+    def _getInstance(self, clazz, conn):
         """
-        try:
-            self.handle
-        except AttributeError:
-            return
+        Find or create a new instance of the class.
         
-        self.stop_capture()
-
-        error = tc.ExitCamera(self.handle) 
-        if error != 0:
-            log.error(f"Closing ThorCam failed (code {error})")
-        del self.handle
-        self.meminfo = None
+        If an instance already exists, but is locked, an exception is raised.
+        
+        Parameters
+        ----------
+        clazz
+            The Pyro object being accessed.
+        conn
+            The connection object the request is being made from.
+        
+        Returns
+        -------
+        instance : clazz
+            The instance of the Pyro object being accessed.
+        
+        Raises
+        ------
+        ConnectionRefusedError
+            If an instance exists but is locked by a different connection.
+        """
+        self._last_requestor = conn
+        obj = super()._getInstance(clazz, conn)
+        if issubclass(obj.__class__, Lockable):
+            lock_owner, username = self.locked_instances.get(obj._pyroId, (None, ""))
+            if lock_owner is None or lock_owner == conn:
+                return obj
+            if lock_owner != conn:
+                raise ConnectionRefusedError(f"Pyro object is locked (by '{username or lock_owner}')")
 
+    def clientDisconnect(self, conn):
+        """
+        Automatically releases any locked resources in the event of a client 
+        disconnect.
 
-class UC480Client(ThorCamClient):
-    pass
+        Parameters
+        ----------
+        conn : SocketConnection
+            The SocketConnection object that was disconnected.
+        """
+        for pyroId in list(self.locked_instances.keys()):
+            owner, username = self.locked_instances[pyroId][0]
+            if conn == owner:
+                del self.locked_instances[pyroId]
+            log.info(f"Client connection closed, releasing lock owned by '{username}'.")
```

### Comparing `PyroLab-0.2.1/pyrolab/manager.py` & `PyroLab-0.3.0/src/pyrolab/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 Server Resources
 ----------------
@@ -22,23 +20,22 @@
 capabilities in cases where multiple instruments are hosted from the same
 computer, each instrument is created in its own Daemon using the 
 Python ``multiprocessing`` module.
 """
 
 from __future__ import annotations
 
-import importlib
 import logging
 import multiprocessing
 import threading
 import time
 from datetime import datetime
 from multiprocessing import current_process
 from multiprocessing.queues import Queue
-from typing import TYPE_CHECKING, Dict, List, Tuple, Type
+from typing import TYPE_CHECKING, Dict, Tuple
 
 from Pyro5.core import locate_ns
 
 from pyrolab import RUNTIME_CONFIG
 from pyrolab.configure import GlobalConfiguration, PyroLabConfiguration
 from pyrolab.nameserver import start_ns_loop
 
@@ -47,15 +44,14 @@
 
     from pyrolab.configure import (
         DaemonConfiguration,
         NameServerConfiguration,
         ServiceConfiguration,
     )
     from pyrolab.server import Daemon
-    from pyrolab.service import Service
 
 
 log = logging.getLogger(__name__)
 
 
 class NameServerRunner(multiprocessing.Process):
     """
@@ -272,22 +268,19 @@
     def run(self) -> None:
         """
         Creates and runs the child process.
 
         When the kill signal is received, gracefully shuts down and removes
         its registration from the nameserver.
         """
-        log.info(f"Starting")
+        log.info(f"Starting daemon {self.name}")
 
         # Set Pyro5 settings for daemon
-        log.info("got here")
         self.daemonconfig.update_pyro_config()
-        log.info("also got here")
         daemon, uris = self.setup_daemon()
-        log.info('are we out of the woods')
 
         GLOBAL_CONFIG = PyroLabConfiguration.from_file(RUNTIME_CONFIG)
 
         # Register all services with the nameserver
         log.debug("Registering services with nameserver")
         for sname, sinfo in self.serviceconfigs.items():
             for ns in sinfo.nameservers:
```

### Comparing `PyroLab-0.2.1/pyrolab/nameserver.py` & `PyroLab-0.3.0/src/pyrolab/nameserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 Nameserver
 ==========
@@ -14,23 +12,21 @@
 import logging
 import socket
 import sys
 from typing import Callable
 
 from Pyro5.nameserver import BroadcastServer, NameServerDaemon, start_ns
 
-from pyrolab import PYROLAB_DATA_DIR
+from pyrolab import NAMESERVER_STORAGE
 from pyrolab.configure import NameServerConfiguration
 
 log = logging.getLogger(__name__)
 
 
-NAMESERVER_DATA_DIR = PYROLAB_DATA_DIR / "nameserver" / "data"
-NAMESERVER_DATA_DIR.mkdir(parents=True, exist_ok=True)
-STORAGE_FILE = NAMESERVER_DATA_DIR / "storage"
+STORAGE_FILE = NAMESERVER_STORAGE / "storage"
 
 
 # # Inheriting from the Nameserver
 # class NameServer(Pyro5.nameserver.NameServer):
 #     """
 #     PyroLab specific NameServer with custom functionality including the ability
 #     to reject duplicate registration names.
```

### Comparing `PyroLab-0.2.1/pyrolab/pyrolabd.py` & `PyroLab-0.3.0/src/pyrolab/pyrolabd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 PyroLab Daemon
 ===============
@@ -256,8 +254,11 @@
             uri = daemon.register(pyrolabd, "pyrolabd")
             ii = InstanceInfo(pid=os.getpid(), uri=str(uri))
             with LOCKFILE.open("w") as f:
                 f.write(ii.json())
             daemon.requestLoop()
         finally:
             LOCKFILE.unlink()
-            RUNTIME_CONFIG.unlink()
+            try:
+                RUNTIME_CONFIG.unlink()
+            except FileNotFoundError:
+                print("Runtime configuration not found (and therefore not removed).")
```

### Comparing `PyroLab-0.2.1/pyrolab/service.py` & `PyroLab-0.3.0/src/pyrolab/service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 Service
 =======
@@ -12,14 +10,17 @@
 """
 
 from __future__ import annotations
 
 import logging
 from typing import Callable, Optional
 
+from pyrolab.server import expose
+
+
 log = logging.getLogger(__name__)
 
 
 class Service:
     """
     Abstract base class provides a common interface for services and instruments.
 
@@ -54,7 +55,28 @@
         if not isinstance(instance_mode, str):
             raise TypeError(f"instance_mode must be a string, but is {type(instance_mode)}")
         if instance_mode not in ("single", "session", "percall"):
             raise ValueError(f"invalid instance mode: {instance_mode}")
         if instance_creator and not callable(instance_creator):
             raise TypeError("instance_creator must be a callable")
         cls._pyroInstancing = (instance_mode, instance_creator)
+
+    @expose
+    def ping(self) -> bool:
+        """
+        Returns a bool (True) to indicate that the Daemon is alive and can be
+        communicated with.
+
+        Returns
+        -------
+        result : bool
+            True, meaning communication was established.
+        """
+        return True
+    
+    @expose
+    def pyrolab_version(self) -> str:
+        """
+        Return the version of PyroLab running the device.
+        """
+        from pyrolab import __version__
+        return __version__
```

### Comparing `PyroLab-0.2.1/pyrolab/utils.py` & `PyroLab-0.3.0/src/pyrolab/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright © PyroLab Project Contributors
 # Licensed under the terms of the GNU GPLv3+ License
 # (see pyrolab/__init__.py for details)
 
 """
 Utils
 =====
```


# Comparing `tmp/Pytrace_EyeOfThePython-0.0.2.tar.gz` & `tmp/Pytrace_EyeOfThePython-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\frand\Desktop\EyeOfThePython\dist\.tmp-qu0z33py\Pytrace_EyeOfThePython-0.0.2.tar", last modified: Sun Apr 23 16:56:22 2023, max compression
+gzip compressed data, was "C:\Users\frand\Desktop\EyeOfThePython\dist\.tmp-uzwqshq6\Pytrace_EyeOfThePython-0.0.3.tar", last modified: Sun Apr 23 17:03:16 2023, max compression
```

## Comparing `Pytrace_EyeOfThePython-0.0.2.tar` & `Pytrace_EyeOfThePython-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/
--rw-rw-rw-   0        0        0     1551 2022-04-11 12:34:27.000000 Pytrace_EyeOfThePython-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      462 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-23 13:08:24.000000 Pytrace_EyeOfThePython-0.0.2/README.md
--rw-rw-rw-   0        0        0      110 2023-04-23 15:10:18.000000 Pytrace_EyeOfThePython-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      561 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/src/EyeOfThePython/
--rw-rw-rw-   0        0        0    10504 2023-04-19 16:37:08.000000 Pytrace_EyeOfThePython-0.0.2/src/EyeOfThePython/Pytrace_EyeOfThePython.py
--rw-rw-rw-   0        0        0        0 2023-04-23 13:09:07.000000 Pytrace_EyeOfThePython-0.0.2/src/EyeOfThePython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/src/Pytrace_EyeOfThePython.egg-info/
--rw-rw-rw-   0        0        0      462 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/src/Pytrace_EyeOfThePython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/src/Pytrace_EyeOfThePython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/src/Pytrace_EyeOfThePython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-23 16:56:22.000000 Pytrace_EyeOfThePython-0.0.2/src/Pytrace_EyeOfThePython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/
+-rw-rw-rw-   0        0        0     1551 2022-04-11 12:34:27.000000 Pytrace_EyeOfThePython-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      462 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-23 13:08:24.000000 Pytrace_EyeOfThePython-0.0.3/README.md
+-rw-rw-rw-   0        0        0      110 2023-04-23 15:10:18.000000 Pytrace_EyeOfThePython-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      561 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/src/EyeOfThePython/
+-rw-rw-rw-   0        0        0    10504 2023-04-19 16:37:08.000000 Pytrace_EyeOfThePython-0.0.3/src/EyeOfThePython/Pytrace_EyeOfThePython.py
+-rw-rw-rw-   0        0        0        0 2023-04-23 13:09:07.000000 Pytrace_EyeOfThePython-0.0.3/src/EyeOfThePython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/src/Pytrace_EyeOfThePython.egg-info/
+-rw-rw-rw-   0        0        0      462 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/src/Pytrace_EyeOfThePython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/src/Pytrace_EyeOfThePython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/src/Pytrace_EyeOfThePython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-23 17:03:16.000000 Pytrace_EyeOfThePython-0.0.3/src/Pytrace_EyeOfThePython.egg-info/top_level.txt
```

### Comparing `Pytrace_EyeOfThePython-0.0.2/LICENSE` & `Pytrace_EyeOfThePython-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Pytrace_EyeOfThePython-0.0.2/setup.cfg` & `Pytrace_EyeOfThePython-0.0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7974 7261 6365 5f45 7965 4f66   = Pytrace_EyeOf
 00000020: 5468 6550 7974 686f 6e0d 0a76 6572 7369  ThePython..versi
-00000030: 6f6e 203d 2030 2e30 2e32 0d0a 6175 7468  on = 0.0.2..auth
+00000030: 6f6e 203d 2030 2e30 2e33 0d0a 6175 7468  on = 0.0.3..auth
 00000040: 6f72 203d 2045 7269 6b20 4672 616e 646f  or = Erik Frando
 00000050: 6665 720d 0a61 7574 686f 725f 656d 6169  fer..author_emai
 00000060: 6c20 3d20 6572 696b 2e66 7261 6e64 6f66  l = erik.frandof
 00000070: 6572 2e33 3635 4067 6d61 696c 2e63 6f6d  er.365@gmail.com
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5079 7468 6f6e 2074 7261 6369 6e67 2061  Python tracing a
 000000a0: 7070 6c69 6361 7469 6f6e 0d0a 6c6f 6e67  pplication..long
@@ -15,15 +15,15 @@
 000000e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 000000f0: 636f 6d2f 736e 6f77 6d61 6e69 7374 612f  com/snowmanista/
 00000100: 5079 5472 6163 650d 0a63 6c61 7373 6966  PyTrace..classif
 00000110: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
 00000120: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000130: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
 00000140: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000150: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000150: 7070 726f 7665 6420 3a3a 2042 5344 204c  pproved :: BSD L
 00000160: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
 00000170: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
 00000180: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
 00000190: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
 000001a0: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
 000001b0: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 000001c0: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
```

### Comparing `Pytrace_EyeOfThePython-0.0.2/src/EyeOfThePython/Pytrace_EyeOfThePython.py` & `Pytrace_EyeOfThePython-0.0.3/src/EyeOfThePython/Pytrace_EyeOfThePython.py`

 * *Files identical despite different names*


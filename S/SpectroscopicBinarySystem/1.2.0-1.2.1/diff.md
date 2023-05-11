# Comparing `tmp/SpectroscopicBinarySystem-1.2.0.tar.gz` & `tmp/SpectroscopicBinarySystem-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.2.0.tar", last modified: Thu May 11 11:33:03 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.2.1.tar", last modified: Thu May 11 11:45:38 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.2.0.tar` & `SpectroscopicBinarySystem-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:33:03.806035 SpectroscopicBinarySystem-1.2.0/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     4760 2023-05-11 11:33:03.806035 SpectroscopicBinarySystem-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4369 2023-05-11 11:30:08.000000 SpectroscopicBinarySystem-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 11:33:03.803369 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4760 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-11 11:33:03.000000 SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-05-11 11:33:03.815788 SpectroscopicBinarySystem-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 11:33:03.804376 SpectroscopicBinarySystem-1.2.0/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    31287 2023-05-11 11:02:14.000000 SpectroscopicBinarySystem-1.2.0/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:45:38.678811 SpectroscopicBinarySystem-1.2.1/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4759 2023-05-11 11:45:38.678811 SpectroscopicBinarySystem-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4368 2023-05-11 11:45:04.000000 SpectroscopicBinarySystem-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 11:45:38.665145 SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4759 2023-05-11 11:45:38.000000 SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-11 11:45:38.000000 SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:45:38.000000 SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-11 11:45:38.000000 SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-11 11:45:38.000000 SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-05-11 11:45:38.680388 SpectroscopicBinarySystem-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 11:45:38.676647 SpectroscopicBinarySystem-1.2.1/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    31282 2023-05-11 11:44:48.000000 SpectroscopicBinarySystem-1.2.1/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.2.0/LICENSE` & `SpectroscopicBinarySystem-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.2.0/PKG-INFO` & `SpectroscopicBinarySystem-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.44)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.2.1)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.2.0/README.md` & `SpectroscopicBinarySystem-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.44)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.2.1)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.44)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.2.1)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.2.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.2.1/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.2.0/setup.cfg` & `SpectroscopicBinarySystem-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
+00000030: 7273 696f 6e20 3d20 312e 322e 310d 0a61  rsion = 1.2.1..a
 00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
 00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
 00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
 00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
 00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
 00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
 000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.2.0/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.2.1/spectroscopicbinarysystem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,15 @@
             xindex = self.__findNearest(self._model_x, s.getPhase())
             delta = s.getRV() - self._model_y[xindex]
             self._residuals.append(delta)
             fmt = instruments[label] if group_by_instruments else 'o'
             axs[1].errorbar(s.getPhase(), delta,
                             yerr=0, fmt=fmt, ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
-        print(f'- Residuals mean STD : {np.std(self._residuals)} km/s')
+        print(f'- Residuals STD : {np.std(self._residuals)} km/s')
 
     def plotRadialVelocityCurve(self, title="", subtitle="", rv_y_multiple=10, residual_y_multiple=None, savefig=False, dpi=150, font_family='monospace', font_size=9, group_by_instruments=False):
         if not self._orbital_solution:
             self.__solveSystem()
 
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
```


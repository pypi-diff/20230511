# Comparing `tmp/scipion-em-aretomo-3.6.3.tar.gz` & `tmp/scipion-em-aretomo-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-aretomo-3.6.3.tar", last modified: Sat Apr  8 16:18:19 2023, max compression
+gzip compressed data, was "scipion-em-aretomo-3.6.5.tar", last modified: Thu May 11 11:19:38 2023, max compression
```

## Comparing `scipion-em-aretomo-3.6.3.tar` & `scipion-em-aretomo-3.6.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/aretomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/protocols/protocol_aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/aretomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/tests/test_protocols_aretomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.591440 scipion-em-aretomo-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-11 11:19:38.591440 scipion-em-aretomo-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/aretomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/protocols/protocol_aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/aretomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/aretomo/tests/test_protocols_aretomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:19:38.587440 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 11:19:38.000000 scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:19:38.591440 scipion-em-aretomo-3.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-11 11:17:36.000000 scipion-em-aretomo-3.6.5/setup.py
```

### Comparing `scipion-em-aretomo-3.6.3/CHANGES.txt` & `scipion-em-aretomo-3.6.5/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+3.6.5: allow unsorted tilt series
+3.6.4: adding type hints
 3.6.3: reduce number of Set[item] calls
 3.6.2:
  - fix applyTransform in the convert step
  - add interpolated flag
 3.6.1:
  - add aretomo 1.3.4, remove support for versions < 1.1.0
  - fix alignment matrix for excluded TS views
```

### Comparing `scipion-em-aretomo-3.6.3/LICENSE` & `scipion-em-aretomo-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/PKG-INFO` & `scipion-em-aretomo-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.6.3
+Version: 3.6.5
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.6.3/README.rst` & `scipion-em-aretomo-3.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/aretomo/__init__.py` & `scipion-em-aretomo-3.6.5/aretomo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.6.3'
+__version__ = '3.6.5'
 _logo = "aretomo_logo.png"
 _references = ['Zheng2022']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = ARETOMO_HOME
     _pathVars = [ARETOMO_HOME, ARETOMO_CUDA_LIB]
@@ -61,30 +61,30 @@
         # Get AreTomo CUDA library path if defined
         cudaLib = cls.getVar(ARETOMO_CUDA_LIB, pwem.Config.CUDA_LIB)
         environ.addLibrary(cudaLib)
 
         return environ
 
     @classmethod
-    def versionGE(cls, version):
+    def versionGE(cls, version: str) -> bool:
         """ Return True if current version of AreTomo is newer
          or equal than the input argument.
          Params:
             version: string version (semantic version, e.g 1.0.12)
         """
         v1 = cls.getActiveVersion()
         if v1 not in cls._supportedVersions:
             raise Exception("This version of AreTomo is not supported: ", v1)
 
         if cls._supportedVersions.index(v1) < cls._supportedVersions.index(version):
             return False
         return True
 
     @classmethod
-    def getProgram(cls):
+    def getProgram(cls) -> str:
         """ Return the program binary that will be used. """
         return cls.getHome('bin', cls.getVar(ARETOMO_BIN))
 
     @classmethod
     def defineBinaries(cls, env):
         for v in cls._supportedVersions:
             env.addPackage('aretomo', version=v,
```

### Comparing `scipion-em-aretomo-3.6.3/aretomo/bibtex.py` & `scipion-em-aretomo-3.6.5/aretomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/aretomo/constants.py` & `scipion-em-aretomo-3.6.5/aretomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/aretomo/convert.py` & `scipion-em-aretomo-3.6.5/aretomo/convert.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+import os
 import numpy as np
+from typing import Union, List, NamedTuple, Type
 
 
-def getTransformationMatrix(matrix):
+def getTransformationMatrix(matrix: np.ndarray) -> np.ndarray:
     """ This method takes an IMOD-based transformation matrix (*.xf) and
     returns a 3D matrix containing the transformation matrices for each
     tilt-image belonging to the tilt-series. """
 
     numberLines = matrix.shape[0]
     frameMatrix = np.empty([3, 3, numberLines])
 
@@ -45,37 +47,45 @@
         frameMatrix[2, 0, row] = 0.0
         frameMatrix[2, 1, row] = 0.0
         frameMatrix[2, 2, row] = 1.0
 
     return frameMatrix
 
 
-def readAlnFile(alignFn, newVersion=False):
+class AretomoAln(NamedTuple):
+    sections: List[int]
+    imod_matrix: np.ndarray
+    tilt_angles: List[float]
+    tilt_axes: List[float]
+
+
+def readAlnFile(alignFn: Union[str, os.PathLike],
+                newVersion: bool = False) -> Type[AretomoAln]:
     """ Read AreTomo output alignment file (.aln):
     aln2xf conversion taken from https://github.com/brisvag/stemia/blob/main/stemia/aretomo/aln2xf.py
     """
     # Read number of sections, as we need to ignore local alignments part of the file
     with open(alignFn) as f:
         f.readline()
         if newVersion:
             numSec = f.readline().strip("#").split()[-1]
         else:
             numSec = f.readline().strip("#").split()[0]
 
     data = np.loadtxt(alignFn, dtype=float, comments='#', max_rows=int(numSec))
-    sec_nums = list(data[:, 0].astype(int))  # SEC
-    tilt_angs = data[:, -1]  # TILT
-    tilt_axes = data[:, 1]  # ROT
+    AretomoAln.sections = list(data[:, 0].astype(int))  # SEC
+    AretomoAln.tilt_angles = data[:, -1]  # TILT
+    AretomoAln.tilt_axes = data[:, 1]  # ROT
     angles = -np.radians(data[:, 1])  # ROT
     shifts = data[:, [3, 4]]  # TX, TY
 
     c, s = np.cos(angles), np.sin(angles)
     rot = np.empty((len(angles), 2, 2))
     rot[:, 0, 0] = c
     rot[:, 0, 1] = -s
     rot[:, 1, 0] = s
     rot[:, 1, 1] = c
 
     shifts_rot = np.einsum('ijk,ik->ij', rot, shifts)
-    imod_matrix = np.concatenate([rot.reshape(-1, 4), -shifts_rot], axis=1)
+    AretomoAln.imod_matrix = np.concatenate([rot.reshape(-1, 4), -shifts_rot], axis=1)
 
-    return sec_nums, imod_matrix, tilt_angs, tilt_axes
+    return AretomoAln
```

### Comparing `scipion-em-aretomo-3.6.3/aretomo/protocols/__init__.py` & `scipion-em-aretomo-3.6.5/aretomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/aretomo/protocols/protocol_aretomo.py` & `scipion-em-aretomo-3.6.5/aretomo/protocols/protocol_aretomo.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 from glob import glob
 import numpy as np
+from typing import List, Literal, Tuple, Union, Optional
 
 import pyworkflow.protocol.params as params
 from pyworkflow.constants import BETA
 from pyworkflow.object import Set
 import pyworkflow.utils as pwutils
 from pwem.protocols import EMProtocol
 from pwem.objects import Transform
@@ -49,16 +50,15 @@
 
 OUT_TS = "outputSetOfTiltSeries"
 OUT_TS_ALN = "outputInterpolatedSetOfTiltSeries"
 OUT_TOMO = "outputSetOfTomograms"
 
 
 class ProtAreTomoAlignRecon(EMProtocol, ProtTomoBase):
-    """ Protocol for fiducial-free alignment and reconstruction for tomography.
-    """
+    """ Protocol for fiducial-free alignment and reconstruction for tomography. """
     _label = 'tilt-series align and reconstruct'
     _devStatus = BETA
     _possibleOutputs = {OUT_TS: SetOfTiltSeries,
                         OUT_TS_ALN: SetOfTiltSeries,
                         OUT_TOMO: SetOfTomograms}
 
     # --------------------------- DEFINE param functions ----------------------
@@ -247,25 +247,25 @@
 
         form.addHidden(params.GPU_LIST, params.StringParam,
                        default='0', label="Choose GPU IDs")
 
     # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
         for ts in self.inputSetOfTiltSeries.get():
-            tsObjId = ts.getObjId()
-            self._insertFunctionStep(self.convertInputStep, tsObjId)
-            self._insertFunctionStep(self.runAreTomoStep, tsObjId)
-            self._insertFunctionStep(self.createOutputStep, tsObjId)
+            args = (ts.getObjId(), ts.getTsId(),
+                    ts.getFirstItem().getFileName())
+            self._insertFunctionStep(self.convertInputStep, *args)
+            self._insertFunctionStep(self.runAreTomoStep, *args)
+            self._insertFunctionStep(self.createOutputStep, *args)
         self._insertFunctionStep(self.closeOutputSetsStep)
 
     # --------------------------- STEPS functions -----------------------------
-    def convertInputStep(self, tsObjId):
+    def convertInputStep(self, tsObjId: int, tsId: str, tsFn: str):
         ts = self._getSetOfTiltSeries()[tsObjId]
-        tsId = ts.getTsId()
-        tsFn = ts.getFirstItem().getFileName()
+
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
         pwutils.makePath(tmpPrefix)
         pwutils.makePath(extraPrefix)
 
         # Apply the transformation for the input tilt-series
         outputTsFileName = self.getFilePath(tsFn, tmpPrefix, ".mrc")
@@ -278,27 +278,25 @@
         self._generateTltFile(ts, angleFilePath)
 
         if self.useInputProt:
             # Find and copy aln file
             protExtra = self.inputProt.get()._getExtraPath(tsId)
             protAlnBase = self.getFilePath(tsFn, protExtra, ".aln").replace("_even", "*").replace("_odd", "*")
             protAln = glob(protAlnBase)
-            if len(protAln):
+            if protAln:
                 pwutils.copyFile(protAln[0],
                                  self.getFilePath(tsFn, extraPrefix, ".aln"))
                 self.info(f"Using input alignment: {protAln[0]}")
             else:
                 raise FileNotFoundError("Missing input aln file ", protAlnBase)
 
-    def runAreTomoStep(self, tsObjId):
+    def runAreTomoStep(self, tsObjId: int, tsId: str, tsFn: str):
         """ Call AreTomo with the appropriate parameters. """
         tsSet = self._getSetOfTiltSeries()
         ts = tsSet[tsObjId]
-        tsId = ts.getTsId()
-        tsFn = ts.getFirstItem().getFileName()
 
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
 
         args = {
             '-InMrc': self.getFilePath(tsFn, tmpPrefix, ".mrc"),
             '-OutMrc': self.getFilePath(tsFn, extraPrefix, ".mrc"),
@@ -347,25 +345,22 @@
 
         param = ' '.join([f'{k} {str(v)}' for k, v in args.items()])
         param += ' ' + self.extraParams.get()
         program = Plugin.getProgram()
 
         self.runJob(program, param, env=Plugin.getEnviron())
 
-    def createOutputStep(self, tsObjId):
+    def createOutputStep(self, tsObjId: int, tsId: str, tsFn: str):
         ts = self._getSetOfTiltSeries()[tsObjId]
-        tsId = ts.getTsId()
-        tsFn = ts.getFirstItem().getFileName()
         extraPrefix = self._getExtraPath(tsId)
 
         if not (self.makeTomo and self.skipAlign):
-            sec_nums, imod_matrix, tilt_angs, tilt_axes = readAlnFile(
-                self.getFilePath(tsFn, extraPrefix, ".aln"),
-                newVersion=Plugin.versionGE("1.3.0"))
-            alignmentMatrix = getTransformationMatrix(imod_matrix)
+            AretomoAln = readAlnFile(self.getFilePath(tsFn, extraPrefix, ".aln"),
+                                     newVersion=Plugin.versionGE("1.3.0"))
+            alignmentMatrix = getTransformationMatrix(AretomoAln.imod_matrix)
 
         if self.makeTomo:
             outputSetOfTomograms = self.getOutputSetOfTomograms()
             newTomogram = Tomogram()
             newTomogram.setLocation(self.getFilePath(tsFn, extraPrefix, ".mrc"))
 
             # Set tomogram origin
@@ -384,29 +379,30 @@
             self._store(outputSetOfTomograms)
         else:
             if self._saveInterpolated():
                 # Create new set of aligned TS with potentially fewer tilts included
                 outTsAligned = self.getOutputSetOfTiltSeries(OUT_TS_ALN)
                 newTs = TiltSeries(tsId=tsId)
                 newTs.copyInfo(ts)
-                outTsAligned.append(newTs)
                 newTs.setSamplingRate(self._getOutputSampling())
+                outTsAligned.append(newTs)
                 accumDose = 0.
 
-                for secNum, tiltImage in enumerate(ts.iterItems()):
-                    if secNum in sec_nums:
+                for secNum, tiltImage in enumerate(ts.iterItems(orderBy="_index")):
+                    if secNum in AretomoAln.sections:
                         newTi = TiltImage()
-                        newTi.copyInfo(tiltImage, copyTM=False)
+                        newTi.copyInfo(tiltImage, copyId=False, copyTM=False)
 
                         acq = tiltImage.getAcquisition()
                         acq.setTiltAxisAngle(0.)
                         newTi.setAcquisition(acq)
 
-                        newTi.setTiltAngle(tilt_angs[sec_nums.index(secNum)])
-                        newTi.setLocation(sec_nums.index(secNum) + 1,
+                        secIndex = AretomoAln.sections.index(secNum)
+                        newTi.setTiltAngle(AretomoAln.tilt_angles[secIndex])
+                        newTi.setLocation(secIndex + 1,
                                           (self.getFilePath(tsFn, extraPrefix, ".mrc")))
                         newTi.setSamplingRate(self._getOutputSampling())
                         newTs.append(newTi)
                         accumDose = acq.getAccumDose()
 
                 acq = newTs.getAcquisition()
                 acq.setAccumDose(accumDose)  # set accum dose from the last tilt-image
@@ -427,45 +423,46 @@
 
         # Save original TS stack with new alignment,
         # unless making a tomo from pre-aligned TS
         if not (self.makeTomo and self.skipAlign):
             outputSetOfTiltSeries = self.getOutputSetOfTiltSeries(OUT_TS)
             newTs = ts.clone()
             newTs.copyInfo(ts)
-            outputSetOfTiltSeries.append(newTs)
             newTs.setSamplingRate(self._getInputSampling())
+            outputSetOfTiltSeries.append(newTs)
 
-            for secNum, tiltImage in enumerate(ts.iterItems()):
+            for secNum, tiltImage in enumerate(ts.iterItems(orderBy="_index")):
                 newTi = tiltImage.clone()
                 newTi.copyInfo(tiltImage, copyId=True, copyTM=False)
                 transform = Transform()
 
-                if secNum not in sec_nums:
+                if secNum not in AretomoAln.sections:
                     newTi.setEnabled(False)
                     transform.setMatrix(np.identity(3))
                 else:
                     # set tilt angles
+                    secIndex = AretomoAln.sections.index(secNum)
                     acq = tiltImage.getAcquisition()
-                    acq.setTiltAxisAngle(tilt_axes[sec_nums.index(secNum)])
+                    acq.setTiltAxisAngle(AretomoAln.tilt_axes[secIndex])
                     newTi.setAcquisition(acq)
-                    newTi.setTiltAngle(tilt_angs[sec_nums.index(secNum)])
+                    newTi.setTiltAngle(AretomoAln.tilt_angles[secIndex])
 
                     # set Transform
-                    m = alignmentMatrix[:, :, sec_nums.index(secNum)]
-                    self.debug(f"Section {secNum}: {tilt_axes[sec_nums.index(secNum)]}, "
-                               f"{tilt_angs[sec_nums.index(secNum)]}")
+                    m = alignmentMatrix[:, :, secIndex]
+                    self.debug(f"Section {secNum}: {AretomoAln.tilt_axes[secIndex]}, "
+                               f"{AretomoAln.tilt_angles[secIndex]}")
                     transform.setMatrix(m)
 
                 newTi.setTransform(transform)
                 newTi.setSamplingRate(self._getInputSampling())
                 newTs.append(newTi)
 
             # update tilt axis angle for TS with the first value only
             acq = newTs.getAcquisition()
-            acq.setTiltAxisAngle(tilt_axes[0])
+            acq.setTiltAxisAngle(AretomoAln.tilt_axes[0])
             newTs.setAcquisition(acq)
 
             newTs.setDim(self._getSetOfTiltSeries().getDim())
             newTs.write(properties=False)
 
             outputSetOfTiltSeries.update(newTs)
             outputSetOfTiltSeries.write()
@@ -474,15 +471,15 @@
     def closeOutputSetsStep(self):
         for _, outputset in self.iterOutputAttributes():
             outputset.setStreamState(Set.STREAM_CLOSED)
 
         self._store()
 
     # --------------------------- INFO functions ------------------------------
-    def _summary(self):
+    def _summary(self) -> List[str]:
         summary = []
         if hasattr(self, OUT_TOMO):
             summary.append(f"Input tilt-series: "
                            f"{self._getSetOfTiltSeries().getSize()}.\n"
                            f"Tomograms reconstructed: "
                            f"{self.outputSetOfTomograms.getSize()}.\n")
         elif hasattr(self, OUT_TS):
@@ -495,20 +492,20 @@
 
         if self._saveInterpolated() and not self.makeTomo:
             summary.append("*Interpolated TS stack may have a few "
                            "dark tilt images removed.*")
 
         return summary
 
-    def _methods(self):
+    def _methods(self) -> List[str]:
         methods = []
 
         return methods
     
-    def _validate(self):
+    def _validate(self) -> List[str]:
         errors = []
 
         if self.useInputProt:
             if not self.inputProt.hasValue():
                 errors.append("Provide input AreTomo protocol for alignment.")
             if not Plugin.versionGE(V1_1_1):
                 errors.append("Input alignment can be used only with AreTomo v1.1.1+")
@@ -524,74 +521,85 @@
         if self._getSetOfTiltSeries().hasAlignment() and not self.skipAlign:
             errors.append("Input tilt-series already have alignment "
                           "information. You probably want to skip alignment step.")
 
         return errors
     
     # --------------------------- UTILS functions -----------------------------
-    def getFilePath(self, tsFn, prefix, ext=None):
+    def getFilePath(self,
+                    tsFn: Union[str, os.PathLike],
+                    prefix: str,
+                    ext: Optional[str] = None) -> Union[str, os.PathLike]:
         fileName, fileExtension = os.path.splitext(os.path.basename(tsFn))
-
         if ext is not None:
             fileExtension = ext
 
         return os.path.join(prefix, fileName + fileExtension)
 
-    def getOutputSetOfTomograms(self):
+    def getOutputSetOfTomograms(self) -> SetOfTomograms:
         if hasattr(self, OUT_TOMO):
             self.outputSetOfTomograms.enableAppend()
         else:
             outputSetOfTomograms = self._createSetOfTomograms()
             outputSetOfTomograms.copyInfo(self._getSetOfTiltSeries())
             outputSetOfTomograms.setSamplingRate(self._getOutputSampling())
             outputSetOfTomograms.setStreamState(Set.STREAM_OPEN)
             self._defineOutputs(**{OUT_TOMO: outputSetOfTomograms})
             self._defineSourceRelation(self.inputSetOfTiltSeries,
                                        outputSetOfTomograms)
         return self.outputSetOfTomograms
 
-    def getOutputSetOfTiltSeries(self, outputName=OUT_TS):
+    def getOutputSetOfTiltSeries(self,
+                                 outputName: Literal[OUT_TS, OUT_TS_ALN] = OUT_TS) -> SetOfTiltSeries:
         if hasattr(self, outputName):
             getattr(self, outputName).enableAppend()
         else:
-            suffix = "_interpolated" if outputName == OUT_TS_ALN else ""
+            if outputName == OUT_TS_ALN:
+                suffix = "_interpolated"
+                pixSize = self._getOutputSampling()
+            else:
+                suffix = ""
+                pixSize = self._getInputSampling()
+
             outputSetOfTiltSeries = self._createSetOfTiltSeries(suffix=suffix)
             outputSetOfTiltSeries.copyInfo(self._getSetOfTiltSeries())
             # Dimensions will be updated later
             outputSetOfTiltSeries.setDim(self._getSetOfTiltSeries().getDim())
-            if outputName == OUT_TS_ALN:
-                outputSetOfTiltSeries.setSamplingRate(self._getOutputSampling())
-            else:
-                outputSetOfTiltSeries.setSamplingRate(self._getInputSampling())
+            outputSetOfTiltSeries.setSamplingRate(pixSize)
             outputSetOfTiltSeries.setStreamState(Set.STREAM_OPEN)
             self._defineOutputs(**{outputName: outputSetOfTiltSeries})
             self._defineSourceRelation(self.inputSetOfTiltSeries,
                                        outputSetOfTiltSeries)
         return getattr(self, outputName)
 
-    def _getSetOfTiltSeries(self):
+    def _getSetOfTiltSeries(self) -> SetOfTiltSeries:
         return self.inputSetOfTiltSeries.get()
 
-    def _getOutputSampling(self):
+    def _getOutputSampling(self) -> float:
         return self._getInputSampling() * self.binFactor.get()
 
-    def _getInputSampling(self):
+    def _getInputSampling(self) -> float:
         return self._getSetOfTiltSeries().getSamplingRate()
 
-    def _getOutputDim(self, fn):
+    def _getOutputDim(self, fn: str) -> Tuple[int, int, int]:
         ih = ImageHandler()
         x, y, z, _ = ih.getDimensions(fn)
         return (x, y, z)
 
-    def _generateTltFile(self, ts, outputFn):
+    def _generateTltFile(self, ts: TiltSeries,
+                         outputFn: os.PathLike) -> None:
         """ Generate .tlt file with tilt angles and accumulated dose. """
-        tsParams = ts.aggregate(["COUNT"], "_tiltAngle",
-                                ["_tiltAngle", "_acquisition._accumDose"])
+        angleList = []
+
+        for ti in ts.iterItems(orderBy="_index"):
+            accDose = ti.getAcquisition().getAccumDose()
+            tAngle = ti.getTiltAngle()
+            angleList.append((tAngle, accDose))
 
         with open(outputFn, 'w') as f:
             if self.doDW:
-                f.writelines(f"{i['_tiltAngle']:0.3f} {i['_acquisition._accumDose']:0.3f}\n" for i in tsParams)
+                f.writelines(f"{i[0]:0.3f} {i[1]:0.3f}\n" for i in angleList)
             else:
-                f.writelines(f"{i['_tiltAngle']:0.3f}\n" for i in tsParams)
+                f.writelines(f"{i[0]:0.3f}\n" for i in angleList)
 
-    def _saveInterpolated(self):
+    def _saveInterpolated(self) -> bool:
         return self.saveStack
```

### Comparing `scipion-em-aretomo-3.6.3/aretomo/protocols.conf` & `scipion-em-aretomo-3.6.5/aretomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/aretomo/tests/__init__.py` & `scipion-em-aretomo-3.6.5/aretomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/aretomo/tests/test_protocols_aretomo.py` & `scipion-em-aretomo-3.6.5/aretomo/tests/test_protocols_aretomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/PKG-INFO` & `scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.6.3
+Version: 3.6.5
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/SOURCES.txt` & `scipion-em-aretomo-3.6.5/scipion_em_aretomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.3/setup.py` & `scipion-em-aretomo-3.6.5/setup.py`

 * *Files identical despite different names*


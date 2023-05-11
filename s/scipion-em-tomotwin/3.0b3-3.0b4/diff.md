# Comparing `tmp/scipion-em-tomotwin-3.0b3.tar.gz` & `tmp/scipion-em-tomotwin-3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomotwin-3.0b3.tar", last modified: Sat Oct  8 15:44:23 2022, max compression
+gzip compressed data, was "scipion-em-tomotwin-3.0b4.tar", last modified: Sun Nov 27 14:38:51 2022, max compression
```

## Comparing `scipion-em-tomotwin-3.0b3.tar` & `scipion-em-tomotwin-3.0b4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:44:23.773902 scipion-em-tomotwin-3.0b3/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4489 2022-10-08 15:44:23.773902 scipion-em-tomotwin-3.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:44:23.769902 scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4489 2022-10-08 15:44:23.000000 scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-10-08 15:44:23.000000 scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 15:44:23.000000 scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-08 15:44:23.000000 scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-08 15:44:23.000000 scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-08 15:44:23.000000 scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-08 15:44:23.773902 scipion-em-tomotwin-3.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8493 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:44:23.769902 scipion-em-tomotwin-3.0b3/tomotwin/
--rw-r--r--   0 runner    (1001) docker     (121)     6412 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:44:23.769902 scipion-em-tomotwin-3.0b3/tomotwin/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12296 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/protocols/protocol_picking_ref.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:44:23.773902 scipion-em-tomotwin-3.0b3/tomotwin/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/tests/test_protocols_tomotwin.py
--rw-r--r--   0 runner    (1001) docker     (121)   130513 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/tomotwin_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 15:44:23.773902 scipion-em-tomotwin-3.0b3/tomotwin/viewers/
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3953 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-10-08 15:42:19.000000 scipion-em-tomotwin-3.0b3/tomotwin/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 14:38:51.164096 scipion-em-tomotwin-3.0b4/
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2022-11-27 14:38:51.164096 scipion-em-tomotwin-3.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 14:38:51.160096 scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2022-11-27 14:38:51.000000 scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2022-11-27 14:38:51.000000 scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 14:38:51.000000 scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-27 14:38:51.000000 scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2022-11-27 14:38:51.000000 scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-27 14:38:51.000000 scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 14:38:51.164096 scipion-em-tomotwin-3.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     8493 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 14:38:51.160096 scipion-em-tomotwin-3.0b4/tomotwin/
+-rw-r--r--   0 runner    (1001) docker     (122)     6434 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1584 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 14:38:51.160096 scipion-em-tomotwin-3.0b4/tomotwin/protocols/
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12587 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/protocols/protocol_picking_ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 14:38:51.160096 scipion-em-tomotwin-3.0b4/tomotwin/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3336 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/tests/test_protocols_tomotwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)   130513 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/tomotwin_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 14:38:51.160096 scipion-em-tomotwin-3.0b4/tomotwin/viewers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4553 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2022-11-27 14:36:43.000000 scipion-em-tomotwin-3.0b4/tomotwin/wizards.py
```

### Comparing `scipion-em-tomotwin-3.0b3/LICENSE` & `scipion-em-tomotwin-3.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/PKG-INFO` & `scipion-em-tomotwin-3.0b4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-tomotwin
-Version: 3.0b3
+Version: 3.0b4
 Summary: Plugin to use TomoTwin within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomotwin
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomotwin/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomotwin/
@@ -67,30 +67,33 @@
         -----------------------
         *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
         PATH (not recommended), which can lead to execution problems mixing scipion
         python with conda ones. One example of this could can be seen below but
         depending on your conda version and shell you will need something different:
         CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
         
-        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.1.2):
+        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.2.1.6):
         Command to activate the TomoTwin environment.
         
+        *TOMOTWIN_MODEL* (default = software/em/tomotwin_model-052022/tomotwin_model_p120_052022_loss.pth):
+        Path to the pre-trained model.
+        
         *NAPARI_ENV_ACTIVATION* (default = conda activate napari):
         Command to activate the Napari viewer (boxmanager) environment.
         
         Verifying
         ---------
         To check the installation, simply run the following Scipion test:
         
         ``scipion test tomotwin.tests.test_protocols_tomotwin.TestTomoTwinRefPicking``
         
         Supported versions
         ------------------
         
-        0.1.2
+        0.1.2, 0.2.1.6
         
         Protocols
         ----------
         
         * reference-based picking
         
         References
```

### Comparing `scipion-em-tomotwin-3.0b3/README.rst` & `scipion-em-tomotwin-3.0b4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -57,30 +57,33 @@
 -----------------------
 *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
 PATH (not recommended), which can lead to execution problems mixing scipion
 python with conda ones. One example of this could can be seen below but
 depending on your conda version and shell you will need something different:
 CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
 
-*TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.1.2):
+*TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.2.1.6):
 Command to activate the TomoTwin environment.
 
+*TOMOTWIN_MODEL* (default = software/em/tomotwin_model-052022/tomotwin_model_p120_052022_loss.pth):
+Path to the pre-trained model.
+
 *NAPARI_ENV_ACTIVATION* (default = conda activate napari):
 Command to activate the Napari viewer (boxmanager) environment.
 
 Verifying
 ---------
 To check the installation, simply run the following Scipion test:
 
 ``scipion test tomotwin.tests.test_protocols_tomotwin.TestTomoTwinRefPicking``
 
 Supported versions
 ------------------
 
-0.1.2
+0.1.2, 0.2.1.6
 
 Protocols
 ----------
 
 * reference-based picking
 
 References
```

### Comparing `scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/PKG-INFO` & `scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-tomotwin
-Version: 3.0b3
+Version: 3.0b4
 Summary: Plugin to use TomoTwin within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomotwin
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomotwin/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomotwin/
@@ -67,30 +67,33 @@
         -----------------------
         *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
         PATH (not recommended), which can lead to execution problems mixing scipion
         python with conda ones. One example of this could can be seen below but
         depending on your conda version and shell you will need something different:
         CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
         
-        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.1.2):
+        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.2.1.6):
         Command to activate the TomoTwin environment.
         
+        *TOMOTWIN_MODEL* (default = software/em/tomotwin_model-052022/tomotwin_model_p120_052022_loss.pth):
+        Path to the pre-trained model.
+        
         *NAPARI_ENV_ACTIVATION* (default = conda activate napari):
         Command to activate the Napari viewer (boxmanager) environment.
         
         Verifying
         ---------
         To check the installation, simply run the following Scipion test:
         
         ``scipion test tomotwin.tests.test_protocols_tomotwin.TestTomoTwinRefPicking``
         
         Supported versions
         ------------------
         
-        0.1.2
+        0.1.2, 0.2.1.6
         
         Protocols
         ----------
         
         * reference-based picking
         
         References
```

### Comparing `scipion-em-tomotwin-3.0b3/scipion_em_tomotwin.egg-info/SOURCES.txt` & `scipion-em-tomotwin-3.0b4/scipion_em_tomotwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/setup.py` & `scipion-em-tomotwin-3.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/__init__.py` & `scipion-em-tomotwin-3.0b4/tomotwin/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import pwem
 import pyworkflow.utils as pwutils
 from pyworkflow import Config
 
 from .constants import *
 
 
-__version__ = '3.0b3'
+__version__ = '3.0b4'
 _references = ['Rice2022']
 _logo = "tomotwin_logo.png"
 
 
 class Plugin(pwem.Plugin):
     _pathVars = [TOMOTWIN_MODEL]
     _url = "https://tomotwin-cryoet.readthedocs.io/en/latest/index.html"
@@ -82,27 +82,27 @@
 
     @classmethod
     def defineBinaries(cls, env):
         for ver in VERSIONS:
             cls.addTomoTwinPackage(env, ver,
                                    default=ver == TOMOTWIN_DEFAULT_VER_NUM)
 
-        url = "https://owncloud.gwdg.de/index.php/s/PmothfUVKh4NSfD/download"
+        url = "https://ftp.gwdg.de/pub/misc/sphire/TomoTwin/models/tomotwin_model_p120_052022_loss.pth"
         env.addPackage("tomotwin_model", version="052022",
                        tar='void.tgz',
                        commands=[(f"wget -O {DEFAULT_MODEL} {url}",
                                   DEFAULT_MODEL)],
                        neededProgs=["wget"],
                        default=True)
 
         env.addPackage("napari", version="latest", tar="void.tgz",
                        commands=[(f"{cls.getCondaActivationCmd()} "
                                   "conda create -y -n napari -c conda-forge "
                                   "python=3.10 && conda activate napari && "
-                                  "pip install 'napari[all]>=0.4.16.rc8' "
+                                  "pip install 'napari[all]==0.4.17' "
                                   "napari-boxmanager && touch installed",
                                   "./installed")],
                        default=True)
 
     @classmethod
     def addTomoTwinPackage(cls, env, version, default=False):
         ENV_NAME = getTomoTwinEnvName(version)
```

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/bibtex.py` & `scipion-em-tomotwin-3.0b4/tomotwin/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/constants.py` & `scipion-em-tomotwin-3.0b4/tomotwin/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 # **************************************************************************
 
 
 def getTomoTwinEnvName(version):
     return "tomotwin-%s" % version
 
 
-VERSIONS = ['0.1.2']
+VERSIONS = ['0.1.2', '0.2.1.6']
 TOMOTWIN_DEFAULT_VER_NUM = VERSIONS[-1]
 
 DEFAULT_ENV_NAME = getTomoTwinEnvName(TOMOTWIN_DEFAULT_VER_NUM)
 DEFAULT_ACTIVATION_CMD = 'conda activate ' + DEFAULT_ENV_NAME
 TOMOTWIN_ENV_ACTIVATION = 'TOMOTWIN_ENV_ACTIVATION'
 NAPARI_ENV_ACTIVATION = 'NAPARI_ENV_ACTIVATION'
 
 TOMOTWIN_MODEL = 'TOMOTWIN_MODEL'
-DEFAULT_MODEL = 'tomotwin_model_p120_052022.pth'
+DEFAULT_MODEL = 'tomotwin_model_p120_052022_loss.pth'
```

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/convert.py` & `scipion-em-tomotwin-3.0b4/tomotwin/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/protocols/__init__.py` & `scipion-em-tomotwin-3.0b4/tomotwin/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/protocols/protocol_picking_ref.py` & `scipion-em-tomotwin-3.0b4/tomotwin/protocols/protocol_picking_ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,39 +72,39 @@
                            'Tomograms should be without denoising or '
                            'lowpass filtering.')
         form.addParam('inputRefs', params.PointerParam,
                       pointerClass="SetOfVolumes",
                       label='Reference volumes', important=True,
                       help='Specify a set of 3D volumes. They will be '
                            'rescaled to match the tomograms pixel size.')
-        form.addParam('boxSize', params.IntParam, default=37,
-                      label="Box size (px)",
-                      help="The box size only influences the non-maximum "
-                           "suppression. The ideal box size is a tight box "
-                           "size around the protein.")
         form.addParam('numCpus', params.IntParam, default=4,
                       label="Number of CPUs",
                       help="*Important!* This is different from number of threads "
                            "above as threads are used for GPU parallelization. "
                            "Provide here the number of *CPU cores* for tomotwin locate "
                            "process.")
 
         form.addSection(label="Advanced params")
         line = form.addLine("Batch size for embedding")
-        line.addParam('batchTomos', params.IntParam, default=64,
+        line.addParam('batchTomos', params.IntParam, default=256,
                       label="Tomograms")
-        line.addParam('batchRefs', params.IntParam, default=128,
+        line.addParam('batchRefs', params.IntParam, default=12,
                       label="References")
 
         line = form.addLine("Z-range for sliding (px)")
         line.addParam('zMin', params.IntParam, default=0,
                       label="Min")
         line.addParam('zMax', params.IntParam, default=0,
                       label="Max")
 
+        form.addParam('boxSize', params.IntParam, default=37,
+                      label="Box size (px)",
+                      help="The box size only influences the non-maximum "
+                           "suppression. The ideal box size is a tight box "
+                           "size around the protein.")
         form.addParam('tolerance', params.FloatParam,
                       default=0.2,
                       label="Tolerance value")
         form.addParam('globalMin', params.FloatParam,
                       default=0.5,
                       label="Global minimum",
                       help="Global minimum of the find max procedure. "
@@ -214,16 +214,26 @@
         for tomoObjId, coord3DSet in coord3DSetDict.items():
             self._updateOutputSet(name, coord3DSet,
                                   state=coord3DSet.STREAM_CLOSED)
 
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         errors = []
+
+        if self.inputTomos.get().getSamplingRate() - 10.0 > 0.1:
+            errors.append("Input tomograms must be at 10 A/px")
+
         return errors
 
+    def _warnings(self):
+        warnings = []
+
+        if self.boxSize != 37:
+            warnings.append("It's strongly recommended to use 37 px box!")
+
     def getSummary(self, coord3DSet):
         summary = list()
         summary.append("Number of particles picked: %s" % coord3DSet.getSize())
         summary.append("Particle size: %s" % coord3DSet.getBoxSize())
         return "\n".join(summary)
 
     def _methods(self):
@@ -236,15 +246,15 @@
 
     # --------------------------- UTILS functions ------------------------------
     def _getEmbedTomoArgs(self, tomoId):
         args = [
             f"tomogram -m {Plugin.getVar(TOMOTWIN_MODEL)}",
             f"-v {tomoId}.mrc",
             f"-b {self.batchTomos.get()}",
-            f"-o embed/tomos"
+            f"-s 2 -o embed/tomos"
         ]
 
         if self.zMin > 0 and self.zMax > 0:
             args.append(f"-z {self.zMin} {self.zMax}")
 
         return args
```

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/tests/__init__.py` & `scipion-em-tomotwin-3.0b4/tomotwin/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/tests/test_protocols_tomotwin.py` & `scipion-em-tomotwin-3.0b4/tomotwin/tests/test_protocols_tomotwin.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from pyworkflow.tests import BaseTest, setupTestProject
+from pyworkflow.utils import magentaStr
 from pwem.protocols import ProtImportVolumes
 
 from tomo.protocols import ProtImportTomograms
 from tomo.tests import DataSet
 
 from ..protocols.protocol_picking_ref import ProtTomoTwinRefPicking
 
@@ -38,32 +39,34 @@
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet("emd_10439")
         cls.tomo = cls.dataset.getFile('tomoEmd10439')
         cls.subtomos = cls.dataset.getFile('subtomograms/emd_10439-01*.mrc')
 
     def test_run(self):
+        print(magentaStr("\n==> Importing data - tomograms:"))
         protImportTomo = self.newProtocol(ProtImportTomograms,
                                           filesPath=self.tomo,
-                                          samplingRate=13.68)
+                                          samplingRate=10)
         self.launchProtocol(protImportTomo)
         self.assertIsNotNone(protImportTomo.outputTomograms,
                              msg="There was a problem with tomogram import")
 
+        print(magentaStr("\n==> Importing data - volumes:"))
         protImportVols = self.newProtocol(ProtImportVolumes,
-                                          filesPath=self.subtomos, samplingRate=13.68)
+                                          filesPath=self.subtomos, samplingRate=10)
         self.launchProtocol(protImportVols)
         self.assertIsNotNone(protImportVols.outputVolumes,
                              "There was a problem with volumes import")
 
+        print(magentaStr("\n==> Testing tomotwin - reference-based picking:"))
         protPicking = self.newProtocol(ProtTomoTwinRefPicking,
                                        inputTomos=protImportTomo.outputTomograms,
                                        inputRefs=protImportVols.outputVolumes,
-                                       boxSize=37,
                                        batchTomos=128,
                                        batchRefs=12,
                                        zMin=200, zMax=210)
         self.launchProtocol(protPicking)
         outputCoords = protPicking.output3DCoordinates
         self.assertIsNotNone(outputCoords, "Tomotwin reference-based picking has failed")
-        self.assertAlmostEqual(outputCoords.getSize(), 3192, delta=30)
+        self.assertAlmostEqual(outputCoords.getSize(), 3164, delta=100)
         self.assertEqual(outputCoords.getBoxSize(), 37)
```

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/tomotwin_logo.png` & `scipion-em-tomotwin-3.0b4/tomotwin/tomotwin_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/viewers/__init__.py` & `scipion-em-tomotwin-3.0b4/tomotwin/viewers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *
 # * Authors:     David Herreros Calero (dherreros@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
```

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/viewers/viewers_data.py` & `scipion-em-tomotwin-3.0b4/tomotwin/viewers/viewers_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # *              Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk) [2]
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC [1]
 # * MRC Laboratory of Molecular Biology (MRC-LMB) [2]
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
```

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/viewers/views_tkinter_tree.py` & `scipion-em-tomotwin-3.0b4/tomotwin/viewers/views_tkinter_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # *              Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk) [2]
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC [1]
 # * MRC Laboratory of Molecular Biology (MRC-LMB) [2]
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
```

### Comparing `scipion-em-tomotwin-3.0b3/tomotwin/wizards.py` & `scipion-em-tomotwin-3.0b4/tomotwin/wizards.py`

 * *Files identical despite different names*


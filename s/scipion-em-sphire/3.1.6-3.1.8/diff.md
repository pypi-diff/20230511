# Comparing `tmp/scipion-em-sphire-3.1.6.tar.gz` & `tmp/scipion-em-sphire-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-sphire-3.1.6.tar", last modified: Mon Mar 20 10:31:19 2023, max compression
+gzip compressed data, was "scipion-em-sphire-3.1.8.tar", last modified: Thu May 11 07:57:01 2023, max compression
```

## Comparing `scipion-em-sphire-3.1.6.tar` & `scipion-em-sphire-3.1.8.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:31:19.376918 scipion-em-sphire-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-20 10:31:19.376918 scipion-em-sphire-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:31:19.372918 scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-20 10:31:19.000000 scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-20 10:31:19.000000 scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:31:19.000000 scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-20 10:31:19.000000 scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-20 10:31:19.000000 scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 10:31:19.376918 scipion-em-sphire-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:31:19.372918 scipion-em-sphire-3.1.6/sphire/
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:31:19.372918 scipion-em-sphire-3.1.6/sphire/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols/protocol_cryolo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols/protocol_cryolo_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols/protocol_cryolo_tomo_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols/protocol_cryolo_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols/protocol_janni_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/sphire_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:31:19.376918 scipion-em-sphire-3.1.6/sphire/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/tests/test_protocol_cryolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-03-20 10:29:18.000000 scipion-em-sphire-3.1.6/sphire/tests/test_protocol_janni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.161172 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.161172 scipion-em-sphire-3.1.8/sphire/
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.161172 scipion-em-sphire-3.1.8/sphire/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_napari_tomo_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_tomo_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_tomo_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_janni_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/sphire_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/sphire/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/tests/test_protocol_cryolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/tests/test_protocol_janni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/sphire/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/viewers/viewer_napari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/viewers/views_tkinter_tree.py
```

### Comparing `scipion-em-sphire-3.1.6/CHANGES.txt` & `scipion-em-sphire-3.1.8/CHANGES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+3.1.8: Fix: coordinates 3d sent to napari are not flipped on Y axis.
+3.1.7:
+     - Creating a manual picking protocol using napari-boxmanager
+     - Creating a tomogram training protocol
+     - Adding the filaments options to cryolo tomogram picking protocol
 3.1.6: fix pretrained_weights param
 3.1.5: fix auto picking streaming
 3.1.4: add a check for empty cbox files
 3.1.3: add cryolo 1.9.3, fix actual cryolo version, fix setuptools dependency
 3.1.2:
     - Fix installation? Forcing python3.8?
     - Output creation ot tomo picking improved: Using pointer to tomos so streaming works
```

### Comparing `scipion-em-sphire-3.1.6/LICENSE` & `scipion-em-sphire-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/PKG-INFO` & `scipion-em-sphire-3.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: scipion-em-sphire
-Version: 3.1.6
+Version: 3.1.8
 Summary: Plugin to use Sphire programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-sphire
-Author: I2PC, Jose Miguel de La Rosa, Jorge Jiménez
+Author: I2PC, Jose Miguel de La Rosa Trevin, Jorge Jiménez
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-sphire/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-sphire/
 Description: =============
         Sphire plugin
         =============
```

### Comparing `scipion-em-sphire-3.1.6/README.rst` & `scipion-em-sphire-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/PKG-INFO` & `scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: scipion-em-sphire
-Version: 3.1.6
+Version: 3.1.8
 Summary: Plugin to use Sphire programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-sphire
-Author: I2PC, Jose Miguel de La Rosa, Jorge Jiménez
+Author: I2PC, Jose Miguel de La Rosa Trevin, Jorge Jiménez
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-sphire/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-sphire/
 Description: =============
         Sphire plugin
         =============
```

### Comparing `scipion-em-sphire-3.1.6/scipion_em_sphire.egg-info/SOURCES.txt` & `scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,31 @@
 README.rst
 requirements.txt
 setup.py
 scipion_em_sphire.egg-info/PKG-INFO
 scipion_em_sphire.egg-info/SOURCES.txt
 scipion_em_sphire.egg-info/dependency_links.txt
 scipion_em_sphire.egg-info/entry_points.txt
+scipion_em_sphire.egg-info/requires.txt
 scipion_em_sphire.egg-info/top_level.txt
 sphire/__init__.py
 sphire/bibtex.py
 sphire/constants.py
 sphire/convert.py
 sphire/objects.py
 sphire/protocols.conf
 sphire/sphire_logo.png
 sphire/protocols/__init__.py
 sphire/protocols/protocol_base.py
 sphire/protocols/protocol_cryolo_import.py
+sphire/protocols/protocol_cryolo_napari_tomo_picking.py
 sphire/protocols/protocol_cryolo_picking.py
 sphire/protocols/protocol_cryolo_tomo_picking.py
+sphire/protocols/protocol_cryolo_tomo_training.py
 sphire/protocols/protocol_cryolo_training.py
 sphire/protocols/protocol_janni_denoise.py
 sphire/tests/__init__.py
 sphire/tests/test_protocol_cryolo.py
-sphire/tests/test_protocol_janni.py
+sphire/tests/test_protocol_janni.py
+sphire/viewers/__init__.py
+sphire/viewers/viewer_napari.py
+sphire/viewers/views_tkinter_tree.py
```

### Comparing `scipion-em-sphire-3.1.6/setup.py` & `scipion-em-sphire-3.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -88,15 +91,15 @@
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
     url='https://github.com/scipion-em/scipion-em-sphire',  # Optional
 
     # This should be your name or the name of the organization which owns the
     # project.
-    author='I2PC, Jose Miguel de La Rosa, Jorge Jiménez',  # Optional
+    author='I2PC, Jose Miguel de La Rosa Trevin, Jorge Jiménez',  # Optional
 
     # This should be a valid email address corresponding to the author listed
     # above.
     author_email='scipion@cnb.csic.es',  # Optional
 
     # Classifiers help users find your project by categorizing it.
     #
@@ -139,15 +142,15 @@
     packages=find_packages(),
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    #install_requires=[],  # Optional
+    install_requires=[requirements],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

### Comparing `scipion-em-sphire-3.1.6/sphire/__init__.py` & `scipion-em-sphire-3.1.8/sphire/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pwem
 import pyworkflow.utils as pwutils
+from pyworkflow.utils import runJob, weakImport
 
 from .constants import *
 
 
-__version__ = '3.1.6'
+__version__ = '3.1.8'
 _logo = "sphire_logo.png"
 _references = ['Wagner2019']
 
 
 class Plugin(pwem.Plugin):
     _pathVars = [CRYOLO_CUDA_LIB]
     _url = 'https://github.com/scipion-em/scipion-em-sphire'
@@ -129,25 +130,56 @@
                        tar='void.tgz',
                        commands=cryolo_commands,
                        neededProgs=cls.getDependencies(),
                        default=default,
                        vars=installEnvVars)
 
     @classmethod
+    def addNapariPackage(cls, env, version, default=False):
+        ENV_NAME = getNaparyEnvName(version)
+        NAPARI_INSTALLED = f"napari_{version}_installed"
+        installCmd = [cls.getCondaActivationCmd(),
+                      f'conda create -y -n {ENV_NAME} -c conda-forge',
+                      'python=3.10 napari=0.4.17 pyqt pip &&',
+                      f'conda activate {ENV_NAME} &&',
+                      f'pip install napari_boxmanager=={version}']
+
+        # Flag installation finished
+        installCmd.append(f'&& touch {NAPARI_INSTALLED}')
+
+        napari_commands = [(" ".join(installCmd), NAPARI_INSTALLED)]
+
+        envPath = os.environ.get('PATH', "")
+        # keep path since conda likely in there
+        installEnvVars = {'PATH': envPath} if envPath else None
+        env.addPackage(f'napari', version=version,
+                       tar='void.tgz',
+                       commands=napari_commands,
+                       neededProgs=cls.getDependencies(),
+                       default=default,
+                       vars=installEnvVars)
+
+    @classmethod
     def defineBinaries(cls, env):
         def _add(version, **kwargs):
             cls.addCryoloPackage(env, version, **kwargs)
             kwargs['useCpu'] = True
             cls.addCryoloPackage(env, version, **kwargs)
 
+        def _addNapari(version,  **kwargs):
+            cls.addNapariPackage(env, version, default=False)
+
         _add(V1_8_2)
         _add(V1_8_4)
         _add(V1_8_5)
         _add(V1_9_3, default=True)
 
+        with weakImport('tomo'):
+            _addNapari(defaultVersion, default=True)
+
         def _addModel(model, version, link, filename, default=False):
             env.addPackage(model, version=version,
                            tar='void.tgz',
                            commands=[(f"wget {link}/{filename}", filename)],
                            neededProgs=["wget"],
                            default=default)
 
@@ -181,7 +213,19 @@
     @classmethod
     def runCryolo(cls, protocol, program, args, cwd=None, useCpu=False):
         """ Run crYOLO command from a given protocol. """
         fullProgram = '%s %s && %s' % (cls.getCondaActivationCmd(),
                                        cls.getCryoloEnvActivation(useCpu), program)
         protocol.runJob(fullProgram, args, env=cls.getEnviron(), cwd=cwd,
                         numberOfMpi=1)
+
+    @classmethod
+    def runNapariBoxManager(cls, protocol, program, args):
+        """ Run Napari boxmanager from a given protocol. """
+        launchPath = protocol._getExtraPath()
+        fullProgram = '%s %s && cd %s && %s' % (cls.getCondaActivationCmd(),
+                                                NAPARI_ACTIVATION_CMD,
+                                                launchPath,
+                                                program)
+        runJob(None, fullProgram, args, env=cls.getEnviron(), cwd=None,
+               numberOfMpi=1)
+
```

### Comparing `scipion-em-sphire-3.1.6/sphire/bibtex.py` & `scipion-em-sphire-3.1.8/sphire/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/sphire/constants.py` & `scipion-em-sphire-3.1.8/sphire/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 import os
 
 
 def getCryoloEnvName(version, useCpu=False):
     return f"cryolo{'CPU' if useCpu else ''}-{version}"
 
 
+def getNaparyEnvName(version):
+    return f"napari-{version}"
+
+
 V1_8_2 = "1.8.2"
 V1_8_4 = "1.8.4"
 V1_8_5 = "1.8.5"
 V1_9_3 = "1.9.3"
 
 VERSIONS = [V1_8_2, V1_8_4, V1_8_5, V1_9_3]
 CRYOLO_DEFAULT_VER_NUM = VERSIONS[-1]
@@ -94,7 +98,21 @@
 
 JANNI_GENMOD_VAR = 'JANNI_GENERIC_MODEL'
 JANNI_GENMOD = "janni_model"
 JANNI_GENMOD_20190703 = "20190703"
 JANNI_GENMOD_20190703_FN = f"gmodel_janni_{JANNI_GENMOD_20190703}.h5"
 JANNI_GENMOD_DEFAULT = os.path.join(f"{JANNI_GENMOD}-{JANNI_GENMOD_20190703}",
                                     JANNI_GENMOD_20190703_FN)
+
+# Napari variables
+V0_3_11 = '0.3.11'
+
+defaultVersion = V0_3_11
+
+NAPARI_ACTIVATION_CMD = 'conda activate %s' % getNaparyEnvName(defaultVersion)
+NAPARI_BOXMANAGER = 'napari_boxmanager'
+CBOX_FILAMENTS_FOLDER = 'CBOX_FILAMENTS_TRACED'
+NAPARI_VIEWER_CBOX_FILES = 'napariViewerCboxFiles'
+
+# Filament parameters
+STRAIGHTNESS_METHOD = ['NONE', 'LINE_STRAIGHTNESS', 'RMSD']
+DIRECTIONAL_METHOD = ['CONVOLUTION', 'PREDICTED']
```

### Comparing `scipion-em-sphire-3.1.6/sphire/convert.py` & `scipion-em-sphire-3.1.8/sphire/convert.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,22 +21,25 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+import logging
+logger = logging.getLogger(__name__)
 import os
 from emtable import Table
 
 import pyworkflow.utils as pwutils
 from pwem.emlib.image import ImageHandler
 from pwem.convert import Ccp4Header
 
 import sphire.constants as constants
+from tomo.constants import BOTTOM_LEFT_CORNER
 
 with pwutils.weakImport('tomo'):
     from tomo.objects import Coordinate3D
 
 
 class CoordBoxWriter:
     """ Helper class to write a .BOX file for cryolo. """
@@ -49,62 +52,113 @@
         self._boxSize = boxSize
         self._halfBox = int(boxSize / 2)
         self._yFlipHeight = yFlipHeight
 
     def open(self, filename):
         """ Open a new filename to write, close previous one if open. """
         self.close()
-        self._file = open(filename, 'w')
+        self._file = open(filename, 'a+')
 
     def writeCoord(self, coord):
         box = self._boxSize
         half = self._halfBox
         x = coord.getX() - half
         if self._yFlipHeight is None:
             y = coord.getY() - half
         else:
             y = self._yFlipHeight - coord.getY() - half
         score = getattr(coord, '_cryoloScore', 0.0)
         self._file.write("%s\t%s\t%s\t%s\t%s\n" % (x, y, box, box, score))
 
+    def writeCoordinate3DHeader(self):
+        HEADER = """
+data_cryolo
+
+loop_
+_CoordinateX #1
+_CoordinateY #2
+_CoordinateZ #3
+_Width #4
+_Height #5
+_Depth #6
+_filamentid #7
+_Confidence #8
+_EstWidth #9
+_EstHeight #10
+_NumBoxes #11
+"""
+        self._file.write(HEADER)
+
+    def writeCoord3D(self, coord3d):
+        box = self._boxSize
+        half = self._halfBox
+        x = coord3d.getX(BOTTOM_LEFT_CORNER) - half
+        if self._yFlipHeight is None:
+            y = coord3d.getY(BOTTOM_LEFT_CORNER) - half
+        else:
+            y = self._yFlipHeight - coord3d.getY(BOTTOM_LEFT_CORNER) - half
+        z = coord3d.getZ(BOTTOM_LEFT_CORNER)
+        groupId = coord3d.getGroupId()
+        self._file.write("%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s\n"
+                         % (x, y, z, box, box, box, groupId, box, box, box, 10))
+
+    def writeIncludeBlock(self, zCoordinates):
+        INCLUDE_BLOCK = """
+data_cryolo_include
+
+loop_
+_slice_index #1
+"""
+        self._file.write(INCLUDE_BLOCK)
+        for zCoordinate in zCoordinates:
+            self._file.write("%s\n" % zCoordinate)
+
     def close(self):
         if self._file:
             self._file.close()
 
 
 class CoordBoxReader:
     """ Helper class to read coordinates from .CBOX files. """
     def __init__(self, boxSize, yFlipHeight=None, boxSizeEstimated=False):
         """
         :param boxSize: The box size of the coordinates that will be read
         :param yFlipHeight: if not None, the y coordinates will be flipped
         """
-        self._halfBox = boxSize / 2.0
+        self._file = None
+        self._boxSize = boxSize
+        self._halfBox = boxSize / 2.0 if self._boxSize is not None else None
         self._yFlipHeight = yFlipHeight
         self._boxSizeEstimated = boxSizeEstimated
 
     def iterCoords(self, filename):
         for row in Table.iterRows(filename, tableName='cryolo'):
             x = row.CoordinateX
             y = row.CoordinateY
             z = row.get("CoordinateZ", 0.0)
             score = row.get("Confidence", 0.0)
+            groupId = int(row.get('filamentid', 0))
+            width = int(row.get('Width', 0))
+
+            if self._boxSize is None:
+                self._boxSize = width
+                self._halfBox = self._boxSize / 2.0
 
             if not self._boxSizeEstimated:
                 x += self._halfBox
                 y += self._halfBox
 
             sciX = round(x)
             sciY = round(y)
             sciZ = round(z) if not isinstance(z, str) else 0  # avoid <NA> values
 
             if self._yFlipHeight is not None:
                 sciY = self._yFlipHeight - sciY
 
-            yield sciX, sciY, sciZ, score
+            yield sciX, sciY, sciZ, score, groupId, width
 
 
 def writeSetOfCoordinates(boxDir, coordSet, micList=None):
     """ Convert a SetOfCoordinates to Cryolo box files.
     Params:
         boxDir: the output directory where to generate the files.
         coordSet: the input SetOfCoordinates that will be converted.
@@ -144,36 +198,85 @@
 def readSetOfCoordinates3D(tomogram, coord3DSet, coordsFile, boxSize,
                            origin=None):
     reader = CoordBoxReader(boxSize)
     coord3DSet.enableAppend()
 
     coord = Coordinate3D()
 
-    for x, y, z, _ in reader.iterCoords(coordsFile):
+    for x, y, z, score, groupId, width in reader.iterCoords(coordsFile):
         # Clean up objId to add as a new coordinate
         coord.setObjId(None)
         coord.setVolume(tomogram)
         coord.setPosition(x, y, z, origin)
+        coord.setGroupId(groupId)
         coord3DSet.append(coord)
 
+    coord3DSet.setBoxSize(boxSize if boxSize is not None else width)
+
+
+def writeSetOfCoordinates3D(boxDir, coord3DSet, tomoList=None):
+    """ Convert a SetOfCoordinates to Cryolo cbox files.
+    Params:
+        boxDir: the output directory where to generate the files.
+        coordSet: the input SetOfCoordinates that will be converted.
+        tomoList: if not None, only coordinates from this micrographs
+            will be written.
+    """
+    tomoSet = coord3DSet.getPrecedents()
+    tomoIdSet = tomoSet.getIdSet() if tomoList is None else set(m.getObjId()
+                                                                for m in tomoList)
+
+    # Get first tomo from to
+    tomo = tomoSet.getFirstItem()
+
+    writer = CoordBoxWriter(coord3DSet.getBoxSize())
+    lastTomoId = None
+    doWrite = True
+    zCoorList = []
+    for coord in coord3DSet.iterCoordinates():
+        tomoId = coord.getVolume().getObjId()
+        tomo = tomoSet[tomoId]
+
+        if tomoId != lastTomoId:
+            if lastTomoId is not None:
+                writer.writeIncludeBlock(zCoorList)
+            doWrite = tomoId in tomoIdSet
+            if doWrite:
+                zCoorList = []
+                writer.open(os.path.join(boxDir, getMicFn(tomo, "cbox")))
+                writer.writeCoordinate3DHeader()
+            lastTomoId = tomoId
+
+        if doWrite:
+            writer.writeCoord3D(coord)
+            zValue = coord.getZ(BOTTOM_LEFT_CORNER)
+            if zValue not in zCoorList:
+                zCoorList.append(zValue)
+
+    writer.writeIncludeBlock(zCoorList)
+
+    writer.close()
+
 
 def needToFlipOnY(filename):
     """ Returns true if we need to flip coordinates on Y"""
     ext = pwutils.getExt(filename)
 
     if ext in ".mrc":
         header = Ccp4Header(filename, readHeader=True)
-        return header.getISPG() != 0  # ISPG 1, cryolo will not flip the image
-
+        flip = header.getISPG() != 0  # ISPG 1, cryolo will not flip the image
+        logger.info("File %s DOES%s need flipping the coordinates on Y based on its headers." % (filename,"" if flip else "N'T"))
+        return flip
     return ext in constants.CRYOLO_SUPPORTED_FORMATS
 
 
 def getFlipYHeight(filename):
     """ Return y-Height if flipping is needed, None otherwise """
     x, y, z, n = ImageHandler().getDimensions(filename)
+    logger.info("Calculating if %s need flipping on Y." % filename)
     return y if needToFlipOnY(filename) else None
 
 
 def convertMicrographs(micList, micDir):
     """ Convert (or simply link) input micrographs into the given directory
     in a format that is compatible with crYOLO.
     """
@@ -193,20 +296,23 @@
         func = _convert
         ext = '.mrc'
 
     for mic in micList:
         func(mic, getMicFn(mic, ext.lstrip(".")))
 
 
+convertTomograms = convertMicrographs
+
+
 def getMicFn(mic, ext='mrc'):
     """ Return a name for the micrograph based on its filename. """
     return pwutils.replaceBaseExt(mic.getFileName(), ext)
 
 
 def roundInputSize(inputSize):
-    """ Returns the closest value to inputSize th is multiple of 32"""
+    """ Returns the closest value to inputSize that is multiple of 32"""
     rounded = int(32 * round(float(inputSize) / 32))
 
     if rounded != inputSize:
         print("Input size (%s) will be rounded to %s, the closest "
               "multiple of 32." % (inputSize, rounded))
     return rounded
```

### Comparing `scipion-em-sphire-3.1.6/sphire/objects.py` & `scipion-em-sphire-3.1.8/sphire/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/sphire/protocols/__init__.py` & `scipion-em-sphire-3.1.8/sphire/protocols/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,7 +28,10 @@
 
 from .protocol_cryolo_training import SphireProtCRYOLOTraining
 from .protocol_cryolo_picking import SphireProtCRYOLOPicking
 from .protocol_cryolo_import import SphireProtCryoloImport
 from .protocol_janni_denoise import SphireProtJanniDenoising
 with weakImport('tomo'):
     from .protocol_cryolo_tomo_picking import SphireProtCRYOLOTomoPicking
+    from .protocol_cryolo_napari_tomo_picking import SphireProtCRYOLONapariTomoPicker
+    from .protocol_cryolo_tomo_training import SphireProtCRYOLOTomoTraining
+
```

### Comparing `scipion-em-sphire-3.1.6/sphire/protocols/protocol_base.py` & `scipion-em-sphire-3.1.8/sphire/protocols/protocol_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,23 +283,28 @@
     def usingCpu(self):
         if self._IS_TRAIN:
             return False
         else:
             return not self.useGpu.get()
 
     def getInputModel(self):
-        if self.inputModelFrom == INPUT_MODEL_GENERAL:
-            m = Plugin.getModelFn(CRYOLO_GENMOD_VAR)
-        elif self.inputModelFrom == INPUT_MODEL_GENERAL_DENOISED:
-            m = Plugin.getModelFn(CRYOLO_GENMOD_NN_VAR)
-        elif self.inputModelFrom == INPUT_MODEL_GENERAL_NS:
-            m = Plugin.getModelFn(CRYOLO_NS_GENMOD_VAR)
+        if self._IS_TRAIN:
+            if self.inputModelFrom == INPUT_MODEL_GENERAL:
+                m = Plugin.getModelFn(CRYOLO_GENMOD_VAR)
+            else:
+                m = os.path.abspath(self.inputModel.get().getPath())
         else:
-            m = os.path.abspath(self.inputModel.get().getPath())
-
+            if self.inputModelFrom == INPUT_MODEL_GENERAL:
+                m = Plugin.getModelFn(CRYOLO_GENMOD_VAR)
+            elif self.inputModelFrom == INPUT_MODEL_GENERAL_DENOISED:
+                m = Plugin.getModelFn(CRYOLO_GENMOD_NN_VAR)
+            elif self.inputModelFrom == INPUT_MODEL_GENERAL_NS:
+                m = Plugin.getModelFn(CRYOLO_NS_GENMOD_VAR)
+            else:
+                m = os.path.abspath(self.inputModel.get().getPath())
         return m
 
     def getEstimatedBoxSize(self, path):
         sizeSummaryFilePattern = os.path.join(path,
                                               'size_distribution_summary*.txt')
         boxSize = None
         try:
```

### Comparing `scipion-em-sphire-3.1.6/sphire/protocols/protocol_cryolo_import.py` & `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/sphire/protocols/protocol_cryolo_picking.py` & `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_picking.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
-from glob import glob
 
 import pyworkflow.utils as pwutils
 from pyworkflow.object import Integer
 import pyworkflow.protocol.params as params
 import pyworkflow.protocol.constants as cons
 from pwem.protocols import ProtParticlePickingAuto
 import pwem.objects as emobj
@@ -138,15 +137,15 @@
         coord = emobj.Coordinate()
         coord._cryoloScore = emobj.Float()
 
         for mic in micDoneList:
             cboxFile = convert.getMicFn(mic, "cbox")
             coordsFile = self._getExtraPath(cboxFile)
             if os.path.exists(coordsFile) and os.path.getsize(coordsFile):
-                for x, y, z, score in reader.iterCoords(coordsFile):
+                for x, y, z, score, _, _ in reader.iterCoords(coordsFile):
                     # Clean up objId to add as a new coordinate
                     coord.setObjId(None)
                     coord.setPosition(x, y)
                     coord.setMicrograph(mic)
                     coord._cryoloScore.set(score)
                     # Add it to the set
                     outputCoords.append(coord)
```

### Comparing `scipion-em-sphire-3.1.6/sphire/protocols/protocol_cryolo_tomo_picking.py` & `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_training.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # **************************************************************************
 # *
-# * Authors: Yunior C. Fonseca Reyna    (cfonseca@cnb.csic.es)
+# * Authors:     David Maluenda (dmaluenda@cnb.csic.es)
+# *              Peter Horvath (phorvath@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -20,130 +21,134 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-import os
-
-import pyworkflow.utils as pwutils
-from pyworkflow import BETA
-from pyworkflow.object import Integer, Float
+from pwem.protocols import ProtParticlePicking
 import pyworkflow.protocol.params as params
-
-from tomo.objects import SetOfCoordinates3D
-from tomo.protocols import ProtTomoPicking
-import tomo.constants as tomoConst
+import pyworkflow.utils as pwutils
+from pyworkflow.object import Integer
 
 from .. import Plugin
-from ..constants import INPUT_MODEL_GENERAL_DENOISED
+from ..objects import CryoloModel
 from .protocol_base import ProtCryoloBase
 import sphire.convert as convert
 
 
-class SphireProtCRYOLOTomoPicking(ProtCryoloBase, ProtTomoPicking):
-    """ Picks particles in a set of tomograms.
-    """
-    _label = 'cryolo tomo picking'
-    _devStatus = BETA
-    _possibleOutputs = {'output3DCoordinates': SetOfCoordinates3D}
+class SphireProtCRYOLOTraining(ProtCryoloBase, ProtParticlePicking):
+    """ Train crYOLO picker using a set of coordinates. """
+    _label = 'cryolo training'
+    MODEL = 'model.h5'
+    TRAIN = ['train_annotations', 'train_images']
+    _IS_TRAIN = True
 
-    def __init__(self, **kwargs):
-        ProtTomoPicking.__init__(self, **kwargs)
-
-    # --------------------------- DEFINE param functions ----------------------
-    def _defineParams(self, form):
-        ProtTomoPicking._defineParams(self, form)
+    # -------------------------- DEFINE param functions -----------------------
+    def _defineTrainParams(self, form):
         ProtCryoloBase._defineParams(self, form)
 
-        form.addSection(label="Tracing")
-        form.addParam('searchRange', params.IntParam, default=-1,
-                      label="Search range (px)",
-                      help="Search range in pixel. On default it will "
-                           "choose 25 percent of the box size (default: -1).")
-        form.addParam('minLength', params.IntParam, default=5,
-                      label="Minimum length",
-                      help="The minimum number of boxes in one trace to be "
-                           "considered as valid particle (default: 5).")
-        form.addParam('memory', params.IntParam, default=0,
-                      label="Tracing memory",
-                      help="The maximum number of frames during which a "
-                           "particle can vanish, then reappear nearby, "
-                           "and be considered the same particle (default: 0).")
-
-        form.addParallelSection(threads=1, mpi=1)
-
-        # Default box size --> 50
-        form.getParam('boxSize').default = Integer(50)
-        # Default lowpass --> 0.3
-        form.getParam('absCutOffFreq').default = Float(0.3)
+        form.addSection(label="Training")
+        form.addParam('eFlagParam', params.IntParam, default=10,
+                      label="Early stop patience",
+                      help="The training stops when the 'loss' metric on the "
+                           "validation data does not improve 10 times in a row. "
+                           "This is typically enough. In case want to give the "
+                           "training more time to find the best model you might "
+                           "increase this parameters to a higher value (e.g 15).")
+        form.addParam('nb_epochVal', params.IntParam, default=200,
+                      label="Maximum number of iterations",
+                      help="Maximum number of epochs the network will train. "
+                           "Basically never reach this number, as crYOLO "
+                           "stops training if it recognize that the validation "
+                           "loss is not improving anymore.")
+        form.addParam('learning_rates', params.FloatParam, default=1e-4,
+                      label="Learning rates",
+                      help="If the number is too small convergence can be slow.")
+        form.addParam('batchSize', params.IntParam, default=4,
+                      label="Batch size",
+                      help="The number of images crYOLO process in parallel "
+                           "during training.")
+
+        form.addParallelSection(threads=1, mpi=0)
 
+        # Default box size --> 100
+        form.getParam('boxSize').default = Integer(100)
+
+    def _defineParams(self, form):
+        ProtParticlePicking._defineParams(self, form)
+        form.addParam('inputCoordinates', params.PointerParam,
+                      pointerClass='SetOfCoordinates',
+                      label='Input coordinates', important=True,
+                      help="Please select a set of coordinates, obtained "
+                           "from a previous picking run. Typically the "
+                           "coordinates from ~ 10 micrographs is "
+                           "a good start.")
+        self._defineTrainParams(form)
+
+    # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
+        self._insertFunctionStep(self.convertInputStep)
         self._insertFunctionStep(self.createConfigStep)
-        self._insertFunctionStep(self.pickTomogramsStep)
-        self._insertFunctionStep(self.createOutputStep)
 
-    # -------------------------- STEPS functions ------------------------------
-    def pickTomogramsStep(self):
-        """This function picks from a given set of Tomograms"""
-        inputTomos = self.inputTomograms.get()
-        tomogramsList = [t.clone() for t in inputTomos.iterItems()]
-
-        tomogramsDir = self._getTmpPath("tomograms")
-        outputDir = self._getExtraPath()
-        pwutils.cleanPath(tomogramsDir)
-        pwutils.makePath(tomogramsDir)
-
-        # Create folder with linked tomograms
-        convert.convertMicrographs(tomogramsList, tomogramsDir)
-
-        args = "-c %s" % self._getExtraPath('config.json')
-        args += " -w %s" % self.getInputModel()
-        args += " -i %s/" % tomogramsDir
-        args += " -o %s/" % outputDir
-        args += " -t %0.3f" % self.conservPickVar
-        args += " -nc %d" % self.numCpus.get()
-        args += " --tomogram"
-        args += " -tsr %d" % self.searchRange.get()
-        args += " -tmem %d" % self.memory.get()
-        args += " -tmin %d" % self.minLength.get()
+        if self.doFineTune:
+            self._insertFunctionStep(self.cryoloTrainingStep,
+                                     ' --fine_tune -lft 2')
+        else:
+            self._insertFunctionStep(self.cryoloTrainingStep)
 
-        if not self.usingCpu():
-            args += " -g %(GPU)s"  # Add GPU that will be set by the executor
+        self._insertFunctionStep(self.createOutputStep)
+
+    # --------------------------- STEPS functions -----------------------------
+    def convertInputStep(self):
+        """ Converts a set of coordinates to box files and binaries to mrc.
+        It generates 2 folders: one for the box files and another for
+        the mrc files.
+        """
+        inputMics = self.inputMicrographs.get()
+        coordSet = self.inputCoordinates.get()
+
+        paths = []
+        for d in self.TRAIN:
+            paths.append(self._getExtraPath(d))
+            pwutils.makePath(paths[-1])
+
+        micList = [mic.clone() for mic in inputMics]
+        convert.writeSetOfCoordinates(paths[0], coordSet, micList)
+        convert.convertMicrographs(micList, paths[1])
+
+    def cryoloTrainingStep(self, extraArgs=''):
+        params = " -c config.json"
+        params += " -w %d" % (0 if self.doFineTune else 5)
+        params += " -g %(GPU)s"
+        params += " -nc %d" % self.numCpus.get()
+        params += " -e %d" % self.eFlagParam
+        if self.lowPassFilter:
+            params += " --cleanup"
+        params += extraArgs
 
-        if self.lowPassFilter or self.inputModelFrom == INPUT_MODEL_GENERAL_DENOISED:
-            args += ' --cleanup'
+        Plugin.runCryolo(self, 'cryolo_train.py', params,
+                         cwd=self._getExtraPath())
 
-        Plugin.runCryolo(self, 'cryolo_predict.py', args,
-                         useCpu=not self.useGpu.get())
+        pwutils.moveFile(self._getExtraPath(self.MODEL),
+                         self.getOutputModelPath())
 
     def createOutputStep(self):
-        setOfTomograms = self.inputTomograms.get()
-        outputPath = self._getExtraPath("CBOX_3D")
-        suffix = self._getOutputSuffix(SetOfCoordinates3D)
-
-        setOfCoord3D = self._createSetOfCoordinates3D(self.inputTomograms, suffix)
-        setOfCoord3D.setName("tomoCoord")
-        setOfCoord3D.setSamplingRate(setOfTomograms.getSamplingRate())
-
-        if self.boxSize.get():  # Box size can be provided by the user
-            boxSize = self.boxSize.get()
-        else:  # If not crYOLO estimates it
-            boxSize = self.getEstimatedBoxSize(self._getExtraPath('DISTR'))
-
-        setOfCoord3D.setBoxSize(boxSize)
-
-        for tomogram in setOfTomograms.iterItems():
-
-            filePath = os.path.join(outputPath, convert.getMicFn(tomogram, "cbox"))
-            if os.path.exists(filePath) and os.path.getsize(filePath):
-                tomogramClone = tomogram.clone()
-                tomogramClone.copyInfo(tomogram)
-                convert.readSetOfCoordinates3D(tomogramClone, setOfCoord3D, filePath,
-                                               boxSize,
-                                               origin=tomoConst.BOTTOM_LEFT_CORNER)
-
-
-        name = self.OUTPUT_PREFIX + suffix
-        self._defineOutputs(**{name: setOfCoord3D})
-        self._defineSourceRelation(setOfTomograms, setOfCoord3D)
+        """ Register the output model. """
+        self._defineOutputs(outputModel=CryoloModel(self.getOutputModelPath()))
+
+    # --------------------------- INFO functions ------------------------------
+    def _summary(self):
+        summary = []
+
+        if self.doFineTune:
+            summary.append(f"Fine-tuning using "
+                           f"{self.getEnumText('inputModelFrom')} model: "
+                           f"{self.getInputModel()}")
+        else:
+            summary.append("Training a new model from scratch")
+
+        return summary
+
+    # -------------------------- UTILS functions ------------------------------
+    def getOutputModelPath(self):
+        return self._getPath(self.MODEL)
```

### Comparing `scipion-em-sphire-3.1.6/sphire/protocols/protocol_janni_denoise.py` & `scipion-em-sphire-3.1.8/sphire/protocols/protocol_janni_denoise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/sphire/protocols.conf` & `scipion-em-sphire-3.1.8/sphire/protocols.conf`

 * *Files 12% similar despite different names*

```diff
@@ -14,10 +14,12 @@
 		{"tag": "protocol_group", "text": "Preprocess", "openItem": "False", "children": [
 		    {"tag": "protocol", "value": "SphireProtJanniDenoising", "text": "default"}
         ]}
 	]}]
 Tomography = [
 	{"tag": "section", "text": "Particles", "children": [
 		{"tag": "protocol_group", "text": "Picking", "openItem": "False", "children": [
-		    {"tag": "protocol", "value": "SphireProtCRYOLOTomoPicking",   "text": "default"}
+		    {"tag": "protocol", "value": "SphireProtCRYOLOTomoPicking",   "text": "default"},
+		    {"tag": "protocol", "value": "SphireProtCRYOLONapariTomoPicker",   "text": "default"},
+		    {"tag": "protocol", "value": "SphireProtCRYOLOTomoTraining",   "text": "default"}
 		]}
 	]}]
```

### Comparing `scipion-em-sphire-3.1.6/sphire/sphire_logo.png` & `scipion-em-sphire-3.1.8/sphire/sphire_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/sphire/tests/__init__.py` & `scipion-em-sphire-3.1.8/sphire/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.6/sphire/tests/test_protocol_cryolo.py` & `scipion-em-sphire-3.1.8/sphire/tests/test_protocol_cryolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,35 +69,37 @@
 
         def _convert(coordsIn, yFlipHeight=None):
             tmpFile = os.path.join(boxDir, 'tmp.cbox')
             # Write input coordinates
             writer = convert.CoordBoxWriter(boxSize, yFlipHeight=yFlipHeight)
             writer.open(tmpFile)
             writer._file.write(HEADER)  # required for cbox
-            for x, y, _, _ in coordsIn:
+            for x, y, _, _, _, _ in coordsIn:
                 writer.writeCoord(emobj.Coordinate(x=x, y=y))
             writer.close()
 
             reader = convert.CoordBoxReader(boxSize, yFlipHeight=yFlipHeight)
             coordsOut = [c for c in reader.iterCoords(tmpFile)]
 
             return coordsOut
 
-        coordsIn = [(100, 100, 0., 0.), (100, 200, 0., 0.),
-                    (200, 100, 0., 0.), (200, 200, 0., 0.)]
+        coordsIn = [(100, 100, 0., 0., 0, 100), (100, 200, 0., 0.,  0, 100),
+                    (200, 100, 0., 0.,  0, 100), (200, 200, 0., 0.,  0, 100)]
 
         # Case 1: No flip
         coordsOut = _convert(coordsIn)
         for c1, c2 in zip(coordsIn, coordsOut):
             self.assertEqual(c1, c2)
 
         # Case 2: Flipping on Y
-        coordsOut = _convert(coordsIn, yFlipHeight=300)
+        yFlipHeight = 300
+        coordsOut = _convert(coordsIn, yFlipHeight=yFlipHeight)
         for c1, c2 in zip(coordsIn, coordsOut):
-            self.assertEqual(c1, c2)
+            self.assertNotEqual(c1, c2)
+            self.assertEqual(yFlipHeight - c1[1], c2[1])
 
     def testConvertMic(self):
         """Check extension of the input micrographs"""
         micDir = self.getOutputPath('micDir')
         os.mkdir(micDir)
 
         mrcMic = TestSphireConvert.ds.getFile('micrographs/006.mrc')
@@ -413,19 +415,19 @@
 
         print(magentaStr(f"\n==> Importing data - tomograms:"))
         cls.launchProtocol(protImport)
         return protImport
 
     def test_pickingTomograms(self):
         protImport = self._runImportTomograms()
-        self.assertIsNotNone(protImport.outputTomograms,
+        self.assertIsNotNone(protImport.Tomograms,
                              "There was a problem with Import Tomograms protocol")
 
         sphireProtCRYOLOTomoPicking = self.newProtocol(protocols.SphireProtCRYOLOTomoPicking,
-                                                       inputTomograms=protImport.outputTomograms,
+                                                       inputTomograms=protImport.Tomograms,
                                                        inputModelFrom=INPUT_MODEL_GENERAL,
                                                        lowPassFilter=False)
 
         print(magentaStr(f"\n==> Testing sphire - cryolo tomo picking:"))
         self.launchProtocol(sphireProtCRYOLOTomoPicking)
         self.assertIsNotNone(sphireProtCRYOLOTomoPicking.output3DCoordinates,
                              "There was a problem with tomo picking protocol")
```

### Comparing `scipion-em-sphire-3.1.6/sphire/tests/test_protocol_janni.py` & `scipion-em-sphire-3.1.8/sphire/tests/test_protocol_janni.py`

 * *Files identical despite different names*


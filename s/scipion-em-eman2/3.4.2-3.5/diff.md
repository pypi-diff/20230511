# Comparing `tmp/scipion-em-eman2-3.4.2.tar.gz` & `tmp/scipion-em-eman2-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-eman2-3.4.2.tar", last modified: Sun Feb  5 14:52:55 2023, max compression
+gzip compressed data, was "scipion-em-eman2-3.5.tar", last modified: Thu May 11 12:28:05 2023, max compression
```

## Comparing `scipion-em-eman2-3.4.2.tar` & `scipion-em-eman2-3.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:52:55.688207 scipion-em-eman2-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-02-05 14:52:55.688207 scipion-em-eman2-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:52:55.684207 scipion-em-eman2-3.4.2/eman2/
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:52:55.684207 scipion-em-eman2-3.4.2/eman2/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/e2converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2602 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/e2ih.py
--rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/eman2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:52:55.688207 scipion-em-eman2-3.4.2/eman2/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_autopick_boxer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_boxing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_initialmodel_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)    34150 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_refine2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    22667 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_refine2d_bispec.py
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_refineasy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols/protocol_tiltvalidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:52:55.688207 scipion-em-eman2-3.4.2/eman2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/tests/test_protocols_eman.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:52:55.688207 scipion-em-eman2-3.4.2/eman2/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38970 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/eman2/viewers/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 14:52:55.688207 scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-02-05 14:52:55.000000 scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-05 14:52:55.000000 scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 14:52:55.000000 scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-05 14:52:55.000000 scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-05 14:52:55.000000 scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-05 14:52:55.000000 scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 14:52:55.688207 scipion-em-eman2-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-02-05 14:49:30.000000 scipion-em-eman2-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:28:05.982957 scipion-em-eman2-3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-11 12:28:05.982957 scipion-em-eman2-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:28:05.974958 scipion-em-eman2-3.5/eman2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:28:05.974958 scipion-em-eman2-3.5/eman2/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/e2converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2602 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/e2ih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/eman2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:28:05.978958 scipion-em-eman2-3.5/eman2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_autopick_boxer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_boxing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_initialmodel_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34004 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_refine2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_refine2d_bispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26311 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_refineasy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols/protocol_tiltvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:28:05.978958 scipion-em-eman2-3.5/eman2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/tests/test_protocols_eman.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:28:05.978958 scipion-em-eman2-3.5/eman2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38970 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/eman2/viewers/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:28:05.978958 scipion-em-eman2-3.5/scipion_em_eman2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-11 12:28:05.000000 scipion-em-eman2-3.5/scipion_em_eman2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-11 12:28:05.000000 scipion-em-eman2-3.5/scipion_em_eman2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:28:05.000000 scipion-em-eman2-3.5/scipion_em_eman2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 12:28:05.000000 scipion-em-eman2-3.5/scipion_em_eman2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 12:28:05.000000 scipion-em-eman2-3.5/scipion_em_eman2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 12:28:05.000000 scipion-em-eman2-3.5/scipion_em_eman2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:28:05.982957 scipion-em-eman2-3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-11 12:25:40.000000 scipion-em-eman2-3.5/setup.py
```

### Comparing `scipion-em-eman2-3.4.2/CHANGES.txt` & `scipion-em-eman2-3.5/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.5 - use conda for installation, older versions not supported
 3.4.2 - eman 2.9 binary dropped
 3.4.1 - add possible outputs dict
 3.4: eman 2.99 (continuous build) added
 3.3.3 - minor changes
 3.3.2 - fix major bug in shifts conversion
 3.3.1: eman 2.91 added
 3.3:
```

### Comparing `scipion-em-eman2-3.4.2/LICENSE` & `scipion-em-eman2-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/PKG-INFO` & `scipion-em-eman2-3.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 1.2
 Name: scipion-em-eman2
-Version: 3.4.2
-Summary: Plugin to use EMAN2 programs within the Scipion framework
+Version: 3.5
+Summary: Plugin to use EMAN programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-eman2
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-eman2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-eman2/
-Description: ============
-        EMAN2 plugin
-        ============
+Description: ===========
+        EMAN plugin
+        ===========
         
         This plugin provides wrappers around several programs of `EMAN <https://blake.bcm.edu/emanwiki/EMAN2>`_ software suite.
         
         .. image:: https://img.shields.io/pypi/v/scipion-em-eman2.svg
                 :target: https://pypi.python.org/pypi/scipion-em-eman2
                 :alt: PyPI release
         
@@ -56,18 +56,30 @@
         
             * install
         
             .. code-block::
         
                 scipion installp -p /path/to/scipion-em-eman2 --devel
         
-        EMAN2 binaries will be installed automatically with the plugin, but you can also link an existing installation.
+        EMAN software will be installed automatically with the plugin but you can also use an existing installation by providing *EMAN_ENV_ACTIVATION* (see below).
         
-            * Default installation path assumed is ``software/em/eman-2.99``, if you want to change it, set *EMAN2_HOME* in ``scipion.conf`` file pointing to the folder where the EMAN2 is installed.
-            * The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
+        **Important:** you need to have conda (miniconda3 or anaconda3) pre-installed to use this program.
+        
+        Configuration variables
+        -----------------------
+        *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
+        PATH (not recommended), which can lead to execution problems mixing scipion
+        python with conda ones. One example of this could can be seen below but
+        depending on your conda version and shell you will need something different:
+        CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
+        
+        *EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.47):
+        Command to activate the EMAN environment.
+        
+        The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
         
         To check the installation, simply run one of the following Scipion tests:
         
         .. code-block::
         
            scipion test eman2.tests.test_protocols_eman.TestEmanTiltValidate
            scipion test eman2.tests.test_protocols_eman.TestEmanRefineEasy
@@ -81,15 +93,15 @@
            scipion test eman2.tests.test_protocols_eman.TestEmanAutopick
         
         A complete list of tests can also be seen by executing ``scipion test --show --grep eman``
         
         Supported versions
         ------------------
         
-        2.91, 2.99 (continuous build)
+        2.99.47
         
         Protocols
         ---------
         
         * boxer
         * boxer auto
         * ctf auto
@@ -104,10 +116,10 @@
         References
         ----------
         
         1. \G. Tang, L. Peng, P.R. Baldwin, D.S. Mann, W. Jiang, I. Rees & S.J. Ludtke. (2007) EMAN2: an extensible image processing suite for electron microscopy. J Struct Biol. 157, 38-46. PMID: 16859925
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-eman2-3.4.2/README.rst` & `scipion-em-eman2-3.5/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-============
-EMAN2 plugin
-============
+===========
+EMAN plugin
+===========
 
 This plugin provides wrappers around several programs of `EMAN <https://blake.bcm.edu/emanwiki/EMAN2>`_ software suite.
 
 .. image:: https://img.shields.io/pypi/v/scipion-em-eman2.svg
         :target: https://pypi.python.org/pypi/scipion-em-eman2
         :alt: PyPI release
 
@@ -46,18 +46,30 @@
 
     * install
 
     .. code-block::
 
         scipion installp -p /path/to/scipion-em-eman2 --devel
 
-EMAN2 binaries will be installed automatically with the plugin, but you can also link an existing installation.
+EMAN software will be installed automatically with the plugin but you can also use an existing installation by providing *EMAN_ENV_ACTIVATION* (see below).
 
-    * Default installation path assumed is ``software/em/eman-2.99``, if you want to change it, set *EMAN2_HOME* in ``scipion.conf`` file pointing to the folder where the EMAN2 is installed.
-    * The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
+**Important:** you need to have conda (miniconda3 or anaconda3) pre-installed to use this program.
+
+Configuration variables
+-----------------------
+*CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
+PATH (not recommended), which can lead to execution problems mixing scipion
+python with conda ones. One example of this could can be seen below but
+depending on your conda version and shell you will need something different:
+CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
+
+*EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.47):
+Command to activate the EMAN environment.
+
+The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
 
 To check the installation, simply run one of the following Scipion tests:
 
 .. code-block::
 
    scipion test eman2.tests.test_protocols_eman.TestEmanTiltValidate
    scipion test eman2.tests.test_protocols_eman.TestEmanRefineEasy
@@ -71,15 +83,15 @@
    scipion test eman2.tests.test_protocols_eman.TestEmanAutopick
 
 A complete list of tests can also be seen by executing ``scipion test --show --grep eman``
 
 Supported versions
 ------------------
 
-2.91, 2.99 (continuous build)
+2.99.47
 
 Protocols
 ---------
 
 * boxer
 * boxer auto
 * ctf auto
```

### Comparing `scipion-em-eman2-3.4.2/eman2/bibtex.py` & `scipion-em-eman2-3.5/eman2/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/constants.py` & `scipion-em-eman2-3.5/eman2/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-EMAN2_HOME = 'EMAN2_HOME'
 EMAN2SCRATCHDIR = 'EMAN2SCRATCHDIR'
 
 # Supported versions
-VERSIONS = ['2.91', '2.99']
+VERSIONS = ['2.99.47']
+EMAN_DEFAULT_VER_NUM = VERSIONS[-1]
+
+DEFAULT_ENV_NAME = f"eman-{EMAN_DEFAULT_VER_NUM}"
+DEFAULT_ACTIVATION_CMD = 'conda activate ' + DEFAULT_ENV_NAME
+EMAN_ENV_ACTIVATION = 'EMAN_ENV_ACTIVATION'
 
 # ------------------ Constants values -----------------------------------------
 
 # ctf processing type
 HIRES = 0
 MIDRES = 1
 LORES = 2
```

### Comparing `scipion-em-eman2-3.4.2/eman2/convert/__init__.py` & `scipion-em-eman2-3.5/eman2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/convert/convert.py` & `scipion-em-eman2-3.5/eman2/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/convert/dataimport.py` & `scipion-em-eman2-3.5/eman2/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/e2converter.py` & `scipion-em-eman2-3.5/eman2/e2converter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/e2ih.py` & `scipion-em-eman2-3.5/eman2/e2ih.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/eman2_logo.png` & `scipion-em-eman2-3.5/eman2/eman2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/__init__.py` & `scipion-em-eman2-3.5/eman2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_autopick_boxer.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_autopick_boxer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_boxing.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_boxing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_ctf.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_initialmodel.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_initialmodel_sgd.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_initialmodel_sgd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_reconstruct.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_reconstruct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_refine2d.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_refine2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     def _createIterTemplates(self, currRun):
         """ Setup the regex on how to find iterations. """
         clsFn = self._getExtraPath(self._getFileName('classes', run=currRun, iter=1))
         self._iterTemplate = clsFn.replace('classes_01', 'classes_??')
         # Iterations will be identify by classes_XX_ where XX is the iteration
         #  number and is restricted to only 2 digits.
-        self._iterRegex = re.compile('classes_(\d{2})')
+        self._iterRegex = re.compile(r'classes_(\d{2})')
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('doContinue', BooleanParam, default=False,
                       label='Continue from a previous run?',
                       help='If you set to *Yes*, you should select a previous '
@@ -511,15 +511,15 @@
         args2 = self._commonParams()
         args = args1 + args2
 
         return args
 
     def _prepareContinueParams(self):
         args = " --input=%s" % self._getParticlesStack()
-        runN = self._getRun() - 1 if not Plugin.versionGE('2.91') else self._getRun()
+        runN = self._getRun()
         args += " --initial=r2d_%02d/classes_%02d.hdf" % \
                 (runN, self._getIt())
         args += self._commonParams()
 
         return args
 
     def _commonParams(self):
@@ -566,26 +566,26 @@
         if self.extraParams.hasValue():
             args += " " + self.extraParams.get()
 
         return args
 
     def _getRun(self):
         if not self.doContinue:
-            return 0 if Plugin.versionGE('2.91') else 1
+            return 0
         else:
             contRun = self.continueRun.get()
             files = sorted(glob(contRun._getExtraPath("r2d_??")))
             if files:
                 f = files[-1]
                 runNumber = int(f.split("_")[-1]) + 1
                 return runNumber
 
     def _getIt(self):
         contRun = self.continueRun.get()
-        runN = self._getRun() - 1 if not Plugin.versionGE('2.91') else self._getRun()
+        runN = self._getRun()
         files = sorted(glob(contRun._getExtraPath("r2d_%02d/classes_??.hdf" % runN)))
         if files:
             i = files[-1]
             iterNumber = int(i.split("_")[-1].replace('.hdf', ''))
             return iterNumber
         else:
             return 1
```

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_refine2d_bispec.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_refine2d_bispec.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     def _createIterTemplates(self, currRun):
         """ Setup the regex on how to find iterations. """
         clsFn = self._getExtraPath(self._getFileName('classes', run=currRun, iter=1))
         self._iterTemplate = clsFn.replace('classes_01', 'classes_??')
         # Iterations will be identify by classes_XX_ where XX is the iteration
         #  number and is restricted to only 2 digits.
-        self._iterRegex = re.compile('classes_(\d{2})')
+        self._iterRegex = re.compile(r'classes_(\d{2})')
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputBispec', PointerParam,
                       label='Choose e2ctf auto protocol',
                       pointerClass='EmanProtCTFAuto',
@@ -381,15 +381,15 @@
     def _iterTextFile(self, iterN):
         with open(self._getFileName('results', iter=iterN)) as f:
             for line in f:
                 if '#' not in line and line.strip():
                     yield [float(x) for x in line.split()]
 
     def _getRun(self):
-        return 0 if Plugin.versionGE('2.91') else 1
+        return 0
 
     def _getIterNumber(self, index):
         """ Return the list of iteration files, give the iterTemplate. """
         result = None
         files = sorted(glob(self._iterTemplate))
         if files:
             f = files[index]
```

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_refineasy.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_refineasy.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     def _createIterTemplates(self, currRun):
         """ Setup the regex on how to find iterations. """
         self._iterTemplate = self._getFileName('mapFull', run=currRun,
                                                iter=1).replace('threed_01',
                                                                'threed_??')
         # Iterations will be identify by threed_XX_ where XX is the iteration
         # number and is restricted to only 2 digits.
-        self._iterRegex = re.compile('threed_(\d{2})')
+        self._iterRegex = re.compile(r'threed_(\d{2})')
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('doContinue', BooleanParam, default=False,
                       label='Continue from a previous run?',
                       help='If you set to *Yes*, you should select a previous '
@@ -269,15 +269,15 @@
         self._insertFunctionStep('createOutputStep')
 
     # --------------------------- STEPS functions -----------------------------
     def createLinkSteps(self):
         continueRun = self.continueRun.get()
         prevPartDir = continueRun._getExtraPath("particles")
         currPartDir = self._getExtraPath("particles")
-        runN = self._getRun() - 1 if not Plugin.versionGE('2.91') else self._getRun()
+        runN = self._getRun()
         prevRefDir = continueRun._getExtraPath("refine_%02d" % runN)
         currRefDir = self._getExtraPath("refine_%02d" % runN)
         prevSetsDir = continueRun._getExtraPath("sets")
         currSetsDir = self._getExtraPath("sets")
 
         createLink(prevPartDir, currPartDir)
         createLink(prevRefDir, currRefDir)
@@ -388,15 +388,15 @@
         params = {'imgsFn': self._getParticlesStack(),
                   'volume': refVolFn}
 
         args = args1 % params + args2
         return args
 
     def _prepareContinueParams(self):
-        runN = self._getRun() - 1 if not Plugin.versionGE('2.91') else self._getRun()
+        runN = self._getRun()
         args1 = "--startfrom=refine_%02d" % runN
         args2 = self._commonParams()
         args = args1 + args2
         return args
 
     def _commonParams(self):
         args = " --targetres=%(resol)f --speed=%(speed)d --sym=%(sym)s "
@@ -451,15 +451,15 @@
 
         if self.extraParams.hasValue():
             args += ' ' + self.extraParams.get()
         return args
 
     def _getRun(self):
         if not self.doContinue:
-            return 0 if Plugin.versionGE('2.91') else 1
+            return 0
         else:
             files = sorted(glob(self.continueRun.get()._getExtraPath("refine*")))
             if files:
                 f = files[-1]
                 refineNumber = int(f.split("_")[-1]) + 1
                 return refineNumber
```

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols/protocol_tiltvalidate.py` & `scipion-em-eman2-3.5/eman2/protocols/protocol_tiltvalidate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/protocols.conf` & `scipion-em-eman2-3.5/eman2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/tests/test_protocols_eman.py` & `scipion-em-eman2-3.5/eman2/tests/test_protocols_eman.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/viewers/__init__.py` & `scipion-em-eman2-3.5/eman2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/eman2/viewers/viewers.py` & `scipion-em-eman2-3.5/eman2/viewers/viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/PKG-INFO` & `scipion-em-eman2-3.5/scipion_em_eman2.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 1.2
 Name: scipion-em-eman2
-Version: 3.4.2
-Summary: Plugin to use EMAN2 programs within the Scipion framework
+Version: 3.5
+Summary: Plugin to use EMAN programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-eman2
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-eman2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-eman2/
-Description: ============
-        EMAN2 plugin
-        ============
+Description: ===========
+        EMAN plugin
+        ===========
         
         This plugin provides wrappers around several programs of `EMAN <https://blake.bcm.edu/emanwiki/EMAN2>`_ software suite.
         
         .. image:: https://img.shields.io/pypi/v/scipion-em-eman2.svg
                 :target: https://pypi.python.org/pypi/scipion-em-eman2
                 :alt: PyPI release
         
@@ -56,18 +56,30 @@
         
             * install
         
             .. code-block::
         
                 scipion installp -p /path/to/scipion-em-eman2 --devel
         
-        EMAN2 binaries will be installed automatically with the plugin, but you can also link an existing installation.
+        EMAN software will be installed automatically with the plugin but you can also use an existing installation by providing *EMAN_ENV_ACTIVATION* (see below).
         
-            * Default installation path assumed is ``software/em/eman-2.99``, if you want to change it, set *EMAN2_HOME* in ``scipion.conf`` file pointing to the folder where the EMAN2 is installed.
-            * The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
+        **Important:** you need to have conda (miniconda3 or anaconda3) pre-installed to use this program.
+        
+        Configuration variables
+        -----------------------
+        *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
+        PATH (not recommended), which can lead to execution problems mixing scipion
+        python with conda ones. One example of this could can be seen below but
+        depending on your conda version and shell you will need something different:
+        CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
+        
+        *EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.47):
+        Command to activate the EMAN environment.
+        
+        The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
         
         To check the installation, simply run one of the following Scipion tests:
         
         .. code-block::
         
            scipion test eman2.tests.test_protocols_eman.TestEmanTiltValidate
            scipion test eman2.tests.test_protocols_eman.TestEmanRefineEasy
@@ -81,15 +93,15 @@
            scipion test eman2.tests.test_protocols_eman.TestEmanAutopick
         
         A complete list of tests can also be seen by executing ``scipion test --show --grep eman``
         
         Supported versions
         ------------------
         
-        2.91, 2.99 (continuous build)
+        2.99.47
         
         Protocols
         ---------
         
         * boxer
         * boxer auto
         * ctf auto
@@ -104,10 +116,10 @@
         References
         ----------
         
         1. \G. Tang, L. Peng, P.R. Baldwin, D.S. Mann, W. Jiang, I. Rees & S.J. Ludtke. (2007) EMAN2: an extensible image processing suite for electron microscopy. J Struct Biol. 157, 38-46. PMID: 16859925
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-eman2-3.4.2/scipion_em_eman2.egg-info/SOURCES.txt` & `scipion-em-eman2-3.5/scipion_em_eman2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.4.2/setup.py` & `scipion-em-eman2-3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
     version=__version__,  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description='Plugin to use EMAN2 programs within the Scipion framework',  # Required
+    description='Plugin to use EMAN programs within the Scipion framework',  # Required
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
@@ -103,15 +103,15 @@
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 4 - Beta',
 
         # Indicate who your project is intended for
         #   'Intended Audience :: Users',
 
         # Pick your license as you wish
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```


# Comparing `tmp/robotframework-sysrepolibrary-0.1.0.tar.gz` & `tmp/robotframework-sysrepolibrary-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-sysrepolibrary-0.1.0.tar", last modified: Tue Apr 25 17:42:58 2023, max compression
+gzip compressed data, was "robotframework-sysrepolibrary-0.1.1.tar", last modified: Thu May 11 14:41:31 2023, max compression
```

## Comparing `robotframework-sysrepolibrary-0.1.0.tar` & `robotframework-sysrepolibrary-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-04-25 17:42:58.968278 robotframework-sysrepolibrary-0.1.0/
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     1162 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/.gitlab-ci.yml
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      536 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/CODEOWNERS
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     5259 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     4544 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/CONTRIBUTING.md
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     1469 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/LICENSE
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      275 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/MANIFEST.in
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     8254 2023-04-25 17:42:58.968278 robotframework-sysrepolibrary-0.1.0/PKG-INFO
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     5452 2023-04-25 17:42:42.000000 robotframework-sysrepolibrary-0.1.0/README.md
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      654 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/SECURITY.md
-drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-04-25 17:42:58.964278 robotframework-sysrepolibrary-0.1.0/docs/
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      638 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/Makefile
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      804 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/make.bat
-drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-04-25 17:42:58.964278 robotframework-sysrepolibrary-0.1.0/docs/source/
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      364 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/source/SysrepoLibrary.rst
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     1157 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/source/conf.py
-drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-04-25 17:42:58.964278 robotframework-sysrepolibrary-0.1.0/docs/source/generated/
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      120 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/source/generated/SysrepoLibrary.rst
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      450 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/source/index.rst
--rw-rw-r--   0 andrej    (1000) andrej    (1000)       57 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/source/modules.rst
--rw-rw-r--   0 andrej    (1000) andrej    (1000)       33 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/docs/source/readme_link.md
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     1583 2023-04-25 17:42:42.000000 robotframework-sysrepolibrary-0.1.0/pyproject.toml
--rw-rw-r--   0 andrej    (1000) andrej    (1000)       38 2023-04-25 17:42:58.968278 robotframework-sysrepolibrary-0.1.0/setup.cfg
-drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-04-25 17:42:58.964278 robotframework-sysrepolibrary-0.1.0/src/
-drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-04-25 17:42:58.968278 robotframework-sysrepolibrary-0.1.0/src/SysrepoLibrary/
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     7773 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/src/SysrepoLibrary/SysrepoLibrary.py
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      351 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/src/SysrepoLibrary/__init__.py
-drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-04-25 17:42:58.968278 robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/
--rw-rw-r--   0 andrej    (1000) andrej    (1000)     8254 2023-04-25 17:42:58.000000 robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/PKG-INFO
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      670 2023-04-25 17:42:58.000000 robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/SOURCES.txt
--rw-rw-r--   0 andrej    (1000) andrej    (1000)        1 2023-04-25 17:42:58.000000 robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/dependency_links.txt
--rw-rw-r--   0 andrej    (1000) andrej    (1000)       63 2023-04-25 17:42:58.000000 robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/requires.txt
--rw-rw-r--   0 andrej    (1000) andrej    (1000)       15 2023-04-25 17:42:58.000000 robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/top_level.txt
--rw-rw-r--   0 andrej    (1000) andrej    (1000)      376 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.0/tox.ini
+drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     1162 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/.gitlab-ci.yml
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      536 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/CODEOWNERS
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     5259 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     4544 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/CONTRIBUTING.md
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     1469 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/LICENSE
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      275 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/MANIFEST.in
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     9008 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/PKG-INFO
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     6199 2023-05-11 14:41:00.000000 robotframework-sysrepolibrary-0.1.1/README.md
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      654 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/SECURITY.md
+drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/docs/
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      638 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/Makefile
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      804 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/make.bat
+drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/docs/source/
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      364 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/source/SysrepoLibrary.rst
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     1157 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/source/conf.py
+drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/docs/source/generated/
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      120 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/source/generated/SysrepoLibrary.rst
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      450 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/source/index.rst
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)       57 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/source/modules.rst
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)       33 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/docs/source/readme_link.md
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     1590 2023-05-11 14:41:00.000000 robotframework-sysrepolibrary-0.1.1/pyproject.toml
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)       38 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/setup.cfg
+drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-05-11 14:41:31.336738 robotframework-sysrepolibrary-0.1.1/src/
+drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/src/SysrepoLibrary/
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     7773 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/src/SysrepoLibrary/SysrepoLibrary.py
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      351 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/src/SysrepoLibrary/__init__.py
+drwxrwxr-x   0 andrej    (1000) andrej    (1000)        0 2023-05-11 14:41:31.344738 robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)     9008 2023-05-11 14:41:31.000000 robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/PKG-INFO
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      670 2023-05-11 14:41:31.000000 robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)        1 2023-05-11 14:41:31.000000 robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)       63 2023-05-11 14:41:31.000000 robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/requires.txt
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)       15 2023-05-11 14:41:31.000000 robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/top_level.txt
+-rw-rw-r--   0 andrej    (1000) andrej    (1000)      376 2023-04-19 11:18:54.000000 robotframework-sysrepolibrary-0.1.1/tox.ini
```

### Comparing `robotframework-sysrepolibrary-0.1.0/.gitlab-ci.yml` & `robotframework-sysrepolibrary-0.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/CODEOWNERS` & `robotframework-sysrepolibrary-0.1.1/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/CODE_OF_CONDUCT.md` & `robotframework-sysrepolibrary-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/CONTRIBUTING.md` & `robotframework-sysrepolibrary-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/LICENSE` & `robotframework-sysrepolibrary-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/PKG-INFO` & `robotframework-sysrepolibrary-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-sysrepolibrary
-Version: 0.1.0
+Version: 0.1.1
 Summary: A testing library for Robot Framework that utilizes the Sysrepo tool internally
 Author-email: Juraj Vijtiuk <juraj.vijtiuk@sartura.hr>, Andrej Gardijan <andrej.gardijan@sartura.hr>
 Maintainer-email: Juraj Vijtiuk <juraj.vijtiuk@sartura.hr>, Andrej Gardijan <andrej.gardijan@sartura.hr>
 License: Copyright (c) 2023 Deutsche Telekom AG.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -12,17 +12,17 @@
         
         2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
         
         3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: Homepage, https://lab.sartura.hr/dt/robotframework-sysrepolibrary
-Project-URL: Bug Reports, https://lab.sartura.hr/dt/robotframework-sysrepolibrary/-/issues
-Project-URL: Source, https://lab.sartura.hr/dt/robotframework-sysrepolibrary
+Project-URL: Homepage, https://github.com/telekom/sysrepo-library-robot-framework
+Project-URL: Bug Reports, https://github.com/telekom/sysrepo-library-robot-framework/issues
+Project-URL: Source, https://github.com/telekom/sysrepo-library-robot-framework
 Keywords: sysrepo,robot,robotframework,networking,linux,testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Robot Framework
@@ -39,14 +39,15 @@
     Sysrepo Robot Framework Library
 </h1>
 
 <p align="center">
     <a href="/../../commits/" title="Last Commit"><img src="https://img.shields.io/github/last-commit/telekom/sysrepo-library-robot-framework?style=flat"></a>
     <a href="/../../issues" title="Open Issues"><img src="https://img.shields.io/github/issues/telekom/sysrepo-library-robot-framework?style=flat"></a>
     <a href="./LICENSE" title="License"><img src="https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat"></a>
+    <a href="https://pypi.org/project/robotframework-sysrepolibrary/" title="PyPi robotframework-sysrepolibrary"><img src="https://img.shields.io/static/v1?label=PyPi&message=robotframework-sysrepolibrary&color=blue&labelColor=yellow"></a>
 </p>
 
 <p align="center">
   <a href="#development">Development</a> •
   <a href="#documentation">Documentation</a> •
   <a href="#support-and-feedback">Support</a> •
   <a href="#how-to-contribute">Contribute</a> •
@@ -69,14 +70,26 @@
 * libyang
 * sysrepo
 * pip
 * setuptools
 * wheel
 * build
 
+#### Installation
+The recommended installation method is using [pip](http://pip-installer.org):
+```
+$ python3 -m pip install robotframework-sysrepolibrary
+```
+
+With recent versions of `pip` it is also possible to install directly from the [GitHub](https://github.com/telekom/sysrepo-library-robot-framework) repository. 
+To install from the latest source from the master branch, use the following command:
+```
+$ python3 -m pip install git+https://github.com/telekom/sysrepo-library-robot-framework.git
+```
+
 #### Build
 
 First clone the repository:
 
 ```
 $ git clone https://github.com/telekom/sysrepo-library-robot-framework
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: robotframework-sysrepolibrary Version: 0.1.0
+Metadata-Version: 2.1 Name: robotframework-sysrepolibrary Version: 0.1.1
 Summary: A testing library for Robot Framework that utilizes the Sysrepo tool
 internally Author-email: Juraj Vijtiuk
 vijtiuk@sartura.hr>, Andrej Gardijan
 gardijan@sartura.hr> Maintainer-email: Juraj Vijtiuk
 vijtiuk@sartura.hr>, Andrej Gardijan
 gardijan@sartura.hr> License: Copyright (c) 2023 Deutsche Telekom AG.
 Redistribution and use in source and binary forms, with or without
@@ -20,71 +20,80 @@
 EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
 INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: Homepage, https://
-lab.sartura.hr/dt/robotframework-sysrepolibrary Project-URL: Bug Reports,
-https://lab.sartura.hr/dt/robotframework-sysrepolibrary/-/issues Project-URL:
-Source, https://lab.sartura.hr/dt/robotframework-sysrepolibrary Keywords:
+github.com/telekom/sysrepo-library-robot-framework Project-URL: Bug Reports,
+https://github.com/telekom/sysrepo-library-robot-framework/issues Project-URL:
+Source, https://github.com/telekom/sysrepo-library-robot-framework Keywords:
 sysrepo,robot,robotframework,networking,linux,testing Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: Operating System :: POSIX :: Linux Classifier:
 Topic :: System :: Networking Requires-Python: >=3.6.0 Description-Content-
 Type: text/markdown Provides-Extra: docs Provides-Extra: tests License-File:
 LICENSE
                  ****** Sysrepo Robot Framework Library ******
    [https://img.shields.io/github/last-commit/telekom/sysrepo-library-robot-
  framework?style=flat] [https://img.shields.io/github/issues/telekom/sysrepo-
   library-robot-framework?style=flat] [https://img.shields.io/badge/License-
-                     BSD%203--Clause-blue.svg?style=flat]
+     BSD%203--Clause-blue.svg?style=flat] [https://img.shields.io/static/
+                     v1?label=PyPi&message=robotframework-
+                 sysrepolibrary&color=blue&labelColor=yellow]
  Development â¢ Documentation â¢ Support â¢ Contribute â¢ Contributors â¢
                                    Licensing
 The goal of this project is to provide a way to use sysrepo with the [Robot
 Framework](https://github.com/robotframework/robotframework). ## About this
 component This repository contains a Robot Framework Python library wrapper
 around the [sysrepo-python](https://github.com/sysrepo/sysrepo-python) sysrepo
 bindings. The [examples](./examples/) directory contains a simple example test
 that connects to sysrepo and does some basic validity checks. ## Development
 The following additional dependencies are required to work on the library: *
-libyang * sysrepo * pip * setuptools * wheel * build #### Build First clone the
-repository: ``` $ git clone https://github.com/telekom/sysrepo-library-robot-
-framework ``` To build the library run the following commands: ``` $ python3 -
-m venv sysrepolibrary-venv $ source sysrepolibrary-venv/bin/activate $ python3
--m pip install --upgrade pip setuptools wheel build ``` To install it: ``` $
-python3 -m pip install . ``` To install the additional dependencies as well
-(generating the documentation and testing): ``` $ python3 -m pip install .
-[docs,tests] ``` ## Code of Conduct This project has adopted the [Contributor
-Covenant](https://www.contributor-covenant.org/) in version 2.0 as our code of
-conduct. Please see the details in our [CODE_OF_CONDUCT.md]
-(CODE_OF_CONDUCT.md). All contributors must abide by the code of conduct. ##
-Working Language We decided to apply _English_ as the primary project language.
-Consequently, all content will be made available primarily in English. We also
-ask all interested people to use English as language to create issues, in their
-code (comments, documentation etc.) and when you send requests to us. The
-application itself and all end-user facing content will be made available in
-other languages as needed. ## Documentation The documentation for the Sysrepo
-Robot Framework Library can be generated using the [Sphinx](https://www.sphinx-
-doc.org/en/master/) documentation generator tool. The documentation sources are
-located in [docs/source](./docs/source) To build the documentation as `HTML`
-files run while in the root directory: ``` $ sphinx-build -b html docs/source
-docs/build/html ``` The `-b` option selects a builder in this example it's
-`HTML`. To quickly generate the docs use the scripts in the `docs/` directory.
-Execute `make` without an argument while in the directory to see which targets
-are available. Example for `HTML`: ``` docs/$ make html ``` ## Support and
-Feedback The following channels are available for discussions, feedback, and
-support requests: | Type | Channel | | ------------------ | -------------------
+libyang * sysrepo * pip * setuptools * wheel * build #### Installation The
+recommended installation method is using [pip](http://pip-installer.org): ``` $
+python3 -m pip install robotframework-sysrepolibrary ``` With recent versions
+of `pip` it is also possible to install directly from the [GitHub](https://
+github.com/telekom/sysrepo-library-robot-framework) repository. To install from
+the latest source from the master branch, use the following command: ``` $
+python3 -m pip install git+https://github.com/telekom/sysrepo-library-robot-
+framework.git ``` #### Build First clone the repository: ``` $ git clone https:
+//github.com/telekom/sysrepo-library-robot-framework ``` To build the library
+run the following commands: ``` $ python3 -m venv sysrepolibrary-venv $ source
+sysrepolibrary-venv/bin/activate $ python3 -m pip install --upgrade pip
+setuptools wheel build ``` To install it: ``` $ python3 -m pip install . ``` To
+install the additional dependencies as well (generating the documentation and
+testing): ``` $ python3 -m pip install .[docs,tests] ``` ## Code of Conduct
+This project has adopted the [Contributor Covenant](https://www.contributor-
+covenant.org/) in version 2.0 as our code of conduct. Please see the details in
+our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). All contributors must abide by
+the code of conduct. ## Working Language We decided to apply _English_ as the
+primary project language. Consequently, all content will be made available
+primarily in English. We also ask all interested people to use English as
+language to create issues, in their code (comments, documentation etc.) and
+when you send requests to us. The application itself and all end-user facing
+content will be made available in other languages as needed. ## Documentation
+The documentation for the Sysrepo Robot Framework Library can be generated
+using the [Sphinx](https://www.sphinx-doc.org/en/master/) documentation
+generator tool. The documentation sources are located in [docs/source](./docs/
+source) To build the documentation as `HTML` files run while in the root
+directory: ``` $ sphinx-build -b html docs/source docs/build/html ``` The `-b`
+option selects a builder in this example it's `HTML`. To quickly generate the
+docs use the scripts in the `docs/` directory. Execute `make` without an
+argument while in the directory to see which targets are available. Example for
+`HTML`: ``` docs/$ make html ``` ## Support and Feedback The following channels
+are available for discussions, feedback, and support requests: | Type | Channel
+| | ------------------ | ------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
------------------ | | **Issues** | [https://img.shields.io/github/issues/
-telekom/sysrepo-library-robot-framework?style=flat-square]
+------------------------------------------------------------- | | **Issues** |
+[https://img.shields.io/github/issues/telekom/sysrepo-library-robot-
+framework?style=flat-square]
  | | **Other Requests** | [https://img.shields.io/badge/email-
 Open%20Source%20Team-green?logo=mail.ru&style=flat-square&logoColor=white] | ##
 How to Contribute Contribution and feedback is encouraged and always welcome.
 For more information about how to contribute, the project structure, as well as
 additional contribution information, see our [Contribution Guidelines](./
 CONTRIBUTING.md). By participating in this project, you agree to abide by its
 [Code of Conduct](./CODE_OF_CONDUCT.md) at all times. ## Contributors Our
```

### Comparing `robotframework-sysrepolibrary-0.1.0/README.md` & `robotframework-sysrepolibrary-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     Sysrepo Robot Framework Library
 </h1>
 
 <p align="center">
     <a href="/../../commits/" title="Last Commit"><img src="https://img.shields.io/github/last-commit/telekom/sysrepo-library-robot-framework?style=flat"></a>
     <a href="/../../issues" title="Open Issues"><img src="https://img.shields.io/github/issues/telekom/sysrepo-library-robot-framework?style=flat"></a>
     <a href="./LICENSE" title="License"><img src="https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat"></a>
+    <a href="https://pypi.org/project/robotframework-sysrepolibrary/" title="PyPi robotframework-sysrepolibrary"><img src="https://img.shields.io/static/v1?label=PyPi&message=robotframework-sysrepolibrary&color=blue&labelColor=yellow"></a>
 </p>
 
 <p align="center">
   <a href="#development">Development</a> •
   <a href="#documentation">Documentation</a> •
   <a href="#support-and-feedback">Support</a> •
   <a href="#how-to-contribute">Contribute</a> •
@@ -32,14 +33,26 @@
 * libyang
 * sysrepo
 * pip
 * setuptools
 * wheel
 * build
 
+#### Installation
+The recommended installation method is using [pip](http://pip-installer.org):
+```
+$ python3 -m pip install robotframework-sysrepolibrary
+```
+
+With recent versions of `pip` it is also possible to install directly from the [GitHub](https://github.com/telekom/sysrepo-library-robot-framework) repository. 
+To install from the latest source from the master branch, use the following command:
+```
+$ python3 -m pip install git+https://github.com/telekom/sysrepo-library-robot-framework.git
+```
+
 #### Build
 
 First clone the repository:
 
 ```
 $ git clone https://github.com/telekom/sysrepo-library-robot-framework
 ```
```

#### html2text {}

```diff
@@ -1,52 +1,61 @@
                  ****** Sysrepo Robot Framework Library ******
    [https://img.shields.io/github/last-commit/telekom/sysrepo-library-robot-
  framework?style=flat] [https://img.shields.io/github/issues/telekom/sysrepo-
   library-robot-framework?style=flat] [https://img.shields.io/badge/License-
-                     BSD%203--Clause-blue.svg?style=flat]
+     BSD%203--Clause-blue.svg?style=flat] [https://img.shields.io/static/
+                     v1?label=PyPi&message=robotframework-
+                 sysrepolibrary&color=blue&labelColor=yellow]
  Development â¢ Documentation â¢ Support â¢ Contribute â¢ Contributors â¢
                                    Licensing
 The goal of this project is to provide a way to use sysrepo with the [Robot
 Framework](https://github.com/robotframework/robotframework). ## About this
 component This repository contains a Robot Framework Python library wrapper
 around the [sysrepo-python](https://github.com/sysrepo/sysrepo-python) sysrepo
 bindings. The [examples](./examples/) directory contains a simple example test
 that connects to sysrepo and does some basic validity checks. ## Development
 The following additional dependencies are required to work on the library: *
-libyang * sysrepo * pip * setuptools * wheel * build #### Build First clone the
-repository: ``` $ git clone https://github.com/telekom/sysrepo-library-robot-
-framework ``` To build the library run the following commands: ``` $ python3 -
-m venv sysrepolibrary-venv $ source sysrepolibrary-venv/bin/activate $ python3
--m pip install --upgrade pip setuptools wheel build ``` To install it: ``` $
-python3 -m pip install . ``` To install the additional dependencies as well
-(generating the documentation and testing): ``` $ python3 -m pip install .
-[docs,tests] ``` ## Code of Conduct This project has adopted the [Contributor
-Covenant](https://www.contributor-covenant.org/) in version 2.0 as our code of
-conduct. Please see the details in our [CODE_OF_CONDUCT.md]
-(CODE_OF_CONDUCT.md). All contributors must abide by the code of conduct. ##
-Working Language We decided to apply _English_ as the primary project language.
-Consequently, all content will be made available primarily in English. We also
-ask all interested people to use English as language to create issues, in their
-code (comments, documentation etc.) and when you send requests to us. The
-application itself and all end-user facing content will be made available in
-other languages as needed. ## Documentation The documentation for the Sysrepo
-Robot Framework Library can be generated using the [Sphinx](https://www.sphinx-
-doc.org/en/master/) documentation generator tool. The documentation sources are
-located in [docs/source](./docs/source) To build the documentation as `HTML`
-files run while in the root directory: ``` $ sphinx-build -b html docs/source
-docs/build/html ``` The `-b` option selects a builder in this example it's
-`HTML`. To quickly generate the docs use the scripts in the `docs/` directory.
-Execute `make` without an argument while in the directory to see which targets
-are available. Example for `HTML`: ``` docs/$ make html ``` ## Support and
-Feedback The following channels are available for discussions, feedback, and
-support requests: | Type | Channel | | ------------------ | -------------------
+libyang * sysrepo * pip * setuptools * wheel * build #### Installation The
+recommended installation method is using [pip](http://pip-installer.org): ``` $
+python3 -m pip install robotframework-sysrepolibrary ``` With recent versions
+of `pip` it is also possible to install directly from the [GitHub](https://
+github.com/telekom/sysrepo-library-robot-framework) repository. To install from
+the latest source from the master branch, use the following command: ``` $
+python3 -m pip install git+https://github.com/telekom/sysrepo-library-robot-
+framework.git ``` #### Build First clone the repository: ``` $ git clone https:
+//github.com/telekom/sysrepo-library-robot-framework ``` To build the library
+run the following commands: ``` $ python3 -m venv sysrepolibrary-venv $ source
+sysrepolibrary-venv/bin/activate $ python3 -m pip install --upgrade pip
+setuptools wheel build ``` To install it: ``` $ python3 -m pip install . ``` To
+install the additional dependencies as well (generating the documentation and
+testing): ``` $ python3 -m pip install .[docs,tests] ``` ## Code of Conduct
+This project has adopted the [Contributor Covenant](https://www.contributor-
+covenant.org/) in version 2.0 as our code of conduct. Please see the details in
+our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). All contributors must abide by
+the code of conduct. ## Working Language We decided to apply _English_ as the
+primary project language. Consequently, all content will be made available
+primarily in English. We also ask all interested people to use English as
+language to create issues, in their code (comments, documentation etc.) and
+when you send requests to us. The application itself and all end-user facing
+content will be made available in other languages as needed. ## Documentation
+The documentation for the Sysrepo Robot Framework Library can be generated
+using the [Sphinx](https://www.sphinx-doc.org/en/master/) documentation
+generator tool. The documentation sources are located in [docs/source](./docs/
+source) To build the documentation as `HTML` files run while in the root
+directory: ``` $ sphinx-build -b html docs/source docs/build/html ``` The `-b`
+option selects a builder in this example it's `HTML`. To quickly generate the
+docs use the scripts in the `docs/` directory. Execute `make` without an
+argument while in the directory to see which targets are available. Example for
+`HTML`: ``` docs/$ make html ``` ## Support and Feedback The following channels
+are available for discussions, feedback, and support requests: | Type | Channel
+| | ------------------ | ------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
------------------ | | **Issues** | [https://img.shields.io/github/issues/
-telekom/sysrepo-library-robot-framework?style=flat-square]
+------------------------------------------------------------- | | **Issues** |
+[https://img.shields.io/github/issues/telekom/sysrepo-library-robot-
+framework?style=flat-square]
  | | **Other Requests** | [https://img.shields.io/badge/email-
 Open%20Source%20Team-green?logo=mail.ru&style=flat-square&logoColor=white] | ##
 How to Contribute Contribution and feedback is encouraged and always welcome.
 For more information about how to contribute, the project structure, as well as
 additional contribution information, see our [Contribution Guidelines](./
 CONTRIBUTING.md). By participating in this project, you agree to abide by its
 [Code of Conduct](./CODE_OF_CONDUCT.md) at all times. ## Contributors Our
```

### Comparing `robotframework-sysrepolibrary-0.1.0/SECURITY.md` & `robotframework-sysrepolibrary-0.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/docs/Makefile` & `robotframework-sysrepolibrary-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/docs/make.bat` & `robotframework-sysrepolibrary-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/docs/source/conf.py` & `robotframework-sysrepolibrary-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/pyproject.toml` & `robotframework-sysrepolibrary-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 	"robotframework-sysrepolibrary"
-version = "0.1.0"
+version = "0.1.1"
 description = "A testing library for Robot Framework that utilizes the Sysrepo tool internally"
 readme = { file = "README.md", content-type = "text/markdown" }
 
 requires-python = ">=3.6.0"
 
 license = { file = "LICENSE" }
 
@@ -45,15 +45,15 @@
 
 tests = [
     "tox"
 ]
 
 
 [project.urls] 
-"Homepage" = "https://lab.sartura.hr/dt/robotframework-sysrepolibrary"
-"Bug Reports" = "https://lab.sartura.hr/dt/robotframework-sysrepolibrary/-/issues"
-"Source" = "https://lab.sartura.hr/dt/robotframework-sysrepolibrary"
+"Homepage" = "https://github.com/telekom/sysrepo-library-robot-framework"
+"Bug Reports" = "https://github.com/telekom/sysrepo-library-robot-framework/issues"
+"Source" = "https://github.com/telekom/sysrepo-library-robot-framework"
 
 
 [build-system]
 requires      = ["setuptools>=42.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `robotframework-sysrepolibrary-0.1.0/src/SysrepoLibrary/SysrepoLibrary.py` & `robotframework-sysrepolibrary-0.1.1/src/SysrepoLibrary/SysrepoLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/PKG-INFO` & `robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-sysrepolibrary
-Version: 0.1.0
+Version: 0.1.1
 Summary: A testing library for Robot Framework that utilizes the Sysrepo tool internally
 Author-email: Juraj Vijtiuk <juraj.vijtiuk@sartura.hr>, Andrej Gardijan <andrej.gardijan@sartura.hr>
 Maintainer-email: Juraj Vijtiuk <juraj.vijtiuk@sartura.hr>, Andrej Gardijan <andrej.gardijan@sartura.hr>
 License: Copyright (c) 2023 Deutsche Telekom AG.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -12,17 +12,17 @@
         
         2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
         
         3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: Homepage, https://lab.sartura.hr/dt/robotframework-sysrepolibrary
-Project-URL: Bug Reports, https://lab.sartura.hr/dt/robotframework-sysrepolibrary/-/issues
-Project-URL: Source, https://lab.sartura.hr/dt/robotframework-sysrepolibrary
+Project-URL: Homepage, https://github.com/telekom/sysrepo-library-robot-framework
+Project-URL: Bug Reports, https://github.com/telekom/sysrepo-library-robot-framework/issues
+Project-URL: Source, https://github.com/telekom/sysrepo-library-robot-framework
 Keywords: sysrepo,robot,robotframework,networking,linux,testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Robot Framework
@@ -39,14 +39,15 @@
     Sysrepo Robot Framework Library
 </h1>
 
 <p align="center">
     <a href="/../../commits/" title="Last Commit"><img src="https://img.shields.io/github/last-commit/telekom/sysrepo-library-robot-framework?style=flat"></a>
     <a href="/../../issues" title="Open Issues"><img src="https://img.shields.io/github/issues/telekom/sysrepo-library-robot-framework?style=flat"></a>
     <a href="./LICENSE" title="License"><img src="https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat"></a>
+    <a href="https://pypi.org/project/robotframework-sysrepolibrary/" title="PyPi robotframework-sysrepolibrary"><img src="https://img.shields.io/static/v1?label=PyPi&message=robotframework-sysrepolibrary&color=blue&labelColor=yellow"></a>
 </p>
 
 <p align="center">
   <a href="#development">Development</a> •
   <a href="#documentation">Documentation</a> •
   <a href="#support-and-feedback">Support</a> •
   <a href="#how-to-contribute">Contribute</a> •
@@ -69,14 +70,26 @@
 * libyang
 * sysrepo
 * pip
 * setuptools
 * wheel
 * build
 
+#### Installation
+The recommended installation method is using [pip](http://pip-installer.org):
+```
+$ python3 -m pip install robotframework-sysrepolibrary
+```
+
+With recent versions of `pip` it is also possible to install directly from the [GitHub](https://github.com/telekom/sysrepo-library-robot-framework) repository. 
+To install from the latest source from the master branch, use the following command:
+```
+$ python3 -m pip install git+https://github.com/telekom/sysrepo-library-robot-framework.git
+```
+
 #### Build
 
 First clone the repository:
 
 ```
 $ git clone https://github.com/telekom/sysrepo-library-robot-framework
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: robotframework-sysrepolibrary Version: 0.1.0
+Metadata-Version: 2.1 Name: robotframework-sysrepolibrary Version: 0.1.1
 Summary: A testing library for Robot Framework that utilizes the Sysrepo tool
 internally Author-email: Juraj Vijtiuk
 vijtiuk@sartura.hr>, Andrej Gardijan
 gardijan@sartura.hr> Maintainer-email: Juraj Vijtiuk
 vijtiuk@sartura.hr>, Andrej Gardijan
 gardijan@sartura.hr> License: Copyright (c) 2023 Deutsche Telekom AG.
 Redistribution and use in source and binary forms, with or without
@@ -20,71 +20,80 @@
 EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
 INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: Homepage, https://
-lab.sartura.hr/dt/robotframework-sysrepolibrary Project-URL: Bug Reports,
-https://lab.sartura.hr/dt/robotframework-sysrepolibrary/-/issues Project-URL:
-Source, https://lab.sartura.hr/dt/robotframework-sysrepolibrary Keywords:
+github.com/telekom/sysrepo-library-robot-framework Project-URL: Bug Reports,
+https://github.com/telekom/sysrepo-library-robot-framework/issues Project-URL:
+Source, https://github.com/telekom/sysrepo-library-robot-framework Keywords:
 sysrepo,robot,robotframework,networking,linux,testing Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: Operating System :: POSIX :: Linux Classifier:
 Topic :: System :: Networking Requires-Python: >=3.6.0 Description-Content-
 Type: text/markdown Provides-Extra: docs Provides-Extra: tests License-File:
 LICENSE
                  ****** Sysrepo Robot Framework Library ******
    [https://img.shields.io/github/last-commit/telekom/sysrepo-library-robot-
  framework?style=flat] [https://img.shields.io/github/issues/telekom/sysrepo-
   library-robot-framework?style=flat] [https://img.shields.io/badge/License-
-                     BSD%203--Clause-blue.svg?style=flat]
+     BSD%203--Clause-blue.svg?style=flat] [https://img.shields.io/static/
+                     v1?label=PyPi&message=robotframework-
+                 sysrepolibrary&color=blue&labelColor=yellow]
  Development â¢ Documentation â¢ Support â¢ Contribute â¢ Contributors â¢
                                    Licensing
 The goal of this project is to provide a way to use sysrepo with the [Robot
 Framework](https://github.com/robotframework/robotframework). ## About this
 component This repository contains a Robot Framework Python library wrapper
 around the [sysrepo-python](https://github.com/sysrepo/sysrepo-python) sysrepo
 bindings. The [examples](./examples/) directory contains a simple example test
 that connects to sysrepo and does some basic validity checks. ## Development
 The following additional dependencies are required to work on the library: *
-libyang * sysrepo * pip * setuptools * wheel * build #### Build First clone the
-repository: ``` $ git clone https://github.com/telekom/sysrepo-library-robot-
-framework ``` To build the library run the following commands: ``` $ python3 -
-m venv sysrepolibrary-venv $ source sysrepolibrary-venv/bin/activate $ python3
--m pip install --upgrade pip setuptools wheel build ``` To install it: ``` $
-python3 -m pip install . ``` To install the additional dependencies as well
-(generating the documentation and testing): ``` $ python3 -m pip install .
-[docs,tests] ``` ## Code of Conduct This project has adopted the [Contributor
-Covenant](https://www.contributor-covenant.org/) in version 2.0 as our code of
-conduct. Please see the details in our [CODE_OF_CONDUCT.md]
-(CODE_OF_CONDUCT.md). All contributors must abide by the code of conduct. ##
-Working Language We decided to apply _English_ as the primary project language.
-Consequently, all content will be made available primarily in English. We also
-ask all interested people to use English as language to create issues, in their
-code (comments, documentation etc.) and when you send requests to us. The
-application itself and all end-user facing content will be made available in
-other languages as needed. ## Documentation The documentation for the Sysrepo
-Robot Framework Library can be generated using the [Sphinx](https://www.sphinx-
-doc.org/en/master/) documentation generator tool. The documentation sources are
-located in [docs/source](./docs/source) To build the documentation as `HTML`
-files run while in the root directory: ``` $ sphinx-build -b html docs/source
-docs/build/html ``` The `-b` option selects a builder in this example it's
-`HTML`. To quickly generate the docs use the scripts in the `docs/` directory.
-Execute `make` without an argument while in the directory to see which targets
-are available. Example for `HTML`: ``` docs/$ make html ``` ## Support and
-Feedback The following channels are available for discussions, feedback, and
-support requests: | Type | Channel | | ------------------ | -------------------
+libyang * sysrepo * pip * setuptools * wheel * build #### Installation The
+recommended installation method is using [pip](http://pip-installer.org): ``` $
+python3 -m pip install robotframework-sysrepolibrary ``` With recent versions
+of `pip` it is also possible to install directly from the [GitHub](https://
+github.com/telekom/sysrepo-library-robot-framework) repository. To install from
+the latest source from the master branch, use the following command: ``` $
+python3 -m pip install git+https://github.com/telekom/sysrepo-library-robot-
+framework.git ``` #### Build First clone the repository: ``` $ git clone https:
+//github.com/telekom/sysrepo-library-robot-framework ``` To build the library
+run the following commands: ``` $ python3 -m venv sysrepolibrary-venv $ source
+sysrepolibrary-venv/bin/activate $ python3 -m pip install --upgrade pip
+setuptools wheel build ``` To install it: ``` $ python3 -m pip install . ``` To
+install the additional dependencies as well (generating the documentation and
+testing): ``` $ python3 -m pip install .[docs,tests] ``` ## Code of Conduct
+This project has adopted the [Contributor Covenant](https://www.contributor-
+covenant.org/) in version 2.0 as our code of conduct. Please see the details in
+our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). All contributors must abide by
+the code of conduct. ## Working Language We decided to apply _English_ as the
+primary project language. Consequently, all content will be made available
+primarily in English. We also ask all interested people to use English as
+language to create issues, in their code (comments, documentation etc.) and
+when you send requests to us. The application itself and all end-user facing
+content will be made available in other languages as needed. ## Documentation
+The documentation for the Sysrepo Robot Framework Library can be generated
+using the [Sphinx](https://www.sphinx-doc.org/en/master/) documentation
+generator tool. The documentation sources are located in [docs/source](./docs/
+source) To build the documentation as `HTML` files run while in the root
+directory: ``` $ sphinx-build -b html docs/source docs/build/html ``` The `-b`
+option selects a builder in this example it's `HTML`. To quickly generate the
+docs use the scripts in the `docs/` directory. Execute `make` without an
+argument while in the directory to see which targets are available. Example for
+`HTML`: ``` docs/$ make html ``` ## Support and Feedback The following channels
+are available for discussions, feedback, and support requests: | Type | Channel
+| | ------------------ | ------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
------------------ | | **Issues** | [https://img.shields.io/github/issues/
-telekom/sysrepo-library-robot-framework?style=flat-square]
+------------------------------------------------------------- | | **Issues** |
+[https://img.shields.io/github/issues/telekom/sysrepo-library-robot-
+framework?style=flat-square]
  | | **Other Requests** | [https://img.shields.io/badge/email-
 Open%20Source%20Team-green?logo=mail.ru&style=flat-square&logoColor=white] | ##
 How to Contribute Contribution and feedback is encouraged and always welcome.
 For more information about how to contribute, the project structure, as well as
 additional contribution information, see our [Contribution Guidelines](./
 CONTRIBUTING.md). By participating in this project, you agree to abide by its
 [Code of Conduct](./CODE_OF_CONDUCT.md) at all times. ## Contributors Our
```

### Comparing `robotframework-sysrepolibrary-0.1.0/src/robotframework_sysrepolibrary.egg-info/SOURCES.txt` & `robotframework-sysrepolibrary-0.1.1/src/robotframework_sysrepolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*


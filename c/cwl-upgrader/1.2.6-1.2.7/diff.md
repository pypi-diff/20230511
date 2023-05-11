# Comparing `tmp/cwl-upgrader-1.2.6.tar.gz` & `tmp/cwl-upgrader-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwl-upgrader-1.2.6.tar", last modified: Tue May  2 08:30:33 2023, max compression
+gzip compressed data, was "cwl-upgrader-1.2.7.tar", last modified: Thu May 11 11:23:32 2023, max compression
```

## Comparing `cwl-upgrader-1.2.6.tar` & `cwl-upgrader-1.2.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       91 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     6361 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      992 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.911933 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-02 08:30:33.000000 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1086 2023-05-02 08:30:33.000000 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 08:30:33.000000 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       56 2023-05-02 08:30:33.000000 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-02 08:30:33.000000 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       12 2023-05-02 08:30:33.000000 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 08:30:30.000000 cwl-upgrader-1.2.6/cwl_upgrader.egg-info/zip-safe
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.911933 cwl-upgrader-1.2.6/cwlupgrader/
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/cwlupgrader/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    34460 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/cwlupgrader/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/cwlupgrader/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2305 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.911933 cwl-upgrader-1.2.6/testdata/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/testdata/draft-3/
--rw-r--r--   0 michael   (1000) michael   (1000)    11102 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/draft-3/attributor-prok-cheetah.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      625 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/draft-3/wf.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/testdata/v1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)      433 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/1st-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      385 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/arguments.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8843 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/attributor-prok-cheetah.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1157 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/conflict-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      312 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/listing_deep1-arr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      307 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/tar-param.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      489 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.0/wf.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/testdata/v1.1/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1425 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.1/conflict-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      425 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.1/listing_deep1-arr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.1/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.1/networkaccess.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/testdata/v1.2/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.2/1st-workflow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      495 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.2/arguments.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.2/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.2/networkaccess.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      443 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/testdata/v1.2/tar-param.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:33.915933 cwl-upgrader-1.2.6/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4215 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/tests/test_complete.py
--rw-r--r--   0 michael   (1000) michael   (1000)      537 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/tests/test_output_dir.py
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-02 08:30:27.000000 cwl-upgrader-1.2.6/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       91 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     6361 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      992 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1086 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       56 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       12 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 11:23:29.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/zip-safe
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/cwlupgrader/
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/cwlupgrader/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    34460 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/cwlupgrader/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/cwlupgrader/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2305 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/testdata/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/testdata/draft-3/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11102 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/draft-3/attributor-prok-cheetah.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      625 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/draft-3/wf.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/testdata/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      433 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/1st-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      385 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/arguments.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8843 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/attributor-prok-cheetah.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1157 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/conflict-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      312 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/listing_deep1-arr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      307 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/tar-param.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      489 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/wf.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/testdata/v1.1/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1425 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/conflict-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      425 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/listing_deep1-arr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/networkaccess.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/testdata/v1.2/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/1st-workflow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      495 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/arguments.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/networkaccess.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      443 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/tar-param.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4202 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/test_complete.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      537 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/test_output_dir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/util.py
```

### Comparing `cwl-upgrader-1.2.6/LICENSE.txt` & `cwl-upgrader-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/Makefile` & `cwl-upgrader-1.2.7/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # `[[` conditional expressions.
 PYSOURCES=$(wildcard cwlupgrader/**.py tests/*.py) setup.py
 DEVPKGS=diff_cover black pylint pep257 pydocstyle flake8 tox tox-pyenv \
 	isort wheel autoflake flake8-bugbear pyupgrade bandit \
 	-rtest-requirements.txt -rmypy-requirements.txt
 DEBDEVPKGS=pylint python3-coverage sloccount \
 	   python3-flake8 shellcheck
-VERSION=1.2.6  # please also update setup.py
+VERSION=1.2.7  # please also update setup.py
 
 ## all                    : default task (install cwl-upgrader in dev mode)
 all: dev
 
 ## help                   : print this help message and exit
 help: Makefile
 	@sed -n 's/^##//p' $<
```

### Comparing `cwl-upgrader-1.2.6/PKG-INFO` & `cwl-upgrader-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cwl-upgrader
-Version: 1.2.6
+Version: 1.2.7
 Summary: Common Workflow Language standalone document upgrader
 Home-page: https://github.com/common-workflow-language/cwl-upgrader
 Author: Common Workflow Language contributors
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Download-URL: https://github.com/common-workflow-language/cwl-upgrader
 Description: =====================================================
```

### Comparing `cwl-upgrader-1.2.6/README.rst` & `cwl-upgrader-1.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/cwl_upgrader.egg-info/PKG-INFO` & `cwl-upgrader-1.2.7/cwl_upgrader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cwl-upgrader
-Version: 1.2.6
+Version: 1.2.7
 Summary: Common Workflow Language standalone document upgrader
 Home-page: https://github.com/common-workflow-language/cwl-upgrader
 Author: Common Workflow Language contributors
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Download-URL: https://github.com/common-workflow-language/cwl-upgrader
 Description: =====================================================
```

### Comparing `cwl-upgrader-1.2.6/cwl_upgrader.egg-info/SOURCES.txt` & `cwl-upgrader-1.2.7/cwl_upgrader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/cwlupgrader/main.py` & `cwl-upgrader-1.2.7/cwlupgrader/main.py`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/setup.py` & `cwl-upgrader-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 README = os.path.join(SETUP_DIR, "README.rst")
 
 NEEDS_PYTEST = {"pytest", "test", "ptr"}.intersection(sys.argv)
 PYTEST_RUNNER = ["pytest-runner", "pytest-cov"] if NEEDS_PYTEST else []
 
 setup(
     name="cwl-upgrader",
-    version="1.2.6",
+    version="1.2.7",
     description="Common Workflow Language standalone document upgrader",
     long_description=open(README).read(),
     author="Common Workflow Language contributors",
     author_email="common-workflow-language@googlegroups.com",
     url="https://github.com/common-workflow-language/cwl-upgrader",
     download_url="https://github.com/common-workflow-language/cwl-upgrader",
     license="Apache 2.0",
     packages=["cwlupgrader", "cwlupgrader.tests"],
     include_package_data=True,
     package_dir={"cwlupgrader.tests": "tests"},
     package_data={"cwlupgrader.tests": ["../testdata/**/*.cwl"]},
     install_requires=[
         "setuptools",
-        "ruamel.yaml >= 0.16.0, < 0.17.23;python_version>='3.10'",
-        "ruamel.yaml >= 0.15.98, < 0.17.23;python_version>='3.9'",
-        "ruamel.yaml >= 0.15.78, < 0.17.23;python_version>='3.8'",
-        "ruamel.yaml >= 0.15.71, < 0.17.23",
+        "ruamel.yaml >= 0.16.0, < 0.17.27;python_version>='3.10'",
+        "ruamel.yaml >= 0.15.98, < 0.17.27;python_version>='3.9'",
+        "ruamel.yaml >= 0.15.78, < 0.17.27;python_version>='3.8'",
+        "ruamel.yaml >= 0.15.71, < 0.17.27",
         "schema_salad",
     ],
     entry_points={"console_scripts": ["cwl-upgrader = cwlupgrader.main:main"]},
     python_requires=">=3.6, <4",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
```

### Comparing `cwl-upgrader-1.2.6/testdata/draft-3/attributor-prok-cheetah.cwl` & `cwl-upgrader-1.2.7/testdata/draft-3/attributor-prok-cheetah.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/testdata/draft-3/wf.cwl` & `cwl-upgrader-1.2.7/testdata/draft-3/wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/testdata/v1.0/attributor-prok-cheetah.cwl` & `cwl-upgrader-1.2.7/testdata/v1.0/attributor-prok-cheetah.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/testdata/v1.0/conflict-wf.cwl` & `cwl-upgrader-1.2.7/testdata/v1.0/conflict-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/testdata/v1.1/conflict-wf.cwl` & `cwl-upgrader-1.2.7/testdata/v1.1/conflict-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/tests/test_complete.py` & `cwl-upgrader-1.2.7/tests/test_complete.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,19 +96,18 @@
     )
     assert filecmp.cmp(
         get_data("testdata/v1.1/conflict-wf.cwl"),
         tmp_path / "conflict-wf.cwl",
         shallow=False,
     )
 
+
 def test_multi_version_upgrade_external_steps(tmp_path: Path) -> None:
     """Test 1.0 to 1.2 upgrade of Workflow with external steps."""
-    main(
-        [f"--dir={tmp_path}", get_data("testdata/v1.0/1st-workflow.cwl")]
-    )
+    main([f"--dir={tmp_path}", get_data("testdata/v1.0/1st-workflow.cwl")])
     assert filecmp.cmp(
         get_data("testdata/v1.2/arguments.cwl"),
         tmp_path / "arguments.cwl",
         shallow=False,
     )
     assert filecmp.cmp(
         get_data("testdata/v1.2/tar-param.cwl"),
```

### Comparing `cwl-upgrader-1.2.6/tests/test_output_dir.py` & `cwl-upgrader-1.2.7/tests/test_output_dir.py`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.6/tests/util.py` & `cwl-upgrader-1.2.7/tests/util.py`

 * *Files identical despite different names*


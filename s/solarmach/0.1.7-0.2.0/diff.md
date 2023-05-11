# Comparing `tmp/solarmach-0.1.7.tar.gz` & `tmp/solarmach-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarmach-0.1.7.tar", last modified: Thu Apr 27 13:55:43 2023, max compression
+gzip compressed data, was "solarmach-0.2.0.tar", last modified: Thu May 11 14:29:48 2023, max compression
```

## Comparing `solarmach-0.1.7.tar` & `solarmach-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.048822 solarmach-0.1.7/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.1.7/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.1.7/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-04-27 13:55:43.048822 solarmach-0.1.7/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5268 2023-04-27 13:45:25.000000 solarmach-0.1.7/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.1.7/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.040822 solarmach-0.1.7/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.1.7/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.1.7/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.1.7/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.1.7/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.1.7/examples/example.ipynb
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.1.7/examples/solarmach.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.1.7/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.1.7/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.1.7/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       61 2022-07-06 11:55:56.000000 solarmach-0.1.7/requirements.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2077 2023-04-27 13:55:43.048822 solarmach-0.1.7/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.1.7/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/solarmach/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    30813 2023-04-27 13:35:33.000000 solarmach-0.1.7/solarmach/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/solarmach/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.1.7/solarmach/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.1.7/solarmach/tests/test.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-27 13:55:43.044823 solarmach-0.1.7/solarmach.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      556 2023-04-27 13:55:43.000000 solarmach-0.1.7/solarmach.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.1.7/solarmach.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      147 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-04-27 13:55:42.000000 solarmach-0.1.7/solarmach.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.1.7/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.0/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.2.0/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-11 14:29:48.427020 solarmach-0.2.0/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5268 2023-04-27 13:45:25.000000 solarmach-0.2.0/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.2.0/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.415020 solarmach-0.2.0/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.2.0/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.2.0/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.2.0/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.2.0/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.423020 solarmach-0.2.0/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.2.0/examples/example.ipynb
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.2.0/examples/solarmach.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.0/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.2.0/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.2.0/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       84 2023-05-11 14:24:48.000000 solarmach-0.2.0/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2103 2023-05-11 14:29:48.431020 solarmach-0.2.0/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.2.0/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/solarmach/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    51602 2023-05-11 14:20:54.000000 solarmach-0.2.0/solarmach/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    23221 2023-05-11 14:20:54.000000 solarmach-0.2.0/solarmach/pfss_utilities.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/solarmach/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.2.0/solarmach/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.2.0/solarmach/tests/test.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/solarmach.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      584 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.2.0/solarmach.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      169 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.2.0/tox.ini
```

### Comparing `solarmach-0.1.7/LICENSE.rst` & `solarmach-0.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/PKG-INFO` & `solarmach-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.1.7
+Version: 0.2.0
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solarmach-0.1.7/README.rst` & `solarmach-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/code_of_conduct.md` & `solarmach-0.2.0/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/docs/Makefile` & `solarmach-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/docs/conf.py` & `solarmach-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/docs/make.bat` & `solarmach-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/examples/example.ipynb` & `solarmach-0.2.0/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/examples/solarmach.png` & `solarmach-0.2.0/examples/solarmach.png`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/licenses/LICENSE.rst` & `solarmach-0.2.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/licenses/TEMPLATE_LICENSE.rst` & `solarmach-0.2.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/setup.cfg` & `solarmach-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -24,20 +24,24 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
 	astroquery
+	drms
 	Jinja2
+	lxml
 	matplotlib
 	numpy
 	pandas
+	pfsspy
 	scipy
 	sunpy
+	zeep
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
```

### Comparing `solarmach-0.1.7/setup.py` & `solarmach-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/solarmach/tests/test.py` & `solarmach-0.2.0/solarmach/tests/test.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.1.7/solarmach.egg-info/PKG-INFO` & `solarmach-0.2.0/solarmach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.1.7
+Version: 0.2.0
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solarmach-0.1.7/solarmach.egg-info/SOURCES.txt` & `solarmach-0.2.0/solarmach.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/index.rst
 docs/make.bat
 examples/example.ipynb
 examples/solarmach.png
 licenses/LICENSE.rst
 licenses/TEMPLATE_LICENSE.rst
 solarmach/__init__.py
+solarmach/pfss_utilities.py
 solarmach/version.py
 solarmach.egg-info/PKG-INFO
 solarmach.egg-info/SOURCES.txt
 solarmach.egg-info/dependency_links.txt
 solarmach.egg-info/not-zip-safe
 solarmach.egg-info/requires.txt
 solarmach.egg-info/top_level.txt
```

### Comparing `solarmach-0.1.7/tox.ini` & `solarmach-0.2.0/tox.ini`

 * *Files identical despite different names*


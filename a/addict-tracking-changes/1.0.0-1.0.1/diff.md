# Comparing `tmp/addict-tracking-changes-1.0.0.tar.gz` & `tmp/addict-tracking-changes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addict-tracking-changes-1.0.0.tar", last modified: Thu May 11 10:04:20 2023, max compression
+gzip compressed data, was "addict-tracking-changes-1.0.1.tar", last modified: Thu May 11 12:42:30 2023, max compression
```

## Comparing `addict-tracking-changes-1.0.0.tar` & `addict-tracking-changes-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      141 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/.flake8
--rw-r--r--   0        0        0     1886 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2022-11-29 03:20:21.000000 addict-tracking-changes-1.0.0/LICENSE
--rw-r--r--   0        0        0      325 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/Pipfile
--rw-r--r--   0        0        0    41152 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/Pipfile.lock
--rw-r--r--   0        0        0     5078 2023-05-11 09:44:16.809627 addict-tracking-changes-1.0.0/README.md
--rw-r--r--   0        0        0     1146 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/badge_coverage.svg
--rw-r--r--   0        0        0     1177 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/badge_flake8.svg
--rw-r--r--   0        0        0     1115 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/badge_tests.svg
--rw-r--r--   0        0        0      634 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     5873 2023-05-11 09:44:16.839627 addict-tracking-changes-1.0.0/docs/addict.rst
--rw-r--r--   0        0        0     1950 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      503 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/make.bat
--rw-r--r--   0        0        0     1116 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/usage.rst
--rw-r--r--   0        0        0      408 2023-05-11 09:44:16.789627 addict-tracking-changes-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0     3544 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/noxfile.py
--rw-r--r--   0        0        0      723 2023-05-11 09:44:16.799627 addict-tracking-changes-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2245 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/back.svg
--rw-r--r--   0        0        0     2666 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/file.svg
--rw-r--r--   0        0        0     7400 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/flake8stats.txt
--rw-r--r--   0        0        0     1109 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/index.html
--rw-r--r--   0        0        0     3669 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.__init__.report.html
--rw-r--r--   0        0        0     8223 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.__init__.source.html
--rw-r--r--   0        0        0     2999 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.addict.report.html
--rw-r--r--   0        0        0    89377 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.addict.source.html
--rw-r--r--   0        0        0     7273 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/styles.css
--rw-r--r--   0        0        0     4565 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/junit/junit.xml
--rw-r--r--   0        0        0     1471 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.0/src/addict_tracking_changes/__init__.py
--rw-r--r--   0        0        0    13290 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.0/src/addict_tracking_changes/addict.py
--rw-r--r--   0        0        0     1115 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/tests-badge.svg
--rw-r--r--   0        0        0    14497 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.0/tests/addict_test.py
--rw-r--r--   0        0        0     5580 1970-01-01 00:00:00.000000 addict-tracking-changes-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.1/.flake8
+-rw-r--r--   0        0        0     1886 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1070 2022-11-29 03:20:21.000000 addict-tracking-changes-1.0.1/LICENSE
+-rw-r--r--   0        0        0      325 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.1/Pipfile
+-rw-r--r--   0        0        0    41152 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.1/Pipfile.lock
+-rw-r--r--   0        0        0     5078 2023-05-11 09:44:16.809627 addict-tracking-changes-1.0.1/README.md
+-rw-r--r--   0        0        0     1146 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.1/badge_coverage.svg
+-rw-r--r--   0        0        0     1177 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.1/badge_flake8.svg
+-rw-r--r--   0        0        0     1115 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.1/badge_tests.svg
+-rw-r--r--   0        0        0      634 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0     5873 2023-05-11 09:44:16.839627 addict-tracking-changes-1.0.1/docs/addict.rst
+-rw-r--r--   0        0        0     1950 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0      503 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     1116 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.1/docs/usage.rst
+-rw-r--r--   0        0        0      408 2023-05-11 09:44:16.789627 addict-tracking-changes-1.0.1/mkdocs.yml
+-rw-r--r--   0        0        0     3544 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.1/noxfile.py
+-rw-r--r--   0        0        0      795 2023-05-11 12:39:05.765919 addict-tracking-changes-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2245 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/back.svg
+-rw-r--r--   0        0        0     2666 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/file.svg
+-rw-r--r--   0        0        0     7400 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/flake8stats.txt
+-rw-r--r--   0        0        0     1109 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/index.html
+-rw-r--r--   0        0        0     3669 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.__init__.report.html
+-rw-r--r--   0        0        0     8223 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.__init__.source.html
+-rw-r--r--   0        0        0     2999 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.addict.report.html
+-rw-r--r--   0        0        0    89377 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.addict.source.html
+-rw-r--r--   0        0        0     7273 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/flake8/styles.css
+-rw-r--r--   0        0        0     4565 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/reports/junit/junit.xml
+-rw-r--r--   0        0        0     1471 2023-05-11 12:41:51.084309 addict-tracking-changes-1.0.1/src/addict_tracking_changes/__init__.py
+-rw-r--r--   0        0        0    13290 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.1/src/addict_tracking_changes/addict.py
+-rw-r--r--   0        0        0     1115 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.1/tests-badge.svg
+-rw-r--r--   0        0        0    14497 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.1/tests/addict_test.py
+-rw-r--r--   0        0        0     5603 1970-01-01 00:00:00.000000 addict-tracking-changes-1.0.1/PKG-INFO
```

### Comparing `addict-tracking-changes-1.0.0/.gitignore` & `addict-tracking-changes-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/LICENSE` & `addict-tracking-changes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/Pipfile.lock` & `addict-tracking-changes-1.0.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/README.md` & `addict-tracking-changes-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/badge_coverage.svg` & `addict-tracking-changes-1.0.1/badge_coverage.svg`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/badge_flake8.svg` & `addict-tracking-changes-1.0.1/badge_flake8.svg`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/badge_tests.svg` & `addict-tracking-changes-1.0.1/badge_tests.svg`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/docs/Makefile` & `addict-tracking-changes-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/docs/addict.rst` & `addict-tracking-changes-1.0.1/docs/addict.rst`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/docs/conf.py` & `addict-tracking-changes-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/docs/make.bat` & `addict-tracking-changes-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/docs/usage.rst` & `addict-tracking-changes-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/noxfile.py` & `addict-tracking-changes-1.0.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/back.svg` & `addict-tracking-changes-1.0.1/reports/flake8/back.svg`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/file.svg` & `addict-tracking-changes-1.0.1/reports/flake8/file.svg`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/flake8stats.txt` & `addict-tracking-changes-1.0.1/reports/flake8/flake8stats.txt`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/index.html` & `addict-tracking-changes-1.0.1/reports/flake8/index.html`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.__init__.report.html` & `addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.__init__.report.html`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.__init__.source.html` & `addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.__init__.source.html`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.addict.report.html` & `addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.addict.report.html`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.addict.source.html` & `addict-tracking-changes-1.0.1/reports/flake8/src.addict_tracking_changes.addict.source.html`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/flake8/styles.css` & `addict-tracking-changes-1.0.1/reports/flake8/styles.css`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/reports/junit/junit.xml` & `addict-tracking-changes-1.0.1/reports/junit/junit.xml`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/src/addict_tracking_changes/__init__.py` & `addict-tracking-changes-1.0.1/src/addict_tracking_changes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 """
 
 from .addict import Dict
 from .addict import Dict as Addict
 from .addict import walker
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `addict-tracking-changes-1.0.0/src/addict_tracking_changes/addict.py` & `addict-tracking-changes-1.0.1/src/addict_tracking_changes/addict.py`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/tests-badge.svg` & `addict-tracking-changes-1.0.1/tests-badge.svg`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/tests/addict_test.py` & `addict-tracking-changes-1.0.1/tests/addict_test.py`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-1.0.0/PKG-INFO` & `addict-tracking-changes-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: addict-tracking-changes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Addict dictionary enhanced with ability to track changes -- currently only supports field additions
 Maintainer-email: Kabira K <kabira@monallabs.in>
+Requires-Python: >3.11
 Description-Content-Type: text/markdown
 Project-URL: Documentation, https://ofjustpy.github.io/addict-tracking-changes/
 Project-URL: Home, https://webworks.monallabs.in/ofjustpy/addict-tracking-changes
 Project-URL: Source, https://github.com/ofjustpy/addict-tracking-changes
 
 # [addict-tracking-changes](https://github.com/Monallabs-org/addict-tracking-changes)
```


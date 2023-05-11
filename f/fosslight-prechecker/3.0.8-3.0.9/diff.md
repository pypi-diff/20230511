# Comparing `tmp/fosslight_prechecker-3.0.8.tar.gz` & `tmp/fosslight_prechecker-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fosslight_prechecker-3.0.8.tar", last modified: Wed Oct 12 12:09:27 2022, max compression
+gzip compressed data, was "dist/fosslight_prechecker-3.0.9.tar", last modified: Wed Oct 19 05:30:19 2022, max compression
```

## Comparing `fosslight_prechecker-3.0.8.tar` & `fosslight_prechecker-3.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      119 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2953 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2012 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       78 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1603 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_oss_pkg/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_oss_pkg/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2857 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_oss_pkg/_convert.py
--rw-r--r--   0 runner    (1001) docker     (116)     2648 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_oss_pkg/_parsing_excel.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/
--rwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16683 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/_add.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3472 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/_constant.py
--rw-r--r--   0 runner    (1001) docker     (116)     1659 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    11239 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/_precheck.py
--rw-r--r--   0 runner    (1001) docker     (116)    14152 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/_result.py
--rw-r--r--   0 runner    (1001) docker     (116)     5030 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/_result_html.py
--rw-r--r--   0 runner    (1001) docker     (116)     2335 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/resources/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2022-10-12 12:09:19.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker/resources/convert_license.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2953 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      798 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      120 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       78 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2022-10-12 12:09:27.000000 fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      119 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2953 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2012 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       78 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1603 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_oss_pkg/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_oss_pkg/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2857 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_oss_pkg/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2648 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_oss_pkg/_parsing_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/
+-rwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16683 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/_add.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3472 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1659 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    11239 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/_precheck.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14152 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/_result.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5030 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/_result_html.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2346 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/resources/
+-rw-r--r--   0 runner    (1001) docker     (116)      605 2022-10-19 05:30:03.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker/resources/convert_license.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2953 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      798 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      120 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       78 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2022-10-19 05:30:19.000000 fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/top_level.txt
```

### Comparing `fosslight_prechecker-3.0.8/LICENSE` & `fosslight_prechecker-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/PKG-INFO` & `fosslight_prechecker-3.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_prechecker
-Version: 3.0.8
+Version: 3.0.9
 Summary: FOSSLight Prechecker
 Home-page: https://github.com/fosslight/fosslight_prechecker
 Author: LG Electronics
 License: GPL-3.0-only
 Download-URL: https://github.com/fosslight/fosslight_prechecker
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_prechecker-3.0.8/README.md` & `fosslight_prechecker-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/setup.py` & `fosslight_prechecker-3.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_prechecker',
-        version='3.0.8',
+        version='3.0.9',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Prechecker',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='GPL-3.0-only',
         author='LG Electronics',
```

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_oss_pkg/_convert.py` & `fosslight_prechecker-3.0.9/src/fosslight_oss_pkg/_convert.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_oss_pkg/_parsing_excel.py` & `fosslight_prechecker-3.0.9/src/fosslight_oss_pkg/_parsing_excel.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/_add.py` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/_add.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/_constant.py` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/_constant.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/_help.py` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/_precheck.py` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/_precheck.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/_result.py` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/_result.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/_result_html.py` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/_result_html.py`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/cli.py` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fosslight_prechecker._precheck import run_lint, PKG_NAME
 from fosslight_oss_pkg._convert import convert_report
 from fosslight_prechecker._add import add_content
 
 
 def main():
     parser = argparse.ArgumentParser(description='FOSSLight Prechecker', prog='fosslight_prechecker', add_help=False)
-    parser.add_argument('mode', help='lint | convert | add', choices=['lint', 'add', 'convert'])
+    parser.add_argument('mode', nargs='?', help='lint | convert | add', choices=['lint', 'add', 'convert'])
     parser.add_argument('-h', '--help', help='Print help message', action='store_true', dest='help')
     parser.add_argument('-i', '--ignore', help='Do not write log to file', action='store_false', dest='log')
     parser.add_argument('-v', '--version', help='Print FOSSLight Prechecker version', action='store_true', dest='version')
     parser.add_argument('-n', '--no', help='Disable automatic exclude mode', action='store_true', dest='disable')
     parser.add_argument('-p', '--path', help='Path to check', type=str, dest='path', default="")
     parser.add_argument('-f', '--format', help='Format of ouput', type=str, dest='format', default="")
     parser.add_argument('-o', '--output', help='Output file name', type=str, dest='output', default="")
```

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker/resources/convert_license.json` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker/resources/convert_license.json`

 * *Files identical despite different names*

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/PKG-INFO` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-prechecker
-Version: 3.0.8
+Version: 3.0.9
 Summary: FOSSLight Prechecker
 Home-page: https://github.com/fosslight/fosslight_prechecker
 Author: LG Electronics
 License: GPL-3.0-only
 Download-URL: https://github.com/fosslight/fosslight_prechecker
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_prechecker-3.0.8/src/fosslight_prechecker.egg-info/SOURCES.txt` & `fosslight_prechecker-3.0.9/src/fosslight_prechecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


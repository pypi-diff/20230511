# Comparing `tmp/sphinx-pdj-theme-0.3.0.tar.gz` & `tmp/sphinx-pdj-theme-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-pdj-theme-0.3.0.tar", last modified: Sun May  7 17:12:25 2023, max compression
+gzip compressed data, was "sphinx-pdj-theme-0.3.1.tar", last modified: Wed May 10 06:43:57 2023, max compression
```

## Comparing `sphinx-pdj-theme-0.3.0.tar` & `sphinx-pdj-theme-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/
--rw-rw-r--   0 juca      (1001) juca      (1001)     1079 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/LICENSE
--rw-rw-r--   0 juca      (1001) juca      (1001)       75 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/MANIFEST.in
--rw-rw-r--   0 juca      (1001) juca      (1001)     1122 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/PKG-INFO
--rw-rw-r--   0 juca      (1001) juca      (1001)      640 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/README.md
--rw-rw-r--   0 juca      (1001) juca      (1001)      435 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/README.rst
--rw-rw-r--   0 juca      (1001) juca      (1001)      672 2023-05-07 17:11:51.000000 sphinx-pdj-theme-0.3.0/pyproject.toml
--rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/setup.cfg
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/
--rw-rw-r--   0 juca      (1001) juca      (1001)      242 2023-05-07 17:08:32.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__init__.py
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/
--rw-rw-r--   0 juca      (1001) juca      (1001)      837 2023-05-07 05:57:19.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/__init__.cpython-311.pyc
--rwxrwxrwx   0 juca      (1001) juca      (1001)      534 2020-06-27 23:51:54.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 juca      (1001) juca      (1001)     1035 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/breadcrumbs.html
--rw-rw-r--   0 juca      (1001) juca      (1001)     1328 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/footer.html
--rw-rw-r--   0 juca      (1001) juca      (1001)     7198 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout.html
--rw-rw-r--   0 juca      (1001) juca      (1001)     7341 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout_old.html
--rw-rw-r--   0 juca      (1001) juca      (1001)     1614 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/search.html
--rw-rw-r--   0 juca      (1001) juca      (1001)      354 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/searchbox.html
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.931728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/
--rw-rw-r--   0 juca      (1001) juca      (1001)     3403 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/badge_only.css
--rw-rw-r--   0 juca      (1001) juca      (1001)     5164 2023-05-07 16:27:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/darker.css
--rw-rw-r--   0 juca      (1001) juca      (1001)    19589 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/img.css
--rw-rw-r--   0 juca      (1001) juca      (1001)    10251 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/pdj.css
--rw-rw-r--   0 juca      (1001) juca      (1001)    90920 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/theme.css
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/
--rw-rw-r--   0 juca      (1001) juca      (1001)    38205 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 juca      (1001) juca      (1001)   202148 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 juca      (1001) juca      (1001)    80652 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 juca      (1001) juca      (1001)    44432 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/
--rw-rw-r--   0 juca      (1001) juca      (1001)     3260 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/moon.svg
--rw-rw-r--   0 juca      (1001) juca      (1001)     1127 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/porao-branco.png
--rw-rw-r--   0 juca      (1001) juca      (1001)    18468 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/sun.svg
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/
--rw-rw-r--   0 juca      (1001) juca      (1001)      351 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/pdj.js
--rw-rw-r--   0 juca      (1001) juca      (1001)     1675 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/theme.js
--rw-rw-r--   0 juca      (1001) juca      (1001)      138 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/theme.conf
--rw-rw-r--   0 juca      (1001) juca      (1001)     1219 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/versions.html
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/
--rwxrwxrwx   0 juca      (1001) juca      (1001)     1122 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/PKG-INFO
--rwxrwxrwx   0 juca      (1001) juca      (1001)     1236 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/SOURCES.txt
--rwxrwxrwx   0 juca      (1001) juca      (1001)        1 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 juca      (1001) juca      (1001)       57 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/entry_points.txt
--rwxrwxrwx   0 juca      (1001) juca      (1001)       17 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/top_level.txt
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.838680 sphinx-pdj-theme-0.3.1/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1079 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/LICENSE
+-rw-rw-r--   0 juca      (1001) juca      (1001)       75 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/MANIFEST.in
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1122 2023-05-10 06:43:57.838680 sphinx-pdj-theme-0.3.1/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      640 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.1/README.md
+-rw-rw-r--   0 juca      (1001) juca      (1001)      435 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/README.rst
+-rw-rw-r--   0 juca      (1001) juca      (1001)      672 2023-05-10 06:42:56.000000 sphinx-pdj-theme-0.3.1/pyproject.toml
+-rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-05-10 06:43:57.838680 sphinx-pdj-theme-0.3.1/setup.cfg
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.834680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      242 2023-05-07 17:08:32.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/__init__.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.834680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/__pycache__/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      818 2023-05-07 17:34:00.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/__pycache__/__init__.cpython-311.pyc
+-rwxrwxrwx   0 juca      (1001) juca      (1001)      534 2020-06-27 23:51:54.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1035 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/breadcrumbs.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1328 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/footer.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     7182 2023-05-10 06:42:24.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/layout.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     7341 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/layout_old.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1614 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/search.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)      354 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/searchbox.html
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.830680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.838680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     3403 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/badge_only.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)     5164 2023-05-07 16:27:25.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/darker.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    19589 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/img.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    10251 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/pdj.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    90920 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/theme.css
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.838680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/
+-rw-rw-r--   0 juca      (1001) juca      (1001)    38205 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 juca      (1001) juca      (1001)   202148 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 juca      (1001) juca      (1001)    80652 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 juca      (1001) juca      (1001)    44432 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.838680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/img/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     3260 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/img/moon.svg
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1127 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/img/porao-branco.png
+-rw-rw-r--   0 juca      (1001) juca      (1001)    18468 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/img/sun.svg
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.838680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/js/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      351 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/js/pdj.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1675 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/js/theme.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)      138 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/theme.conf
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1219 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/versions.html
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-10 06:43:57.834680 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/
+-rwxrwxrwx   0 juca      (1001) juca      (1001)     1122 2023-05-10 06:43:57.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/PKG-INFO
+-rwxrwxrwx   0 juca      (1001) juca      (1001)     1236 2023-05-10 06:43:57.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/SOURCES.txt
+-rwxrwxrwx   0 juca      (1001) juca      (1001)        1 2023-05-10 06:43:57.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/dependency_links.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       57 2023-05-10 06:43:57.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/entry_points.txt
+-rwxrwxrwx   0 juca      (1001) juca      (1001)       17 2023-05-10 06:43:57.000000 sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/top_level.txt
```

### Comparing `sphinx-pdj-theme-0.3.0/LICENSE` & `sphinx-pdj-theme-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/PKG-INFO` & `sphinx-pdj-theme-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-pdj-theme
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cool theme for sphinx documentation
 Author: Juca Crispim
 Project-URL: Homepage, https://github.com/jucacrispim/sphinx_pdj_theme/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `sphinx-pdj-theme-0.3.0/README.md` & `sphinx-pdj-theme-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/pyproject.toml` & `sphinx-pdj-theme-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sphinx-pdj-theme"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Juca Crispim" },
 ]
 description = "A cool theme for sphinx documentation"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/__init__.cpython-311.pyc` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/__pycache__/__init__.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,91 +1,85 @@
 magic:    0xa70d0d0a
-moddate:  0x473b5764 (Sun May  7 05:46:47 2023 UTC)
-files sz: 261
+moddate:  0x10db5764 (Sun May  7 17:08:32 2023 UTC)
+files sz: 242
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
-   code
-      0x9700640064016c005a0064025a01640384005a02640484005a03640153
-      00
+   code 0x9700640064016c005a00640284005a01640384005a0264015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
-     3          10 LOAD_CONST               2 ('0.2.1')
-                12 STORE_NAME               1 (VERSION)
+     4          10 LOAD_CONST               2 (<code object get_html_theme_path, file "/home/juca/mysrc/sphinx_pdj_theme/sphinx_pdj_theme/__init__.py", line 4>)
+                12 MAKE_FUNCTION            0
+                14 STORE_NAME               1 (get_html_theme_path)
    
-     6          14 LOAD_CONST               3 (<code object get_html_theme_path, file "/home/juca/mysrc/mongomotor/sphinx_pdj_theme/__init__.py", line 6>)
-                16 MAKE_FUNCTION            0
-                18 STORE_NAME               2 (get_html_theme_path)
-   
-    12          20 LOAD_CONST               4 (<code object setup, file "/home/juca/mysrc/mongomotor/sphinx_pdj_theme/__init__.py", line 12>)
-                22 MAKE_FUNCTION            0
-                24 STORE_NAME               3 (setup)
-                26 LOAD_CONST               1 (None)
-                28 RETURN_VALUE
+    10          16 LOAD_CONST               3 (<code object setup, file "/home/juca/mysrc/sphinx_pdj_theme/sphinx_pdj_theme/__init__.py", line 10>)
+                18 MAKE_FUNCTION            0
+                20 STORE_NAME               2 (setup)
+                22 LOAD_CONST               1 (None)
+                24 RETURN_VALUE
    consts
       0
       None
-      '0.2.1'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007400000000000000000000006a
             010000000000000000a00300000000000000000000000000000000000000
             00740800000000000000000000a6010000ab010000000000000000a60100
             00ab0100000000000000007d007c005300
-           6           0 RESUME                   0
+           4           0 RESUME                   0
          
-           8           2 LOAD_GLOBAL              0 (os)
+           6           2 LOAD_GLOBAL              0 (os)
                       14 LOAD_ATTR                1 (path)
                       24 LOAD_METHOD              2 (abspath)
                       46 LOAD_GLOBAL              0 (os)
                       58 LOAD_ATTR                1 (path)
                       68 LOAD_METHOD              3 (dirname)
                       90 LOAD_GLOBAL              8 (__file__)
                      102 PRECALL                  1
                      106 CALL                     1
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               0 (cur_dir)
          
-           9         132 LOAD_FAST                0 (cur_dir)
+           7         132 LOAD_FAST                0 (cur_dir)
                      134 RETURN_VALUE
          consts
             'Return list of HTML theme paths.'
          names      ('os', 'path', 'abspath', 'dirname', '__file__')
          varnames   ('cur_dir',)
          freevars   ()
          cellvars   ()
-         filename   '/home/juca/mysrc/mongomotor/sphinx_pdj_theme/__init__.py'
+         filename   '/home/juca/mysrc/sphinx_pdj_theme/sphinx_pdj_theme/__init__.py'
          name       'get_html_theme_path'
-         firstlineno 6
+         firstlineno 4
          lnotab 0x02028201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000640174
             0300000000000000000000a6000000ab000000000000000000a6020000ab
             020000000000000000010064005300
-          12           0 RESUME                   0
+          10           0 RESUME                   0
          
-          13           2 LOAD_FAST                0 (app)
+          11           2 LOAD_FAST                0 (app)
                        4 LOAD_METHOD              0 (add_html_theme)
                       26 LOAD_CONST               1 ('sphinx_pdj_theme')
                       28 LOAD_GLOBAL              3 (NULL + get_html_theme_path)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 PRECALL                  2
                       58 CALL                     2
@@ -95,19 +89,19 @@
          consts
             None
             'sphinx_pdj_theme'
          names      ('add_html_theme', 'get_html_theme_path')
          varnames   ('app',)
          freevars   ()
          cellvars   ()
-         filename   '/home/juca/mysrc/mongomotor/sphinx_pdj_theme/__init__.py'
+         filename   '/home/juca/mysrc/sphinx_pdj_theme/sphinx_pdj_theme/__init__.py'
          name       'setup'
-         firstlineno 12
+         firstlineno 10
          lnotab 0x0201
-   names      ('os', 'VERSION', 'get_html_theme_path', 'setup')
+   names      ('os', 'get_html_theme_path', 'setup')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/juca/mysrc/mongomotor/sphinx_pdj_theme/__init__.py'
+   filename   '/home/juca/mysrc/sphinx_pdj_theme/sphinx_pdj_theme/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080204030606
+   lnotab 0x00ff020108030606
```

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/breadcrumbs.html` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/footer.html` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout.html` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     {%- block meta %}{%- endblock %}
 
 
     {%- block link %}{%- endblock %}
     <!-- Add jQuery library -->
 
     {%- block script %}
-    <script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"></script>
+    <script type="text/javascript" src="https://code.jquery.com/jquery-latest.min.js"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/modernizr/2.6.2/modernizr.min.js"></script>
     <script type="module" src="https://googlechromelabs.github.io/dark-mode-toggle/src/dark-mode-toggle.mjs"></script>
     {%- endblock %}
 
   </head>
 
   <body class="wy-body-for-nav" role="document">
@@ -151,15 +151,15 @@
 	    <!-- </ul> -->
 	    <!-- <hr/> -->
 	  </div>
           <div role="main" class="{%- if flatpage %} flatpage {%- endif %}">
 
 	    <div id="content" class="hfeed entry-container hentry">
       	<div id="dark-mode-toggle-container">
-	  <dark-mode-toggle appearance="toggle" dark="switch to light mode" light="switch to dark mode" permanent="true">
+	  <dark-mode-toggle appearance="toggle" dark="switch to light mode" light="switch to dark mode">
 	  </dark-mode-toggle>
 	</div>
 
               {%- block body %}
 	      {%- endblock %}
 	    </div>
             {% include "footer.html" %}
```

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout_old.html` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/layout_old.html`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/search.html` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/badge_only.css` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/darker.css` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/darker.css`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/img.css` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/img.css`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/pdj.css` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/pdj.css`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/theme.css` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/moon.svg` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/img/moon.svg`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/porao-branco.png` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/img/porao-branco.png`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/sun.svg` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/img/sun.svg`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/theme.js` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/versions.html` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme/versions.html`

 * *Files identical despite different names*

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/PKG-INFO` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-pdj-theme
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cool theme for sphinx documentation
 Author: Juca Crispim
 Project-URL: Homepage, https://github.com/jucacrispim/sphinx_pdj_theme/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/SOURCES.txt` & `sphinx-pdj-theme-0.3.1/sphinx_pdj_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*


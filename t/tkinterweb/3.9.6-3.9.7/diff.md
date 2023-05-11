# Comparing `tmp/tkinterweb-3.9.6.tar.gz` & `tmp/tkinterweb-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tkinterweb-3.9.6.tar", last modified: Sat Jun 19 18:21:46 2021, max compression
+gzip compressed data, was "dist/tkinterweb-3.9.7.tar", last modified: Mon Jun 21 13:47:18 2021, max compression
```

## Comparing `tkinterweb-3.9.6.tar` & `tkinterweb-3.9.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:46.084205 tkinterweb-3.9.6/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)       39 2021-04-09 18:22:49.000000 tkinterweb-3.9.6/MANIFEST.in
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2018 2021-06-19 18:21:46.082901 tkinterweb-3.9.6/PKG-INFO
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     1094 2021-06-02 22:29:12.000000 tkinterweb-3.9.6/README.md
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)       38 2021-06-19 18:21:46.084706 tkinterweb-3.9.6/setup.cfg
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      949 2021-06-19 18:21:29.000000 tkinterweb-3.9.6/setup.py
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:45.935906 tkinterweb-3.9.6/tkinterweb/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2011 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/__init__.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    50540 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/bindings.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    17235 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/htmlwidgets.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2736 2021-06-19 18:21:03.000000 tkinterweb-3.9.6/tkinterweb/imageutils.py
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2229 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/lrucache.py
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:45.981632 tkinterweb-3.9.6/tkinterweb/tkhtml/
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:45.858928 tkinterweb-3.9.6/tkinterweb/tkhtml/Darwin/
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:45.999536 tkinterweb-3.9.6/tkinterweb/tkhtml/Darwin/64-bit/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)   311164 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Darwin/64-bit/Tkhtml30.dylib
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      124 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Darwin/64-bit/pkgIndex.tcl
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:45.867784 tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:46.017780 tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/32-bit/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)   376749 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/32-bit/Tkhtml30.so
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      121 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/32-bit/pkgIndex.tcl
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:46.036816 tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/64-bit/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)   410836 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/64-bit/Tkhtml30.so
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      121 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/64-bit/pkgIndex.tcl
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:45.880270 tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:46.052177 tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/32-bit/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)   266240 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/32-bit/Tkhtml30.dll
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      126 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/32-bit/pkgIndex.tcl
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:46.079211 tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/64-bit/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)   712377 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/64-bit/Tkhtml30.dll
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      126 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/64-bit/pkgIndex.tcl
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    64541 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/tkhtml/combobox.tcl
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)    19403 2021-06-19 18:19:29.000000 tkinterweb-3.9.6/tkinterweb/utilities.py
-drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-19 18:21:45.978309 tkinterweb-3.9.6/tkinterweb.egg-info/
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2018 2021-06-19 18:21:44.000000 tkinterweb-3.9.6/tkinterweb.egg-info/PKG-INFO
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)      824 2021-06-19 18:21:44.000000 tkinterweb-3.9.6/tkinterweb.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)        1 2021-06-19 18:21:44.000000 tkinterweb-3.9.6/tkinterweb.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)        7 2021-06-19 18:21:44.000000 tkinterweb-3.9.6/tkinterweb.egg-info/requires.txt
--rwxrwxrwx   0 andrew    (1000) andrew    (1000)       11 2021-06-19 18:21:44.000000 tkinterweb-3.9.6/tkinterweb.egg-info/top_level.txt
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.549263 tkinterweb-3.9.7/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)       39 2021-04-09 18:22:49.000000 tkinterweb-3.9.7/MANIFEST.in
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2018 2021-06-21 13:47:18.547830 tkinterweb-3.9.7/PKG-INFO
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)     1094 2021-06-02 22:29:12.000000 tkinterweb-3.9.7/README.md
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)       38 2021-06-21 13:47:18.549816 tkinterweb-3.9.7/setup.cfg
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)      949 2021-06-21 13:46:21.000000 tkinterweb-3.9.7/setup.py
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.397648 tkinterweb-3.9.7/tkinterweb/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2011 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/__init__.py
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)    50564 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/bindings.py
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)    17235 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/htmlwidgets.py
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2736 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/imageutils.py
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2229 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/lrucache.py
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.433810 tkinterweb-3.9.7/tkinterweb/tkhtml/
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.355856 tkinterweb-3.9.7/tkinterweb/tkhtml/Darwin/
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.463183 tkinterweb-3.9.7/tkinterweb/tkhtml/Darwin/64-bit/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)   311164 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Darwin/64-bit/Tkhtml30.dylib
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)      124 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Darwin/64-bit/pkgIndex.tcl
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.359831 tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.481297 tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/32-bit/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)   376749 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/32-bit/Tkhtml30.so
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)      121 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/32-bit/pkgIndex.tcl
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.500611 tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/64-bit/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)   410836 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/64-bit/Tkhtml30.so
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)      121 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/64-bit/pkgIndex.tcl
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.364189 tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.517002 tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/32-bit/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)   266240 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/32-bit/Tkhtml30.dll
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)      126 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/32-bit/pkgIndex.tcl
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.544108 tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/64-bit/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)   712377 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/64-bit/Tkhtml30.dll
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)      126 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/64-bit/pkgIndex.tcl
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)    64540 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/tkhtml/combobox.tcl
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)    19403 2021-06-21 13:43:42.000000 tkinterweb-3.9.7/tkinterweb/utilities.py
+drwxrwxrwx   0 andrew    (1000) andrew    (1000)        0 2021-06-21 13:47:18.425619 tkinterweb-3.9.7/tkinterweb.egg-info/
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)     2018 2021-06-21 13:47:16.000000 tkinterweb-3.9.7/tkinterweb.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)      824 2021-06-21 13:47:16.000000 tkinterweb-3.9.7/tkinterweb.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)        1 2021-06-21 13:47:16.000000 tkinterweb-3.9.7/tkinterweb.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)        7 2021-06-21 13:47:16.000000 tkinterweb-3.9.7/tkinterweb.egg-info/requires.txt
+-rwxrwxrwx   0 andrew    (1000) andrew    (1000)       11 2021-06-21 13:47:16.000000 tkinterweb-3.9.7/tkinterweb.egg-info/top_level.txt
```

### Comparing `tkinterweb-3.9.6/PKG-INFO` & `tkinterweb-3.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkinterweb
-Version: 3.9.6
+Version: 3.9.7
 Summary: HTML/CSS viewer for Tkinter - bindings for Tkhtml3
 Home-page: https://github.com/Andereoo/TkinterWeb
 License: MIT
 Description: # TkinterWeb 
         **A fast and lightweight cross-platform webbrowser for Tkinter.**
         
         &nbsp;
```

### Comparing `tkinterweb-3.9.6/README.md` & `tkinterweb-3.9.7/README.md`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/setup.py` & `tkinterweb-3.9.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="tkinterweb",
-    version="3.9.6",
+    version="3.9.7",
     description="HTML/CSS viewer for Tkinter - bindings for Tkhtml3",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Andereoo/TkinterWeb",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `tkinterweb-3.9.6/tkinterweb/__init__.py` & `tkinterweb-3.9.7/tkinterweb/__init__.py`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/bindings.py` & `tkinterweb-3.9.7/tkinterweb/bindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         for child in (self.tk.call(node, "children")):
             self.title_change_func(self.tk.call(child, "text"))
 
     def on_base(self, node):
         """Handle <base> elements"""
         try:
             href = self.get_node_attribute(node, "href")
-            self.base_url = href
+            self.base_url = urljoin(self.base_url, href)
         except Exception:
             self.message_func(
                 "Error setting base url: a <base> element has been found without an href attribute.")
 
     def on_a(self, node):
         """Handle <a> elements"""
         self.tk.call(node, "dynamic", "set", "link")
```

### Comparing `tkinterweb-3.9.6/tkinterweb/htmlwidgets.py` & `tkinterweb-3.9.7/tkinterweb/htmlwidgets.py`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/imageutils.py` & `tkinterweb-3.9.7/tkinterweb/imageutils.py`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/lrucache.py` & `tkinterweb-3.9.7/tkinterweb/lrucache.py`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/tkhtml/Darwin/64-bit/Tkhtml30.dylib` & `tkinterweb-3.9.7/tkinterweb/tkhtml/Darwin/64-bit/Tkhtml30.dylib`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/32-bit/Tkhtml30.so` & `tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/32-bit/Tkhtml30.so`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/tkhtml/Linux/64-bit/Tkhtml30.so` & `tkinterweb-3.9.7/tkinterweb/tkhtml/Linux/64-bit/Tkhtml30.so`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/32-bit/Tkhtml30.dll` & `tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/32-bit/Tkhtml30.dll`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/tkhtml/Windows/64-bit/Tkhtml30.dll` & `tkinterweb-3.9.7/tkinterweb/tkhtml/Windows/64-bit/Tkhtml30.dll`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb/tkhtml/combobox.tcl` & `tkinterweb-3.9.7/tkinterweb/tkhtml/combobox.tcl`

 * *Files 0% similar despite different names*

```diff
@@ -2185,8 +2185,7 @@
         if {[llength [info commands ::tk::$command]] == 1} {
             proc $proc {args} "uplevel ::tk::$command \$args"
         }
     }
 }
 
 # end of combobox.tcl
-
```

### Comparing `tkinterweb-3.9.6/tkinterweb/utilities.py` & `tkinterweb-3.9.7/tkinterweb/utilities.py`

 * *Files identical despite different names*

### Comparing `tkinterweb-3.9.6/tkinterweb.egg-info/PKG-INFO` & `tkinterweb-3.9.7/tkinterweb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkinterweb
-Version: 3.9.6
+Version: 3.9.7
 Summary: HTML/CSS viewer for Tkinter - bindings for Tkhtml3
 Home-page: https://github.com/Andereoo/TkinterWeb
 License: MIT
 Description: # TkinterWeb 
         **A fast and lightweight cross-platform webbrowser for Tkinter.**
         
         &nbsp;
```

### Comparing `tkinterweb-3.9.6/tkinterweb.egg-info/SOURCES.txt` & `tkinterweb-3.9.7/tkinterweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/aksharify-2.2.2.tar.gz` & `tmp/aksharify-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.2.2.tar", last modified: Wed May 10 18:57:13 2023, max compression
+gzip compressed data, was "aksharify-2.2.3.tar", last modified: Wed May 10 19:49:07 2023, max compression
```

## Comparing `aksharify-2.2.2.tar` & `aksharify-2.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 18:57:13.053513 aksharify-2.2.2/
--rw-rw-rw-   0        0        0     1094 2023-05-09 13:06:55.000000 aksharify-2.2.2/LICENSE.md
--rw-rw-rw-   0        0        0     4328 2023-05-10 18:57:13.037423 aksharify-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3812 2023-05-10 18:55:03.000000 aksharify-2.2.2/README.md
--rw-rw-rw-   0        0        0      622 2023-05-10 18:50:25.000000 aksharify-2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 18:57:13.053513 aksharify-2.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 18:57:12.881677 aksharify-2.2.2/src/
--rw-rw-rw-   0        0        0        0 2023-05-09 16:00:52.000000 aksharify-2.2.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 18:57:13.037423 aksharify-2.2.2/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4328 2023-05-10 18:57:12.000000 aksharify-2.2.2/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-10 18:57:12.000000 aksharify-2.2.2/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 18:57:12.000000 aksharify-2.2.2/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 18:57:12.000000 aksharify-2.2.2/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-10 18:57:12.000000 aksharify-2.2.2/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3038 2023-05-10 18:51:29.000000 aksharify-2.2.2/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-10 19:49:07.866711 aksharify-2.2.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-09 13:06:55.000000 aksharify-2.2.3/LICENSE.md
+-rw-rw-rw-   0        0        0     4425 2023-05-10 19:49:07.866711 aksharify-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3909 2023-05-10 19:21:28.000000 aksharify-2.2.3/README.md
+-rw-rw-rw-   0        0        0      622 2023-05-10 19:48:28.000000 aksharify-2.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 19:49:07.866711 aksharify-2.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 19:49:07.825653 aksharify-2.2.3/src/
+-rw-rw-rw-   0        0        0        0 2023-05-09 16:00:52.000000 aksharify-2.2.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 19:49:07.864679 aksharify-2.2.3/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4425 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3137 2023-05-10 19:42:24.000000 aksharify-2.2.3/src/aksharify.py
```

### Comparing `aksharify-2.2.2/LICENSE.md` & `aksharify-2.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.2.2/PKG-INFO` & `aksharify-2.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.2
+Version: 2.2.3
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,14 +39,21 @@
 
 ```sh
 python -m pip install aksharify
 ```
 
 ## Usage
 
+```python
+from aksharify import TextArt
+
+art = TextArt("Julia.png")
+art.image.show()
+```
+
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
 - [x] NumberiFy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.2 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.2.3 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
@@ -13,16 +13,17 @@
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
 make sure you have one of recent versions of Python installed on your computer.
-### Installation ```sh python -m pip install aksharify ``` ## Usage _For
-examples from user community, please refer to the [primepatel.github.io/
+### Installation ```sh python -m pip install aksharify ``` ## Usage ```python
+from aksharify import TextArt art = TextArt("Julia.png") art.image.show() ```
+_For examples from user community, please refer to the [primepatel.github.io/
 aksharify](https://primepatel.github.io/aksharify)_  ## Roadmap - [x] NumberiFy
 - [-] Predifined order of characters - [-] Getting images from URL - [-
 ] EmojiFy See the [open issues](https://github.com/github_username/repo_name/
 issues) for a full list of proposed features (and known issues).  ##
 Contributing Contributions are what make the open source community such a
 wonderful place to learn, be inspired, and create. Any contributions you make
 are `appreciated greatly`. If you have a suggestion that would make this
```

### Comparing `aksharify-2.2.2/README.md` & `aksharify-2.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 
 ```sh
 python -m pip install aksharify
 ```
 
 ## Usage
 
+```python
+from aksharify import TextArt
+
+art = TextArt("Julia.png")
+art.image.show()
+```
+
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
 - [x] NumberiFy
```

#### html2text {}

```diff
@@ -6,16 +6,17 @@
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
 make sure you have one of recent versions of Python installed on your computer.
-### Installation ```sh python -m pip install aksharify ``` ## Usage _For
-examples from user community, please refer to the [primepatel.github.io/
+### Installation ```sh python -m pip install aksharify ``` ## Usage ```python
+from aksharify import TextArt art = TextArt("Julia.png") art.image.show() ```
+_For examples from user community, please refer to the [primepatel.github.io/
 aksharify](https://primepatel.github.io/aksharify)_  ## Roadmap - [x] NumberiFy
 - [-] Predifined order of characters - [-] Getting images from URL - [-
 ] EmojiFy See the [open issues](https://github.com/github_username/repo_name/
 issues) for a full list of proposed features (and known issues).  ##
 Contributing Contributions are what make the open source community such a
 wonderful place to learn, be inspired, and create. Any contributions you make
 are `appreciated greatly`. If you have a suggestion that would make this
```

### Comparing `aksharify-2.2.2/pyproject.toml` & `aksharify-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.2.2"
+version = "2.2.3"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `aksharify-2.2.2/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.2.3/src/aksharify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.2
+Version: 2.2.3
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,14 +39,21 @@
 
 ```sh
 python -m pip install aksharify
 ```
 
 ## Usage
 
+```python
+from aksharify import TextArt
+
+art = TextArt("Julia.png")
+art.image.show()
+```
+
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
 - [x] NumberiFy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.2 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.2.3 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
@@ -13,16 +13,17 @@
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
 make sure you have one of recent versions of Python installed on your computer.
-### Installation ```sh python -m pip install aksharify ``` ## Usage _For
-examples from user community, please refer to the [primepatel.github.io/
+### Installation ```sh python -m pip install aksharify ``` ## Usage ```python
+from aksharify import TextArt art = TextArt("Julia.png") art.image.show() ```
+_For examples from user community, please refer to the [primepatel.github.io/
 aksharify](https://primepatel.github.io/aksharify)_  ## Roadmap - [x] NumberiFy
 - [-] Predifined order of characters - [-] Getting images from URL - [-
 ] EmojiFy See the [open issues](https://github.com/github_username/repo_name/
 issues) for a full list of proposed features (and known issues).  ##
 Contributing Contributions are what make the open source community such a
 wonderful place to learn, be inspired, and create. Any contributions you make
 are `appreciated greatly`. If you have a suggestion that would make this
```

### Comparing `aksharify-2.2.2/src/aksharify.py` & `aksharify-2.2.3/src/aksharify.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     def asciify(self):
         self.ascii_text = ""
         div = 255//(len(self.ascii_chars))
         bwdata = self.image.convert('L').getdata()
         for line_no in range(self.h):
             for pixel in range(line_no*self.w, line_no*self.w + self.w):
                 self.ascii_text += self.ascii_chars[bwdata[pixel]//div -1]
-        return self.ascii_text
     
     def numberify(self, first_char=0):
         for i in self.ascii_chars:
             if not i.isnumeric():
                 raise TypeError
         self.asciify()
         if first_char != 0:
@@ -72,13 +71,16 @@
     def ascii_show(self):
         text = ""
         for line_no in range(self.h):
             text += self.ascii_text[line_no*self.w:line_no*self.w + self.w] + "\n"
         print(text)
 
     def text_output(self, fname):
+        text = ""
+        for line_no in range(self.h):
+            text += self.ascii_text[line_no*self.w:line_no*self.w + self.w] + "\n"
         with open(fname + ".txt", "w") as file:
-            file.write(self.ascii_text)
+            file.write(text)
     
     def color_output(self, fname):
         with open(fname + ".html", "w") as file:
             file.write(self.ascii_html)
```


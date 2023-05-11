# Comparing `tmp/waifuim.py-4.2.2.tar.gz` & `tmp/waifuim.py-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waifuim.py-4.2.2.tar", last modified: Tue Mar 21 19:18:51 2023, max compression
+gzip compressed data, was "waifuim.py-4.2.3.tar", last modified: Thu May 11 11:58:20 2023, max compression
```

## Comparing `waifuim.py-4.2.2.tar` & `waifuim.py-4.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 19:18:50.994529 waifuim.py-4.2.2/
--rw-rw-rw-   0        0        0     1082 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/LICENSE
--rw-rw-rw-   0        0        0     4313 2023-03-21 19:18:50.994529 waifuim.py-4.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3240 2023-03-21 19:10:23.000000 waifuim.py-4.2.2/README.md
--rw-rw-rw-   0        0        0       86 2023-03-21 19:18:50.997520 waifuim.py-4.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1493 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 19:18:50.978572 waifuim.py-4.2.2/waifuim/
--rw-rw-rw-   0        0        0     1252 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/waifuim/__init__.py
--rw-rw-rw-   0        0        0    16582 2023-03-21 18:45:31.000000 waifuim.py-4.2.2/waifuim/aioclient.py
--rw-rw-rw-   0        0        0     1974 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/waifuim/exceptions.py
--rw-rw-rw-   0        0        0     1134 2023-03-21 18:42:55.000000 waifuim.py-4.2.2/waifuim/moduleinfo.py
--rw-rw-rw-   0        0        0      801 2023-03-06 16:41:48.000000 waifuim.py-4.2.2/waifuim/types.py
--rw-rw-rw-   0        0        0     1519 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/waifuim/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-21 19:18:50.993532 waifuim.py-4.2.2/waifuim.py.egg-info/
--rw-rw-rw-   0        0        0     4313 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 11:58:20.156646 waifuim.py-4.2.3/
+-rw-rw-rw-   0        0        0     1082 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/LICENSE
+-rw-rw-rw-   0        0        0     4313 2023-05-11 11:58:20.156646 waifuim.py-4.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3240 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-11 11:58:20.156646 waifuim.py-4.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:58:20.141640 waifuim.py-4.2.3/waifuim/
+-rw-rw-rw-   0        0        0     1252 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/waifuim/__init__.py
+-rw-rw-rw-   0        0        0    16582 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/waifuim/aioclient.py
+-rw-rw-rw-   0        0        0     1974 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/waifuim/exceptions.py
+-rw-rw-rw-   0        0        0     1134 2023-05-11 11:56:35.000000 waifuim.py-4.2.3/waifuim/moduleinfo.py
+-rw-rw-rw-   0        0        0     1238 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/waifuim/types.py
+-rw-rw-rw-   0        0        0     1519 2023-05-11 11:54:20.000000 waifuim.py-4.2.3/waifuim/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:58:20.156646 waifuim.py-4.2.3/waifuim.py.egg-info/
+-rw-rw-rw-   0        0        0     4313 2023-05-11 11:58:20.000000 waifuim.py-4.2.3/waifuim.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-11 11:58:20.000000 waifuim.py-4.2.3/waifuim.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:58:20.000000 waifuim.py-4.2.3/waifuim.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-11 11:58:20.000000 waifuim.py-4.2.3/waifuim.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 11:58:20.000000 waifuim.py-4.2.3/waifuim.py.egg-info/top_level.txt
```

### Comparing `waifuim.py-4.2.2/LICENSE` & `waifuim.py-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.2/PKG-INFO` & `waifuim.py-4.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuim.py
-Version: 4.2.2
+Version: 4.2.3
 Summary: A Python wrapper for waifu.im API.
 Home-page: https://github.com/Waifu-im/waifuim.py
 Author: Buco
 Author-email: bucolo33fr@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/Waifu-im/waifuim.py/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `waifuim.py-4.2.2/README.md` & `waifuim.py-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.2/setup.py` & `waifuim.py-4.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.2/waifuim/__init__.py` & `waifuim.py-4.2.3/waifuim/__init__.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.2/waifuim/aioclient.py` & `waifuim.py-4.2.3/waifuim/aioclient.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.2/waifuim/exceptions.py` & `waifuim.py-4.2.3/waifuim/exceptions.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.2/waifuim/moduleinfo.py` & `waifuim.py-4.2.3/waifuim/moduleinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE."""
 
 __author__ = 'Buco'
-__version__ = '4.2.2'
+__version__ = '4.2.3'
```

### Comparing `waifuim.py-4.2.2/waifuim/types.py` & `waifuim.py-4.2.3/waifuim/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,50 @@
 from dateutil.parser import parse
 
 
+class Artist:
+    """Represents an API Artist."""
+
+    def __init__(self, data):
+        for key, values in data.items():
+            setattr(self, key.lower(), values)
+
+    def __str__(self):
+        return self.name
+
+    def __eq__(self, other):
+        return isinstance(other, Artist) and self.artist_id == other.artist_id
+
+
 class Tag:
     """Represents an API tag."""
+
     def __init__(self, data):
         for key, values in data.items():
             setattr(self, key.lower(), values)
 
     def __str__(self):
         return self.name
 
     def __eq__(self, other):
         return isinstance(other, Tag) and self.tag_id == other.tag_id
 
 
 class Image:
     """Represents an API Image."""
+
     def __init__(self, data):
         for key, values in data.items():
             setattr(self, key.lower(), values)
+
         self.tags = [Tag(tag) for tag in self.tags]
+
+        if self.artist is not None:
+            self.artist = Artist(self.artist)
+
         self.uploaded_at = parse(self.uploaded_at)
 
     def __str__(self):
         return self.url
 
     def __eq__(self, other):
         return isinstance(other, Image) and self.image_id == other.image_id
```

### Comparing `waifuim.py-4.2.2/waifuim/utils.py` & `waifuim.py-4.2.3/waifuim/utils.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.2/waifuim.py.egg-info/PKG-INFO` & `waifuim.py-4.2.3/waifuim.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuim.py
-Version: 4.2.2
+Version: 4.2.3
 Summary: A Python wrapper for waifu.im API.
 Home-page: https://github.com/Waifu-im/waifuim.py
 Author: Buco
 Author-email: bucolo33fr@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/Waifu-im/waifuim.py/issues
 Classifier: Development Status :: 5 - Production/Stable
```


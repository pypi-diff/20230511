# Comparing `tmp/roastedbyai-0.1.0.tar.gz` & `tmp/roastedbyai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roastedbyai-0.1.0.tar", last modified: Thu May 11 11:10:31 2023, max compression
+gzip compressed data, was "roastedbyai-0.1.1.tar", last modified: Thu May 11 11:23:22 2023, max compression
```

## Comparing `roastedbyai-0.1.0.tar` & `roastedbyai-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:10:31.702263 roastedbyai-0.1.0/
--rw-rw-rw-   0        0        0     1097 2023-05-11 10:58:37.000000 roastedbyai-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2552 2023-05-11 11:10:31.702263 roastedbyai-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      944 2023-05-08 18:30:04.000000 roastedbyai-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 11:10:31.693702 roastedbyai-0.1.0/roastedbyai/
--rw-rw-rw-   0        0        0     1207 2023-05-11 11:09:12.000000 roastedbyai-0.1.0/roastedbyai/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-05-11 11:09:12.000000 roastedbyai-0.1.0/roastedbyai/errors.py
--rw-rw-rw-   0        0        0     6592 2023-05-11 11:08:06.000000 roastedbyai-0.1.0/roastedbyai/roasted.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:10:31.700264 roastedbyai-0.1.0/roastedbyai.egg-info/
--rw-rw-rw-   0        0        0     2552 2023-05-11 11:10:31.000000 roastedbyai-0.1.0/roastedbyai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-11 11:10:31.000000 roastedbyai-0.1.0/roastedbyai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:10:31.000000 roastedbyai-0.1.0/roastedbyai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-11 11:10:31.000000 roastedbyai-0.1.0/roastedbyai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 11:10:31.000000 roastedbyai-0.1.0/roastedbyai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 11:10:31.702263 roastedbyai-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3097 2023-05-11 11:10:25.000000 roastedbyai-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:23:22.394282 roastedbyai-0.1.1/
+-rw-rw-rw-   0        0        0     1097 2023-05-11 10:58:37.000000 roastedbyai-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2554 2023-05-11 11:23:22.393281 roastedbyai-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2023-05-11 11:11:09.000000 roastedbyai-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 11:23:22.388143 roastedbyai-0.1.1/roastedbyai/
+-rw-rw-rw-   0        0        0     1207 2023-05-11 11:11:18.000000 roastedbyai-0.1.1/roastedbyai/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-05-11 11:09:12.000000 roastedbyai-0.1.1/roastedbyai/errors.py
+-rw-rw-rw-   0        0        0     6574 2023-05-11 11:22:55.000000 roastedbyai-0.1.1/roastedbyai/roasted.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:23:22.392281 roastedbyai-0.1.1/roastedbyai.egg-info/
+-rw-rw-rw-   0        0        0     2554 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 11:23:22.000000 roastedbyai-0.1.1/roastedbyai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 11:23:22.394282 roastedbyai-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3097 2023-05-11 11:10:25.000000 roastedbyai-0.1.1/setup.py
```

### Comparing `roastedbyai-0.1.0/LICENSE` & `roastedbyai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roastedbyai-0.1.0/PKG-INFO` & `roastedbyai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roastedbyai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to get roasted by AI (using Selenium).
 Home-page: https://github.com/jvherck/roastedbyai
 Author: jvherck
 Author-email: contact@janvh.be
 Maintainer: jvherck
 Maintainer-email: contact@janvh.be
 License: MIT License
@@ -40,15 +40,15 @@
 https://roastedby.ai as the website doesn't have an official API.
 
 
 ---
 
 
 ## How to install
-Run `pip install roastbyai`
+Run `pip install roastbyai` \
 If that doesn't work, try `py -m pip install roastedbyai`
 
 
 ---
 
 
 ## Usage
```

### Comparing `roastedbyai-0.1.0/README.md` & `roastedbyai-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 https://roastedby.ai as the website doesn't have an official API.
 
 
 ---
 
 
 ## How to install
-Run `pip install roastbyai`
+Run `pip install roastbyai` \
 If that doesn't work, try `py -m pip install roastedbyai`
 
 
 ---
 
 
 ## Usage
```

### Comparing `roastedbyai-0.1.0/roastedbyai/__init__.py` & `roastedbyai-0.1.1/roastedbyai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .roasted import *
 from .errors import *
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `roastedbyai-0.1.0/roastedbyai/errors.py` & `roastedbyai-0.1.1/roastedbyai/errors.py`

 * *Files identical despite different names*

### Comparing `roastedbyai-0.1.0/roastedbyai/roasted.py` & `roastedbyai-0.1.1/roastedbyai/roasted.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,23 +69,23 @@
                 (By.CLASS_NAME, 'inputBox')
             )
         )
         self._input_box = self._driver.find_element(by=By.CLASS_NAME, value='inputBox')
 
 
     @property
-    async def aimessages(self):
+    def aimessages(self):
         return self._aimessages
 
     @property
-    async def usermessages(self):
+    def usermessages(self):
         return self._usermessages
 
     @property
-    async def alive(self):
+    def alive(self):
         return self._alive
 
 
     def _scrollToBottom(self):
         self._driver.execute_script(
             """
             var elem = document.getElementsByClassName("chatMessages")[0];
```

### Comparing `roastedbyai-0.1.0/roastedbyai.egg-info/PKG-INFO` & `roastedbyai-0.1.1/roastedbyai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roastedbyai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to get roasted by AI (using Selenium).
 Home-page: https://github.com/jvherck/roastedbyai
 Author: jvherck
 Author-email: contact@janvh.be
 Maintainer: jvherck
 Maintainer-email: contact@janvh.be
 License: MIT License
@@ -40,15 +40,15 @@
 https://roastedby.ai as the website doesn't have an official API.
 
 
 ---
 
 
 ## How to install
-Run `pip install roastbyai`
+Run `pip install roastbyai` \
 If that doesn't work, try `py -m pip install roastedbyai`
 
 
 ---
 
 
 ## Usage
```

### Comparing `roastedbyai-0.1.0/setup.py` & `roastedbyai-0.1.1/setup.py`

 * *Files identical despite different names*


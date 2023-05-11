# Comparing `tmp/pyutils_basstal-0.4.3.tar.gz` & `tmp/pyutils_basstal-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutils_basstal-0.4.3.tar", last modified: Wed May 10 06:00:38 2023, max compression
+gzip compressed data, was "pyutils_basstal-0.4.4.tar", last modified: Thu May 11 04:06:12 2023, max compression
```

## Comparing `pyutils_basstal-0.4.3.tar` & `pyutils_basstal-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 06:00:38.776602 pyutils_basstal-0.4.3/
--rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1473 2023-05-10 06:00:38.775604 pyutils_basstal-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-05-10 05:03:43.000000 pyutils_basstal-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 06:00:38.755658 pyutils_basstal-0.4.3/pyutils/
--rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.3/pyutils/__init__.py
--rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.3/pyutils/autoupgrade.py
--rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.3/pyutils/executor.py
--rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.3/pyutils/fsext.py
--rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.3/pyutils/shorthand.py
--rw-rw-rw-   0        0        0     6209 2023-05-10 05:59:40.000000 pyutils_basstal-0.4.3/pyutils/simplelogger.py
--rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.3/pyutils/templite.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:00:38.775604 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/
--rw-rw-rw-   0        0        0     1473 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 06:00:38.776602 pyutils_basstal-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     8847 2023-05-10 05:35:50.000000 pyutils_basstal-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:12.157134 pyutils_basstal-0.4.4/
+-rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1473 2023-05-11 04:06:12.157134 pyutils_basstal-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-05-10 05:03:43.000000 pyutils_basstal-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:12.133128 pyutils_basstal-0.4.4/pyutils/
+-rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.4/pyutils/__init__.py
+-rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.4/pyutils/autoupgrade.py
+-rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.4/pyutils/executor.py
+-rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.4/pyutils/fsext.py
+-rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.4/pyutils/shorthand.py
+-rw-rw-rw-   0        0        0     6455 2023-05-11 03:33:38.000000 pyutils_basstal-0.4.4/pyutils/simplelogger.py
+-rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.4/pyutils/templite.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:12.156165 pyutils_basstal-0.4.4/pyutils_basstal.egg-info/
+-rw-rw-rw-   0        0        0     1473 2023-05-11 04:06:12.000000 pyutils_basstal-0.4.4/pyutils_basstal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-11 04:06:12.000000 pyutils_basstal-0.4.4/pyutils_basstal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 04:06:12.000000 pyutils_basstal-0.4.4/pyutils_basstal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-11 04:06:12.000000 pyutils_basstal-0.4.4/pyutils_basstal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 04:06:12.000000 pyutils_basstal-0.4.4/pyutils_basstal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 04:06:12.158132 pyutils_basstal-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     8847 2023-05-11 04:05:38.000000 pyutils_basstal-0.4.4/setup.py
```

### Comparing `pyutils_basstal-0.4.3/LICENSE.txt` & `pyutils_basstal-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/PKG-INFO` & `pyutils_basstal-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutils_basstal
-Version: 0.4.3
+Version: 0.4.4
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.3/README.md` & `pyutils_basstal-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/pyutils/autoupgrade.py` & `pyutils_basstal-0.4.4/pyutils/autoupgrade.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/pyutils/executor.py` & `pyutils_basstal-0.4.4/pyutils/executor.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/pyutils/fsext.py` & `pyutils_basstal-0.4.4/pyutils/fsext.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/pyutils/shorthand.py` & `pyutils_basstal-0.4.4/pyutils/shorthand.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/pyutils/simplelogger.py` & `pyutils_basstal-0.4.4/pyutils/simplelogger.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 ######################
 #       Log          #
 ######################
 ######################
 
 ErrorRaiseExcpetion = False
 
-logging.basicConfig(level=logging.INFO, datefmt='%y-%m-%d %H:%M:%S', format='%(message)s')
+if sys.version_info >= (3, 9):
+    logging.basicConfig(level=logging.INFO, datefmt='%y-%m-%d %H:%M:%S', format='%(message)s', encoding='utf-8')
+else:
+    logging.basicConfig(level=logging.INFO, datefmt='%y-%m-%d %H:%M:%S', format='%(message)s')
 
 
 class SimpleLogger(object):
     # 这是原来的 error/warning logger
     _logger = logging.getLogger("error_logger")
     _logger.setLevel(logging.ERROR)
     _logger.handlers.clear()
@@ -43,15 +46,16 @@
             '32': Fore.GREEN,
             '33': Fore.YELLOW,
             '34': Fore.BLUE,
             '35': Fore.MAGENTA,
             '36': Fore.CYAN,
             '37': Fore.WHITE
         }
-        color = color_map.get(str(color_code), Fore.RESET)
+        # jenkins 无法识别 Fore.RESET，这里将 Fore.RESET 替换为 ''
+        color = color_map.get(str(color_code), '')
 
         if bold:
             return f'{Style.BRIGHT}{color}{message}{Style.RESET_ALL}'
         else:
             return f'{color}{message}{Style.RESET_ALL}'
 
     @staticmethod
@@ -82,15 +86,15 @@
         message = SimpleLogger._color_message(message, 31, bold)
         SimpleLogger._logger.error(message)
 
     @staticmethod
     def addFileHandler(file_path):
         if file_path in SimpleLogger.__hanlder_cache:
             return
-        file_handler = logging.FileHandler(file_path)
+        file_handler = logging.FileHandler(file_path, encoding='utf-8')
 
         class NoEscapeSeqFormatter(logging.Formatter):
             _ansi_escape = re.compile(r'(\x9B|\x1B\[)[0-?]*[ -/]*[@-~]')
 
             def format(self, record):
                 record.msg = self._ansi_escape.sub('', record.getMessage())
                 return super().format(record)
```

### Comparing `pyutils_basstal-0.4.3/pyutils/templite.py` & `pyutils_basstal-0.4.4/pyutils/templite.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/pyutils_basstal.egg-info/PKG-INFO` & `pyutils_basstal-0.4.4/pyutils_basstal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutils-basstal
-Version: 0.4.3
+Version: 0.4.4
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.3/pyutils_basstal.egg-info/SOURCES.txt` & `pyutils_basstal-0.4.4/pyutils_basstal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.3/setup.py` & `pyutils_basstal-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="pyutils_basstal",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.3",  # Required
+    version="0.4.4",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="self used py utils",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```


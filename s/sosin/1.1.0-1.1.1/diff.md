# Comparing `tmp/sosin-1.1.0.tar.gz` & `tmp/sosin-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.1.0.tar", last modified: Wed May 10 08:13:48 2023, max compression
+gzip compressed data, was "sosin-1.1.1.tar", last modified: Thu May 11 05:23:12 2023, max compression
```

## Comparing `sosin-1.1.0.tar` & `sosin-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.631873 sosin-1.1.0/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-05-10 08:13:48.630872 sosin-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 08:13:48.631873 sosin-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-05-10 08:13:43.000000 sosin-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.586562 sosin-1.1.0/sosin/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.1.0/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.602434 sosin-1.1.0/sosin/databases/
--rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.0/sosin/databases/fs.py
--rw-rw-rw-   0        0        0     9667 2023-05-10 06:56:55.000000 sosin-1.1.0/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.605646 sosin-1.1.0/sosin/rpa/
--rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.1.0/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.0/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.625581 sosin-1.1.0/sosin/utils/
--rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/secret.py
--rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.0/sosin/utils/zip.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.629873 sosin-1.1.0/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.0/sosin/web/content.py
--rw-rw-rw-   0        0        0     5505 2023-05-10 08:13:43.000000 sosin-1.1.0/sosin/web/session.py
--rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4796 2023-04-24 07:25:27.000000 sosin-1.1.0/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.599924 sosin-1.1.0/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/top_level.txt
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.531532 sosin-1.1.1/
+-rwx------   0 sosin      (501) staff       (20)     1083 2023-04-17 11:46:46.000000 sosin-1.1.1/LICENSE
+-rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-11 05:23:12.531263 sosin-1.1.1/PKG-INFO
+-rwx------   0 sosin      (501) staff       (20)      863 2023-04-17 11:46:46.000000 sosin-1.1.1/README.md
+-rw-r--r--   0 sosin      (501) staff       (20)       38 2023-05-11 05:23:12.531632 sosin-1.1.1/setup.cfg
+-rwx------   0 sosin      (501) staff       (20)      994 2023-05-11 05:22:59.000000 sosin-1.1.1/setup.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.527333 sosin-1.1.1/sosin/
+-rwx------   0 sosin      (501) staff       (20)        0 2023-04-17 12:05:52.000000 sosin-1.1.1/sosin/__init__.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.528392 sosin-1.1.1/sosin/databases/
+-rwx------   0 sosin      (501) staff       (20)     4934 2023-04-24 10:38:48.000000 sosin-1.1.1/sosin/databases/fs.py
+-rwx------   0 sosin      (501) staff       (20)     9667 2023-05-10 06:56:55.000000 sosin-1.1.1/sosin/databases/rdb.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.528710 sosin-1.1.1/sosin/rpa/
+-rwx------   0 sosin      (501) staff       (20)    10828 2023-04-22 13:06:11.000000 sosin-1.1.1/sosin/rpa/email_mgr.py
+-rwx------   0 sosin      (501) staff       (20)     3698 2023-05-10 06:56:55.000000 sosin-1.1.1/sosin/rpa/sms_mgr.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.529657 sosin-1.1.1/sosin/utils/
+-rwx------   0 sosin      (501) staff       (20)     1687 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/currency.py
+-rwx------   0 sosin      (501) staff       (20)      304 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/log.py
+-rwx------   0 sosin      (501) staff       (20)      527 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/progress.py
+-rwx------   0 sosin      (501) staff       (20)      385 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/utils/secret.py
+-rwx------   0 sosin      (501) staff       (20)      885 2023-05-10 06:56:55.000000 sosin-1.1.1/sosin/utils/zip.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.530614 sosin-1.1.1/sosin/web/
+-rwx------   0 sosin      (501) staff       (20)     1055 2023-04-18 14:49:45.000000 sosin-1.1.1/sosin/web/content.py
+-rwx------   0 sosin      (501) staff       (20)     5506 2023-05-10 10:02:28.000000 sosin-1.1.1/sosin/web/session.py
+-rwx------   0 sosin      (501) staff       (20)     1018 2023-04-17 11:46:46.000000 sosin-1.1.1/sosin/web/translate.py
+-rwx------   0 sosin      (501) staff       (20)     4796 2023-04-24 07:25:27.000000 sosin-1.1.1/sosin/web/virtual.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-11 05:23:12.528072 sosin-1.1.1/sosin.egg-info/
+-rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/PKG-INFO
+-rw-r--r--   0 sosin      (501) staff       (20)      471 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/SOURCES.txt
+-rw-r--r--   0 sosin      (501) staff       (20)        1 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/dependency_links.txt
+-rw-r--r--   0 sosin      (501) staff       (20)       32 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/requires.txt
+-rw-r--r--   0 sosin      (501) staff       (20)        6 2023-05-11 05:23:12.000000 sosin-1.1.1/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.1.0/LICENSE` & `sosin-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/PKG-INFO` & `sosin-1.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.1.0
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.1.1
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: svstar94@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
+
+
```

### Comparing `sosin-1.1.0/README.md` & `sosin-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/setup.py` & `sosin-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.1.0",
+    version                             = "1.1.1",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'beautifulsoup4', 'PyMySQL',],
```

### Comparing `sosin-1.1.0/sosin/databases/fs.py` & `sosin-1.1.1/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/databases/rdb.py` & `sosin-1.1.1/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/rpa/email_mgr.py` & `sosin-1.1.1/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/rpa/sms_mgr.py` & `sosin-1.1.1/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/utils/currency.py` & `sosin-1.1.1/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/utils/progress.py` & `sosin-1.1.1/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/utils/zip.py` & `sosin-1.1.1/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/web/content.py` & `sosin-1.1.1/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/web/session.py` & `sosin-1.1.1/sosin/web/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     Session Manager
     """
 
     history:list[requests.Response] = []
 
     def __init__(self, cookie_path:str='./cookie', history_mode:bool=False) -> None:
         self._headers = { 'User-Agent': 'Mozilla/5.0' }
+        self._cookies = {}
         self._cookie_path = cookie_path
         self._mode = history_mode
         
         try:
             open(cookie_path, 'r')
             self._load_cookies()
-        except:
-            self._cookies = {}
+        except: pass
 
     def __del__(self):
         self._save_cookies()
     
     # ------------------------------------------------------------------------
     # Request Management
     def get(self, url:str, headers:dict={}, cookies:dict={}, **kwargs) -> requests.Response:
```

### Comparing `sosin-1.1.0/sosin/web/translate.py` & `sosin-1.1.1/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin/web/virtual.py` & `sosin-1.1.1/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.0/sosin.egg-info/PKG-INFO` & `sosin-1.1.1/sosin.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.1.0
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.1.1
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: svstar94@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
+
+
```


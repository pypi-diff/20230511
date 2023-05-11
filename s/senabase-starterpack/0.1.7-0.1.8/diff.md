# Comparing `tmp/senabase-starterpack-0.1.7.tar.gz` & `tmp/senabase-starterpack-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senabase-starterpack-0.1.7.tar", last modified: Mon May  8 08:40:27 2023, max compression
+gzip compressed data, was "senabase-starterpack-0.1.8.tar", last modified: Thu May 11 21:37:27 2023, max compression
```

## Comparing `senabase-starterpack-0.1.7.tar` & `senabase-starterpack-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.496457 senabase-starterpack-0.1.7/
--rw-rw-rw-   0        0        0     1090 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1188 2023-05-08 08:40:27.495459 senabase-starterpack-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      875 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.488460 senabase-starterpack-0.1.7/senabase/
--rw-rw-rw-   0        0        0        0 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/senabase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.490465 senabase-starterpack-0.1.7/senabase/starterpack/
--rw-rw-rw-   0        0        0        0 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/senabase/starterpack/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-08 00:34:12.000000 senabase-starterpack-0.1.7/senabase/starterpack/database.py
--rw-rw-rw-   0        0        0     1886 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.7/senabase/starterpack/log.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:40:27.494457 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/
--rw-rw-rw-   0        0        0     1188 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 08:40:27.000000 senabase-starterpack-0.1.7/senabase_starterpack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 08:40:27.496457 senabase-starterpack-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-05-08 08:40:23.000000 senabase-starterpack-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:37:27.742311 senabase-starterpack-0.1.8/
+-rw-rw-rw-   0        0        0     1090 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1519 2023-05-11 21:37:27.742311 senabase-starterpack-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2023-05-11 21:33:54.000000 senabase-starterpack-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 21:37:27.742311 senabase-starterpack-0.1.8/senabase/
+-rw-rw-rw-   0        0        0        0 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.8/senabase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:37:27.742311 senabase-starterpack-0.1.8/senabase/starterpack/
+-rw-rw-rw-   0        0        0        0 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.8/senabase/starterpack/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-08 00:34:12.000000 senabase-starterpack-0.1.8/senabase/starterpack/database.py
+-rw-rw-rw-   0        0        0     1886 2023-05-07 23:47:08.000000 senabase-starterpack-0.1.8/senabase/starterpack/log.py
+-rw-rw-rw-   0        0        0      956 2023-05-10 02:50:11.000000 senabase-starterpack-0.1.8/senabase/starterpack/telegram.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:37:27.742311 senabase-starterpack-0.1.8/senabase_starterpack.egg-info/
+-rw-rw-rw-   0        0        0     1519 2023-05-11 21:37:27.000000 senabase-starterpack-0.1.8/senabase_starterpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-05-11 21:37:27.000000 senabase-starterpack-0.1.8/senabase_starterpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 21:37:27.000000 senabase-starterpack-0.1.8/senabase_starterpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-11 21:37:27.000000 senabase-starterpack-0.1.8/senabase_starterpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 21:37:27.000000 senabase-starterpack-0.1.8/senabase_starterpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 21:37:27.742311 senabase-starterpack-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-05-09 12:42:06.000000 senabase-starterpack-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:37:27.742311 senabase-starterpack-0.1.8/test/
+-rw-rw-rw-   0        0        0     2761 2023-05-11 21:22:26.000000 senabase-starterpack-0.1.8/test/test.py
```

### Comparing `senabase-starterpack-0.1.7/LICENSE` & `senabase-starterpack-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `senabase-starterpack-0.1.7/PKG-INFO` & `senabase-starterpack-0.1.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: senabase-starterpack
-Version: 0.1.7
-Summary: senabase starterpack library
-Home-page: https://github.com/parkssie/senabase-starterpack
-Author: Jungkyu Park
-Author-email: parkssie@me.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # senabase-starterpack
 
 senabase-starterpack is personal library for fast prototyping.
 
 ## Installation
 
 Use `pip` to download it from [PyPI](https://pypi.org/project/senabase-starterpack/)
@@ -20,16 +9,17 @@
 ```shell
 $ pip install senabase-starterpack
 ```
 
 The minimum required versions of the respective tools are:
 
 ```
-psycopg2-binary>=2.9.*
-pyyaml>=6.*
+psycopg2-binary>=2.9.1
+pyyaml>=6.0
+requests>=2.30.0
 ```
 
 ## Example
 
 ### PostgreSQLHandler
 
 Postgresql starterpack
@@ -54,7 +44,22 @@
 log = SimpleLogger()
 log.configure('proto')
 
 log.i('Information')
 log.d('Debug')
 log.e(Exception('Example exception'))
 ```
+
+### telegram
+
+Telegram message sender
+
+```python
+from senabase.starterpack.telegram import TelegramHandler
+
+token = '0000000000'
+chat_id = '00000000'
+message = 'Hello'
+telegram_handler = TelegramHandler()
+telegram_handler.configure(token)
+res = telegram_handler.send_message(chat_id, message)
+```
```

### Comparing `senabase-starterpack-0.1.7/senabase/starterpack/database.py` & `senabase-starterpack-0.1.8/senabase/starterpack/database.py`

 * *Files identical despite different names*

### Comparing `senabase-starterpack-0.1.7/senabase/starterpack/log.py` & `senabase-starterpack-0.1.8/senabase/starterpack/log.py`

 * *Files identical despite different names*

### Comparing `senabase-starterpack-0.1.7/setup.py` & `senabase-starterpack-0.1.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(name='senabase-starterpack',
-      version='0.1.7',
+      version='0.1.8',
       description='senabase starterpack library',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Jungkyu Park',
       author_email='parkssie@me.com',
       url='https://github.com/parkssie/senabase-starterpack',
       python_requires='>=3.10',
-      packages=find_packages(".", exclude=["prototypes"]),
+      packages=find_packages(".", exclude=["test"]),
       install_requires=[
           'psycopg2-binary>=2.9.1',
           'pyyaml>=6.0',
+          'requests>=2.30.0',
       ])
```


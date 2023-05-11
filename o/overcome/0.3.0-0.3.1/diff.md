# Comparing `tmp/overcome-0.3.0.tar.gz` & `tmp/overcome-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overcome-0.3.0.tar", last modified: Wed Mar 15 02:58:53 2023, max compression
+gzip compressed data, was "overcome-0.3.1.tar", last modified: Wed May 10 09:18:24 2023, max compression
```

## Comparing `overcome-0.3.0.tar` & `overcome-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-03-15 02:58:53.935410 overcome-0.3.0/
--rw-r--r--   0 jaume     (1000) jaume     (1000)    35147 2022-05-08 02:56:34.000000 overcome-0.3.0/LICENSE.txt
--rw-r--r--   0 jaume     (1000) jaume     (1000)     5100 2023-03-15 02:58:53.935410 overcome-0.3.0/PKG-INFO
--rw-r--r--   0 jaume     (1000) jaume     (1000)     4438 2023-02-13 01:53:51.000000 overcome-0.3.0/README.md
--rw-r--r--   0 jaume     (1000) jaume     (1000)       85 2022-05-08 02:49:10.000000 overcome-0.3.0/pyproject.toml
--rw-r--r--   0 jaume     (1000) jaume     (1000)      836 2023-03-15 02:58:53.935410 overcome-0.3.0/setup.cfg
-drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-03-15 02:58:53.935410 overcome-0.3.0/src/
-drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-03-15 02:58:53.935410 overcome-0.3.0/src/overcome/
--rw-r--r--   0 jaume     (1000) jaume     (1000)        0 2022-11-14 02:21:54.000000 overcome-0.3.0/src/overcome/__init__.py
--rw-r--r--   0 jaume     (1000) jaume     (1000)    11503 2023-03-15 02:23:04.000000 overcome-0.3.0/src/overcome/overcome.py
-drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-03-15 02:58:53.935410 overcome-0.3.0/src/overcome/position/
--rw-r--r--   0 jaume     (1000) jaume     (1000)        0 2022-12-06 07:10:28.000000 overcome-0.3.0/src/overcome/position/__init__.py
--rw-r--r--   0 jaume     (1000) jaume     (1000)     1462 2022-12-08 08:34:40.000000 overcome-0.3.0/src/overcome/position/evaluation.py
--rw-r--r--   0 jaume     (1000) jaume     (1000)      178 2023-03-13 02:48:29.000000 overcome-0.3.0/src/overcome/position/positions.py
-drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-03-15 02:58:53.935410 overcome-0.3.0/src/overcome/stack/
--rw-r--r--   0 jaume     (1000) jaume     (1000)        0 2023-03-14 05:42:33.000000 overcome-0.3.0/src/overcome/stack/__init__.py
--rw-r--r--   0 jaume     (1000) jaume     (1000)     1146 2023-03-14 14:48:44.000000 overcome-0.3.0/src/overcome/stack/measuredstack.py
--rw-r--r--   0 jaume     (1000) jaume     (1000)     2650 2022-12-30 14:59:28.000000 overcome-0.3.0/src/overcome/stack/stack.py
-drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-03-15 02:58:53.935410 overcome-0.3.0/src/overcome.egg-info/
--rw-r--r--   0 jaume     (1000) jaume     (1000)     5100 2023-03-15 02:58:53.000000 overcome-0.3.0/src/overcome.egg-info/PKG-INFO
--rw-r--r--   0 jaume     (1000) jaume     (1000)      475 2023-03-15 02:58:53.000000 overcome-0.3.0/src/overcome.egg-info/SOURCES.txt
--rw-r--r--   0 jaume     (1000) jaume     (1000)        1 2023-03-15 02:58:53.000000 overcome-0.3.0/src/overcome.egg-info/dependency_links.txt
--rw-r--r--   0 jaume     (1000) jaume     (1000)       27 2023-03-15 02:58:53.000000 overcome-0.3.0/src/overcome.egg-info/requires.txt
--rw-r--r--   0 jaume     (1000) jaume     (1000)        9 2023-03-15 02:58:53.000000 overcome-0.3.0/src/overcome.egg-info/top_level.txt
+drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-05-10 09:18:24.341259 overcome-0.3.1/
+-rw-r--r--   0 jaume     (1000) jaume     (1000)    35147 2022-05-08 02:56:34.000000 overcome-0.3.1/LICENSE.txt
+-rw-r--r--   0 jaume     (1000) jaume     (1000)     5100 2023-05-10 09:18:24.341259 overcome-0.3.1/PKG-INFO
+-rw-r--r--   0 jaume     (1000) jaume     (1000)     4438 2023-02-13 01:53:51.000000 overcome-0.3.1/README.md
+-rw-r--r--   0 jaume     (1000) jaume     (1000)       85 2022-05-08 02:49:10.000000 overcome-0.3.1/pyproject.toml
+-rw-r--r--   0 jaume     (1000) jaume     (1000)      836 2023-05-10 09:18:24.341259 overcome-0.3.1/setup.cfg
+drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-05-10 09:18:24.337259 overcome-0.3.1/src/
+drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-05-10 09:18:24.337259 overcome-0.3.1/src/overcome/
+-rw-r--r--   0 jaume     (1000) jaume     (1000)        0 2022-11-14 02:21:54.000000 overcome-0.3.1/src/overcome/__init__.py
+-rw-r--r--   0 jaume     (1000) jaume     (1000)    11568 2023-05-10 09:14:55.000000 overcome-0.3.1/src/overcome/overcome.py
+drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-05-10 09:18:24.337259 overcome-0.3.1/src/overcome/position/
+-rw-r--r--   0 jaume     (1000) jaume     (1000)        0 2022-12-06 07:10:28.000000 overcome-0.3.1/src/overcome/position/__init__.py
+-rw-r--r--   0 jaume     (1000) jaume     (1000)     1462 2022-12-08 08:34:40.000000 overcome-0.3.1/src/overcome/position/evaluation.py
+-rw-r--r--   0 jaume     (1000) jaume     (1000)      178 2023-03-13 02:48:29.000000 overcome-0.3.1/src/overcome/position/positions.py
+drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-05-10 09:18:24.341259 overcome-0.3.1/src/overcome/stack/
+-rw-r--r--   0 jaume     (1000) jaume     (1000)        0 2023-05-10 09:14:30.000000 overcome-0.3.1/src/overcome/stack/__init__.py
+-rw-r--r--   0 jaume     (1000) jaume     (1000)     1146 2023-05-10 09:14:30.000000 overcome-0.3.1/src/overcome/stack/measuredstack.py
+-rw-r--r--   0 jaume     (1000) jaume     (1000)     2650 2023-05-10 09:14:30.000000 overcome-0.3.1/src/overcome/stack/stack.py
+drwxr-xr-x   0 jaume     (1000) jaume     (1000)        0 2023-05-10 09:18:24.337259 overcome-0.3.1/src/overcome.egg-info/
+-rw-r--r--   0 jaume     (1000) jaume     (1000)     5100 2023-05-10 09:18:24.000000 overcome-0.3.1/src/overcome.egg-info/PKG-INFO
+-rw-r--r--   0 jaume     (1000) jaume     (1000)      475 2023-05-10 09:18:24.000000 overcome-0.3.1/src/overcome.egg-info/SOURCES.txt
+-rw-r--r--   0 jaume     (1000) jaume     (1000)        1 2023-05-10 09:18:24.000000 overcome-0.3.1/src/overcome.egg-info/dependency_links.txt
+-rw-r--r--   0 jaume     (1000) jaume     (1000)       27 2023-05-10 09:18:24.000000 overcome-0.3.1/src/overcome.egg-info/requires.txt
+-rw-r--r--   0 jaume     (1000) jaume     (1000)        9 2023-05-10 09:18:24.000000 overcome-0.3.1/src/overcome.egg-info/top_level.txt
```

### Comparing `overcome-0.3.0/LICENSE.txt` & `overcome-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `overcome-0.3.0/PKG-INFO` & `overcome-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overcome
-Version: 0.3.0
+Version: 0.3.1
 Summary: Overcome is a data transformer to calculate the potential buying and selling earnings from the "high", "low" and "close" trading history values.
 Home-page: https://github.com/westial/overcome
 Author: Jaume Mila Bea
 Author-email: jaume@westial.com
 Project-URL: Bug Tracker, https://github.com/westial/overcome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `overcome-0.3.0/README.md` & `overcome-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `overcome-0.3.0/setup.cfg` & `overcome-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = overcome
-version = 0.3.0
+version = 0.3.1
 author = Jaume Mila Bea
 author_email = jaume@westial.com
 description = Overcome is a data transformer to calculate the potential buying and selling earnings from the "high", "low" and "close" trading history values.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/westial/overcome
 project_urls =
```

### Comparing `overcome-0.3.0/src/overcome/overcome.py` & `overcome-0.3.1/src/overcome/overcome.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,16 @@
         values_iter = np.nditer(
             high_low_close,
             order='C',
             flags=['external_loop']
         )
         with values_iter:
             for index, [high, low, close] in enumerate(values_iter):
+                if np.isnan(close):
+                    continue
                 self.__update_earnings(
                     high,
                     low,
                     earn_buying,
                     earn_selling,
                     buying_lengths,
                     selling_lengths
```

### Comparing `overcome-0.3.0/src/overcome/position/evaluation.py` & `overcome-0.3.1/src/overcome/position/evaluation.py`

 * *Files identical despite different names*

### Comparing `overcome-0.3.0/src/overcome/stack/measuredstack.py` & `overcome-0.3.1/src/overcome/stack/measuredstack.py`

 * *Files identical despite different names*

### Comparing `overcome-0.3.0/src/overcome/stack/stack.py` & `overcome-0.3.1/src/overcome/stack/stack.py`

 * *Files identical despite different names*

### Comparing `overcome-0.3.0/src/overcome.egg-info/PKG-INFO` & `overcome-0.3.1/src/overcome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overcome
-Version: 0.3.0
+Version: 0.3.1
 Summary: Overcome is a data transformer to calculate the potential buying and selling earnings from the "high", "low" and "close" trading history values.
 Home-page: https://github.com/westial/overcome
 Author: Jaume Mila Bea
 Author-email: jaume@westial.com
 Project-URL: Bug Tracker, https://github.com/westial/overcome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```


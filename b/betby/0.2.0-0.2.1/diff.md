# Comparing `tmp/betby-0.2.0.tar.gz` & `tmp/betby-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.2.0.tar", last modified: Wed May 10 22:56:11 2023, max compression
+gzip compressed data, was "betby-0.2.1.tar", last modified: Wed May 10 23:09:26 2023, max compression
```

## Comparing `betby-0.2.0.tar` & `betby-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 22:56:11.516549 betby-0.2.0/
--rw-rw-rw-   0        0        0      539 2023-05-10 22:56:11.515583 betby-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 22:56:11.488623 betby-0.2.0/betby/
--rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.0/betby/__init__.py
--rw-rw-rw-   0        0        0     5966 2023-05-10 22:45:08.000000 betby-0.2.0/betby/markets.py
-drwxrwxrwx   0        0        0        0 2023-05-10 22:56:11.509595 betby-0.2.0/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-10 22:56:09.000000 betby-0.2.0/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-10 22:56:10.000000 betby-0.2.0/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 22:56:09.000000 betby-0.2.0/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 22:56:09.000000 betby-0.2.0/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 22:56:11.517577 betby-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-10 22:54:37.000000 betby-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 23:09:26.212397 betby-0.2.1/
+-rw-rw-rw-   0        0        0      539 2023-05-10 23:09:26.211399 betby-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 23:09:26.185469 betby-0.2.1/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.1/betby/__init__.py
+-rw-rw-rw-   0        0        0     5952 2023-05-10 23:07:54.000000 betby-0.2.1/betby/markets.py
+drwxrwxrwx   0        0        0        0 2023-05-10 23:09:26.206412 betby-0.2.1/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-10 23:09:23.000000 betby-0.2.1/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-10 23:09:25.000000 betby-0.2.1/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 23:09:23.000000 betby-0.2.1/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 23:09:23.000000 betby-0.2.1/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 23:09:26.213394 betby-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-05-10 23:08:19.000000 betby-0.2.1/setup.py
```

### Comparing `betby-0.2.0/PKG-INFO` & `betby-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.0
+Version: 0.2.1
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.0/betby/markets.py` & `betby-0.2.1/betby/markets.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             kf_v = (1 - mar_1) / ver
         if 1 / kf >= 0.5:
             kf = kf_round(kf_v, max)
         else:
             kf = kf_round((1 - m) * kf_v / (kf_v - 1 + m), max)
         return kf
 
-    def get_matrix(self, avg_1, avg_2):
+    def get_matrix(self):
         avg_1 = avg_1 * (time_full - time) / time_full
         avg_2 = avg_2 * (time_full - time) / time_full
         if poisson:
             matrix = np.zeros((poisson, poisson))
             for i in range(poisson):
                 for j in range(poisson):
                     prob = (exp(-avg_1) * avg_1 ** i / factorial(i)) * (
```

### Comparing `betby-0.2.0/betby.egg-info/PKG-INFO` & `betby-0.2.1/betby.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.0
+Version: 0.2.1
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.0/setup.py` & `betby-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betby",
-    version="0.2.0",
+    version="0.2.1",
     author="Ayrat Badrutdinov",
     author_email="a.badrutdinov@betby.com",
     description="Betby libraries",
     packages=["betby"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```


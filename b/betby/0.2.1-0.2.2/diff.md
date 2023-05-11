# Comparing `tmp/betby-0.2.1.tar.gz` & `tmp/betby-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.2.1.tar", last modified: Wed May 10 23:09:26 2023, max compression
+gzip compressed data, was "betby-0.2.2.tar", last modified: Wed May 10 23:17:21 2023, max compression
```

## Comparing `betby-0.2.1.tar` & `betby-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 23:09:26.212397 betby-0.2.1/
--rw-rw-rw-   0        0        0      539 2023-05-10 23:09:26.211399 betby-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 23:09:26.185469 betby-0.2.1/betby/
--rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.1/betby/__init__.py
--rw-rw-rw-   0        0        0     5952 2023-05-10 23:07:54.000000 betby-0.2.1/betby/markets.py
-drwxrwxrwx   0        0        0        0 2023-05-10 23:09:26.206412 betby-0.2.1/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-10 23:09:23.000000 betby-0.2.1/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-10 23:09:25.000000 betby-0.2.1/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 23:09:23.000000 betby-0.2.1/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 23:09:23.000000 betby-0.2.1/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 23:09:26.213394 betby-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-10 23:08:19.000000 betby-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 23:17:21.786810 betby-0.2.2/
+-rw-rw-rw-   0        0        0      539 2023-05-10 23:17:21.784814 betby-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 23:17:21.752900 betby-0.2.2/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.2/betby/__init__.py
+-rw-rw-rw-   0        0        0     5962 2023-05-10 23:16:03.000000 betby-0.2.2/betby/markets.py
+drwxrwxrwx   0        0        0        0 2023-05-10 23:17:21.779827 betby-0.2.2/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-10 23:17:19.000000 betby-0.2.2/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-10 23:17:20.000000 betby-0.2.2/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 23:17:19.000000 betby-0.2.2/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 23:17:19.000000 betby-0.2.2/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 23:17:21.787807 betby-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-05-10 23:16:24.000000 betby-0.2.2/setup.py
```

### Comparing `betby-0.2.1/PKG-INFO` & `betby-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.1
+Version: 0.2.2
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.1/betby/markets.py` & `betby-0.2.2/betby/markets.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         if 1 / kf >= 0.5:
             kf = kf_round(kf_v, max)
         else:
             kf = kf_round((1 - m) * kf_v / (kf_v - 1 + m), max)
         return kf
 
     def get_matrix(self):
-        avg_1 = avg_1 * (time_full - time) / time_full
-        avg_2 = avg_2 * (time_full - time) / time_full
+        avg_1 = self.avg_1 * (time_full - time) / time_full
+        avg_2 = self.avg_2 * (time_full - time) / time_full
         if poisson:
             matrix = np.zeros((poisson, poisson))
             for i in range(poisson):
                 for j in range(poisson):
                     prob = (exp(-avg_1) * avg_1 ** i / factorial(i)) * (
                                 exp(-avg_2) * avg_2 ** j / factorial(j))
                     matrix[i, j] = prob
```

### Comparing `betby-0.2.1/betby.egg-info/PKG-INFO` & `betby-0.2.2/betby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.1
+Version: 0.2.2
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.1/setup.py` & `betby-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betby",
-    version="0.2.1",
+    version="0.2.2",
     author="Ayrat Badrutdinov",
     author_email="a.badrutdinov@betby.com",
     description="Betby libraries",
     packages=["betby"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```


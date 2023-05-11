# Comparing `tmp/betby-0.2.3.tar.gz` & `tmp/betby-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.2.3.tar", last modified: Thu May 11 09:55:12 2023, max compression
+gzip compressed data, was "betby-0.2.4.tar", last modified: Thu May 11 10:16:12 2023, max compression
```

## Comparing `betby-0.2.3.tar` & `betby-0.2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 09:55:12.354224 betby-0.2.3/
--rw-rw-rw-   0        0        0      539 2023-05-11 09:55:12.352101 betby-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 09:55:12.332157 betby-0.2.3/betby/
--rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.3/betby/__init__.py
--rw-rw-rw-   0        0        0     6238 2023-05-11 09:53:02.000000 betby-0.2.3/betby/markets.py
-drwxrwxrwx   0        0        0        0 2023-05-11 09:55:12.349110 betby-0.2.3/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-11 09:55:10.000000 betby-0.2.3/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-11 09:55:11.000000 betby-0.2.3/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 09:55:10.000000 betby-0.2.3/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 09:55:10.000000 betby-0.2.3/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 09:55:12.354224 betby-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-11 09:53:28.000000 betby-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:16:12.149424 betby-0.2.4/
+-rw-rw-rw-   0        0        0      539 2023-05-11 10:16:12.147429 betby-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 10:16:12.127457 betby-0.2.4/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.4/betby/__init__.py
+-rw-rw-rw-   0        0        0     6248 2023-05-11 10:15:06.000000 betby-0.2.4/betby/markets.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:16:12.144436 betby-0.2.4/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-11 10:16:09.000000 betby-0.2.4/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-11 10:16:11.000000 betby-0.2.4/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 10:16:09.000000 betby-0.2.4/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 10:16:09.000000 betby-0.2.4/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 10:16:12.150422 betby-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-05-11 10:15:16.000000 betby-0.2.4/setup.py
```

### Comparing `betby-0.2.3/PKG-INFO` & `betby-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.3
+Version: 0.2.4
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.3/betby/markets.py` & `betby-0.2.4/betby/markets.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         avg_2 = self.avg_2 * (self.time_full - self.time) / self.time_full
         if self.poisson:
             matrix = np.zeros((self.poisson, self.poisson))
             for i in range(self.poisson):
                 for j in range(self.poisson):
                     prob = (exp(-avg_1) * avg_1 ** i / factorial(i)) * (
                                 exp(-avg_2) * avg_2 ** j / factorial(j))
-                    matrix[i, j] = prob
-            return matrix
+                    self.matrix[i, j] = prob
+            return self.matrix
 
     def total(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         self.result.update({'TOTAL': {'outcomes': []}})
         for val in range(2 * self.poisson):
             for i in range(self.poisson):
                 for j in range(self.poisson):
```

### Comparing `betby-0.2.3/betby.egg-info/PKG-INFO` & `betby-0.2.4/betby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.3
+Version: 0.2.4
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


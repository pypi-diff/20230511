# Comparing `tmp/fastapi2postman-0.1.0.tar.gz` & `tmp/fastapi2postman-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi2postman-0.1.0.tar", last modified: Thu May 11 12:23:16 2023, max compression
+gzip compressed data, was "fastapi2postman-0.1.1.tar", last modified: Thu May 11 12:43:32 2023, max compression
```

## Comparing `fastapi2postman-0.1.0.tar` & `fastapi2postman-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 12:23:16.032284 fastapi2postman-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-05-11 11:36:46.000000 fastapi2postman-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1241 2023-05-11 12:23:16.027230 fastapi2postman-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       35 2023-05-11 11:36:46.000000 fastapi2postman-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 12:23:16.027230 fastapi2postman-0.1.0/fastapi2postman.egg-info/
--rw-rw-rw-   0        0        0     1241 2023-05-11 12:23:15.000000 fastapi2postman-0.1.0/fastapi2postman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-05-11 12:23:15.000000 fastapi2postman-0.1.0/fastapi2postman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 12:23:15.000000 fastapi2postman-0.1.0/fastapi2postman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-11 12:23:15.000000 fastapi2postman-0.1.0/fastapi2postman.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-05-11 12:23:15.000000 fastapi2postman-0.1.0/fastapi2postman.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-11 12:23:15.000000 fastapi2postman-0.1.0/fastapi2postman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2040 2023-05-11 12:08:06.000000 fastapi2postman-0.1.0/fastapi2postman.py
--rw-rw-rw-   0        0        0       42 2023-05-11 12:23:16.034324 fastapi2postman-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1590 2023-05-11 11:54:53.000000 fastapi2postman-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:43:32.973895 fastapi2postman-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-05-11 11:36:46.000000 fastapi2postman-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1241 2023-05-11 12:43:32.973895 fastapi2postman-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1769 2023-05-11 12:37:57.000000 fastapi2postman-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 12:43:32.973895 fastapi2postman-0.1.1/fastapi2postman.egg-info/
+-rw-rw-rw-   0        0        0     1241 2023-05-11 12:43:32.000000 fastapi2postman-0.1.1/fastapi2postman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-11 12:43:32.000000 fastapi2postman-0.1.1/fastapi2postman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 12:43:32.000000 fastapi2postman-0.1.1/fastapi2postman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-11 12:43:32.000000 fastapi2postman-0.1.1/fastapi2postman.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-05-11 12:43:32.000000 fastapi2postman-0.1.1/fastapi2postman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-11 12:43:32.000000 fastapi2postman-0.1.1/fastapi2postman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2050 2023-05-11 12:38:53.000000 fastapi2postman-0.1.1/fastapi2postman.py
+-rw-rw-rw-   0        0        0       42 2023-05-11 12:43:32.989521 fastapi2postman-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1590 2023-05-11 12:41:42.000000 fastapi2postman-0.1.1/setup.py
```

### Comparing `fastapi2postman-0.1.0/LICENSE` & `fastapi2postman-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi2postman-0.1.0/PKG-INFO` & `fastapi2postman-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi2postman
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI APIs to Postman collections
 Home-page: https://github.com/ashhadahsan/fastapi2postman
 Author: Ashhad Ahsan Rehman
 Author-email: ashhadahsan@gmail.com
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastapi2postman-0.1.0/fastapi2postman.egg-info/PKG-INFO` & `fastapi2postman-0.1.1/fastapi2postman.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi2postman
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI APIs to Postman collections
 Home-page: https://github.com/ashhadahsan/fastapi2postman
 Author: Ashhad Ahsan Rehman
 Author-email: ashhadahsan@gmail.com
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastapi2postman-0.1.0/fastapi2postman.py` & `fastapi2postman-0.1.1/fastapi2postman.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,12 +61,12 @@
                 "url": f'http://{args.host}:{args.port}{route["url"]}',
                 "method": route["method"],
             },
         }
         collection["item"].append(item)
 
     with open(args.output, "w") as f:
-        json.dump(collection, f)
+        json.dump(collection, f, indent=4)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fastapi2postman-0.1.0/setup.py` & `fastapi2postman-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fastapi2postman",
-    version="0.1.0",
+    version="0.1.1",
     description="FastAPI APIs to Postman collections",
     author="Ashhad Ahsan Rehman",
     license="MIT",
     author_email="ashhadahsan@gmail.com",
     url="https://github.com/ashhadahsan/fastapi2postman",
     packages=find_packages(),
     platforms=["OS Independent"],
```


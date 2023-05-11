# Comparing `tmp/jcmutils-1.4.1.tar.gz` & `tmp/jcmutils-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.4.1.tar", last modified: Wed May 10 04:18:01 2023, max compression
+gzip compressed data, was "jcmutils-1.4.2.tar", last modified: Thu May 11 10:06:52 2023, max compression
```

## Comparing `jcmutils-1.4.1.tar` & `jcmutils-1.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 04:18:01.418849 jcmutils-1.4.1/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.1/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 04:18:01.418849 jcmutils-1.4.1/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.1/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 04:18:01.418849 jcmutils-1.4.1/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.1/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.4.1/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.1/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.1/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8781 2023-05-10 04:17:24.000000 jcmutils-1.4.1/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 04:18:01.418849 jcmutils-1.4.1/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-10 04:18:01.418849 jcmutils-1.4.1/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-05-10 04:17:38.000000 jcmutils-1.4.1/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-11 10:06:52.483250 jcmutils-1.4.2/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.2/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-11 10:06:52.483250 jcmutils-1.4.2/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.2/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-11 10:06:52.483250 jcmutils-1.4.2/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.2/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.4.2/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.2/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.2/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-11 10:05:05.000000 jcmutils-1.4.2/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-11 10:06:52.483250 jcmutils-1.4.2/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-11 10:06:52.483250 jcmutils-1.4.2/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-05-11 10:05:31.000000 jcmutils-1.4.2/setup.py
```

### Comparing `jcmutils-1.4.1/LICENSE` & `jcmutils-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.1/README.md` & `jcmutils-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.1/jcmutils/dataset_utils.py` & `jcmutils-1.4.2/jcmutils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.1/jcmutils/gen_sources.py` & `jcmutils-1.4.2/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.1/jcmutils/logger.py` & `jcmutils-1.4.2/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.1/jcmutils/solver.py` & `jcmutils-1.4.2/jcmutils/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             logger.debug(f"key {key} successfully saved")
             total_results += field
             if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
                 field = np.rot90(field, 2)
                 total_results += field
                 logger.debug("key was rotated for symmetry")
 
-        logger.debug(f"printing max value of results:{np.max(total_results)}")
+        logger.info(f"printing max value of results:{np.max(total_results)}")
         vmaxa = np.max(total_results) if vmax is None else vmax
         sfield = (total_results/ vmaxa)*235
         file_name = target_directory.rstrip('/') + '/' + "total_result.jpg"
         cv2.imwrite(file_name,sfield)
         cost_time = self.__count_time(last_time)
         logger.info(f"all target image saved completed! cost {cost_time}")
```

### Comparing `jcmutils-1.4.1/setup.py` & `jcmutils-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.4.1'
+VERSION = '1.4.2'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```


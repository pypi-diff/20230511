# Comparing `tmp/sunnydays-1.0.0.tar.gz` & `tmp/sunnydays-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunnydays-1.0.0.tar", last modified: Thu May 11 18:36:13 2023, max compression
+gzip compressed data, was "sunnydays-1.1.0.tar", last modified: Thu May 11 18:45:16 2023, max compression
```

## Comparing `sunnydays-1.0.0.tar` & `sunnydays-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:36:13.077734 sunnydays-1.0.0/
--rw-rw-rw-   0        0        0      256 2023-05-11 18:36:13.077734 sunnydays-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-11 18:36:13.077734 sunnydays-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-05-11 18:32:34.000000 sunnydays-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:36:13.060843 sunnydays-1.0.0/sunnyday/
--rw-rw-rw-   0        0        0       37 2023-05-11 18:20:18.000000 sunnydays-1.0.0/sunnyday/__init__.py
--rw-rw-rw-   0        0        0     1197 2023-05-11 18:14:49.000000 sunnydays-1.0.0/sunnyday/sunnyday.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:36:13.076614 sunnydays-1.0.0/sunnydays.egg-info/
--rw-rw-rw-   0        0        0      256 2023-05-11 18:36:13.000000 sunnydays-1.0.0/sunnydays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-11 18:36:13.000000 sunnydays-1.0.0/sunnydays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:36:13.000000 sunnydays-1.0.0/sunnydays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-11 18:36:13.000000 sunnydays-1.0.0/sunnydays.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-11 18:36:13.000000 sunnydays-1.0.0/sunnydays.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 18:45:16.900371 sunnydays-1.1.0/
+-rw-rw-rw-   0        0        0      256 2023-05-11 18:45:16.899370 sunnydays-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-11 18:45:16.900371 sunnydays-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-05-11 18:44:42.000000 sunnydays-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:45:16.884353 sunnydays-1.1.0/sunnyday/
+-rw-rw-rw-   0        0        0       37 2023-05-11 18:20:18.000000 sunnydays-1.1.0/sunnyday/__init__.py
+-rw-rw-rw-   0        0        0     1197 2023-05-11 18:14:49.000000 sunnydays-1.1.0/sunnyday/sunnyday.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:45:16.898867 sunnydays-1.1.0/sunnydays.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-05-11 18:45:16.000000 sunnydays-1.1.0/sunnydays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-11 18:45:16.000000 sunnydays-1.1.0/sunnydays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:45:16.000000 sunnydays-1.1.0/sunnydays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 18:45:16.000000 sunnydays-1.1.0/sunnydays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 18:45:16.000000 sunnydays-1.1.0/sunnydays.egg-info/top_level.txt
```

### Comparing `sunnydays-1.0.0/sunnyday/sunnyday.py` & `sunnydays-1.1.0/sunnyday/sunnyday.py`

 * *Files identical despite different names*


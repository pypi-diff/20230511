# Comparing `tmp/minipti-1.0.1.tar.gz` & `tmp/minipti-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minipti-1.0.1.tar", last modified: Mon Jan 16 09:32:55 2023, max compression
+gzip compressed data, was "minipti-1.9.0.tar", last modified: Thu May 11 14:30:46 2023, max compression
```

## Comparing `minipti-1.0.1.tar` & `minipti-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 09:32:55.894613 minipti-1.0.1/
--rw-rw-rw-   0        0        0     1082 2023-01-16 09:15:37.000000 minipti-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     8068 2023-01-16 09:32:55.894613 minipti-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7350 2023-01-16 09:22:47.000000 minipti-1.0.1/README.md
--rw-rw-rw-   0        0        0      706 2023-01-16 09:22:21.000000 minipti-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-16 09:32:55.895609 minipti-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-16 09:32:55.856591 minipti-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-16 09:32:55.881614 minipti-1.0.1/src/minipti/
--rw-rw-rw-   0        0        0       49 2023-01-16 09:15:37.000000 minipti-1.0.1/src/minipti/__init__.py
--rw-rw-rw-   0        0        0    13336 2023-01-16 09:21:54.000000 minipti-1.0.1/src/minipti/interferometry.py
--rw-rw-rw-   0        0        0     9128 2023-01-16 09:21:25.000000 minipti-1.0.1/src/minipti/pti.py
-drwxrwxrwx   0        0        0        0 2023-01-16 09:32:55.891609 minipti-1.0.1/src/minipti.egg-info/
--rw-rw-rw-   0        0        0     8068 2023-01-16 09:32:55.000000 minipti-1.0.1/src/minipti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-01-16 09:32:55.000000 minipti-1.0.1/src/minipti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 09:32:55.000000 minipti-1.0.1/src/minipti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-01-16 09:32:55.000000 minipti-1.0.1/src/minipti.egg-info/top_level.txt
+drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:30:46.018442 minipti-1.9.0/
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)     1061 2023-05-11 09:17:20.000000 minipti-1.9.0/LICENSE
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)     4493 2023-05-11 14:30:46.018442 minipti-1.9.0/PKG-INFO
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)     3736 2023-05-11 13:01:56.000000 minipti-1.9.0/README.md
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)      998 2023-05-11 10:18:58.000000 minipti-1.9.0/pyproject.toml
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)       38 2023-05-11 14:30:46.018442 minipti-1.9.0/setup.cfg
+drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:30:46.014443 minipti-1.9.0/src/
+drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:30:46.014443 minipti-1.9.0/src/minipti/
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)      239 2023-05-10 09:18:55.000000 minipti-1.9.0/src/minipti/__init__.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)      399 2023-05-08 17:02:55.000000 minipti-1.9.0/src/minipti/__main__.py
+drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:30:46.014443 minipti-1.9.0/src/minipti/algorithm/
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)       93 2023-05-09 16:58:29.000000 minipti-1.9.0/src/minipti/algorithm/__init__.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)    17825 2023-05-11 12:27:16.000000 minipti-1.9.0/src/minipti/algorithm/interferometry.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)    13828 2023-05-11 13:36:17.000000 minipti-1.9.0/src/minipti/algorithm/pti.py
+drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:30:46.018442 minipti-1.9.0/src/minipti/gui/
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)       64 2023-05-04 07:02:16.000000 minipti-1.9.0/src/minipti/gui/__init__.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)    18829 2023-05-11 06:42:56.000000 minipti-1.9.0/src/minipti/gui/controller.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)    42380 2023-05-11 13:41:38.000000 minipti-1.9.0/src/minipti/gui/model.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)    50562 2023-05-11 13:50:55.000000 minipti-1.9.0/src/minipti/gui/view.py
+drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:30:46.018442 minipti-1.9.0/src/minipti/hardware/
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)       92 2023-05-04 07:02:16.000000 minipti-1.9.0/src/minipti/hardware/__init__.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)     9105 2023-05-09 16:58:29.000000 minipti-1.9.0/src/minipti/hardware/laser.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)    15129 2023-05-11 09:08:15.000000 minipti-1.9.0/src/minipti/hardware/motherboard.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)    10783 2023-05-10 10:15:43.000000 minipti-1.9.0/src/minipti/hardware/serial_device.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)     9682 2023-05-10 09:59:50.000000 minipti-1.9.0/src/minipti/hardware/tec.py
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)     1628 2023-05-04 07:02:16.000000 minipti-1.9.0/src/minipti/json_parser.py
+drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:30:46.014443 minipti-1.9.0/src/minipti.egg-info/
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)     4493 2023-05-11 14:30:46.000000 minipti-1.9.0/src/minipti.egg-info/PKG-INFO
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)      656 2023-05-11 14:30:46.000000 minipti-1.9.0/src/minipti.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)        1 2023-05-11 14:30:46.000000 minipti-1.9.0/src/minipti.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)      129 2023-05-11 14:30:46.000000 minipti-1.9.0/src/minipti.egg-info/requires.txt
+-rw-rw-r--   0 jonas     (1000) jonas     (1000)        8 2023-05-11 14:30:46.000000 minipti-1.9.0/src/minipti.egg-info/top_level.txt
```

### Comparing `minipti-1.0.1/LICENSE` & `minipti-1.9.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 FHNW
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 FHNW
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```


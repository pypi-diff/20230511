# Comparing `tmp/pyobfuse-1.0.0.tar.gz` & `tmp/pyobfuse-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobfuse-1.0.0.tar", last modified: Thu May 11 05:06:58 2023, max compression
+gzip compressed data, was "pyobfuse-2.0.0.tar", last modified: Thu May 11 05:30:46 2023, max compression
```

## Comparing `pyobfuse-1.0.0.tar` & `pyobfuse-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 05:06:58.906778 pyobfuse-1.0.0/
--rw-rw-rw-   0        0        0      289 2023-05-11 05:06:58.906778 pyobfuse-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 05:06:58.905781 pyobfuse-1.0.0/pyobfuse.egg-info/
--rw-rw-rw-   0        0        0      289 2023-05-11 05:06:58.000000 pyobfuse-1.0.0/pyobfuse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-05-11 05:06:58.000000 pyobfuse-1.0.0/pyobfuse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 05:06:58.000000 pyobfuse-1.0.0/pyobfuse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 05:06:58.000000 pyobfuse-1.0.0/pyobfuse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 05:06:58.907767 pyobfuse-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0    34404 2023-05-11 05:06:08.000000 pyobfuse-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:30:46.817592 pyobfuse-2.0.0/
+-rw-rw-rw-   0        0        0      289 2023-05-11 05:30:46.818592 pyobfuse-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 05:30:46.817592 pyobfuse-2.0.0/pyobfuse.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-05-11 05:30:46.000000 pyobfuse-2.0.0/pyobfuse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-05-11 05:30:46.000000 pyobfuse-2.0.0/pyobfuse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:30:46.000000 pyobfuse-2.0.0/pyobfuse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:30:46.000000 pyobfuse-2.0.0/pyobfuse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:30:46.818592 pyobfuse-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0   282171 2023-05-11 05:29:34.000000 pyobfuse-2.0.0/setup.py
```


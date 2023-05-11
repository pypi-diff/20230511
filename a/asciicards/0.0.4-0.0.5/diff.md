# Comparing `tmp/asciicards-0.0.4.tar.gz` & `tmp/asciicards-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciicards-0.0.4.tar", last modified: Sun May  7 00:18:49 2023, max compression
+gzip compressed data, was "asciicards-0.0.5.tar", last modified: Sun May  7 00:28:55 2023, max compression
```

## Comparing `asciicards-0.0.4.tar` & `asciicards-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 00:18:49.415159 asciicards-0.0.4/
--rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      495 2023-05-07 00:18:49.415159 asciicards-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 00:18:49.401146 asciicards-0.0.4/asciicards/
--rw-rw-rw-   0        0        0     1483 2023-05-06 21:01:27.000000 asciicards-0.0.4/asciicards/asciicards.py
-drwxrwxrwx   0        0        0        0 2023-05-07 00:18:49.413157 asciicards-0.0.4/asciicards.egg-info/
--rw-rw-rw-   0        0        0      495 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-05-06 18:24:32.000000 asciicards-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 00:18:49.416160 asciicards-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      520 2023-05-07 00:18:23.000000 asciicards-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:28:55.709711 asciicards-0.0.5/
+-rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      542 2023-05-07 00:28:55.708710 asciicards-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.5/README.md
+-rw-rw-rw-   0        0        0      435 2023-05-07 00:28:33.000000 asciicards-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 00:28:55.709711 asciicards-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 00:28:55.689694 asciicards-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 00:28:55.695698 asciicards-0.0.5/src/asciicards/
+-rw-rw-rw-   0        0        0        0 2023-05-07 00:04:42.000000 asciicards-0.0.5/src/asciicards/__init__.py
+-rw-rw-rw-   0        0        0     1483 2023-05-06 21:01:27.000000 asciicards-0.0.5/src/asciicards/asciicards.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:28:55.706709 asciicards-0.0.5/src/asciicards.egg-info/
+-rw-rw-rw-   0        0        0      542 2023-05-07 00:28:55.000000 asciicards-0.0.5/src/asciicards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-07 00:28:55.000000 asciicards-0.0.5/src/asciicards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 00:28:55.000000 asciicards-0.0.5/src/asciicards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 00:28:55.000000 asciicards-0.0.5/src/asciicards.egg-info/top_level.txt
```

### Comparing `asciicards-0.0.4/LICENSE` & `asciicards-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asciicards-0.0.4/asciicards/asciicards.py` & `asciicards-0.0.5/src/asciicards/asciicards.py`

 * *Files identical despite different names*


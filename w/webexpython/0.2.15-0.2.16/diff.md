# Comparing `tmp/webexpython-0.2.15.tar.gz` & `tmp/webexpython-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexpython-0.2.15.tar", last modified: Tue Apr  4 14:52:04 2023, max compression
+gzip compressed data, was "webexpython-0.2.16.tar", last modified: Thu May 11 14:48:16 2023, max compression
```

## Comparing `webexpython-0.2.15.tar` & `webexpython-0.2.16.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 josh       (501) staff       (20)        0 2023-04-04 14:52:04.000000 webexpython-0.2.15/
--rwxrwxrwx   0 josh       (501) staff       (20)      151 2023-04-04 14:52:04.000000 webexpython-0.2.15/PKG-INFO
--rwxrwxrwx   0 josh       (501) staff       (20)       38 2023-04-04 14:52:04.000000 webexpython-0.2.15/setup.cfg
--rwxrwxrwx   0 josh       (501) staff       (20)      327 2023-04-04 14:52:01.000000 webexpython-0.2.15/setup.py
-drwxrwxrwx   0 josh       (501) staff       (20)        0 2023-04-04 14:52:04.000000 webexpython-0.2.15/webexpython/
--rwxrwxrwx   0 josh       (501) staff       (20)       20 2022-03-17 16:32:34.000000 webexpython-0.2.15/webexpython/__init__.py
--rwxrwxrwx   0 josh       (501) staff       (20)    17953 2023-04-04 14:50:38.000000 webexpython-0.2.15/webexpython/webex.py
-drwxrwxrwx   0 josh       (501) staff       (20)        0 2023-04-04 14:52:04.000000 webexpython-0.2.15/webexpython.egg-info/
--rwxrwxrwx   0 josh       (501) staff       (20)      151 2023-04-04 14:52:04.000000 webexpython-0.2.15/webexpython.egg-info/PKG-INFO
--rwxrwxrwx   0 josh       (501) staff       (20)      227 2023-04-04 14:52:04.000000 webexpython-0.2.15/webexpython.egg-info/SOURCES.txt
--rwxrwxrwx   0 josh       (501) staff       (20)        1 2023-04-04 14:52:04.000000 webexpython-0.2.15/webexpython.egg-info/dependency_links.txt
--rwxrwxrwx   0 josh       (501) staff       (20)        9 2023-04-04 14:52:04.000000 webexpython-0.2.15/webexpython.egg-info/requires.txt
--rwxrwxrwx   0 josh       (501) staff       (20)       12 2023-04-04 14:52:04.000000 webexpython-0.2.15/webexpython.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-11 14:48:16.779152 webexpython-0.2.16/
+-rw-r--r--   0 josh       (501) staff       (20)      198 2023-05-11 14:48:16.778724 webexpython-0.2.16/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-05-11 14:48:16.779289 webexpython-0.2.16/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      327 2023-05-11 14:47:24.000000 webexpython-0.2.16/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-11 14:48:16.775563 webexpython-0.2.16/webexpython/
+-rw-r--r--   0 josh       (501) staff       (20)       20 2022-03-17 16:32:34.000000 webexpython-0.2.16/webexpython/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    24824 2023-05-11 14:47:05.000000 webexpython-0.2.16/webexpython/webex.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-11 14:48:16.778028 webexpython-0.2.16/webexpython.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      198 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      227 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        9 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       12 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/top_level.txt
```


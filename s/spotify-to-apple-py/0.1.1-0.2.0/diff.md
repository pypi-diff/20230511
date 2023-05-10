# Comparing `tmp/spotify-to-apple-py-0.1.1.tar.gz` & `tmp/spotify-to-apple-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-to-apple-py-0.1.1.tar", last modified: Thu Mar 30 04:21:57 2023, max compression
+gzip compressed data, was "dist/spotify-to-apple-py-0.2.0.tar", last modified: Wed May 10 22:13:36 2023, max compression
```

## Comparing `spotify-to-apple-py-0.1.1.tar` & `spotify-to-apple-py-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,9 @@
-drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-03-30 04:21:57.836286 spotify-to-apple-py-0.1.1/
--rw-r--r--   0 bezaamsalu   (501) staff       (20)     1074 2023-02-20 03:14:06.000000 spotify-to-apple-py-0.1.1/LICENSE
--rw-r--r--   0 bezaamsalu   (501) staff       (20)     5628 2023-03-30 04:21:57.835991 spotify-to-apple-py-0.1.1/PKG-INFO
--rw-r--r--   0 bezaamsalu   (501) staff       (20)     3532 2023-03-30 03:52:01.000000 spotify-to-apple-py-0.1.1/README.md
--rw-r--r--   0 bezaamsalu   (501) staff       (20)     2343 2023-03-30 04:10:18.000000 spotify-to-apple-py-0.1.1/pyproject.toml
--rw-r--r--   0 bezaamsalu   (501) staff       (20)       38 2023-03-30 04:21:57.836359 spotify-to-apple-py-0.1.1/setup.cfg
--rw-r--r--   0 bezaamsalu   (501) staff       (20)       38 2023-03-27 01:18:54.000000 spotify-to-apple-py-0.1.1/setup.py
-drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-03-30 04:21:57.833475 spotify-to-apple-py-0.1.1/src/
--rw-r--r--   0 bezaamsalu   (501) staff       (20)        0 2023-03-04 01:27:49.000000 spotify-to-apple-py-0.1.1/src/__init__.py
--rw-r--r--   0 bezaamsalu   (501) staff       (20)     8910 2023-03-30 02:28:47.000000 spotify-to-apple-py-0.1.1/src/spotify_client.py
-drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-03-30 04:21:57.835457 spotify-to-apple-py-0.1.1/src/spotify_to_apple_py.egg-info/
--rw-r--r--   0 bezaamsalu   (501) staff       (20)     5628 2023-03-30 04:21:57.000000 spotify-to-apple-py-0.1.1/src/spotify_to_apple_py.egg-info/PKG-INFO
--rw-r--r--   0 bezaamsalu   (501) staff       (20)      313 2023-03-30 04:21:57.000000 spotify-to-apple-py-0.1.1/src/spotify_to_apple_py.egg-info/SOURCES.txt
--rw-r--r--   0 bezaamsalu   (501) staff       (20)        1 2023-03-30 04:21:57.000000 spotify-to-apple-py-0.1.1/src/spotify_to_apple_py.egg-info/dependency_links.txt
--rw-r--r--   0 bezaamsalu   (501) staff       (20)      250 2023-03-30 04:21:57.000000 spotify-to-apple-py-0.1.1/src/spotify_to_apple_py.egg-info/requires.txt
--rw-r--r--   0 bezaamsalu   (501) staff       (20)       24 2023-03-30 04:21:57.000000 spotify-to-apple-py-0.1.1/src/spotify_to_apple_py.egg-info/top_level.txt
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      265 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/PKG-INFO
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      265 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/PKG-INFO
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      180 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/SOURCES.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)        1 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/top_level.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)        1 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/dependency_links.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      318 2023-05-10 22:13:17.000000 spotify-to-apple-py-0.2.0/setup.py
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)       59 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```


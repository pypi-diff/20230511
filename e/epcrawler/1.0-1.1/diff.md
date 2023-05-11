# Comparing `tmp/epcrawler-1.0.tar.gz` & `tmp/epcrawler-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epcrawler-1.0.tar", last modified: Tue Apr 25 22:15:07 2023, max compression
+gzip compressed data, was "epcrawler-1.1.tar", last modified: Thu May 11 18:06:55 2023, max compression
```

## Comparing `epcrawler-1.0.tar` & `epcrawler-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 22:15:07.434236 epcrawler-1.0/
--rw-rw-rw-   0        0        0    35823 2023-04-25 20:37:14.000000 epcrawler-1.0/LICENSE
--rw-rw-rw-   0        0        0     2024 2023-04-25 22:15:07.434236 epcrawler-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1505 2023-04-25 22:04:04.000000 epcrawler-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 22:15:07.420566 epcrawler-1.0/epcrawler/
--rw-rw-rw-   0        0        0        0 2023-04-25 21:26:30.000000 epcrawler-1.0/epcrawler/__init__.py
--rw-rw-rw-   0        0        0      680 2023-04-25 21:29:54.000000 epcrawler-1.0/epcrawler/__main__.py
--rw-rw-rw-   0        0        0     1738 2023-04-25 21:29:08.000000 epcrawler-1.0/epcrawler/anime_finder.py
--rw-rw-rw-   0        0        0      541 2023-04-25 19:41:37.000000 epcrawler-1.0/epcrawler/test_anime_finder.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:15:07.432283 epcrawler-1.0/epcrawler.egg-info/
--rw-rw-rw-   0        0        0     2024 2023-04-25 22:15:07.000000 epcrawler-1.0/epcrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-04-25 22:15:07.000000 epcrawler-1.0/epcrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 22:15:07.000000 epcrawler-1.0/epcrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-25 22:15:07.000000 epcrawler-1.0/epcrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-04-25 22:15:07.000000 epcrawler-1.0/epcrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 22:15:07.000000 epcrawler-1.0/epcrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      216 2023-04-25 22:15:07.436189 epcrawler-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-04-25 22:14:59.000000 epcrawler-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:55.128660 epcrawler-1.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-25 20:37:14.000000 epcrawler-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2081 2023-05-11 18:06:55.128660 epcrawler-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1562 2023-04-25 22:58:47.000000 epcrawler-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:55.111088 epcrawler-1.1/epcrawler/
+-rw-rw-rw-   0        0        0       39 2023-05-11 17:51:40.000000 epcrawler-1.1/epcrawler/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-05-11 17:44:30.000000 epcrawler-1.1/epcrawler/__main__.py
+-rw-rw-rw-   0        0        0     1682 2023-05-11 17:52:42.000000 epcrawler-1.1/epcrawler/epcrawler.py
+-rw-rw-rw-   0        0        0      534 2023-05-11 17:53:58.000000 epcrawler-1.1/epcrawler/test_anime_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:55.126699 epcrawler-1.1/epcrawler.egg-info/
+-rw-rw-rw-   0        0        0     2081 2023-05-11 18:06:54.000000 epcrawler-1.1/epcrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-05-11 18:06:54.000000 epcrawler-1.1/epcrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:06:54.000000 epcrawler-1.1/epcrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-11 18:06:54.000000 epcrawler-1.1/epcrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-05-11 18:06:54.000000 epcrawler-1.1/epcrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 18:06:54.000000 epcrawler-1.1/epcrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      216 2023-05-11 18:06:55.130614 epcrawler-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-05-11 17:49:07.000000 epcrawler-1.1/setup.py
```

### Comparing `epcrawler-1.0/LICENSE` & `epcrawler-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epcrawler-1.0/PKG-INFO` & `epcrawler-1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epcrawler
-Version: 1.0
+Version: 1.1
 Summary: Scraper to extract episode names from anidb
 Home-page: https://github.com/dgsmiley18/epcrawler
 Author: Douglas Vianna
 Author-email: douglasvianna230@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -14,14 +14,15 @@
 License-File: LICENSE
 
 # Anime Episode Name Scraper
 
 ![GitHub stars](https://img.shields.io/github/stars/dgsmiley18/EpCrawler.svg?style=social&label=Star&maxAge=2592000)
 ![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
 ![License](https://img.shields.io/badge/license-GPLv3-blue.svg)
+![Pip url](https://img.shields.io/pypi/v/epcrawler.svg)
 
 ## **epcrawler** - get episode names from anidb
 
 ## 🎨 Table of Contents
 
 - [Anime Episode Name Scraper](#anime-episode-name-scraper)
   - [**epcrawler** - get episode names from anidb](#epcrawler---get-episode-names-from-anidb)
```

### Comparing `epcrawler-1.0/README.md` & `epcrawler-1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Anime Episode Name Scraper
 
 ![GitHub stars](https://img.shields.io/github/stars/dgsmiley18/EpCrawler.svg?style=social&label=Star&maxAge=2592000)
 ![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
 ![License](https://img.shields.io/badge/license-GPLv3-blue.svg)
+![Pip url](https://img.shields.io/pypi/v/epcrawler.svg)
 
 ## **epcrawler** - get episode names from anidb
 
 ## 🎨 Table of Contents
 
 - [Anime Episode Name Scraper](#anime-episode-name-scraper)
   - [**epcrawler** - get episode names from anidb](#epcrawler---get-episode-names-from-anidb)
```

### Comparing `epcrawler-1.0/epcrawler/__main__.py` & `epcrawler-1.1/epcrawler/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from anime_finder import get_episode_name
+from epcrawler import get_episode_name
 import argparse
-parser = argparse.ArgumentParser(
-    prog="Episode Finder",
-    description="Find the episodes names from your favorite anime!",
-)
 
-# Adds the "--name" argument with an explanation
-parser.add_argument(
-    "-n", 
-    "--name", 
-    help="specify the anime name", 
-    type=str, 
-    required=True,
-)
-parser.add_argument(
-    "-o",
-    "--output",
-    help="specify the output file",
-    default="titles.txt",
-    type=str,
-    required=False,
-)
-if __name__ == "__main__":
-    args = parser.parse_args()
+def main():
+    parser = argparse.ArgumentParser(
+        prog="Episode Finder",
+        description="Find the episodes names from your favorite anime!",
+    )
+
+    # Adds the "--name" argument with an explanation
+    parser.add_argument(
+        "-n", 
+        "--name", 
+        help="specify the anime name", 
+        type=str, 
+        required=True,
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        help="specify the output file",
+        default="titles.txt",
+        type=str,
+        required=False,
+    )
 
     # Displays the information on the console
-    get_episode_name(args.name, args.output)
+    args = parser.parse_args()
+    get_episode_name(args.name, args.output)
+if __name__ == "__main__":
+    main()
```

### Comparing `epcrawler-1.0/epcrawler/anime_finder.py` & `epcrawler-1.1/epcrawler/epcrawler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-import argparse
 from bs4 import BeautifulSoup
 
 
 def get_episode_name(anime_name, output_file):
     # Remove the spaces and replace them with a plus sign
     anime_name = anime_name.replace(" ", "+")
     headers = {
@@ -29,16 +28,15 @@
                 # Find the episode name
                 for tr in trs:
                     ep_name = tr.find("td", class_="title name episode").get_text()
                     # Remove the new line
                     ep_name = ep_name.replace("\n", "")
                     # Remove the spaces
                     ep_name = ep_name.replace(" ", ".")
-                    # print(ep_name)
-                    # escreva os nomes dos episódios no arquivo
+                    # Type the name of the episodes on the file
                     writer.write(ep_name + "\n")
             return print("The file was created successfully!")
         else:
             return print("The output file must be a .txt file")
     except Exception as e:
         print("Error: ", e)
         return None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `epcrawler-1.0/epcrawler/test_anime_finder.py` & `epcrawler-1.1/epcrawler/test_anime_finder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import subprocess
-from anime_finder import get_episode_name
+from epcrawler import get_episode_name
 
 
 def test_episode_name():
     anime_name = "Boku no Hero Academia"
     output_file = "bokunohero.txt"
     get_episode_name(anime_name, output_file)
     with open(output_file, "r") as f:
         content = f.read()
         assert "Izuku.Midoriya:.Origin" in content
         assert "What.It.Takes.to.Be.a.Hero" in content
 
 
 def test_help():
-    output = subprocess.check_output(["python", "anime_finder.py", "--help"])
+    output = subprocess.check_output(["python", "__main__.py", "--help"])
     assert b"specify the anime name" in output
```

### Comparing `epcrawler-1.0/epcrawler.egg-info/PKG-INFO` & `epcrawler-1.1/epcrawler.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epcrawler
-Version: 1.0
+Version: 1.1
 Summary: Scraper to extract episode names from anidb
 Home-page: https://github.com/dgsmiley18/epcrawler
 Author: Douglas Vianna
 Author-email: douglasvianna230@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -14,14 +14,15 @@
 License-File: LICENSE
 
 # Anime Episode Name Scraper
 
 ![GitHub stars](https://img.shields.io/github/stars/dgsmiley18/EpCrawler.svg?style=social&label=Star&maxAge=2592000)
 ![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
 ![License](https://img.shields.io/badge/license-GPLv3-blue.svg)
+![Pip url](https://img.shields.io/pypi/v/epcrawler.svg)
 
 ## **epcrawler** - get episode names from anidb
 
 ## 🎨 Table of Contents
 
 - [Anime Episode Name Scraper](#anime-episode-name-scraper)
   - [**epcrawler** - get episode names from anidb](#epcrawler---get-episode-names-from-anidb)
```

### Comparing `epcrawler-1.0/setup.py` & `epcrawler-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     author_email=metadata['author_email'],
     description=metadata['description'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dgsmiley18/epcrawler",
     packages=["epcrawler"],
     license="GPLv3",
-    entry_points={'console_scripts': ['anime_finder=epcrawler.anime_finder:main']},
+    entry_points={'console_scripts': ['epcrawler=epcrawler.__main__:main']},
     install_requires=[
         "beautifulsoup4",
         "requests"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```


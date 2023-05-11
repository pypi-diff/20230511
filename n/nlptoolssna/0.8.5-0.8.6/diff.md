# Comparing `tmp/nlptoolssna-0.8.5.tar.gz` & `tmp/nlptoolssna-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.8.5.tar", last modified: Sat May  6 12:05:34 2023, max compression
+gzip compressed data, was "nlptoolssna-0.8.6.tar", last modified: Thu May 11 20:52:33 2023, max compression
```

## Comparing `nlptoolssna-0.8.5.tar` & `nlptoolssna-0.8.6.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.705833 nlptoolssna-0.8.5/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-06 12:05:34.705833 nlptoolssna-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.598487 nlptoolssna-0.8.5/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.5/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.560725 nlptoolssna-0.8.5/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.560725 nlptoolssna-0.8.5/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.598487 nlptoolssna-0.8.5/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.5/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.606618 nlptoolssna-0.8.5/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.5/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.5/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.5/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.5/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.5/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.622745 nlptoolssna-0.8.5/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.622745 nlptoolssna-0.8.5/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.5/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.633791 nlptoolssna-0.8.5/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.633791 nlptoolssna-0.8.5/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.5/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.5/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.633791 nlptoolssna-0.8.5/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.5/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.5/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.641863 nlptoolssna-0.8.5/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.8.5/docs/source/api/utils/implication.rst
--rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.8.5/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.8.5/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      240 2023-05-06 11:52:16.000000 nlptoolssna-0.8.5/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.8.5/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.5/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.5/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.8.5/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.5/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.649919 nlptoolssna-0.8.5/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.658589 nlptoolssna-0.8.5/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.5/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.8.5/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.8.5/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.665309 nlptoolssna-0.8.5/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.5/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.8.5/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.8.5/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.8.5/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.8.5/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.8.5/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.673385 nlptoolssna-0.8.5/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.5/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.681328 nlptoolssna-0.8.5/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.5/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.5/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     5289 2023-05-06 11:26:00.000000 nlptoolssna-0.8.5/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.5/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.8.5/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.689507 nlptoolssna-0.8.5/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.5/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0    20573 2023-05-06 11:00:30.000000 nlptoolssna-0.8.5/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0    10525 2023-05-06 12:04:58.000000 nlptoolssna-0.8.5/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     9525 2023-05-06 12:02:03.000000 nlptoolssna-0.8.5/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.5/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.705833 nlptoolssna-0.8.5/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-06 12:05:34.000000 nlptoolssna-0.8.5/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2023-05-06 12:05:34.000000 nlptoolssna-0.8.5/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 12:05:34.000000 nlptoolssna-0.8.5/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-06 12:05:34.000000 nlptoolssna-0.8.5/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.5/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-06 12:05:34.000000 nlptoolssna-0.8.5/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 12:05:34.000000 nlptoolssna-0.8.5/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-06 12:05:34.705833 nlptoolssna-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:34.705833 nlptoolssna-0.8.5/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.5/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.868660 nlptoolssna-0.8.6/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-11 20:52:33.868660 nlptoolssna-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.785004 nlptoolssna-0.8.6/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.6/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.759067 nlptoolssna-0.8.6/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.760070 nlptoolssna-0.8.6/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.786001 nlptoolssna-0.8.6/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.6/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.791004 nlptoolssna-0.8.6/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.6/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.6/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.6/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.6/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.802168 nlptoolssna-0.8.6/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.803165 nlptoolssna-0.8.6/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.6/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.807202 nlptoolssna-0.8.6/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.808790 nlptoolssna-0.8.6/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.6/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.6/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.811812 nlptoolssna-0.8.6/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.6/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.6/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.818808 nlptoolssna-0.8.6/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.8.6/docs/source/api/utils/implication.rst
+-rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.8.6/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.8.6/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.8.6/docs/source/api/utils/text_transliteration.rst
+-rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.8.6/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.8.6/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.6/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.8.6/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.6/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.821808 nlptoolssna-0.8.6/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.825393 nlptoolssna-0.8.6/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.6/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     5067 2023-05-11 20:27:50.000000 nlptoolssna-0.8.6/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.8.6/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.834394 nlptoolssna-0.8.6/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.6/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.8.6/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.8.6/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.8.6/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.8.6/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.8.6/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.836393 nlptoolssna-0.8.6/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.6/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.844621 nlptoolssna-0.8.6/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.6/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.6/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     6376 2023-05-08 18:11:31.000000 nlptoolssna-0.8.6/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.6/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.8.6/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.853623 nlptoolssna-0.8.6/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.6/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    26235 2023-05-11 20:51:14.000000 nlptoolssna-0.8.6/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0    10287 2023-05-11 20:50:47.000000 nlptoolssna-0.8.6/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     7556 2023-05-11 20:46:42.000000 nlptoolssna-0.8.6/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0     9283 2023-05-08 19:13:30.000000 nlptoolssna-0.8.6/nlptools/utils/text_transliteration.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.6/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.864661 nlptoolssna-0.8.6/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-11 20:52:33.000000 nlptoolssna-0.8.6/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1758 2023-05-11 20:52:33.000000 nlptoolssna-0.8.6/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 20:52:33.000000 nlptoolssna-0.8.6/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-11 20:52:33.000000 nlptoolssna-0.8.6/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.6/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-11 20:52:33.000000 nlptoolssna-0.8.6/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 20:52:33.000000 nlptoolssna-0.8.6/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-11 20:52:33.870733 nlptoolssna-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:33.867658 nlptoolssna-0.8.6/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.6/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.8.5/CONTRIBUTING.rst` & `nlptoolssna-0.8.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/LICENSE` & `nlptoolssna-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/PKG-INFO` & `nlptoolssna-0.8.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.5/README.rst` & `nlptoolssna-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/docs/Makefile` & `nlptoolssna-0.8.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/docs/build/html/_images/download.png` & `nlptoolssna-0.8.6/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/docs/build/html/_static/download.png` & `nlptoolssna-0.8.6/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/docs/make.bat` & `nlptoolssna-0.8.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/docs/source/_static/download.png` & `nlptoolssna-0.8.6/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/docs/source/conf.py` & `nlptoolssna-0.8.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/docs/source/installation.rst` & `nlptoolssna-0.8.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.8.6/nlptools/DataDownload/downloader.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,56 +2,80 @@
 import sys
 from pathlib import Path
 import requests  
 import zipfile
 from tqdm import tqdm
 
 urls = {
-    'morph':'https://portal.sina.birzeit.edu/ALMA27012000.pickle'
-    # 'ner': 'http://portal.sina.birzeit.edu/Wj27012000.zip',
+    'morph': 'https://portal.sina.birzeit.edu/ALMA27012000.pickle',
+    'ner': 'http://portal.sina.birzeit.edu/Wj27012000.zip'
+}
+
 #     'salma': 'http://portal.sina.birzeit.edu/SALMA27012000.zip',
 #     'salma2021': 'http://portal.sina.birzeit.edu/SALMA_v2.zip'
 # 
-}
+
 
 def get_appdatadir():
     """
-    Returns the path to the directory where the application data is stored.
-
+    This method checks if the directory exists and creates if it doesn't. And returns the path to the directory where the application data is stored.
+   
     Returns:
     --------
     Path: A pathlib.Path object representing the path to the application data directory.
 
     Raises:
     -------
     None.
 
     **Example:**
 
     .. highlight:: python
     .. code-block:: python
-    
-        get_appdatadir()
+
+        from nlptools.DataDownload import downloader
+
+        path = downloader.get_appdatadir()
 
         Windows: 'C:/Users/<Username>/AppData/Roaming/nlptools'
         MacOS: '/Users/<Username>/Library/Application Support/nlptools'
         Linux: '/home/<Username>/.nlptools'
         Google Colab: '/content/nlptools'
 
     """
     home = str(Path.home())
 
+    # if 'google.colab' in sys.modules:
+    #     return Path('/content/nlptools')
+    # elif sys.platform == 'win32':
+    #     return Path(home, 'AppData/Roaming/nlptools')
+    # elif sys.platform == 'darwin':
+    #     return Path(home, 'Library/Application Support/nlptools')
+    # else:
+    #     return Path(home, '.nlptools')
+
     if 'google.colab' in sys.modules:
-        return Path('/content/nlptools')
+        path = Path('/content/nlptools')
     elif sys.platform == 'win32':
-        return Path(home, 'AppData/Roaming/nlptools')
+        path = Path(home, 'AppData/Roaming/nlptools')
     elif sys.platform == 'darwin':
-        return Path(home, 'Library/Application Support/nlptools')
+        path = Path(home, 'Library/Application Support/nlptools')
     else:
-        return Path(home, '.nlptools')
+        path = Path(home, '.nlptools')
+
+    if not os.path.exists(path):
+        os.makedirs(path)
+
+    return path
+
+
+
+
+
+
 
 
 
 def download_file(url, dest_path=get_appdatadir()):
     """
     Downloads a file from the specified URL and saves it to the specified destination path.
 
@@ -122,12 +146,29 @@
 
     Returns:
         None
     """
     for url in urls.values():
         download_file(url)
 
+def download_files(key=None):
+    """
+    Downloads multiple files from a dictionary of urls using the download_file() function.
+
+    Args:
+        key (optional): The key of the dictionary to specify which URLs to download. If not provided, all URLs will be downloaded.
+
+    Returns:
+        None
+    """
+    if key is None:
+        urls_to_download = urls.values()
+    else:
+        urls_to_download = [urls[key]]
+
+    for url in urls_to_download:
+        download_file(url)
 
 
 
 
 #download_file(downloadLink ,_get_appdatadir())
```

### Comparing `nlptoolssna-0.8.5/nlptools/arabiner/data.py` & `nlptoolssna-0.8.6/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/arabiner/datasets.py` & `nlptoolssna-0.8.6/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/arabiner/helpers.py` & `nlptoolssna-0.8.6/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/arabiner/infer.py` & `nlptoolssna-0.8.6/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/arabiner/transforms.py` & `nlptoolssna-0.8.6/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/data/my_data.pickle` & `nlptoolssna-0.8.6/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/morphology/charsets.py` & `nlptoolssna-0.8.6/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.8.6/nlptools/morphology/morph_analyzer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,86 @@
 
 from nlptools.morphology import settings 
 import re
 from nlptools.morphology.tokenizers_words import simple_word_tokenize
 from nlptools.utils.parser import arStrip
-from nlptools.DataDownload import downloader
 from nlptools.morphology.charsets import AR_CHARSET, AR_DIAC_CHARSET
-import copy
 
 _IS_AR_RE = re.compile(u'^[' + re.escape(u''.join(AR_CHARSET)) + u']+$')
 def find_solution(token, language, task):
     """
     Given a token, this method finds the morphological solution lemma and/or pos based on a spesific language and task.
           
     Args:
-        - token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
-        - language (:obj:`str`): In the current version, `MSA` is only supported. 
-        - task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
+        token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
+        language (:obj:`str`): In the current version, `MSA` is only supported. 
+        task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
 
     Returns:
         list (:obj:`list`): A list of [token, lemma, pos], where:
-            - token: the original input token
-            - lemma: the lemma of the token 
-            - pos: the part-of-speech of the token 
-            If no sloution is found for this token, an empty list is returned.
+           token: the original input token
+           lemma: the lemma of the token 
+           pos: the part-of-speech of the token 
+    Note:
+        If no sloution is found for this token, an empty list is returned.
     """
     if token in settings.div_dic.keys():
         soluation = settings.div_dic[token]
         return  [token, soluation[0], soluation[1]]               
     else:
         return []
 
 def analyze(text, language ='MSA', task ='full'):
    """
     This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that,
     if:
-         - the task is lemmatizer, then the morphological soltuion is only the lemma.
-         - the task is pos, then the morphological soltuion is only the pos.
-         - the task is full, the the morphological soltuion is both the lemma and the pos.
+        the task is lemmatizer, then the morphological soltuion is only the lemma.
+        the task is pos, then the morphological soltuion is only the pos.
+        the task is full, the the morphological soltuion is both the lemma and the pos.
      
     Args:
-        - token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
-        - language (:obj:`str`): In the current version, `MSA` is only supported. 
-        - task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
+        token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
+        language (:obj:`str`): In the current version, `MSA` is only supported. 
+        task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
          
     Returns:
         list (:obj:`list`): A list of [token, lemma, pos], based on the spesified task, where:
-            - token: the original input token
-            - lemma: the lemma of the token 
-            - pos: the part-of-speech of the token 
+           token: the original input token
+           lemma: the lemma of the token 
+           pos: the part-of-speech of the token 
 
-    """
-  
+    **Example:**
+
+     .. highlight:: python
+     .. code-block:: python
+     
+          from nlptools.morphology  import morph_analyzer
+     
+          Return the morpological solution for each token in this text
+          Exampel: task = full 
+          morph_analyzer.analyze('ذهب الولد الى المدرسة')
+           
+           [['ذهب', 'ذَهَبَ۪ 1', 'فعل'],
+           ['الولد', 'وَلَد 1', 'اسم'],
+           ['الى', 'إِلَى 1', 'كلمة وظيفية'],
+           ['المدرسة', 'مَدْرَسَة 1', 'اسم']]
+
+           Exampel: task = pos
+           morph_analyzer.analyze('ذهب الولد الى المدرسة',task='pos')
+           #the output
+           [['ذهب', 'فعل'], ['الولد', 'اسم'], ['الى', 'كلمة وظيفية'], ['المدرسة', 'اسم']]
+
+           Exampel: task = lemmatizer
+           morph_analyzer.analyze('طار العصور فوق الشجرة', task='lemmatizer')
+           [['طار', 'طارِ۪ 1'],
+            ['العصور', 'عَصْر 1'],
+            ['فوق', 'فَوْق 1'],
+            ['الشجرة', 'شَجَرَة 1']]
+     """
+ 
    #@check if the init does not load data correctly, call load_alma inside
    output_list = []
 
    tokens = simple_word_tokenize(text)
 
    for token in tokens:
          result_token =[]
```

### Comparing `nlptoolssna-0.8.5/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.8.6/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/nlptools/utils/implication.py` & `nlptoolssna-0.8.6/nlptools/utils/implication.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Created: 16/03/2021 , By Mohammad A'bed
 # Trello task: https://trello.com/c/nHnmnFAe/19-re-implement-implication-function-in-python
 
 #  The Imply algorithm takes two words as input and produces the matching tuple defined by (Words Matching).
 #  The matching between two words is defined as a tuple:
 #  <w1, w2, implication direction, distance, conflicts, verdict, preferredWord> .
-
+from nlptools.utils.parser import arStrip
 
 class Implication:
+    """
+    The Imply algorithm takes two words as input and produces the matching tuple defined by (Words Matching).
+    he matching between two words is defined as a tuple:
+    <w1, w2, implication direction, distance, conflicts, verdict, preferredWord> .
+    """
     # Diacritic Pair Distance Map
     distanceTable = [
     [0, 0, 1, 1, 1, 1, 1, 1, 15, 16, 16, 16, 0, 0, 0, 0 ],
     [0, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
     [1, 101, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
     [1, 101, 101, 0, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
     [1, 101, 101, 101, 0, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
@@ -66,271 +71,415 @@
             self.verdict = "Incompatible"
             self.direction = -3 # the two words have different letters
             self.distance = 3000
             self.conflicts = 0
             return
 
         self.conflictFlags =  [False for i in range(5)] # reset conflictFlags array to Fales
-        self.word1 = Implication.normalize(inputWord1) # unify alif 
-        self.word2 = Implication.normalize(inputWord2) # unify alif 
+        self.word1 = Implication.normalize_alef(inputWord1) # unify alif 
+        self.word2 = Implication.normalize_alef(inputWord2) # unify alif 
 
         if ( self.word1 ==  self.word2): # If w1 == w2 returns the values bellow 
             self.verdict = "Compatible"
             self.direction = 3 #  Both letters have exactly the same diacritics 
             self.distance = 0
             self.conflicts = 0
             return
         else: # If w1 and w2 are noot exact match
             try:
                 self.lettersDirection = []
                 # build diacritics array for each word 
-                self.word1Diacritics = Implication.getDiacriticsArray(self.word1)
-                self.word2Diacritics = Implication.getDiacriticsArray(self.word2)
+                self.word1Diacritics = Implication.calculate_direction(self.word1)
+                self.word2Diacritics = Implication.calculate_direction(self.word2)
 
                  # defined lettersDirection array with size of word1Diacritics and fill it by zeros
                 for x in range(0 , len(self.word1Diacritics) + 1): 
                     self.lettersDirection.append(0)
             except :
                 # In case of errors returns the values below 
                 self.verdict = "Incompatible"
                 self.direction = -3 # the two words have different letters
                 self.distance = 3000
                 self.conflicts = 0
                 return
 
             # check if diacritics in both words for some of syntax errors then return Incompatible
-            if (  Implication.diacriticsSyntaxErrorIn(self.word1Diacritics) == False and  Implication.diacriticsSyntaxErrorIn(self.word2Diacritics) == False) : 
+            if (Implication.diacriticsSyntaxErrorIn(self.word1Diacritics) == False and  Implication.diacriticsSyntaxErrorIn(self.word2Diacritics) == False) : 
                 # If no syntax error found:
                 self.word1Undiac = Implication.removeDiacritics(self.word1)
                 self.word2Undiac = Implication.removeDiacritics(self.word2)
                 # return compatible if each word is one and same letter regardless of diacritics on this letter
                 if (len(self.word1Undiac) == 1 and len(self.word2Undiac) == 1 and self.word1Undiac == self.word2Undiac): 
                         self.verdict = "Compatible"
                         self.direction = 3  #  Both letters have exactly the same diacritics 
                         self.distance = 0
                         self.conflicts = 0
                 else : # If words are more than letter or deffirent letter then calculate the impication
                     self.lettersDirection[0] = 3 
-                    self.calculateWordsImplication()
+                    self.calculate_words_implication()
                 
             else : # If found syntax error in diacitics in word1 or word2 then return these:
                 self.verdict = "Incompatible"
                 self.direction = -3 # the two words have different letters
                 self.distance = 3000
                 self.conflicts = 0
             
-    def getNonPreferredWord( self , word1,  word2) :
+    def get_non_preferred_word( self , word1,  word2) :
         # this function talkes 2-words and retuen preferredWord 
         word1 = word1.strip()
         word2 = word2.strip()
         if (word1 != "null" and  word1.strip() ) :
             if (word2 != "null" and word2.strip()) :
                 preferredWord = ""
-                preferredWord = Implication.getPreferredWord(word1, word2)
+                preferredWord = Implication.get_preferred_word(word1, word2)
                 if word1== preferredWord:
                     return word2
                 else:
                     return word1
             else :
                 return word1
         
         else :
             if word2 != "null" and word2.strip():
                 return word2 
             else:
                 return "null"
-    def getPreferredWord( self , word1,   word2) :
+    def get_preferred_word( self , word1,   word2) :
         word1 = word1.strip()
         word2 = word2.strip()
         if ( word1 != "null" and word1.strip()) :
             if (word2 != "null" and word2.strip()) :
                 implication =  Implication(word1, word2) 
-                if (implication.getDistance() < 15) :
-                    if ( ( implication.getDirection() == 0 ) or
-                       (implication.getDirection() == 2 ) ):
+                if (implication.get_distance() < 15) :
+                    if ( ( implication.get_direction() == 0 ) or
+                       (implication.get_direction() == 2 ) ):
                         return word1
-                    elif implication.getDirection() == 1 :
+                    elif implication.get_direction() == 1 :
                         return word2
-                    elif implication.getDirection() == 3 :
+                    elif implication.get_direction() == 3 :
                         if ( ( not word1.endswith("َ") ) and ( not word1.endswith("ُ") ) ) : 
                             return word2
                         return word1
 
                 return ""
             else :
                 return word1
         
         else :
             if word2 != "null" and ( not word2.strip() ):
                 return  word2
             else:
                 return "null"
 
-    def normalize( word ):
-        # this function to standardization alif 
-        # If the tanween is before the alif, then it is placed after it, 
+    def normalize_alef(word):
+        """
+        Normalize the alif (ألف) character in the given word according to certain rules.
+
+        Args:
+            word (:obj:`str`): The input word to be normalized.
+
+        Returns:
+            :obj:`str`: The normalized word with alif characters modified based on the rules.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+
+            word = Implication.normalize_alef("ًى")  # Returns "ىً"
+            word = Implication.normalize_alef("ًا")  # Returns "اً"
+            word = Implication.normalize_alef("ٱلكتاب")  # Returns "الكتاب"
+        """
+        # If the tanween is before the alif, then it is placed after it,
         # because in the Arabic language this word is similar
-        if ( word.endswith("ًى") ) :
-            word = word[0 : len(word) - 2] + "ىً"
-        
+        if word.endswith("ًى"):
+            word = word[:len(word) - 2] + "ىً"
+
+        if word.endswith("ًا"):
+            word = word[:len(word) - 2] + "اً"
+        # Replace Alif-dhamma with Alif
+        if word.startswith("ٱ"):
+            word = "ا" + word[1:]
 
-        if ( word.endswith("ًا") )  :
-            word = word[0 : len(word) - 2 ] + "اً"
-        
-        # Replace Alif-dhamma with Alif 
-        if (word.startswith("ٱ")) :
-            word = "ا" + word[1 : ]
-        
         return word
 
 
-    def diacriticsSyntaxErrorIn( diacriticsArray ) :
-        # This funcion return True when the diacritics is incorreclty 
+
+    def diacritics_syntax_error_in(diacritics_array):
+        """
+        Check if the diacritics in the given array are incorrect.
+
+        Args:
+            diacritics_array (:obj:`list`): A list of diacritics to be checked.
+
+        Returns:
+            :obj:`bool`: True if there is a syntax error in the diacritics, False otherwise.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication 
+
+            diacritics = ["َ", "ُ", "ِ", "ّ"]
+            has_error = Implication.diacritics_syntax_error_in(diacritics)  # Returns False
+
+            diacritics = ["َ", "ُ", "ِ", "ٓ"]
+            has_error = Implication.diacritics_syntax_error_in(diacritics)  # Returns True
+        """
         try:
-            # check last letter diacritic
-            if ( Implication.wrongEndDiacritic(diacriticsArray[ len(diacriticsArray) - 1]) ) : 
+            # Check last letter diacritic
+            if Implication.wrong_end_diacritic(diacritics_array[-1]):
                 return True
-            else :
-                # check All letters diacritic except the last letter diacritic
-                for i in range(0 , len(diacriticsArray) - 1 ) :
-                    if (Implication.wrongMiddleDiacritic(diacriticsArray[i])) :
-                        return True 
+            else:
+                # Check all letters diacritic except the last letter diacritic
+                for i in range(len(diacritics_array) - 1):
+                    if Implication.wrong_middle_diacritic(diacritics_array[i]):
+                        return True
                 return False
-            
-        except :
+        except:
             return False
-        
+            
+
+    def wrong_end_diacritic(diac):
+        """
+        Check if the given diacritic is a wrong end diacritic.
+
+        Args:
+            diac (:obj:`int`): The diacritic value to be checked.
+
+        Returns:
+            :obj:`bool`: True if the diacritic is a wrong end diacritic, False otherwise.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication 
 
-    def wrongEndDiacritic( diac ) :
-        # 0 > No Diacritics , 1 > SUKUN, 2 > FATHA, 3 > KASRA, 4 > DAMMA, 5 > FATHATAN, 6 > KASRATAN,
-        #  7 > DAMMATAN, 8 > SHADDA, 9 > SHADDA with FATHA, 10 > SHADDA with KASRA, 11 > SHADDA with DAMMA
-        if (diac >= 0 and diac <= 11) :
+            diacritic = 0
+            is_wrong_end = Implication.wrong_end_diacritic(diacritic)  # Returns False
+
+            diacritic = 85
+            is_wrong_end = Implication.wrong_end_diacritic(diacritic)  # Returns True
+        """
+        if diac >= 0 and diac <= 11:
             return False
-        else :
-            # 85 - 86 - 87: SHADDAH WITH FATHATAN,SHADDAH WITH KASRTA, SHADDAH WITH DHAMTAN
+        else:
+            # 85 - 86 - 87: SHADDAH WITH FATHATAN, SHADDAH WITH KASRTA, SHADDAH WITH DHAMTAN
             return diac < 85 or diac > 87
-        
-    def wrongMiddleDiacritic( diac) :
 
-        if (diac >= 0 and diac <= 4) :
-            return False
-        else :
-            return diac < 8 or diac > 15
             
     
-    def calculateWordsImplication(self):
-
+    def calculate_words_implication(self):
+        """
+        Calculate the implication between two words.
+
+        This method updates the verdict, direction, distance, and conflicts attributes of the object based on the implication between the words.
+
+        Returns:
+            None
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+
+            implication = Implication(word1, word2)
+            implication.calculate_words_implication()
+            # Access the updated attributes
+            verdict = implication.verdict
+            direction = implication.direction
+            distance = implication.distance
+            conflicts = implication.conflicts
+        """
         self.verdict = "Incompatible"
-        self.direction = -2 
+        self.direction = -2
         self.distance = 1000
-        if (Implication.equalWords(self) == False): # If both words are not thge same return these values 
-            if ((len(self.word1Undiac) == 0 and len(self.word2Undiac) == 0)):
-                if (self.word1 == self.word2): 
+
+        if Implication.equal_words(self) is False:
+            if len(self.word1Undiac) == 0 and len(self.word2Undiac) == 0:
+                if self.word1 == self.word2:
                     self.conflicts = 0
                     self.distance = 0
-                    self.direction = 3 
+                    self.direction = 3
                 else:
                     self.conflicts = 1
                     self.distance = 1000
-                    self.direction = -2 
-                
+                    self.direction = -2
             else:
                 self.conflicts = max(len(self.word1Undiac), len(self.word2Undiac))
-            
         else:
-            if (Implication.calculateLettersImplication(self)):
-                self.direction = Implication.calculateDirection(self)
-                if (self.direction == -1) :
+            if Implication.calculate_letters_implication(self):
+                self.direction = Implication.calculate_direction(self)
+                if self.direction == -1:
                     self.distance = 101
                 else:
                     self.verdict = "Compatible"
-                
             else:
-                self.direction = -3 # the two words have different letters
+                self.direction = -3
                 self.distance = 3000
                 self.conflicts = 0
 
-    def equalWords( self ) :
-       # check if the tow words are the same taking into account the alif as the first letter 
-        word1FirstLetter = self.word1Undiac[0 : 1] # First letter in word1 
-        word2FirstLetter = self.word2Undiac[0 : 1] # First letter in word2 
-        self.word1Undiac =  self.word1Undiac[1 : ] # all word1 letters without diacritics except first letter 
-        self.word2Undiac =  self.word2Undiac[1 : ] # all word2 letters without diacritics except first letter 
-        
-        # If both words withot first letter are not equal return false, otherwise continue 
-        if ( self.word1Undiac != self.word2Undiac):
+
+    def equal_words(self):
+        """
+        Check if the two words are equal, taking into account the alif as the first letter.
+
+        This method updates the word1Undiac and word2Undiac attributes by removing the first letter, and returns True if the words are equal, False otherwise.
+
+        Returns:
+            :obj:`bool`: True if the words are equal, False otherwise.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication Implication
+
+            implication = Implication(word1, word2)
+            result = implication.equal_words()
+            if result:
+                print("The words are equal")
+            else:
+                print("The words are not equal")
+        """
+        word1_first_letter = self.word1Undiac[0:1]  # First letter in word1
+        word2_first_letter = self.word2Undiac[0:1]  # First letter in word2
+        self.word1Undiac = self.word1Undiac[1:]  # All word1 letters without diacritics except first letter
+        self.word2Undiac = self.word2Undiac[1:]  # All word2 letters without diacritics except first letter
+
+        if self.word1Undiac != self.word2Undiac:
             return False
 
-        # If the first letter in both words the same and (the other letters are the same) then return true, otherwise continue  
-        if word1FirstLetter == word2FirstLetter :
+        if word1_first_letter == word2_first_letter:
             return True
 
-        # check if first letter is any alif (the other letters are the same) then return below values 
-        if (word1FirstLetter != "ا" or word2FirstLetter != "آ" and word2FirstLetter != "أ" and word2FirstLetter != "إ") :
-            if ((word1FirstLetter == "آ" or word1FirstLetter == "أ" or word1FirstLetter == "إ") and word2FirstLetter == "ا") :
-                self.lettersDirection[0] = 2 # w2 implies w1
+        if word1_first_letter != "ا" or (word2_first_letter not in ["آ", "أ", "إ"]):
+            if (word1_first_letter in ["آ", "أ", "إ"]) and word2_first_letter == "ا":
+                self.lettersDirection[0] = 2  # w2 implies w1
                 self.conflictFlags[3] = True
                 return True
             else:
                 return False
         else:
-            self.lettersDirection[0] = 1 # w1 implies w2
+            self.lettersDirection[0] = 1  # w1 implies w2
             self.conflictFlags[2] = True
             return True
-        
+
         return False
 
-       
-    def calculateLettersImplication(self) :
+    def calculate_letters_implication(self):
+        """
+        Calculate the implication between each pair of diacritics in the words.
+
+        This method updates the lettersDirection, conflictFlags, and distance attributes based on the directionTable and distanceTable values for each pair of diacritics. It returns True after the calculation is completed.
+
+        Returns:
+            bool: True indicating the calculation is completed.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
 
+            from nlptools.utils.implication import Implication
+
+            implication = Implication(word1, word2)
+            result = implication.calculate_letters_implication()
+            if result:
+                print("Letters implication calculation completed")
+        """
         self.distance = 0
-        word1Diac = 0
-        word2Diac = 0
-  
-        for i in range ( 0 , len(self.word1Diacritics) - 1) :
-            word1Diac = self.word1Diacritics[i];
-            word2Diac = self.word2Diacritics[i];
-
-            self.lettersDirection[i + 1] = self.directionTable[word1Diac][word2Diac];
-            self.conflictFlags[self.lettersDirection[i + 1] + 1] = True;
-            self.distance = self.distance + self.distanceTable[word1Diac][word2Diac];
-
-               
-        word1Diac = int( self.word1Diacritics[len(self.word1Diacritics) - 1] ) # last letter diacritics to word1
-        word2Diac = int( self.word2Diacritics[len(self.word1Diacritics) - 1] ) # last letter diacritics to word2
+        word1_diac = 0
+        word2_diac = 0
+
+        for i in range(0, len(self.word1Diacritics) - 1):
+            word1_diac = self.word1Diacritics[i]
+            word2_diac = self.word2Diacritics[i]
+
+            self.lettersDirection[i + 1] = self.directionTable[word1_diac][word2_diac]
+            self.conflictFlags[self.lettersDirection[i + 1] + 1] = True
+            self.distance = self.distance + self.distanceTable[word1_diac][word2_diac]
+
+        word1_diac = int(self.word1Diacritics[len(self.word1Diacritics) - 1])  # last letter diacritics for word1
+        word2_diac = int(self.word2Diacritics[len(self.word1Diacritics) - 1])  # last letter diacritics for word2
         # 8: expresses the presence of shaddah
-        if (word1Diac == 8 or word2Diac == 8) :
-            self.lettersDirection[len(self.lettersDirection) - 1] = self.directionTable[word1Diac][word2Diac]
+        if word1_diac == 8 or word2_diac == 8:
+            self.lettersDirection[len(self.lettersDirection) - 1] = self.directionTable[word1_diac][word2_diac]
             self.conflictFlags[self.lettersDirection[len(self.lettersDirection) - 1] + 1] = True
-            self.distance = self.distance + self.distanceTable[word1Diac][word2Diac]
+            self.distance = self.distance + self.distanceTable[word1_diac][word2_diac]
+        
         return True
 
         
-    def calculateDirection(self ): 
+    def calculate_direction(self):
+        """
+        Calculates the direction of compatibility based on conflict flags.
+
+        Returns:
+            :obj:`int`: The direction of compatibility:
+                -1: Incompatible-diacritics
+                0: Compatible-imply each other
+                1: Compatible-w1 implies w2
+                2: Compatible-w2 implies w1
+                3: Compatible-exactly equal
+                -2147483648: Default value for an invalid direction
+        """
         self.conflicts = 0
-        if (self.conflictFlags[0] == True): 
-            return -1 # Incompatible-diacritics
-        
-        if (self.conflictFlags[2] == True and self.conflictFlags[3] == True ):
-            return 0 # Compatible-imply each other
-        
-        if (self.conflictFlags[2] == True and self.conflictFlags[3] == False ):
-            return 1 # Compatible-w1 implies w2
-        
-        if (self.conflictFlags[2] == False and self.conflictFlags[3] == True ):
-            return 2 # Compatible-w2 implies w1
-        
-        if (self.conflictFlags[4]):
-            return 3 # Compatible-exactly equal
-        
-        return -2147483648
 
+        if self.conflictFlags[0] is True:
+            return -1  # Incompatible-diacritics
 
+        if self.conflictFlags[2] is True and self.conflictFlags[3] is True:
+            return 0  # Compatible-imply each other
 
-    def getDiacriticsArray( word ): 
+        if self.conflictFlags[2] is True and self.conflictFlags[3] is False:
+            return 1  # Compatible-w1 implies w2
+
+        if self.conflictFlags[2] is False and self.conflictFlags[3] is True:
+            return 2  # Compatible-w2 implies w1
+
+        if self.conflictFlags[4]:
+            return 3  # Compatible-exactly equal
+
+        return -2147483648
+
+
+    def calculate_direction( word ):
+        """
+        Converts diacritics in a word to digits and returns the array of diacritics.
+
+        Args:
+            word (:obj:`str`): The word containing diacritics.
+
+        Returns:
+            :obj:`list`: The array of diacritics converted to digits.
+
+        Raises:
+            Exception: If the first character of the word is a digit.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+            word = "مُرَحَّبًا"
+            diacritics = Implication.calculate_direction(word)
+            print(diacritics)
+            Output: [4, 3, 8, 5, 0]
+        """ 
         # Replace diacritics by digits 
         word = word.replace(" ", "") #Space
         word = word.replace("ْ", "1") #SUKUN  
         word = word.replace("َ", "2") #FATHA
         word = word.replace("ِ", "3") #KASRA
         word = word.replace("ُ", "4") #DAMMA
         word = word.replace("ً", "5") #FATHATAN
@@ -382,64 +531,99 @@
         strDiacritics = diacritics
         
         # Convert string array digits to integer digits array 
         for x in range(0 , len(strDiacritics) ):
             diacritics[x] = int(strDiacritics[x])
         return diacritics
     
-    def removeDiacritics( word ): # remove all diacritics from Arabic word
-        word = word.replace(" ", "")
-        word = word.replace("ْ", "") #SUKUN
-        word = word.replace("َ", "") #FATHA
-        word = word.replace("ِ", "") #KASRA
-        word = word.replace("ُ", "") #DAMMA
-        word = word.replace("ً", "") #FATHATAN
-        word = word.replace("ٍ", "") #KASRATAN
-        word = word.replace("ٌ", "") #DAMMATAN
-        word = word.replace("ّ", "") #SHADDA
-        return word
+    # def removeDiacritics( word ): # remove all diacritics from Arabic word
+    #     # word = word.replace(" ", "")
+    #     # word = word.replace("ْ", "") #SUKUN
+    #     # word = word.replace("َ", "") #FATHA
+    #     # word = word.replace("ِ", "") #KASRA
+    #     # word = word.replace("ُ", "") #DAMMA
+    #     # word = word.replace("ً", "") #FATHATAN
+    #     # word = word.replace("ٍ", "") #KASRATAN
+    #     # word = word.replace("ٌ", "") #DAMMATAN
+    #     # word = word.replace("ّ", "") #SHADD
+    #     #word = word.sub(r'[\u064B-\u0650]+', '',word) # Remove all Arabic diacretics [ ًٌٍَُِْ]A
+    #     word = arStrip(word,diacs=False , shaddah=False)
+    #     return word
+
+    def get_letters_array(word):
+        """
+        Retrieves the array of letters from a given word.
+
+        Args:
+            word (:obj:`str`): The word from which to extract the letters.
+
+        Returns:
+            obj:`list`: The array of letters.
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+            word = "مرحبا"
+            letters = get_letters_array(word)
+            print(letters)
+            Output: ['م', 'ر', 'ح', 'ب', 'ا']
+        """
+        word = arStrip(word, diacs=False, shaddah=False)
+        return list(word)
 
-    def getLettersArray(word): # آot used in code 
-        word = removeDiacritics(word)
-        return word.split("")
 
-    def getVerdict(self ): 
+    def get_verdict(self ): 
         return self.verdict
 
 
-    def getDirection(self): 
+    def get_direction(self): 
         return self.direction
 
 
-    def getDistance(self) :
+    def get_distance(self) :
         return self.distance
 
 
-    def getConflicts(self) :
+    def get_conflicts(self) :
         return self.conflicts
 
 
-    def getWord1(self) :
+    def get_word1(self) :
         return self.word1
 
 
-    def getWord2(self) :
+    def get_word2(self) :
         return self.word2 
 
-    def getResult(self):
-       # result: takes one of the values: “Same”, or “Different”, to state whether w1 and w2 are matching.)
-        if ( Implication.getDirection(self) >= 0 and Implication.getDistance(self) < 15):
+    def get_result(self):
+        """
+        Retrieves the result of the comparison between two words.
+
+        Returns:
+            :obj:`str`: The result of the comparison. Can be "Same" or "Different".
+
+        **Example:**
+
+        .. highlight:: python
+        .. code-block:: python
+
+            from nlptools.utils.implication import Implication
+            w1 = "hello"
+            w2 = "hell"
+            implication = Implication(w1, w2)
+            result = implication.get_result()
+            print(result)
+            Output: "Same"
+        """
+        if Implication.get_direction(self) >= 0 and Implication.get_distance(self) < 15:
             self.result = "Same"
         else:
             self.result = "Different"
-        return  self.result 
+        return self.result
+
 
     def toString(self) :
         return self.word1 + "\t" + self.word2 + "\t" + str(self.verdict) + "\t" + str(self.direction) + "\t" + str(self.distance) + "\t"+ str(self.conflicts)
 
-
-# Example:
-#w1 = "كلمة" 
-#w2 = "كلمة" 
-#implication =  Implication(w1 , w2)
-#print(implication.getResult())
-# print(implication.getDirection() )
```

### Comparing `nlptoolssna-0.8.5/nlptools/utils/jaccard.py` & `nlptoolssna-0.8.6/nlptools/utils/jaccard.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 
 def normalize_word(word: str, ignore_all_diacritics_but_not_shadda: bool, ignore_shadda_diacritic: bool) -> str:
     """
     Normalize a given Arabic word by removing diacritics and/or shadda diacritic based on the provided flags.
 
     Args:
-        word: A string representing an Arabic word to be normalized.
-        ignore_all_diacritics_but_not_shadda: A boolean flag indicating whether to remove all diacritics except shadda.
-        ignore_shadda_diacritic: A boolean flag indicating whether to remove shadda diacritic.
+        word (:obj:`str`): A string representing an Arabic word to be normalized.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A boolean flag indicating whether to remove all diacritics except shadda.
+        ignore_shadda_diacritic (:obj:`bool`): A boolean flag indicating whether to remove shadda diacritic.
 
     Returns:
         A string representing the normalized Arabic word.
     """
     if ignore_all_diacritics_but_not_shadda:
         # Remove all diacritics except shadda
         word = arStrip(word, True, True, False, False, False, False)
@@ -33,53 +33,52 @@
 
     
 def get_preferred_word(word1, word2):
     """
     Returns the preferred word among two given words based on their implication.
 
     Args:
-        word1 (:obj:str): The first word to be compared.
-        word2 (:obj:str): The second word to be compared.
+        word1 (:obj:`str`): The first word to be compared.
+        word2 (:obj:`str`): The second word to be compared.
 
     Returns:
         str: The preferred word among the two given words.
     """
     implication = Implication(word1, word2)
     
-    direction = implication.getDirection()
+    direction = implication.get_direction()
     
     if direction in (0, 2):
         return word1
        
     elif direction == 1:
         return word2
        
     elif direction == 3:
         if not word1.endswith("َ") and not word1.endswith("ُ"):
             return word2
         return word1
-
-           
+     
     
 def get_non_preferred_word(word1, word2):
     """
     Find the non-preferred word between the two input words.
 
     Args:
-        word1 (:obj:str): The first word.
-        word2 (:obj:str): The second word.
+        word1 (:obj:`str`): The first word.
+        word2 (:obj:`str`): The second word.
 
     Returns:
-        str: The non-preferred word. If there is no non-preferred word, returns '#'.
+        :obj:`str`: The non-preferred word. If there is no non-preferred word, returns '#'.
 
     """
     # Find non-preferred word if the distance between the two words input is less than 15.
     implication = Implication(word1, word2)
-    if implication.getDistance() < 15:
-        direction = implication.getDirection()
+    if implication.get_distance() < 15:
+        direction = implication.get_direction()
         if direction == 0 or direction == 1:
             return word1
         elif direction == 2:
             return word2
         elif direction == 3:
             if not word1.endswith("َ") and not word1.endswith("ُ"):
                 return word1
@@ -87,21 +86,21 @@
     return "#"
 
 def get_intersection(list1, list2, ignore_all_diacritics_but_not_shadda=False, ignore_shadda_diacritic=False):
     """
     Get the intersection of two lists after normalization and ignoring diacritics based on input flags.
 
     Args:
-        - list1 (:obj:`list`): The first list.
-        - list2 (:obj:`list`): The second list.
-        - ignore_all_diacritics_but_not_shadda (:obj:`bool`, optional): A flag to ignore all diacritics except for the shadda. Defaults to False.
-        - ignore_shadda_diacritic (:obj:`bool`, optional): A flag to ignore the shadda diacritic. Defaults to False.
+        list1 (:obj:`list`): The first list.
+        list2 (:obj:`list`): The second list.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`, optional): A flag to ignore all diacritics except for the shadda. Defaults to False.
+        ignore_shadda_diacritic (:obj:`bool`, optional): A flag to ignore the shadda diacritic. Defaults to False.
 
     Returns:
-        - (:obj:`list`): The intersection of the two lists after normalization and ignoring diacritics.
+         :obj:`list`: The intersection of the two lists after normalization and ignoring diacritics.
 
     """
 
     # Remove all None and empty values from first list
     list1 = [str(i) for i in list1 if i not in (None, ' ', '')]
     list1 = [str(i.strip()) for i in list1]
 
@@ -136,41 +135,36 @@
 
 
 def get_union(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic):
     """
     Finds the union of two lists by removing duplicates and normalizing words.
 
     Args:
-        - list1 (:obj:`list`): The first list.
-        - list2 (:obj:`list`): The second list.
-        - ignore_all_diacritics_but_not_shadda (:obj:`bool`): Whether to ignore all diacritics except shadda or not.
-        - ignore_shadda_diacritic (:obj:`bool`): Whether to ignore shadda diacritic or not.
-
-    Returns:
-        - :obj:`list`: The union of the two lists after removing duplicates and normalizing words.
+        list1 (:obj:`list`): The first list.
+        list2 (:obj:`list`): The second list.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`): Whether to ignore all diacritics except shadda or not.
+        ignore_shadda_diacritic (:obj:`bool`): Whether to ignore shadda diacritic or not.
+   Returns:
+         :obj:`list`: The union of the two lists after removing duplicates and normalizing words.
     """
-    # Remove all None and empty values from the first set
+
     list1 = [str(i) for i in list1 if i not in (None, ' ', '')]
 
-    # Remove all None and empty values from the second set
     list2 = [str(i) for i in list2 if i not in (None, ' ', '')]
 
     union_list = []
 
-    # Add all words found in set#1 to union_list after normalization
     for list1_word in list1:
         word1 = normalize_word(list1_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
         union_list.append(word1)
 
-    # Add all words found in set#2 to union_list after normalization
     for list2_word in list2:
         word2 = normalize_word(list2_word, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
         union_list.append(word2)
 
-    # Remove redundant words by using get_non_preferred_word function
     i = 0
     while i < len(union_list):
         j = i + 1
         while j < len(union_list):
             non_preferred_word = get_non_preferred_word(union_list[i], union_list[j])
             if (non_preferred_word != "#"):
                 union_list.remove(non_preferred_word)
@@ -182,55 +176,55 @@
 
 
 def jaccard_similarity(list1: list, list2: list, ignore_all_diacritics_but_not_shadda: bool, ignore_shadda_diacritic: bool) -> float:
     """
     Calculates the Jaccard similarity coefficient between two lists.
 
     Args:
-        - list1 (:obj:`list`): The first list.
-        - list2 (:obj:`list`): The second list.
-        - ignore_all_diacritics_but_not_shadda (:obj:`bool`): A flag indicating whether to ignore all diacritics except for shadda.
-        - ignore_shadda_diacritic (:obj:`bool`): A flag indicating whether to ignore the shadda diacritic.
+        list1 (:obj:`list`): The first list.
+        list2 (:obj:`list`): The second list.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A flag indicating whether to ignore all diacritics except for shadda.
+        ignore_shadda_diacritic (:obj:`bool`): A flag indicating whether to ignore the shadda diacritic.
 
     Returns:
-        float: The Jaccard similarity coefficient between the two lists.
+         :obj:`float`: The Jaccard similarity coefficient between the two lists.
     """
     # Find the intersection between two sets
     intersection_list = get_intersection(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
     
     # Find the union between two sets
     union_list = get_union(list1, list2, ignore_all_diacritics_but_not_shadda, ignore_shadda_diacritic)
     
     # Calculate the Jaccard similarity coefficient by dividing the length of the intersectionList by the length of the unionList
     return float(len(intersection_list)) / float(len(union_list))
    
 
 
 
-def jaccard(delimiter, str1, str2, selection, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic):
+def jaccard(delimiter, str1, str2, selection, ignoreAllDiacriticsButNotShadda=True, ignoreShaddaDiacritic=True):
     """
     Compute the Jaccard similarity, union, or intersection of two sets of strings.
 
     Args:
         delimiter (:obj:`str`): The delimiter used to split the input strings.
         str1 (:obj:`str`): The first input string to compare.
         str2 (:obj:`str`): The second input string to compare.
         selection (:obj:`str`): The desired operation to perform on the two sets of strings. 
-                         Must be one of "intersection", "union", "jaccardSimilarity", or "jaccardAll".
-        ignoreAllDiacriticsButNotShadda (:obj:`bool`): If True, ignore all diacritics except for the Shadda diacritic.
-        ignoreShaddaDiacritic (:obj:`bool`): If True, ignore the Shadda diacritic.
+                         Must be one of *intersection*, *union*, *jaccardSimilarity*, or *jaccardAll*.
+        ignoreAllDiacriticsButNotShadda (:obj:`bool`): If True, ignore all diacritics except for the Shadda diacritic. (Defualt is True)
+        ignoreShaddaDiacritic (:obj:`bool`): If True, ignore the Shadda diacritic.(Default is True)
 
     Returns:
         The Jaccard similarity, union, or intersection of the two sets of strings, 
         depending on the value of the `selection` argument.
-
-        If `selection` is "jaccardAll", a list of the intersection, union, and Jaccard similarity 
+    
+    Note:
+        - If `selection` is *jaccardAll*, a list of the intersection, union, and Jaccard similarity 
         of the two sets of strings will be returned.
-
-        If an error occurs, the method will return the string "An error has occurred".
+        - If an error occurs, the method will return the string "An error has occurred".
     """
     try:
         list1 = str1.split(delimiter)
         list2 = str2.split(delimiter)
 
         if selection == "intersection":
             intersection = get_intersection(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
```

### Comparing `nlptoolssna-0.8.5/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.8.6/nlptoolssna.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.5/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.8.6/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 docs/source/api/morphology.rst
 docs/source/api/utils.rst
 docs/source/api/DataDownload/downloader.rst
 docs/source/api/morphology/morph_analyzer.rst
 docs/source/api/utils/implication.rst
 docs/source/api/utils/jaccard.rst
 docs/source/api/utils/parser.rst
+docs/source/api/utils/text_transliteration.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
 nlptools/DataDownload/__init__.py
 nlptools/DataDownload/downloader.py
 nlptools/arabiner/__init__.py
 nlptools/arabiner/data.py
@@ -45,14 +46,15 @@
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
 nlptools/utils/__init__.py
 nlptools/utils/implication.py
 nlptools/utils/jaccard.py
 nlptools/utils/parser.py
+nlptools/utils/text_transliteration.py
 nlptools/utils/utils.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
 nlptoolssna.egg-info/dependency_links.txt
 nlptoolssna.egg-info/entry_points.txt
 nlptoolssna.egg-info/not-zip-safe
 nlptoolssna.egg-info/requires.txt
```

### Comparing `nlptoolssna-0.8.5/setup.cfg` & `nlptoolssna-0.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.5/setup.py` & `nlptoolssna-0.8.6/setup.py`

 * *Files identical despite different names*


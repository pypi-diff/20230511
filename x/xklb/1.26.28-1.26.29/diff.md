# Comparing `tmp/xklb-1.26.28.tar.gz` & `tmp/xklb-1.26.29.tar.gz`

## Comparing `xklb-1.26.28.tar` & `xklb-1.26.29.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.28/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.28/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.28/Windows.md
--rw-r--r--   0        0        0   419424 2020-02-02 00:00:00.000000 xklb-1.26.28/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.28/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.28/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/books.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/consts.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/dl_config.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/hn_extract.py
--rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/lb.py
--rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/playback.py
--rw-r--r--   0        0        0    26800 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21844 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.28/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.28/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.28/LICENSE
--rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.28/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.28/pyproject.toml
--rw-r--r--   0        0        0    44039 2020-02-02 00:00:00.000000 xklb-1.26.28/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.29/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.29/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.29/Windows.md
+-rw-r--r--   0        0        0   417004 2020-02-02 00:00:00.000000 xklb-1.26.29/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.29/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.29/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.29/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.29/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.26.29/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.29/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/books.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/consts.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/dl_config.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/lb.py
+-rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/playback.py
+-rw-r--r--   0        0        0    26800 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21844 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.29/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.29/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.29/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.29/LICENSE
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.26.29/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.29/pyproject.toml
+-rw-r--r--   0        0        0    44036 2020-02-02 00:00:00.000000 xklb-1.26.29/PKG-INFO
```

### Comparing `xklb-1.26.28/Windows.md` & `xklb-1.26.29/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/pdm.lock` & `xklb-1.26.29/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -129,23 +129,23 @@
 summary = "YouTube chromecast api"
 dependencies = [
     "requests",
 ]
 
 [[package]]
 name = "catt"
-version = "0.12.10"
+version = "0.12.11"
 requires_python = ">=3.7"
 summary = "Cast All The Things allows you to send videos from many, many online sources to your Chromecast."
 dependencies = [
     "click>=7.1.2",
     "ifaddr>=0.1.7",
-    "pychromecast<13,>=12.1.4",
+    "pychromecast<14,>=13.0.7",
     "requests>=2.23.0",
-    "yt-dlp>=2022.6.22.1",
+    "yt-dlp>=2023.3.4",
 ]
 
 [[package]]
 name = "certifi"
 version = "2023.5.7"
 requires_python = ">=3.6"
 summary = "Python package for providing Mozilla's CA Bundle."
@@ -631,17 +631,17 @@
 summary = "Library for building powerful interactive command lines in Python"
 dependencies = [
     "wcwidth",
 ]
 
 [[package]]
 name = "protobuf"
-version = "3.20.3"
+version = "4.23.0"
 requires_python = ">=3.7"
-summary = "Protocol Buffers"
+summary = ""
 
 [[package]]
 name = "psutil"
 version = "5.8.0"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Cross-platform lib for process and system monitoring in Python."
 
@@ -653,19 +653,19 @@
 [[package]]
 name = "pure-eval"
 version = "0.2.2"
 summary = "Safely evaluate AST nodes without side effects"
 
 [[package]]
 name = "pychromecast"
-version = "12.1.4"
+version = "13.0.7"
 summary = "Python module to talk to Google Chromecast."
 dependencies = [
     "casttube>=0.2.0",
-    "protobuf<4,>=3.19.1",
+    "protobuf>=3.19.1",
     "zeroconf>=0.25.1",
 ]
 
 [[package]]
 name = "pycparser"
 version = "2.21"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
@@ -1404,17 +1404,17 @@
     {url = "https://files.pythonhosted.org/packages/cc/17/9418f28b83c85c0108d8b1822359c22ab09f1ec54d3280d742e56645148c/brotlicffi-1.0.9.2-pp36-pypy36_pp73-win32.whl", hash = "sha256:916b790f967a18a595e61f218c252f83718ac91f24157d622cf0fa710cd26ab7"},
     {url = "https://files.pythonhosted.org/packages/d3/d8/6acbb65e350213ad6bd96180593fad0a269a3baa845c67fed21adee3959d/brotlicffi-1.0.9.2.tar.gz", hash = "sha256:0c248a68129d8fc6a217767406c731e498c3e19a7be05ea0a90c3c86637b7d96"},
 ]
 "casttube 0.2.1" = [
     {url = "https://files.pythonhosted.org/packages/0a/d2/0f5006892e07ea342d57dbeda46027e99a097ffb6218bee1e37f9776ed95/casttube-0.2.1-py3-none-any.whl", hash = "sha256:36f118007f9eead3959cf30de03c1640b53a263569ff2a3971c0521826c835b2"},
     {url = "https://files.pythonhosted.org/packages/78/54/f7e80d701c587940cf1c871fb6327b4a2682df4287896fbf9400cd0bbf21/casttube-0.2.1.tar.gz", hash = "sha256:54d2af8c7949aa9c5db87fb11ef0a478a5d3e7ac6d2d2ac8dd1711e3a516fc82"},
 ]
-"catt 0.12.10" = [
-    {url = "https://files.pythonhosted.org/packages/0c/6d/be6e8682f6d33f763cab155e77879329b78ccd59b096dea01c2bac2d4f13/catt-0.12.10-py3-none-any.whl", hash = "sha256:0f51120b307671d671fcd2cbc3686c1df584e7a78d1589dc1b6468d25a6cd7b1"},
-    {url = "https://files.pythonhosted.org/packages/fa/df/4d1503bf067b3d28b90b0c9ddf8cc4c5430bdc104da5ac7b16c8eddc8f0b/catt-0.12.10.tar.gz", hash = "sha256:a462f126ad2630ef7f57ea66ca3808eee7620b25de74d76a9204c8a87e874c1f"},
+"catt 0.12.11" = [
+    {url = "https://files.pythonhosted.org/packages/3d/f7/def2a94aacaedbaf5f755a09acba713b895eaec1cff33df71569f7148f44/catt-0.12.11.tar.gz", hash = "sha256:d1ba9861f5b017bc98a006e364f862fdfe022dc2fcf6299619868c8b907086d7"},
+    {url = "https://files.pythonhosted.org/packages/62/17/604bfe5fefb961528ee364cdaf77da2fe634938436d93a3050c2f21e9fa9/catt-0.12.11-py3-none-any.whl", hash = "sha256:db2808d0e344381cb2a1fd8729416ef8b926fb3d5f5507b0f4697a79b095731f"},
 ]
 "certifi 2023.5.7" = [
     {url = "https://files.pythonhosted.org/packages/93/71/752f7a4dd4c20d6b12341ed1732368546bc0ca9866139fe812f6009d9ac7/certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
     {url = "https://files.pythonhosted.org/packages/9d/19/59961b522e6757f0c9097e4493fa906031b95b3ebe9360b2c3083561a6b4/certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
 ]
 "cffi 1.15.1" = [
     {url = "https://files.pythonhosted.org/packages/00/05/23a265a3db411b0bfb721bf7a116c7cecaf3eb37ebd48a6ea4dfb0a3244d/cffi-1.15.1-cp27-cp27m-win_amd64.whl", hash = "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e"},
@@ -2259,37 +2259,28 @@
     {url = "https://files.pythonhosted.org/packages/d6/36/55cc2cab22aafbebd52ddac4ccb670b920b54eb6ddbdb8573c79ca870d8a/prawcore-2.3.0-py3-none-any.whl", hash = "sha256:48c17db447fa06a13ca3e722201f443031437708daa736c05a1df895fbcceff5"},
     {url = "https://files.pythonhosted.org/packages/ed/85/13e76be737f3159514cce609b29e95499ba6d2cfa0b88761bab318b5f63e/prawcore-2.3.0.tar.gz", hash = "sha256:daf1ccd4b7a80dc4e6567d48336d782e94a9a6dad83770fc2edf76dc9a84f56d"},
 ]
 "prompt-toolkit 3.0.38" = [
     {url = "https://files.pythonhosted.org/packages/4b/bb/75cdcd356f57d17b295aba121494c2333d26bfff1a837e6199b8b83c415a/prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
     {url = "https://files.pythonhosted.org/packages/87/3f/1f5a0ff475ae6481f4b0d45d4d911824d3218b94ee2a97a8cb84e5569836/prompt_toolkit-3.0.38-py3-none-any.whl", hash = "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"},
 ]
-"protobuf 3.20.3" = [
-    {url = "https://files.pythonhosted.org/packages/00/e7/d23c439c55c90ae2e52184363162f7079ca3e7d86205b411d4e9dc266f81/protobuf-3.20.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b"},
-    {url = "https://files.pythonhosted.org/packages/11/a5/e52b731415ad6ef3d841e9e6e337a690249e800cc7c06f0749afab26348c/protobuf-3.20.3-cp39-cp39-win_amd64.whl", hash = "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7"},
-    {url = "https://files.pythonhosted.org/packages/28/55/b80e8567ec327c060fa39b242392e25690c8899c489ecd7bb65b46b7bb55/protobuf-3.20.3-cp310-cp310-manylinux2014_aarch64.whl", hash = "sha256:f4bd856d702e5b0d96a00ec6b307b0f51c1982c2bf9c0052cf9019e9a544ba99"},
-    {url = "https://files.pythonhosted.org/packages/2a/7c/e7091f0eea6eec70547d28c6c0d8c7335ee58f6b13456608beec8c94a62a/protobuf-3.20.3-cp37-cp37m-manylinux2014_aarch64.whl", hash = "sha256:d9e4432ff660d67d775c66ac42a67cf2453c27cb4d738fc22cb53b5d84c135d4"},
-    {url = "https://files.pythonhosted.org/packages/31/be/80a9c6f16dfa4d41be3edbe655349778ae30882407fa8275eb46b4d34854/protobuf-3.20.3-cp310-cp310-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:9aae4406ea63d825636cc11ffb34ad3379335803216ee3a856787bcf5ccc751e"},
-    {url = "https://files.pythonhosted.org/packages/32/f8/52f598bceb16fe365f4ef8e957ac8890aeb56abf97d365ff5abd8c1250cf/protobuf-3.20.3-cp38-cp38-win_amd64.whl", hash = "sha256:447d43819997825d4e71bf5769d869b968ce96848b6479397e29fc24c4a5dfe9"},
-    {url = "https://files.pythonhosted.org/packages/36/8b/433071fed0058322090a55021bdc8da76d16c7bc9823f5795797803dd6d0/protobuf-3.20.3-cp39-cp39-win32.whl", hash = "sha256:819559cafa1a373b7096a482b504ae8a857c89593cf3a25af743ac9ecbd23480"},
-    {url = "https://files.pythonhosted.org/packages/3c/14/16ef7da61d30a519d84e6841d096fe446c4d8a2c39b083b0376b4785f1f3/protobuf-3.20.3-cp38-cp38-win32.whl", hash = "sha256:c02ce36ec760252242a33967d51c289fd0e1c0e6e5cc9397e2279177716add86"},
-    {url = "https://files.pythonhosted.org/packages/4c/12/62e1d5505c172e1a7f803d83b0b1693f7952c3c271eb2f155703012ae67a/protobuf-3.20.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:74480f79a023f90dc6e18febbf7b8bac7508420f2006fabd512013c0c238f454"},
-    {url = "https://files.pythonhosted.org/packages/55/5b/e3d951e34f8356e5feecacd12a8e3b258a1da6d9a03ad1770f28925f29bc/protobuf-3.20.3.tar.gz", hash = "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2"},
-    {url = "https://files.pythonhosted.org/packages/6f/5e/fc6feb366b0a9f28e0a2de3b062667c521cd9517d4ff55077b8f351ba2f3/protobuf-3.20.3-cp310-cp310-win_amd64.whl", hash = "sha256:67a3598f0a2dcbc58d02dd1928544e7d88f764b47d4a286202913f0b2801c2e7"},
-    {url = "https://files.pythonhosted.org/packages/8d/14/619e24a4c70df2901e1f4dbc50a6291eb63a759172558df326347dce1f0d/protobuf-3.20.3-py2.py3-none-any.whl", hash = "sha256:a7ca6d488aa8ff7f329d4c545b2dbad8ac31464f1d8b1c87ad1346717731e4db"},
-    {url = "https://files.pythonhosted.org/packages/98/07/4c75a689fa173c12b92c9a64a82efad44797b9b2b784c8562f36ab28b551/protobuf-3.20.3-cp37-cp37m-win_amd64.whl", hash = "sha256:8c0c984a1b8fef4086329ff8dd19ac77576b384079247c770f29cc8ce3afa06c"},
-    {url = "https://files.pythonhosted.org/packages/99/25/5825472ecd911f4ac2ac4e9ab039a48b6d03874e2add92fb633e080bf3eb/protobuf-3.20.3-cp39-cp39-manylinux2014_aarch64.whl", hash = "sha256:bf01b5720be110540be4286e791db73f84a2b721072a3711efff6c324cdf074b"},
-    {url = "https://files.pythonhosted.org/packages/9c/d8/dc6a9ee6ec43a1001e3d71cccda70cf50ac0098000fc455023dba3b46ebf/protobuf-3.20.3-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:899dc660cd599d7352d6f10d83c95df430a38b410c1b66b407a6b29265d66469"},
-    {url = "https://files.pythonhosted.org/packages/9f/1a/6848ed1669a6c70bf947d25d64ce6dcc65ccec06e917072df516944fa17e/protobuf-3.20.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:de78575669dddf6099a8a0f46a27e82a1783c557ccc38ee620ed8cc96d3be7d7"},
-    {url = "https://files.pythonhosted.org/packages/b5/b6/ec87636b9381137f17292851461902ceac7632a00476c2afbcd864ed5447/protobuf-3.20.3-cp38-cp38-manylinux2014_aarch64.whl", hash = "sha256:f4c42102bc82a51108e449cbb32b19b180022941c727bac0cfd50170341f16ee"},
-    {url = "https://files.pythonhosted.org/packages/c7/df/ec3ecb8c940b36121c7b77c10acebf3d1c736498aa2f1fe3b6231ee44e76/protobuf-3.20.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:daa564862dd0d39c00f8086f88700fdbe8bc717e993a21e90711acfed02f2402"},
-    {url = "https://files.pythonhosted.org/packages/da/e4/4d62585593e9f962cb02614534f62f930de6a80a0a3784282094a01919b2/protobuf-3.20.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:44246bab5dd4b7fbd3c0c80b6f16686808fab0e4aca819ade6e8d294a29c7050"},
-    {url = "https://files.pythonhosted.org/packages/db/96/948d3fcc1fa816e7ae1d27af59b9d8c5c5e582f3994fd14394f31da95b99/protobuf-3.20.3-cp310-cp310-win32.whl", hash = "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c"},
-    {url = "https://files.pythonhosted.org/packages/ef/d4/765a106ca96d487f94f3c99e46b399218f53735628c3b2d759a832e2adab/protobuf-3.20.3-cp37-cp37m-win32.whl", hash = "sha256:b6cc7ba72a8850621bfec987cb72623e703b7fe2b9127a161ce61e61558ad905"},
-    {url = "https://files.pythonhosted.org/packages/fe/8f/d9db035740002d61b4140aaef53a8bac7e316b18ec8744eb6c1fcf83c310/protobuf-3.20.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:e64857f395505ebf3d2569935506ae0dfc4a15cb80dc25261176c784662cdcc4"},
+"protobuf 4.23.0" = [
+    {url = "https://files.pythonhosted.org/packages/06/38/e72c556c25aaaaafca75018d2d0ebc50c5ab80983dd4def086624fba43f2/protobuf-4.23.0-cp37-abi3-manylinux2014_x86_64.whl", hash = "sha256:ebde3a023b8e11bfa6c890ef34cd6a8b47d586f26135e86c21344fe433daf2e2"},
+    {url = "https://files.pythonhosted.org/packages/15/a9/287edf57651a60336a92f2d959a244ac3184bd3e0d0616b21e1731fc3e5e/protobuf-4.23.0-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:2b94bd6df92d71bd1234a2ffe7ce96ddf6d10cf637a18d6b55ad0a89fbb7fc21"},
+    {url = "https://files.pythonhosted.org/packages/17/ba/29ff6b6ff827178ac7f66ee7fd383342a188ffa6a96084bad1513d942da1/protobuf-4.23.0-cp39-cp39-win32.whl", hash = "sha256:03eee35b60317112a72d19c54d0bff7bc58ff12fea4cd7b018232bd99758ffdf"},
+    {url = "https://files.pythonhosted.org/packages/31/d1/bc0780924e53c7dd0aca42be0c2d933998dbb744c30bdda48bd9e63808a5/protobuf-4.23.0-cp38-cp38-win32.whl", hash = "sha256:d5a35ff54e3f62e8fc7be02bb0d2fbc212bba1a5a9cc2748090690093996f07b"},
+    {url = "https://files.pythonhosted.org/packages/60/1a/79f077c5baf5a9262ed41cc0909c1230ecac5cb4f4960cd97942c88d1726/protobuf-4.23.0.tar.gz", hash = "sha256:5f1eba1da2a2f3f7df469fccddef3cc060b8a16cfe3cc65961ad36b4dbcf59c5"},
+    {url = "https://files.pythonhosted.org/packages/60/db/9579f388a3627b867519f476ab5b3cf8391fbf79e5827f370a86ba911483/protobuf-4.23.0-cp37-abi3-manylinux2014_aarch64.whl", hash = "sha256:9f5a0fbfcdcc364f3986f9ed9f8bb1328fb84114fd790423ff3d7fdb0f85c2d1"},
+    {url = "https://files.pythonhosted.org/packages/6a/a2/c0b1c36c146212815a8307469054bb972b0d82fcecf21c83600d7882574f/protobuf-4.23.0-cp38-cp38-win_amd64.whl", hash = "sha256:e62fb869762b4ba18666370e2f8a18f17f8ab92dd4467295c6d38be6f8fef60b"},
+    {url = "https://files.pythonhosted.org/packages/6f/2e/49169f6fc6b39f77e0fa94bc8a2e300a75d57ca7953cc1dbe15c1ead9efa/protobuf-4.23.0-cp37-cp37m-win_amd64.whl", hash = "sha256:6fe180b56e1169d72ecc4acbd39186339aed20af5384531b8e8979b02bbee159"},
+    {url = "https://files.pythonhosted.org/packages/89/e1/c03399e5bf8b2fb97f0f41e9039583fc78040503559bed5a09ac3ea15421/protobuf-4.23.0-cp310-abi3-win_amd64.whl", hash = "sha256:baca40d067dddd62141a129f244703160d278648b569e90bb0e3753067644711"},
+    {url = "https://files.pythonhosted.org/packages/aa/f1/b17e29296a85eeeebac34a9a631ba4c46e23b632e64ceea86633de1e69e1/protobuf-4.23.0-cp37-cp37m-win32.whl", hash = "sha256:7cb5b9a05ce52c6a782bb97de52679bd3438ff2b7460eff5da348db65650f227"},
+    {url = "https://files.pythonhosted.org/packages/ba/59/bea9d68041fa6899eb47a60c0f3821e88f73ee6f69ad95a557158da40a60/protobuf-4.23.0-cp310-abi3-win32.whl", hash = "sha256:6c16657d6717a0c62d5d740cb354fbad1b0d8cb811669e06fc1caa0ff4799ddd"},
+    {url = "https://files.pythonhosted.org/packages/bf/65/f0ee96df56178e36705b3c97e69f9f7f08f64907632ecbbc08df0d3545da/protobuf-4.23.0-py3-none-any.whl", hash = "sha256:9744e934ea5855d12191040ea198eaf704ac78665d365a89d9572e3b627c2688"},
+    {url = "https://files.pythonhosted.org/packages/d3/3c/6bbbe3a5ccb68f117dc572d8b612efb77dc5824b87687ee52eb61abf965f/protobuf-4.23.0-cp39-cp39-win_amd64.whl", hash = "sha256:36f5370a930cb77c8ad2f4135590c672d0d2c72d4a707c7d0058dce4b4b4a598"},
 ]
 "psutil 5.8.0" = [
     {url = "https://files.pythonhosted.org/packages/10/d6/c5c19e40bb05e2cb5f053f480dfe47e9543a8322f1a5985d7352bf689611/psutil-5.8.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6223d07a1ae93f86451d0198a0c361032c4c93ebd4bf6d25e2fb3edfad9571ef"},
     {url = "https://files.pythonhosted.org/packages/12/80/8d09c345f19af2b29a309f8f9284e3ba1ae1ebd9438419080c14630f743a/psutil-5.8.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6323d5d845c2785efb20aded4726636546b26d3b577aded22492908f7c1bdda7"},
     {url = "https://files.pythonhosted.org/packages/15/28/47c28171fd7eeb83df74f78ccac090211f4a49408f376eb8e78a7bb47dc0/psutil-5.8.0-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:02b8292609b1f7fcb34173b25e48d0da8667bc85f81d7476584d889c6e0f2131"},
     {url = "https://files.pythonhosted.org/packages/18/c9/1db6aa0d28831f60408a6aab9d108c2edbd5a9ed11e5957a91d9d8023898/psutil-5.8.0-cp37-cp37m-win32.whl", hash = "sha256:1bff0d07e76114ec24ee32e7f7f8d0c4b0514b3fae93e3d2aaafd65d22502394"},
     {url = "https://files.pythonhosted.org/packages/19/29/f7a38ee30083f2caa14cc77a6d34c4d5cfd1a69641e87bf1b3d6ba90d0ba/psutil-5.8.0-cp36-cp36m-win32.whl", hash = "sha256:36b3b6c9e2a34b7d7fbae330a85bf72c30b1c827a4366a07443fc4b6270449e2"},
@@ -2321,17 +2312,17 @@
     {url = "https://files.pythonhosted.org/packages/20/e5/16ff212c1e452235a90aeb09066144d0c5a6a8c0834397e03f5224495c4e/ptyprocess-0.7.0.tar.gz", hash = "sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220"},
     {url = "https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl", hash = "sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35"},
 ]
 "pure-eval 0.2.2" = [
     {url = "https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl", hash = "sha256:01eaab343580944bc56080ebe0a674b39ec44a945e6d09ba7db3cb8cec289350"},
     {url = "https://files.pythonhosted.org/packages/97/5a/0bc937c25d3ce4e0a74335222aee05455d6afa2888032185f8ab50cdf6fd/pure_eval-0.2.2.tar.gz", hash = "sha256:2b45320af6dfaa1750f543d714b6d1c520a1688dec6fd24d339063ce0aaa9ac3"},
 ]
-"pychromecast 12.1.4" = [
-    {url = "https://files.pythonhosted.org/packages/41/f9/f0a32fee8cc8827d4b617dcd4a318f92c5f01f531ff61e7c96c5d9fca038/PyChromecast-12.1.4-py2.py3-none-any.whl", hash = "sha256:adfd8aa06d124a6819b55ad6b977f7ecd577a96036d3e68ecc835b41c6f9f81f"},
-    {url = "https://files.pythonhosted.org/packages/c9/fb/a30cd1b46275c2b8a0572dee5faf8176791394961ad122a59558c5bd950c/PyChromecast-12.1.4.tar.gz", hash = "sha256:9e57dc985a4a05db5bdcd5da219cbf6ced25548ca093f8d74bc107b3c554ec00"},
+"pychromecast 13.0.7" = [
+    {url = "https://files.pythonhosted.org/packages/b3/a7/7bd0c86e0c07872a391085c5896257807186c4436365547747cd75239e83/PyChromecast-13.0.7-py2.py3-none-any.whl", hash = "sha256:2327f1a2c3902e7be901f43dc97e65aeebb42f0d0a8b2c29f55453c6cacc3bd0"},
+    {url = "https://files.pythonhosted.org/packages/d9/cb/d3e8dd7384e2bb4db859486b7a73355934288d65c6f45c65ae59f6abea25/PyChromecast-13.0.7.tar.gz", hash = "sha256:0de98e9e5be43269dd41efb16126ab0d5ba941ca4acae024329712851c0c0324"},
 ]
 "pycparser 2.21" = [
     {url = "https://files.pythonhosted.org/packages/5e/0b/95d387f5f4433cb0f53ff7ad859bd2c6051051cebbb564f139a999ab46de/pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
     {url = "https://files.pythonhosted.org/packages/62/d5/5f610ebe421e85889f2e55e33b7f9a6795bd982198517d912eb1c76e1a53/pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
 ]
 "pycryptodome 3.17" = [
     {url = "https://files.pythonhosted.org/packages/05/6e/ffedda1885ccb5ab52911cfd38ee834c5fa1df1f500f0da34f92b52f70e1/pycryptodome-3.17-cp35-abi3-macosx_10_9_universal2.whl", hash = "sha256:e7debd9c439e7b84f53be3cf4ba8b75b3d0b6e6015212355d6daf44ac672e210"},
```

### Comparing `xklb-1.26.28/readme.py` & `xklb-1.26.29/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.29/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.29/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/.github/workflows/push.yaml` & `xklb-1.26.29/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/sql/transfer.sql` & `xklb-1.26.29/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/av.py` & `xklb-1.26.29/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/books.py` & `xklb-1.26.29/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/consts.py` & `xklb-1.26.29/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/db.py` & `xklb-1.26.29/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/dl_config.py` & `xklb-1.26.29/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/dl_extract.py` & `xklb-1.26.29/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/fs_extract.py` & `xklb-1.26.29/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/gui.py` & `xklb-1.26.29/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/hn_extract.py` & `xklb-1.26.29/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/lb.py` & `xklb-1.26.29/xklb/lb.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
     mining:
+      lb extract-links         Extract links from lists of web pages
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
-      lb nfb-films             NFB Director links -> film links (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
     """
 
 
 def print_help(parser) -> None:
     print(usage())
@@ -194,16 +194,16 @@
     subp_surf.set_defaults(func=scripts.streaming_tab_loader)
 
     subp_nouns = add_parser(subparsers, "nouns")
     subp_nouns.set_defaults(func=scripts.nouns)
 
     subp_reddit_selftext = add_parser(subparsers, "reddit-selftext", ["rst"])
     subp_reddit_selftext.set_defaults(func=scripts.reddit_selftext)
-    subp_nfb_directors = add_parser(subparsers, "nfb-films")
-    subp_nfb_directors.set_defaults(func=scripts.nfb_films)
+    subp_nfb_directors = add_parser(subparsers, "extract-links", ["links"])
+    subp_nfb_directors.set_defaults(func=scripts.extract_links)
 
     parser.add_argument("--version", "-V", action="store_true")
     return parser
 
 
 def library(args=None) -> None:
     if args:
```

### Comparing `xklb-1.26.28/xklb/play_actions.py` & `xklb-1.26.29/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/playback.py` & `xklb-1.26.29/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/player.py` & `xklb-1.26.29/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/praw_extract.py` & `xklb-1.26.29/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/stats.py` & `xklb-1.26.29/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/subtitle.py` & `xklb-1.26.29/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/tabs_actions.py` & `xklb-1.26.29/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/tabs_extract.py` & `xklb-1.26.29/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/tube_backend.py` & `xklb-1.26.29/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/tube_extract.py` & `xklb-1.26.29/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/utils.py` & `xklb-1.26.29/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/__init__.py` & `xklb-1.26.29/xklb/scripts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .bigdirs import bigdirs, process_bigdirs
 from .christen import christen
 from .copy_play_counts import copy_play_counts
 from .dedupe import dedupe
 from .merge_dbs import merge_dbs
 from .merge_online_local import merge_online_local
-from .mining.nfb_ca import nfb_films
+from .mining.extract_links import extract_links
 from .mining.nouns import nouns
 from .mining.pushshift import pushshift_extract
 from .mining.reddit_selftext import reddit_selftext
 from .move_list import move_list
 from .optimize_db import optimize_db
 from .redownload import redownload
 from .relmv import relmv
```

### Comparing `xklb-1.26.28/xklb/scripts/bigdirs.py` & `xklb-1.26.29/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/christen.py` & `xklb-1.26.29/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/copy_play_counts.py` & `xklb-1.26.29/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/dedupe.py` & `xklb-1.26.29/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/merge_dbs.py` & `xklb-1.26.29/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/merge_online_local.py` & `xklb-1.26.29/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/move_list.py` & `xklb-1.26.29/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/optimize_db.py` & `xklb-1.26.29/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/redownload.py` & `xklb-1.26.29/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/relmv.py` & `xklb-1.26.29/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/scatter.py` & `xklb-1.26.29/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.29/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/mining/nouns.py` & `xklb-1.26.29/xklb/scripts/mining/nouns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from html.parser import HTMLParser
 from io import StringIO
 
 from xklb.utils import pipe_print
 
-from . import words
+from . import data
 
 """
 extract compound nouns and phrases from unstructured mixed HTML plain text
 
 xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
 """
 
@@ -41,15 +41,15 @@
 def printer(parts) -> None:
     for part in parts:
         part = part.strip()
         if not part:
             continue
 
         part_lookup = part.lower()
-        if part_lookup in words.stop_words or part_lookup in words.prepositions or is_num(part):
+        if part_lookup in data.stop_words or part_lookup in data.prepositions or is_num(part):
             continue
 
         pipe_print(part)
 
 
 def line_processor(txt) -> None:
     txt = strip_tags(txt)
```

### Comparing `xklb-1.26.28/xklb/scripts/mining/pushshift.py` & `xklb-1.26.29/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.26.29/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/xklb/scripts/mining/words.py` & `xklb-1.26.29/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/assets/kotobago.png` & `xklb-1.26.29/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/.gitignore` & `xklb-1.26.29/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/LICENSE` & `xklb-1.26.29/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/README.md` & `xklb-1.26.29/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.028)
+    xk media library subcommands (v1.26.029)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -69,17 +69,17 @@
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
     mining:
+      lb extract-links         Extract links from lists of web pages
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
-      lb nfb-films             NFB Director links -> film links (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
     
 
 </details>
 
 ### Watch online media on your PC
```

### Comparing `xklb-1.26.28/pyproject.toml` & `xklb-1.26.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.28/PKG-INFO` & `xklb-1.26.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.28
+Version: 1.26.29
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.028)
+    xk media library subcommands (v1.26.029)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -151,17 +151,17 @@
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
     mining:
+      lb extract-links         Extract links from lists of web pages
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
-      lb nfb-films             NFB Director links -> film links (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
     
 
 </details>
 
 ### Watch online media on your PC
```


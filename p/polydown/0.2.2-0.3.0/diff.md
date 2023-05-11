# Comparing `tmp/polydown-0.2.2.tar.gz` & `tmp/polydown-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polydown-0.2.2.tar", last modified: Sun Sep 26 14:09:37 2021, max compression
+gzip compressed data, was "polydown-0.3.0.tar", max compression
```

## Comparing `polydown-0.2.2.tar` & `polydown-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-09-26 14:09:37.075504 polydown-0.2.2/
--rw-rw-rw-   0        0        0     1084 2021-09-23 21:54:13.000000 polydown-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     3221 2021-09-26 14:09:37.075504 polydown-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-09-26 14:09:37.066525 polydown-0.2.2/polydown/
--rw-rw-rw-   0        0        0        0 2021-09-23 21:54:13.000000 polydown-0.2.2/polydown/__init__.py
--rw-rw-rw-   0        0        0     1863 2021-09-26 13:37:48.000000 polydown-0.2.2/polydown/__main__.py
--rw-rw-rw-   0        0        0     2558 2021-09-26 14:00:13.000000 polydown-0.2.2/polydown/cli.py
--rw-rw-rw-   0        0        0     5345 2021-09-26 13:27:31.000000 polydown-0.2.2/polydown/downloader.py
--rw-rw-rw-   0        0        0      617 2021-09-26 12:56:04.000000 polydown-0.2.2/polydown/hash_check.py
--rw-rw-rw-   0        0        0     5891 2021-09-26 13:42:11.000000 polydown-0.2.2/polydown/poly.py
--rw-rw-rw-   0        0        0     1137 2021-09-26 10:09:00.000000 polydown-0.2.2/polydown/report.py
--rw-rw-rw-   0        0        0      760 2021-09-26 10:41:14.000000 polydown-0.2.2/polydown/theme.py
-drwxrwxrwx   0        0        0        0 2021-09-26 14:09:37.073521 polydown-0.2.2/polydown.egg-info/
--rw-rw-rw-   0        0        0     3221 2021-09-26 14:09:36.000000 polydown-0.2.2/polydown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2021-09-26 14:09:36.000000 polydown-0.2.2/polydown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-26 14:09:36.000000 polydown-0.2.2/polydown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2021-09-26 14:09:36.000000 polydown-0.2.2/polydown.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2021-09-26 14:09:36.000000 polydown-0.2.2/polydown.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-09-26 14:09:36.000000 polydown-0.2.2/polydown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-26 14:09:37.075504 polydown-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1103 2021-09-24 20:57:38.000000 polydown-0.2.2/setup.py
+-rw-r--r--   0        0        0     1084 2023-01-27 19:32:31.295859 polydown-0.3.0/LICENSE
+-rw-r--r--   0        0        0        0 2021-09-23 21:54:13.843999 polydown-0.3.0/polydown/__init__.py
+-rw-r--r--   0        0        0     2010 2023-05-11 14:10:10.003943 polydown-0.3.0/polydown/__main__.py
+-rw-r--r--   0        0        0     2586 2023-05-11 14:11:31.005921 polydown-0.3.0/polydown/cli.py
+-rw-r--r--   0        0        0     5590 2023-05-11 14:30:31.183437 polydown-0.3.0/polydown/downloader.py
+-rw-r--r--   0        0        0      617 2021-09-26 12:56:04.492884 polydown-0.3.0/polydown/hash_check.py
+-rw-r--r--   0        0        0     6037 2023-05-11 14:24:28.458577 polydown-0.3.0/polydown/poly.py
+-rw-r--r--   0        0        0     1137 2021-09-26 10:09:00.959542 polydown-0.3.0/polydown/report.py
+-rw-r--r--   0        0        0      760 2021-09-26 10:41:14.957821 polydown-0.3.0/polydown/theme.py
+-rw-r--r--   0        0        0     1113 2023-05-11 14:18:35.348630 polydown-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2701 2021-10-01 08:53:42.097440 polydown-0.3.0/README.MD
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 polydown-0.3.0/setup.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 polydown-0.3.0/PKG-INFO
```

### Comparing `polydown-0.2.2/LICENSE` & `polydown-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polydown-0.2.2/PKG-INFO` & `polydown-0.3.0/README.MD`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: polydown
-Version: 0.2.2
-Summary: Batch downloader for polyhaven (polyhaven.com).
-Home-page: https://github.com/agmmnn/polydown
-Author: agmmnn
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
 <div align="center">
 <a href="https://github.com/agmmnn/polydown">
 <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>
 <a href="https://pypi.org/project/polydown/">
 <img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>
 
@@ -88,9 +71,8 @@
 - Python >3.5
 
 ## Dependencies
 - [requests](https://pypi.org/project/requests/)
 - [rich](https://github.com/willmcgugan/rich)
 
 # License
-[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
-
+[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: polydown Version: 0.2.2 Summary: Batch downloader
-for polyhaven (polyhaven.com). Home-page: https://github.com/agmmnn/polydown
-Author: agmmnn License: MIT Platform: UNKNOWN Classifier: Programming Language
-:: Python :: 3 Classifier: Operating System :: OS Independent Classifier:
-License :: OSI Approved :: MIT License Classifier: Environment :: Console
-Classifier: Topic :: Utilities Requires-Python: >=3.5 Description-Content-Type:
-text/markdown License-File: LICENSE ![screenshot](https://user-
-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-
-9d189379d307.gif)
+![screenshot](https://user-images.githubusercontent.com/16024979/134770914-
+bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
  [GitHub_release_(latest_by_date)] [PyPI] Batch downloader for [polyhaven.com]
 (https://polyhaven.com/). Download hdris, textures and models in any sizes you
   want. This project uses Poly Haven's [Public API](https://github.com/Poly-
                               Haven/Public-API).
 # Installation - `pip install polydown` # How to Use ``` $ polydown hdris #
 download all available sizes of all hdris into current folder. > ð
 (polyhaven.com/hdris['all sizes'])=>ð  ``` ``` $ polydown  # download all
```

### Comparing `polydown-0.2.2/polydown/__main__.py` & `polydown-0.3.0/polydown/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,21 @@
     "-o",
     "--overwrite",
     action="store_true",
     default=False,
     help="Overwrite if the files already exists.  otherwise the current task will be skipped.",
 )
 ap.add_argument(
+    "-t",
+    "--tone",
+    action="store_true",
+    default=False,
+    help="Download 8K Tonemapped JPG (only HDRIs).",
+)
+ap.add_argument(
     "-no",
     "--noimgs",
     action="store_true",
     default=False,
     help="Do not download 'preview, render, thumbnail...' images.",
 )
 ap.add_argument("-v", "--version", action="version", version="%(prog)s v" + __version__)
```

### Comparing `polydown-0.2.2/polydown/cli.py` & `polydown-0.3.0/polydown/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     asset_type = args.asset_type[0]
     folder = args.folder
     overwrite = args.overwrite
     sizes = args.sizes
     category = args.category
     noimgs = args.noimgs
     iters = args.iters
+    tone = args.tone
     s = requests.Session()
 
     # ->🔒asset type->
     asset_type_list = list(json.loads(s.get("https://api.polyhaven.com/types").content))
     if asset_type not in asset_type_list:
         print(f"'{asset_type}' is not a valid asset type!")
         exit()
@@ -72,8 +73,8 @@
         + (f"/{category}" if category != None else "")
         + ("['all sizes']" if sizes == [] else str(sizes))
         + f")=>🏠"
         + (f"({folder})" if not folder == "" else "")
         + "\n"
     )
 
-    Poly(asset_type, s, category, down_folder, sizes, overwrite, noimgs, iters)
+    Poly(asset_type, s, category, down_folder, sizes, overwrite, noimgs, iters, tone)
```

### Comparing `polydown-0.2.2/polydown/downloader.py` & `polydown-0.3.0/polydown/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,28 @@
         type,
         asset,
         session,
         down_folder,
         subfolder,
         filename,
         overwrite,
+        tone,
         # --
         url=None,
         md5=None,
         # --
         k=None,
         b=None,
     ):
         self.type = type
         self.asset = asset
         self.s = session
         self.down_folder = down_folder
         self.overwrite = overwrite
+        self.tone = tone
         self.md5 = md5
         self.url = url
         self.subfolder = subfolder
         self.filename = filename
         self.k = k
         self.b = b
 
@@ -104,14 +106,15 @@
 
     def img(self):
         if self.type == "hdris":
             imgs_dict = {
                 "thumb": f"https://cdn.polyhaven.com/asset_img/thumbs/{self.asset}.png",
                 "primary": f"https://cdn.polyhaven.com/asset_img/primary/{self.asset}.png",
                 "renders_lone_monk": f"https://cdn.polyhaven.com/asset_img/renders/{self.asset}/lone_monk.png",
+                "Tonemapped8K": f"https://dl.polyhaven.org/file/ph-assets/HDRIs/extra/Tonemapped%20JPG/{self.asset}.jpg",
             }
         elif self.type == "textures":
             imgs_dict = {
                 "primary": f"https://cdn.polyhaven.com/asset_img/primary/{self.asset}.png",
                 "thumb": f"https://cdn.polyhaven.com/asset_img/thumbs/{self.asset}.png",
                 "renders_clay": f"https://cdn.polyhaven.com/asset_img/renders/{self.asset}/clay.png",
             }
@@ -132,14 +135,16 @@
                 else f"{self.down_folder}/{filename}",
                 "wb",
             ) as f:
                 f.write(r.content)
 
         print(theme.t_img)
         for i in imgs_dict:
+            if i == "Tonemapped8K" and not self.tone:
+                continue
             filename = f"{self.asset}_{i}.png"
             if filename in self.filelist and self.overwrite == False:
                 print(theme.t_skipped_img + filename)
             elif filename in self.filelist and self.overwrite:
                 save_file(imgs_dict[i], filename)
                 print(theme.t_down_ow_img + filename)
             else:
```

### Comparing `polydown-0.2.2/polydown/hash_check.py` & `polydown-0.3.0/polydown/hash_check.py`

 * *Files identical despite different names*

### Comparing `polydown-0.2.2/polydown/poly.py` & `polydown-0.3.0/polydown/poly.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,38 @@
 from .report import Report
 from .downloader import Downloader
 from . import theme
 
 
 class Poly:
     def __init__(
-        self, type, session, category, down_folder, sizes, overwrite, noimgs, iters
+        self,
+        type,
+        session,
+        category,
+        down_folder,
+        sizes,
+        overwrite,
+        noimgs,
+        iters,
+        tone,
     ):
         self.s = session
         self.type = type
         self.asset_url = f"https://api.polyhaven.com/assets?t={type}"
         if category != None:
             self.asset_url = f"https://api.polyhaven.com/assets?t={type}&c={category}"
         self.asset_list = [i for i in json.loads(self.s.get(self.asset_url).content)]
 
         self.down_folder = down_folder
         self.down_sizes = sizes
         self.overwrite = overwrite
         self.noimgs = noimgs
         self.iters = iters
+        self.tone = tone
 
         self.corrupted_files = []
         self.exist_files = 0
         self.downloaded_files = 0
 
         self.report = Report()
         if type == "textures" or type == "models":
@@ -139,14 +149,15 @@
                     self.type,
                     asset,
                     self.s,
                     self.down_folder,
                     None,
                     filename,
                     self.overwrite,
+                    self.tone,
                     url,
                     md5,
                 )
                 dw = Downloader(*args)
                 d = dw.file()
                 print(d[0])
                 self.report.add(d[1])
```

### Comparing `polydown-0.2.2/polydown/report.py` & `polydown-0.3.0/polydown/report.py`

 * *Files identical despite different names*

### Comparing `polydown-0.2.2/polydown/theme.py` & `polydown-0.3.0/polydown/theme.py`

 * *Files identical despite different names*

### Comparing `polydown-0.2.2/polydown.egg-info/PKG-INFO` & `polydown-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,108 @@
-Metadata-Version: 2.1
-Name: polydown
-Version: 0.2.2
-Summary: Batch downloader for polyhaven (polyhaven.com).
-Home-page: https://github.com/agmmnn/polydown
-Author: agmmnn
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
-<div align="center">
-<a href="https://github.com/agmmnn/polydown">
-<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>
-<a href="https://pypi.org/project/polydown/">
-<img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>
-
-Batch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven's [Public API](https://github.com/Poly-Haven/Public-API).
-</div>
-
-# Installation
-
-- `pip install polydown`
-
-# How to Use
-```
-$ polydown hdris
-
-# download all available sizes of all hdris into current folder.
-> 🔗(polyhaven.com/hdris['all sizes'])=>🏠
-```
-```
-$ polydown <asset_type>
-
-# download all assets of this asset type to the current folder in all available sizes.
-# asset types: "hdris", "textures", "models".
-```
-```
-$ polydown textures -c
-
-# list of category in the given asset type.
-```
-```
-$ polydown hdris -f hdris_down -s 2k 4k
-
-# download all hdris with given sizes into "hdris_down" folder.
-# /if there is no such folder it will create it./
-> 🔗(polyhaven.com/hdris['2k', '4k'])=>🏠(hdris_down)
-```
-## Example Usage
-
-```
-$ polydown models -c decorative -f folder -s 1k
-
-# download all "models" with "1k textures" in the "decorative" category into the "folder".
-```
-![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)
-![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)
-
-# Arguments:
-
-```
-<asset_type>      "hdris, textures, models"
--h, --help        show this help message and exit
--f, --folder      target download folder.
--c, --category    category to download.
--s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k
--o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.
--no, --noimgs     do not download 'preview, render, thumbnail...' images.
--it, --iters      amount of iterations.
--v, --version     show program's version number and exit
-```
-
-# To-Do
--   [ ] Unit Tests
--   [ ] Progressbar for current download task(s)
--   [ ] Select the file format to download
--   [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"
-
-# Requirements
-- Python >3.5
-
-## Dependencies
-- [requests](https://pypi.org/project/requests/)
-- [rich](https://github.com/willmcgugan/rich)
-
-# License
-[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
-
+Metadata-Version: 2.1
+Name: polydown
+Version: 0.3.0
+Summary: Batch downloader for polyhaven (polyhaven.com)
+Home-page: https://github.com/agmmnn/polydown
+License: MIT
+Keywords: polyhaven,download,downloader,scrape,hdri,batch
+Author: Gökçe Merdun
+Author-email: agmmnn@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Utilities
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: rich (>=13.3.0,<14.0.0)
+Project-URL: Bug Tracker, https://github.com/agmmnn/polydown/issues
+Project-URL: Changelog, https://github.com/agmmnn/polydown/releases
+Project-URL: Repository, https://github.com/agmmnn/polydown
+Project-URL: Source, https://github.com/agmmnn/polydown
+Description-Content-Type: text/markdown
+
+![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
+<div align="center">
+<a href="https://github.com/agmmnn/polydown">
+<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>
+<a href="https://pypi.org/project/polydown/">
+<img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>
+
+Batch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven's [Public API](https://github.com/Poly-Haven/Public-API).
+</div>
+
+# Installation
+
+- `pip install polydown`
+
+# How to Use
+```
+$ polydown hdris
+
+# download all available sizes of all hdris into current folder.
+> 🔗(polyhaven.com/hdris['all sizes'])=>🏠
+```
+```
+$ polydown <asset_type>
+
+# download all assets of this asset type to the current folder in all available sizes.
+# asset types: "hdris", "textures", "models".
+```
+```
+$ polydown textures -c
+
+# list of category in the given asset type.
+```
+```
+$ polydown hdris -f hdris_down -s 2k 4k
+
+# download all hdris with given sizes into "hdris_down" folder.
+# /if there is no such folder it will create it./
+> 🔗(polyhaven.com/hdris['2k', '4k'])=>🏠(hdris_down)
+```
+## Example Usage
+
+```
+$ polydown models -c decorative -f folder -s 1k
+
+# download all "models" with "1k textures" in the "decorative" category into the "folder".
+```
+![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)
+![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)
+
+# Arguments:
+
+```
+<asset_type>      "hdris, textures, models"
+-h, --help        show this help message and exit
+-f, --folder      target download folder.
+-c, --category    category to download.
+-s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k
+-o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.
+-no, --noimgs     do not download 'preview, render, thumbnail...' images.
+-it, --iters      amount of iterations.
+-v, --version     show program's version number and exit
+```
+
+# To-Do
+-   [ ] Unit Tests
+-   [ ] Progressbar for current download task(s)
+-   [ ] Select the file format to download
+-   [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"
+
+# Requirements
+- Python >3.5
+
+## Dependencies
+- [requests](https://pypi.org/project/requests/)
+- [rich](https://github.com/willmcgugan/rich)
+
+# License
+[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -1,16 +1,25 @@
-Metadata-Version: 2.1 Name: polydown Version: 0.2.2 Summary: Batch downloader
-for polyhaven (polyhaven.com). Home-page: https://github.com/agmmnn/polydown
-Author: agmmnn License: MIT Platform: UNKNOWN Classifier: Programming Language
-:: Python :: 3 Classifier: Operating System :: OS Independent Classifier:
-License :: OSI Approved :: MIT License Classifier: Environment :: Console
-Classifier: Topic :: Utilities Requires-Python: >=3.5 Description-Content-Type:
-text/markdown License-File: LICENSE ![screenshot](https://user-
-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-
-9d189379d307.gif)
+Metadata-Version: 2.1 Name: polydown Version: 0.3.0 Summary: Batch downloader
+for polyhaven (polyhaven.com) Home-page: https://github.com/agmmnn/polydown
+License: MIT Keywords: polyhaven,download,downloader,scrape,hdri,batch Author:
+GÃ¶kÃ§e Merdun Author-email: agmmnn@gmail.com Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Console Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Topic :: Utilities Requires-Dist: aiohttp
+(>=3.8.3,<4.0.0) Requires-Dist: requests (>=2.30.0,<3.0.0) Requires-Dist: rich
+(>=13.3.0,<14.0.0) Project-URL: Bug Tracker, https://github.com/agmmnn/
+polydown/issues Project-URL: Changelog, https://github.com/agmmnn/polydown/
+releases Project-URL: Repository, https://github.com/agmmnn/polydown Project-
+URL: Source, https://github.com/agmmnn/polydown Description-Content-Type: text/
+markdown ![screenshot](https://user-images.githubusercontent.com/16024979/
+134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
  [GitHub_release_(latest_by_date)] [PyPI] Batch downloader for [polyhaven.com]
 (https://polyhaven.com/). Download hdris, textures and models in any sizes you
   want. This project uses Poly Haven's [Public API](https://github.com/Poly-
                               Haven/Public-API).
 # Installation - `pip install polydown` # How to Use ``` $ polydown hdris #
 download all available sizes of all hdris into current folder. > ð
 (polyhaven.com/hdris['all sizes'])=>ð  ``` ``` $ polydown  # download all
```


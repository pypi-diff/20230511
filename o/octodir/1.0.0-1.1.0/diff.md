# Comparing `tmp/octodir-1.0.0.tar.gz` & `tmp/octodir-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\octodir-1.0.0.tar", last modified: Mon Aug 15 01:39:23 2022, max compression
+gzip compressed data, was "octodir-1.1.0.tar", last modified: Wed May 10 22:29:10 2023, max compression
```

## Comparing `octodir-1.0.0.tar` & `octodir-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-08-15 01:39:23.864657 octodir-1.0.0/
--rw-rw-rw-   0        0        0       25 2022-08-14 20:58:31.000000 octodir-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2235 2022-08-15 01:39:23.865656 octodir-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1116 2022-08-15 01:36:17.000000 octodir-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-15 01:39:23.842670 octodir-1.0.0/octodir/
--rw-rw-rw-   0        0        0       34 2022-08-14 19:46:14.000000 octodir-1.0.0/octodir/__init__.py
--rw-rw-rw-   0        0        0      421 2022-08-13 03:40:43.000000 octodir-1.0.0/octodir/octodir_cli.py
--rw-rw-rw-   0        0        0     4489 2022-08-13 03:40:43.000000 octodir-1.0.0/octodir/octodir_core.py
-drwxrwxrwx   0        0        0        0 2022-08-15 01:39:23.862658 octodir-1.0.0/octodir.egg-info/
--rw-rw-rw-   0        0        0     2235 2022-08-15 01:39:23.000000 octodir-1.0.0/octodir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2022-08-15 01:39:23.000000 octodir-1.0.0/octodir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-15 01:39:23.000000 octodir-1.0.0/octodir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-08-15 01:39:23.000000 octodir-1.0.0/octodir.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2022-08-15 01:39:23.000000 octodir-1.0.0/octodir.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-15 01:39:23.000000 octodir-1.0.0/octodir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2022-08-15 00:36:57.000000 octodir-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2022-08-15 01:39:23.867658 octodir-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1575 2022-08-15 01:34:50.000000 octodir-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:29:10.911060 octodir-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 21:58:05.000000 octodir-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-05-10 21:58:05.000000 octodir-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2136 2023-05-10 22:29:10.911060 octodir-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1413 2023-05-10 22:22:18.000000 octodir-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 22:29:10.911060 octodir-1.1.0/octodir/
+-rw-rw-rw-   0        0        0       35 2023-05-10 21:58:05.000000 octodir-1.1.0/octodir/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-05-10 22:22:18.000000 octodir-1.1.0/octodir/octodir_cli.py
+-rw-rw-rw-   0        0        0     4749 2023-05-10 22:22:18.000000 octodir-1.1.0/octodir/octodir_core.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:29:10.911060 octodir-1.1.0/octodir.egg-info/
+-rw-rw-rw-   0        0        0     2136 2023-05-10 22:29:10.000000 octodir-1.1.0/octodir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-05-10 22:29:10.000000 octodir-1.1.0/octodir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 22:29:10.000000 octodir-1.1.0/octodir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-10 22:29:10.000000 octodir-1.1.0/octodir.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-05-10 22:29:10.000000 octodir-1.1.0/octodir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 22:29:10.000000 octodir-1.1.0/octodir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       46 2023-05-10 21:58:05.000000 octodir-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-10 22:29:10.911060 octodir-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1625 2023-05-10 22:23:45.000000 octodir-1.1.0/setup.py
```

### Comparing `octodir-1.0.0/README.md` & `octodir-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-<div align="center">
-    <img src="logo.png">
-</div>
-
-Tool for downloading directories from Github repositories.
-
-# Installation
-  ```
-  $ pip install octodir
-  ```
-
-# Use
-
-## From the console
-
-```
-$ octodir
-```
-
-**You will be asked for the following data:**
-
-* **Full folder url:** Direct url to the target folder
-  * **Example:** `https://github.com/Jalkhov/octodir/tree/stable/octodir`
-* **Output folder**: Absolute path of the output directory
-  * You can enter a dot to download in the current working directory
-
-## In code
-
-```python
-from octodir import Octodir
-
-target = 'https://github.com/Jalkhov/Octodir/tree/stable/octodir'
-folder = '.' # Current working directory
-
-Octo = Octodir(target, folder)
-Octo.dowload_folder()
-```
-
-# Support me <3
-
-<a href="https://www.buymeacoffee.com/Jalkhov" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
+<div align="center">
+    <img src="https://raw.githubusercontent.com/Jalkhov/octodir/main/logo.png">
+</div>
+
+Tool for downloading directories from Github repositories.
+
+ALERT: Not authenticated requests have limits, fixing for add API Key support.
+
+# Installation
+  ```
+  $ pip install octodir
+  ```
+
+# Use
+
+## From the console
+
+```
+$ octodir
+```
+
+**You will be asked for the following data:**
+
+* **Full folder url:** Direct url to the target folder
+  * **Example:** `https://github.com/Jalkhov/octodir/tree/stable/octodir`
+* **Output folder**: Absolute path of the output directory
+  * You can enter a dot to download in the current working directory
+* **API key**: Personal Github Token for prevent requests limit
+
+## In code
+
+```python
+from octodir import Octodir
+
+target = 'https://github.com/Jalkhov/Octodir/tree/stable/octodir'
+folder = '.' # Current working directory
+api_key = '<PERSONAL_GITHUB_TOKEN>'
+
+Octo = Octodir(target, folder, api_key=api_key)
+Octo.dowload_folder()
+```
+
+# Support me <3
+
+<a href="https://www.buymeacoffee.com/Jalkhov" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
```

#### html2text {}

```diff
@@ -1,10 +1,13 @@
-                                  [logo.png]
-Tool for downloading directories from Github repositories. # Installation ``` $
-pip install octodir ``` # Use ## From the console ``` $ octodir ``` **You will
-be asked for the following data:** * **Full folder url:** Direct url to the
-target folder * **Example:** `https://github.com/Jalkhov/octodir/tree/stable/
-octodir` * **Output folder**: Absolute path of the output directory * You can
-enter a dot to download in the current working directory ## In code ```python
-from octodir import Octodir target = 'https://github.com/Jalkhov/Octodir/tree/
-stable/octodir' folder = '.' # Current working directory Octo = Octodir(target,
-folder) Octo.dowload_folder() ``` # Support me <3 [Buy_Me_A_Coffee]
+       [https://raw.githubusercontent.com/Jalkhov/octodir/main/logo.png]
+Tool for downloading directories from Github repositories. ALERT: Not
+authenticated requests have limits, fixing for add API Key support. #
+Installation ``` $ pip install octodir ``` # Use ## From the console ``` $
+octodir ``` **You will be asked for the following data:** * **Full folder url:
+** Direct url to the target folder * **Example:** `https://github.com/Jalkhov/
+octodir/tree/stable/octodir` * **Output folder**: Absolute path of the output
+directory * You can enter a dot to download in the current working directory *
+**API key**: Personal Github Token for prevent requests limit ## In code
+```python from octodir import Octodir target = 'https://github.com/Jalkhov/
+Octodir/tree/stable/octodir' folder = '.' # Current working directory api_key =
+'' Octo = Octodir(target, folder, api_key=api_key) Octo.dowload_folder() ``` #
+Support me <3 [Buy_Me_A_Coffee]
```

### Comparing `octodir-1.0.0/octodir/octodir_core.py` & `octodir-1.1.0/octodir/octodir_core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import json
-import os
-import urllib.request
-
-import requests
-from tqdm import tqdm
-
-
-class repo_info:
-    repo = None
-    target_dir = None
-    branch = None
-
-
-class api_urls:
-    recursive = "https://api.github.com/repos/{}/git/trees/{}?recursive=1"
-    no_recursive = "https://api.github.com/repos/{}/git/trees/{}"
-
-
-class OctodirException(Exception):
-    pass
-
-
-def mkdirs(path):
-    if not os.path.isdir(path):
-        os.makedirs(path)
-
-
-class Octodir(object):
-
-    def __init__(self, folder_url, output_folder):
-        super(Octodir, self).__init__()
-        self.folder_url = folder_url
-        self.output_folder = output_folder
-
-        self.repo = None
-        self.target_dir = None
-        self.branch = None
-
-    def __get_raw_url(self, file_path, url):
-        tmp_url = url.replace(
-            'https://api.github.com/repos/',
-            'https://raw.githubusercontent.com/')
-        tmp_url = tmp_url.split('/git/blobs/')[0]
-        tmp_url = tmp_url + '/' + self.branch + '/' + file_path
-
-        return tmp_url
-
-    def __get_repo_tree(self):
-        api = requests.get(
-            api_urls.recursive.format(self.repo, self.branch)).text
-        files = json.loads(api)
-
-        output = []
-        location = dict()
-        for (k, i) in enumerate(files['tree']):
-            # If the target dir is in file path, that file
-            # is inside target folder
-            if self.target_dir in i['path']:
-                if i['type'] == 'blob':
-                    tmp = [i['path']]
-                    tmp += [self.__get_raw_url(tmp[0], i['url'])]
-                    output.append(tmp)
-                else:
-                    location[i['path']] = k
-        files = output
-        location = location
-
-        return (files, location)
-
-    def __scrutinize_url(self, folder_url):
-        try:
-            cutted_url = folder_url.replace('https://github.com/', '')
-            splitted_url = cutted_url.split('/')
-
-            owner = splitted_url[0]
-            repo = splitted_url[1]
-            branch = splitted_url[3]
-
-            target_dir = [item for item in splitted_url[4:]]
-
-            repo_data = repo_info()
-            repo_data.repo = owner + '/' + repo
-            repo_data.branch = branch
-            repo_data.target_dir = "/".join(target_dir)
-
-            return repo_data
-        except IndexError:
-            raise IndexError('Invalid repo url')
-
-    def __api_response(self):
-        repo_data = self.__scrutinize_url(self.folder_url)
-        api = requests.get(api_urls.no_recursive.format(
-            repo_data.repo, repo_data.branch)).text
-        response = json.loads(api)
-
-        return response
-
-    def __check_valid_output(self):
-        if os.path.isdir(self.output_folder):
-            return True
-        else:
-            raise OctodirException('Invalid output directory')
-
-    def __download(self, target_folder='*', recursive=True):
-        data = self.__get_repo_tree()
-        files = data[0]
-        location = data[1]
-
-        # mkdirs(".")
-
-        if target_folder == '*':
-            start = 0
-        else:
-            tmp_target = target_folder.replace('./', '')
-            tmp_target = tmp_target.replace('../', '')
-
-            # Remove "/"
-            tmp_target = (tmp_target if tmp_target[-1] != '/'
-                          else tmp_target[:-1])
-            start = location[target_folder]
-
-        with tqdm(total=len(files), desc="Downloading folder...") as pbar:
-            for i in files[start:]:
-
-                ndir = i[0].replace(
-                    self.target_dir, self.target_dir.split('/')[-1:][0])
-                if recursive or ndir.split(target_folder)[1].count('/') \
-                        <= 1:
-
-                    # Check output dir variable
-                    mkdirs(os.path.join(self.output_folder, os.path.dirname(ndir)))
-                    urllib.request.urlretrieve(
-                        i[1], os.path.join(self.output_folder, ndir))
-                pbar.update(1)
-
-    def dowload_folder(self):
-        check_repo = self.__api_response()
-        if 'message' in check_repo:
-            raise OctodirException(check_repo['message'])
-        else:
-            if self.__check_valid_output() is True:
-                scrutinized_url = self.__scrutinize_url(self.folder_url)
-                self.repo = scrutinized_url.repo
-                self.target_dir = scrutinized_url.target_dir
-                self.branch = scrutinized_url.branch
-                self.__download()
+import json
+import os
+import urllib.request
+
+import requests
+from tqdm import tqdm
+
+
+class repo_info:
+    repo = None
+    target_dir = None
+    branch = None
+
+
+class api_urls:
+    recursive = "https://api.github.com/repos/{}/git/trees/{}?recursive=1"
+    no_recursive = "https://api.github.com/repos/{}/git/trees/{}"
+
+
+class OctodirException(Exception):
+    pass
+
+
+def mkdirs(path):
+    if not os.path.isdir(path):
+        os.makedirs(path)
+
+
+class Octodir(object):
+
+    def __init__(self, folder_url, output_folder, api_key):
+        super(Octodir, self).__init__()
+        self.folder_url = folder_url
+        self.output_folder = output_folder
+        self.headers = {"Authorization": f"Token {api_key}"}
+        self.repo = None
+        self.target_dir = None
+        self.branch = None
+
+    def __get_raw_url(self, file_path, url):
+        tmp_url = url.replace(
+            'https://api.github.com/repos/',
+            'https://raw.githubusercontent.com/')
+        tmp_url = tmp_url.split('/git/blobs/')[0]
+        tmp_url = tmp_url + '/' + self.branch + '/' + file_path
+
+        return tmp_url
+
+    def __get_repo_tree(self):
+        api = requests.get(
+            api_urls.recursive.format(self.repo, self.branch), headers=self.headers).text
+        files = json.loads(api)
+
+        output = []
+        location = dict()
+        for (k, i) in enumerate(files['tree']):
+            # If the target dir is in file path, that file
+            # is inside target folder
+            if self.target_dir in i['path']:
+                if i['type'] == 'blob':
+                    tmp = [i['path']]
+                    tmp += [self.__get_raw_url(tmp[0], i['url'])]
+                    output.append(tmp)
+                else:
+                    location[i['path']] = k
+        files = output
+        location = location
+
+        return (files, location)
+
+    def __scrutinize_url(self, folder_url):
+        try:
+            cutted_url = folder_url.replace('https://github.com/', '')
+            splitted_url = cutted_url.split('/')
+
+            owner = splitted_url[0]
+            repo = splitted_url[1]
+            branch = splitted_url[3]
+
+            target_dir = [item for item in splitted_url[4:]]
+
+            repo_data = repo_info()
+            repo_data.repo = owner + '/' + repo
+            repo_data.branch = branch
+            repo_data.target_dir = "/".join(target_dir)
+
+            return repo_data
+        except IndexError:
+            raise IndexError('Invalid repo url')
+
+    def __api_response(self):
+        repo_data = self.__scrutinize_url(self.folder_url)
+        api = requests.get(api_urls.no_recursive.format(
+            repo_data.repo, repo_data.branch), headers=self.headers).text
+        response = json.loads(api)
+
+        return response
+
+    def __check_valid_output(self):
+        if os.path.isdir(self.output_folder):
+            return True
+        else:
+            raise OctodirException('Invalid output directory')
+
+    def __download(self, target_folder='*', recursive=True):
+        data = self.__get_repo_tree()
+        files = data[0]
+        location = data[1]
+
+        # mkdirs(".")
+
+        if target_folder == '*':
+            start = 0
+        else:
+            tmp_target = target_folder.replace('./', '')
+            tmp_target = tmp_target.replace('../', '')
+
+            # Remove "/"
+            tmp_target = (tmp_target if tmp_target[-1] != '/'
+                          else tmp_target[:-1])
+            start = location[target_folder]
+
+        with tqdm(total=len(files), desc="Downloading folder...") as pbar:
+            for i in files[start:]:
+
+                ndir = i[0].replace(
+                    self.target_dir, self.target_dir.split('/')[-1:][0])
+                if recursive or ndir.split(target_folder)[1].count('/') \
+                        <= 1:
+
+                    # Check output dir variable
+                    mkdirs(os.path.join(self.output_folder, os.path.dirname(ndir)))
+                    urllib.request.urlretrieve(
+                        i[1], os.path.join(self.output_folder, ndir))
+                pbar.update(1)
+
+    def dowload_folder(self):
+        check_repo = self.__api_response()
+        if 'message' in check_repo:
+            raise OctodirException(check_repo['message'])
+        else:
+            if self.__check_valid_output() is True:
+                scrutinized_url = self.__scrutinize_url(self.folder_url)
+                self.repo = scrutinized_url.repo
+                self.target_dir = scrutinized_url.target_dir
+                self.branch = scrutinized_url.branch
+                self.__download()
```

### Comparing `octodir-1.0.0/setup.py` & `octodir-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import os
-import sys
-
-from setuptools import setup
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-if sys.argv[-1] == "publish":
-    os.system("python setup.py sdist")
-    os.system("twine upload dist/* --skip-existing")
-    sys.exit()
-elif sys.argv[-1] == "test":
-    os.system("python setup.py sdist")
-    os.system("twine upload -r testpypi dist/* --skip-existing")
-    sys.exit()
-
-with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
-    long_description = f.read()
-setup(
-    name='octodir',
-    version="1.0.0",
-    description="Tool for downloading directories from Github repositories",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Jalkhov/octodir",
-    author="Pedro Torcatt",
-    author_email="pedrotorcattsoto@gmail.com",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Programming Language :: Python :: 3",
-        "Natural Language :: English",
-        "Environment :: Console",
-        "License :: OSI Approved :: MIT License",
-    ],
-    keywords="github directory download",
-    packages=["octodir"],
-    include_package_data=True,
-    python_requires=">=3.0",
-    install_requires=open(
-        os.path.join(here, "requirements.txt"), encoding="utf-8"
-    )
-    .read()
-    .split("\n"),
-    project_urls={
-        "Bug Reports": "https://github.com/Jalkhov/octodir/issues",
-        "Source": "https://github.com/Jalkhov/octodir/",
-    },
-    entry_points={"console_scripts": [
-        "octodir=octodir.octodir_cli:octodir_cli"]},
-)
+import os
+import sys
+
+from setuptools import setup
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+if sys.argv[-1] == "publish":
+    os.system("python setup.py sdist")
+    os.system("twine upload dist/* --skip-existing")
+    sys.exit()
+elif sys.argv[-1] == "test":
+    os.system("python setup.py sdist")
+    os.system("twine upload -r testpypi dist/* --skip-existing")
+    sys.exit()
+
+with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+    long_description = f.read()
+setup(
+    name='octodir',
+    version="1.1.0",
+    description="Tool for downloading directories from Github repositories",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Jalkhov/octodir",
+    author="Pedro Torcatt",
+    author_email="pedrotorcattsoto@gmail.com",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Programming Language :: Python :: 3",
+        "Natural Language :: English",
+        "Environment :: Console",
+        "License :: OSI Approved :: MIT License",
+    ],
+    keywords="github directory download",
+    packages=["octodir"],
+    include_package_data=True,
+    python_requires=">=3.0",
+    install_requires=open(
+        os.path.join(here, "requirements.txt"), encoding="utf-8"
+    )
+    .read()
+    .split("\n"),
+    project_urls={
+        "Bug Reports": "https://github.com/Jalkhov/octodir/issues",
+        "Source": "https://github.com/Jalkhov/octodir/",
+    },
+    entry_points={"console_scripts": [
+        "octodir=octodir.octodir_cli:octodir_cli"]},
+)
```


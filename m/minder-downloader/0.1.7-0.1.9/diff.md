# Comparing `tmp/minder_downloader-0.1.7.tar.gz` & `tmp/minder_downloader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minder_downloader-0.1.7.tar", max compression
+gzip compressed data, was "minder_downloader-0.1.9.tar", max compression
```

## Comparing `minder_downloader-0.1.7.tar` & `minder_downloader-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0     2296 2023-03-13 06:58:21.238849 minder_downloader-0.1.7/README.md
--rw-r--r--   0        0        0      140 2023-04-04 19:54:51.041491 minder_downloader-0.1.7/minder_downloader/__init__.py
--rw-r--r--   0        0        0      154 2023-04-18 06:43:58.210176 minder_downloader-0.1.7/minder_downloader/__version__.py
--rw-r--r--   0        0        0     2176 2023-04-18 06:41:56.332419 minder_downloader-0.1.7/minder_downloader/config.py
--rw-r--r--   0        0        0     9556 2023-04-14 12:07:46.275779 minder_downloader-0.1.7/minder_downloader/download.py
--rw-r--r--   0        0        0     2279 2023-04-14 07:08:52.609588 minder_downloader-0.1.7/minder_downloader/info.py
--rw-r--r--   0        0        0      419 2023-03-13 11:49:39.589041 minder_downloader-0.1.7/minder_downloader/update.py
--rw-r--r--   0        0        0     1081 2023-04-08 03:48:59.591442 minder_downloader-0.1.7/minder_downloader/upload.py
--rw-r--r--   0        0        0     5586 2023-04-08 03:49:16.155397 minder_downloader-0.1.7/minder_downloader/utils.py
--rw-r--r--   0        0        0      548 2023-04-18 06:44:01.232789 minder_downloader-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 minder_downloader-0.1.7/setup.py
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 minder_downloader-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2296 2023-03-13 06:58:21.238849 minder_downloader-0.1.9/README.md
+-rw-r--r--   0        0        0      140 2023-03-13 09:18:20.869039 minder_downloader-0.1.9/minder_downloader/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     5456 2023-03-13 09:13:50.205564 minder_downloader-0.1.9/minder_downloader/.ipynb_checkpoints/download-checkpoint.py
+-rw-r--r--   0        0        0     1095 2023-03-13 09:15:50.153142 minder_downloader-0.1.9/minder_downloader/.ipynb_checkpoints/info-checkpoint.py
+-rw-r--r--   0        0        0       87 2023-03-13 09:47:33.407036 minder_downloader-0.1.9/minder_downloader/.ipynb_checkpoints/upload-checkpoint.py
+-rw-r--r--   0        0        0      140 2023-04-04 19:54:51.041491 minder_downloader-0.1.9/minder_downloader/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-18 09:24:53.326367 minder_downloader-0.1.9/minder_downloader/__version__.py
+-rw-r--r--   0        0        0     2269 2023-04-18 09:23:25.959432 minder_downloader-0.1.9/minder_downloader/config.py
+-rw-r--r--   0        0        0     9435 2023-04-18 09:08:59.317069 minder_downloader-0.1.9/minder_downloader/download.py
+-rw-r--r--   0        0        0     2148 2023-04-18 09:16:14.294655 minder_downloader-0.1.9/minder_downloader/info.py
+-rw-r--r--   0        0        0      419 2023-03-13 11:49:39.589041 minder_downloader-0.1.9/minder_downloader/update.py
+-rw-r--r--   0        0        0     1081 2023-04-08 03:48:59.591442 minder_downloader-0.1.9/minder_downloader/upload.py
+-rw-r--r--   0        0        0     5586 2023-04-08 03:49:16.155397 minder_downloader-0.1.9/minder_downloader/utils.py
+-rw-r--r--   0        0        0      548 2023-04-18 09:24:51.193649 minder_downloader-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 minder_downloader-0.1.9/setup.py
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 minder_downloader-0.1.9/PKG-INFO
```

### Comparing `minder_downloader-0.1.7/README.md` & `minder_downloader-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.7/minder_downloader/config.py` & `minder_downloader-0.1.9/minder_downloader/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,34 @@
 
     Returns:
     None
     """
 
     global CONFIG_CHECKED
     if CONFIG_CHECKED:
-        return
+        return os.environ['MINDER_DOWNLOADER_HOME']
     CONFIG_CHECKED = True
 
     root = check_root_folder()
 
     check_token_file(root) # check if token is set at the environment level
+
+    return root
         
 
 
 def check_root_folder():
     root = os.environ.get('MINDER_DOWNLOADER_HOME')
     if root is None:
         root = Path.home()
+
     minder_home = Path(f'{root}{os.sep}.minder')
     if not minder_home.exists():
         minder_home.mkdir(parents=True)
-        os.environ['MINDER_DOWNLOADER_HOME'] = f'{minder_home}'
+    os.environ['MINDER_DOWNLOADER_HOME'] = f'{minder_home}'
     return f'{minder_home}'
 
 
 def check_token_file(root):
     token_path = os.environ.get('RESEARCH_PORTAL_TOKEN_PATH') 
     TOKEN = None 
     info_path = f'{root}{os.sep}info.yaml'
@@ -51,12 +54,13 @@
             TOKEN = tmp['token']
         else:     
             TOKEN = get_token()
     elif Path(token_path).exists(): 
         with open(token_path, 'r') as file:
             TOKEN = file.read() 
     if not (TOKEN is None):
-        tmp['token'] = TOKEN     
+        tmp['token'] = TOKEN    
+        os.environ['MINDER_TOKEN'] = TOKEN
         if not path_exists(info_path):   
             write_yaml(info_path,tmp)
     else:
         raise NameError("Token is missing or wasn't set")
```

### Comparing `minder_downloader-0.1.7/minder_downloader/download.py` & `minder_downloader-0.1.9/minder_downloader/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 from .config import check_config
 
 # Set up logging
 # logging.basicConfig(level=logging.DEBUG)
 # logging.getLogger("urllib3").setLevel(logging.WARNING)
 logging.basicConfig(level=logging.WARNING)
 #
-ROOT = os.environ.get('MINDER_DOWNLOADER_HOME', Path(__file__).parent)
 
 
 
 class MinderDatasetDownload:
     """
     Class for downloading Minder research portal datasets.
 
@@ -82,15 +81,15 @@
         - until: A datetime object representing the end date of the desired data.
         - datasets: A list of strings representing the names of the datasets to download.
         - organizations (optional): A list of strings representing the names of the organizations to download data from.
 
         Returns:
         None
         """
-        check_config()
+        self.root = check_config()
         self.setup()        
         since = since or dt.datetime.now() -  dt.timedelta(days=7)
         until = until or dt.datetime.now()
         self.since = date2iso(since)
         self.until = date2iso(until)
         self.datasets = datasets if type(datasets) is list else [datasets]
         self.datasets_info = _minder_datasets_info()
@@ -105,16 +104,15 @@
         }
         if organizations:
             self.data_request['organizations'] = organizations
         self._request_id = ''
         self._csv_url = pd.DataFrame()
 
     def setup(self) -> None:
-        INFO_PATH = f'{ROOT}{os.sep}info.yaml'
-        os.environ['MINDER_TOKEN'] = load_yaml(INFO_PATH)['token']
+        INFO_PATH = f'{self.root}{os.sep}info.yaml'
         self.server = load_yaml(INFO_PATH)['server'] + '/export'
         self.headers = load_yaml(INFO_PATH)['headers'] 
         self.auth = BearerAuth(os.getenv('MINDER_TOKEN'))
 
 
     def post_request(self) -> None:
         """
```

### Comparing `minder_downloader-0.1.7/minder_downloader/info.py` & `minder_downloader-0.1.9/minder_downloader/info.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 import os 
 from pathlib import Path
 
 
 
 def setup() -> tuple:
     # Load credentials and server information from YAML file
-    check_config()
-    ROOT = os.environ.get('MINDER_DOWNLOADER_HOME', Path(__file__).parent)
-    INFO_PATH = f'{ROOT}{os.sep}info.yaml'
-    os.environ['MINDER_TOKEN'] = load_yaml(INFO_PATH)['token']
-    server = load_yaml(INFO_PATH)['server'] + '/export'
+    root = check_config()
+    info_path = f'{root}{os.sep}info.yaml'
     token = os.getenv('MINDER_TOKEN')
+    server = load_yaml(info_path)['server'] + '/export'
     return server,token
 
 
 def _minder_datasets_info() -> pd.DataFrame:
     """
     Returns a Pandas DataFrame with information about Minder research portal datasets.
     Parameters:
```

### Comparing `minder_downloader-0.1.7/minder_downloader/upload.py` & `minder_downloader-0.1.9/minder_downloader/upload.py`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.7/minder_downloader/utils.py` & `minder_downloader-0.1.9/minder_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.7/pyproject.toml` & `minder_downloader-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "minder-downloader"
-version = "0.1.07"
+version = "0.1.09"
 description = "The minder-downloader module provides a simple interface for downloading datasets and uploading reports using the Minder research portal."
 authors = ["Dr Eyal Soreq <eyal.soreq@ukdri.ac.uk>"]
 readme = "README.md"
 packages = [{include = "minder_downloader"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `minder_downloader-0.1.7/setup.py` & `minder_downloader-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['minder_downloader']
+['minder_downloader', 'minder_downloader..ipynb_checkpoints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24,<2.0',
  'pandas>=1.5,<2.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'minder-downloader',
-    'version': '0.1.7',
+    'version': '0.1.9',
     'description': 'The minder-downloader module provides a simple interface for downloading datasets and uploading reports using the Minder research portal.',
     'long_description': "# Minder Downloader\nThe minder-downloader module is a Python package that provides a user-friendly interface for interacting with the Minder research portal. This package enables users to easily download datasets from the Minder research portal, as well as upload reports to the platform.\n\nThe downloading functionality of the package is straightforward to use. The module handles the authentication and request/response handling, so the user doesn't need to worry about the details of these processes. Once authenticated, users can specify the date range and datasets to download, and the module will return the data as a Pandas DataFrame. This makes it easy to work with the data using Python's powerful data analysis tools.\n\nIn addition to downloading data, the minder-downloader module also provides a simple way to upload reports to the Minder research portal. This can be done by providing the path to a file and the HTML address to upload the file to. The module takes care of the uploading process, making it easy to share reports with collaborators or the wider research community.\n\nOverall, the minder-downloader package provides a convenient and streamlined way to interact with the Minder research portal, whether you need to download data or upload reports.\n\n## Installation\nYou can install minder-downloader using pip:\n\n```bash\npip install minder-downloader\n```\n\n## Usage\nHere is a simple example of how to use minder-downloader to download data from the Minder research portal:\n\n```python\nfrom datetime import datetime, timedelta\nfrom minder_downloader import MinderDatasetDownload\n\n# Define date range and datasets to download\nsince = datetime.now() - timedelta(days=7)\nuntil = datetime.now()\ndatasets = ['example_dataset_1', 'example_dataset_2']\n\n# Create downloader object and download data\ndownloader = MinderDatasetDownload(since, until, datasets)\ndata = downloader.download_data()\n\n# Print downloaded data\nprint(data.head())\n```\n\nThis will download the specified datasets for the past week and print the first few rows of the resulting DataFrame.\n\n## License\nminder-downloader is licensed under the MIT License. See the LICENSE file for details.\n\n## Acknowledgements\nThis module was created by Dr Eyal Soreq. If you find it useful, please consider citing it in your research.",
     'author': 'Dr Eyal Soreq',
     'author_email': 'eyal.soreq@ukdri.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `minder_downloader-0.1.7/PKG-INFO` & `minder_downloader-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minder-downloader
-Version: 0.1.7
+Version: 0.1.9
 Summary: The minder-downloader module provides a simple interface for downloading datasets and uploading reports using the Minder research portal.
 Author: Dr Eyal Soreq
 Author-email: eyal.soreq@ukdri.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


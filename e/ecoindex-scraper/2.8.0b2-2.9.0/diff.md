# Comparing `tmp/ecoindex_scraper-2.8.0b2.tar.gz` & `tmp/ecoindex_scraper-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoindex_scraper-2.8.0b2.tar", max compression
+gzip compressed data, was "ecoindex_scraper-2.9.0.tar", max compression
```

## Comparing `ecoindex_scraper-2.8.0b2.tar` & `ecoindex_scraper-2.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    18648 2022-11-22 10:54:42.855891 ecoindex_scraper-2.8.0b2/LICENSE
--rw-r--r--   0        0        0     3251 2022-11-22 10:54:42.855891 ecoindex_scraper-2.8.0b2/README.md
--rw-r--r--   0        0        0       35 2022-11-22 10:54:42.855891 ecoindex_scraper-2.8.0b2/ecoindex_scraper/__init__.py
--rw-r--r--   0        0        0     6584 2022-11-22 10:54:42.855891 ecoindex_scraper-2.8.0b2/ecoindex_scraper/scrap.py
--rw-r--r--   0        0        0      680 2022-11-22 10:54:42.855891 ecoindex_scraper-2.8.0b2/ecoindex_scraper/utils.py
--rw-r--r--   0        0        0      760 2022-11-22 10:54:42.855891 ecoindex_scraper-2.8.0b2/pyproject.toml
--rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 ecoindex_scraper-2.8.0b2/setup.py
--rw-r--r--   0        0        0     4016 1970-01-01 00:00:00.000000 ecoindex_scraper-2.8.0b2/PKG-INFO
+-rw-r--r--   0        0        0    18648 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/LICENSE
+-rw-r--r--   0        0        0     3251 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/README.md
+-rw-r--r--   0        0        0       35 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/ecoindex_scraper/__init__.py
+-rw-r--r--   0        0        0     6584 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/ecoindex_scraper/scrap.py
+-rw-r--r--   0        0        0      680 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/ecoindex_scraper/utils.py
+-rw-r--r--   0        0        0      757 2022-11-29 10:09:55.139264 ecoindex_scraper-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 ecoindex_scraper-2.9.0/setup.py
+-rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 ecoindex_scraper-2.9.0/PKG-INFO
```

### Comparing `ecoindex_scraper-2.8.0b2/LICENSE` & `ecoindex_scraper-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-2.8.0b2/README.md` & `ecoindex_scraper-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-2.8.0b2/ecoindex_scraper/scrap.py` & `ecoindex_scraper-2.9.0/ecoindex_scraper/scrap.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-2.8.0b2/ecoindex_scraper/utils.py` & `ecoindex_scraper-2.9.0/ecoindex_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-2.8.0b2/pyproject.toml` & `ecoindex_scraper-2.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ecoindex_scraper"
-version = "v2.8.0b2"
+version = "v2.9.0"
 description = "Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser"
 authors = ["Vincent Vatelot <vincent.vatelot@ik.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://www.ecoindex.fr"
 repository = "https://github.com/cnumr/ecoindex_scraper_python"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-ecoindex = {version = "^5.2.0b1", allow-prereleases = true}
-undetected-chromedriver = "3.1.6"
+ecoindex = {version = "^5.3.0", allow-prereleases = true}
+undetected-chromedriver = "^3.1.6"
 Pillow = "^9.2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 black = {version = "^22.10.0", allow-prereleases = true}
 
 [build-system]
```

### Comparing `ecoindex_scraper-2.8.0b2/setup.py` & `ecoindex_scraper-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 ['ecoindex_scraper']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.2.0,<10.0.0',
- 'ecoindex>=5.2.0b1,<6.0.0',
- 'undetected-chromedriver==3.1.6']
+ 'ecoindex>=5.3.0,<6.0.0',
+ 'undetected-chromedriver>=3.1.6,<4.0.0']
 
 setup_kwargs = {
     'name': 'ecoindex-scraper',
-    'version': '2.8.0b2',
+    'version': '2.9.0',
     'description': 'Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser',
     'long_description': '# ECOINDEX SCRAPER PYTHON\n\n![Quality check](https://github.com/cnumr/ecoindex_scrap_python/workflows/Quality%20checks/badge.svg)\n[![PyPI version](https://badge.fury.io/py/ecoindex-scraper.svg)](https://badge.fury.io/py/ecoindex-scraper)\n\nThis module provides a simple interface to get the [Ecoindex](http://www.ecoindex.fr) of a given webpage using module [ecoindex-python](https://pypi.org/project/ecoindex/)\n\n## Requirements\n\n- Python ^3.10 with [pip](https://pip.pypa.io/en/stable/installation/)\n- Google Chrome installed on your computer\n\n## Install\n\n```shell\npip install ecoindex-scraper\n```\n\n## Use\n\n### Get a page analysis\n\nYou can run a page analysis by calling the function `get_page_analysis()`:\n\n```python\n(function) get_page_analysis: (url: HttpUrl, window_size: WindowSize | None = WindowSize(width=1920, height=1080), wait_before_scroll: int | None = 1, wait_after_scroll: int | None = 1) -> Coroutine[Any, Any, Result]\n```\n\nExample:\n\n```python\nimport asyncio\nfrom pprint import pprint\n\nfrom ecoindex_scraper.scrap import EcoindexScraper\n\npprint(\n    asyncio.run(\n        EcoindexScraper(url="http://ecoindex.fr")\n        .init_chromedriver()\n        .get_page_analysis()\n    )\n)\n```\n\nResult example:\n\n```python\nResult(width=1920, height=1080, url=HttpUrl(\'http://ecoindex.fr\', ), size=549.253, nodes=52, requests=12, grade=\'A\', score=90.0, ges=1.2, water=1.8, ecoindex_version=\'5.0.0\', date=datetime.datetime(2022, 9, 12, 10, 54, 46, 773443), page_type=None)\n```\n\n> **Default behaviour:** By default, the page analysis simulates:\n>\n> - Window size of **1920x1080** pixels (can be set with parameter `window_size`)\n> - Wait for **1 second when page is loaded** (can be set with parameter `wait_before_scroll`)\n> - Scroll to the bottom of the page (if it is possible)\n> - Wait for **1 second after** having scrolled to the bottom of the page (can be set with parameter `wait_after_scroll`)\n\n### Get a page analysis and generate a screenshot\n\nIt is possible to generate a screenshot of the analyzed page by adding a `ScreenShot` property to the `EcoindexScraper` object.\nYou have to define an id (can be a string, but it is recommended to use a unique id) and a path to the screenshot file (if the folder does not exist, it will be created).\n\n```python\nimport asyncio\nfrom pprint import pprint\nfrom uuid import uuid1\n\nfrom ecoindex.models import ScreenShot\nfrom ecoindex_scraper.scrap import EcoindexScraper\n\npprint(\n    asyncio.run(\n        EcoindexScraper(\n            url="http://www.ecoindex.fr/",\n            screenshot=ScreenShot(id=str(uuid1()), folder="./screenshots"),\n        )\n        .init_chromedriver()\n        .get_page_analysis()\n    )\n)\n```\n\n## Contribute\n\nYou need [poetry](https://python-poetry.org/) to install and manage dependencies. Once poetry installed, run :\n\n```bash\npoetry install\n```\n\n## Tests\n\n```shell\npoetry run pytest\n```\n\n## Disclaimer\n\nThe LCA values used by [ecoindex_scraper](https://github.com/cnumr/ecoindex_scrap_python) to evaluate environmental impacts are not under free license - ©Frédéric Bordage\nPlease also refer to the mentions provided in the code files for specifics on the IP regime.\n\n## [License](LICENSE)\n\n## [Contributing](CONTRIBUTING.md)\n\n## [Code of conduct](CODE_OF_CONDUCT.md)\n',
     'author': 'Vincent Vatelot',
     'author_email': 'vincent.vatelot@ik.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://www.ecoindex.fr',
```

### Comparing `ecoindex_scraper-2.8.0b2/PKG-INFO` & `ecoindex_scraper-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ecoindex-scraper
-Version: 2.8.0b2
+Version: 2.9.0
 Summary: Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser
 Home-page: http://www.ecoindex.fr
 License: MIT
 Author: Vincent Vatelot
 Author-email: vincent.vatelot@ik.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
-Requires-Dist: ecoindex (>=5.2.0b1,<6.0.0)
-Requires-Dist: undetected-chromedriver (==3.1.6)
+Requires-Dist: ecoindex (>=5.3.0,<6.0.0)
+Requires-Dist: undetected-chromedriver (>=3.1.6,<4.0.0)
 Project-URL: Repository, https://github.com/cnumr/ecoindex_scraper_python
 Description-Content-Type: text/markdown
 
 # ECOINDEX SCRAPER PYTHON
 
 ![Quality check](https://github.com/cnumr/ecoindex_scrap_python/workflows/Quality%20checks/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ecoindex-scraper.svg)](https://badge.fury.io/py/ecoindex-scraper)
```


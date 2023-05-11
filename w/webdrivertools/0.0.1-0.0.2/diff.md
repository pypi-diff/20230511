# Comparing `tmp/webdrivertools-0.0.1.tar.gz` & `tmp/webdrivertools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdrivertools-0.0.1.tar", last modified: Thu May 11 01:57:35 2023, max compression
+gzip compressed data, was "webdrivertools-0.0.2.tar", last modified: Thu May 11 02:03:31 2023, max compression
```

## Comparing `webdrivertools-0.0.1.tar` & `webdrivertools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 01:57:35.789350 webdrivertools-0.0.1/
--rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 webdrivertools-0.0.1/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     3335 2023-05-11 01:57:35.789249 webdrivertools-0.0.1/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     2475 2023-05-11 01:56:46.000000 webdrivertools-0.0.1/README.md
--rw-r--r--   0 leandro    (501) staff       (20)     1012 2023-05-11 01:56:46.000000 webdrivertools-0.0.1/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-11 01:57:35.789380 webdrivertools-0.0.1/setup.cfg
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 01:57:35.788380 webdrivertools-0.0.1/webdrivertools/
--rw-r--r--   0 leandro    (501) staff       (20)      163 2023-05-11 01:56:46.000000 webdrivertools-0.0.1/webdrivertools/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4294 2023-05-11 01:42:53.000000 webdrivertools-0.0.1/webdrivertools/webdrivertools.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 01:57:35.789119 webdrivertools-0.0.1/webdrivertools.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     3335 2023-05-11 01:57:35.000000 webdrivertools-0.0.1/webdrivertools.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      281 2023-05-11 01:57:35.000000 webdrivertools-0.0.1/webdrivertools.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-11 01:57:35.000000 webdrivertools-0.0.1/webdrivertools.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       16 2023-05-11 01:57:35.000000 webdrivertools-0.0.1/webdrivertools.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)       15 2023-05-11 01:57:35.000000 webdrivertools-0.0.1/webdrivertools.egg-info/top_level.txt
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 02:03:31.945246 webdrivertools-0.0.2/
+-rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 webdrivertools-0.0.2/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-11 02:03:31.945132 webdrivertools-0.0.2/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     2480 2023-05-11 02:02:57.000000 webdrivertools-0.0.2/README.md
+-rw-r--r--   0 leandro    (501) staff       (20)     1012 2023-05-11 02:03:03.000000 webdrivertools-0.0.2/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-11 02:03:31.945277 webdrivertools-0.0.2/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 02:03:31.944234 webdrivertools-0.0.2/webdrivertools/
+-rw-r--r--   0 leandro    (501) staff       (20)      163 2023-05-11 01:56:46.000000 webdrivertools-0.0.2/webdrivertools/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4294 2023-05-11 01:42:53.000000 webdrivertools-0.0.2/webdrivertools/webdrivertools.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-11 02:03:31.944981 webdrivertools-0.0.2/webdrivertools.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     3340 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      281 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       16 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       15 2023-05-11 02:03:31.000000 webdrivertools-0.0.2/webdrivertools.egg-info/top_level.txt
```

### Comparing `webdrivertools-0.0.1/LICENSE` & `webdrivertools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webdrivertools-0.0.1/PKG-INFO` & `webdrivertools-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdrivertools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Functions to make life with Selenium easier.
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/webdrivertools
 Project-URL: Bug Tracker, https://github.com/leandropls/webdrivertools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -61,15 +61,15 @@
 
 ```python
 find_element(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
 ```
 
 Find a single HTML element within a webdriver page by attribute or criteria and optional inner text filtering, returning the matched WebElement.
 
-### 
+### click
 
 ```python
 click(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None, retries: int = 3, sleep_between_retries: float = 1) -> None
 ```
 
 Click on an element with an optional innerText filter. Number of retries and sleep between retries can be tweaked according to requirements.
```

### Comparing `webdrivertools-0.0.1/README.md` & `webdrivertools-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 ```python
 find_element(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
 ```
 
 Find a single HTML element within a webdriver page by attribute or criteria and optional inner text filtering, returning the matched WebElement.
 
-### 
+### click
 
 ```python
 click(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None, retries: int = 3, sleep_between_retries: float = 1) -> None
 ```
 
 Click on an element with an optional innerText filter. Number of retries and sleep between retries can be tweaked according to requirements.
```

### Comparing `webdrivertools-0.0.1/pyproject.toml` & `webdrivertools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webdrivertools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Leandro Pereira de Lima e Silva", email="leandro@lls-software.com" },
 ]
 description = "Functions to make life with Selenium easier."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `webdrivertools-0.0.1/webdrivertools/webdrivertools.py` & `webdrivertools-0.0.2/webdrivertools/webdrivertools.py`

 * *Files identical despite different names*

### Comparing `webdrivertools-0.0.1/webdrivertools.egg-info/PKG-INFO` & `webdrivertools-0.0.2/webdrivertools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdrivertools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Functions to make life with Selenium easier.
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/webdrivertools
 Project-URL: Bug Tracker, https://github.com/leandropls/webdrivertools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -61,15 +61,15 @@
 
 ```python
 find_element(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None) -> WebElement
 ```
 
 Find a single HTML element within a webdriver page by attribute or criteria and optional inner text filtering, returning the matched WebElement.
 
-### 
+### click
 
 ```python
 click(driver: WebDriver, value: str, by: str = By.CSS_SELECTOR, innerText: str | None = None, retries: int = 3, sleep_between_retries: float = 1) -> None
 ```
 
 Click on an element with an optional innerText filter. Number of retries and sleep between retries can be tweaked according to requirements.
```


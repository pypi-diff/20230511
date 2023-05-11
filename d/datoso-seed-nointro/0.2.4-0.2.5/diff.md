# Comparing `tmp/datoso_seed_nointro-0.2.4.tar.gz` & `tmp/datoso_seed_nointro-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_nointro-0.2.4.tar", last modified: Fri May  5 05:01:42 2023, max compression
+gzip compressed data, was "datoso_seed_nointro-0.2.5.tar", last modified: Thu May 11 18:49:04 2023, max compression
```

## Comparing `datoso_seed_nointro-0.2.4.tar` & `datoso_seed_nointro-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.598089 datoso_seed_nointro-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/top_level.txt
```

### Comparing `datoso_seed_nointro-0.2.4/LICENSE` & `datoso_seed_nointro-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.4/PKG-INFO` & `datoso_seed_nointro-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso_seed_nointro
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datoso_seed_nointro-0.2.4/README.md` & `datoso_seed_nointro-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.4/pyproject.toml` & `datoso_seed_nointro-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requires-python = ">=3.10"
 license     = {text = "MIT License"}
 authors     = [
     {name = 'Lacides Miranda', email = 'laromicas@hotmail.com'},
 ]
 keywords = ["emulators", "roms"]
 classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
```

### Comparing `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/dats.py` & `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/fetch.py` & `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return (len(firefox_temp_file) == 0) and \
        (len(chrome_temp_file) == 0) and \
        (len(downloaded_files) >= 1)
 
 
 def downloads_disabled(driver) -> bool:
     """Checks if the downloads in Datomatic are disabled."""
-    words = ['temporary suspended', 'temporary disabled']
+    words = ['temporary suspended', 'temporary disabled', 'services may be down']
     return any(word in driver.page_source for word in words)
 
 
 def download_daily(folder_helper):
     """Downloads the Datomatic Love Pack."""
     options = FirefoxOptions()
     # options.add_argument("--headless")
@@ -68,15 +68,15 @@
     sleep_time()
 
     try:
 
         if downloads_disabled(driver):
             print("Downloads suspended")
             driver.close()
-            sys.exit(1)
+            return
 
         print("Getting to file download page")
 
         # driver.manage().timeouts().implicitlyWait(5, TimeUnit.SECONDS)
         download_button = driver.find_element(By.XPATH, "//a[contains(text(), 'Download')]")
         download_button.click()
```

### Comparing `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/rules.py` & `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/PKG-INFO` & `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso-seed-nointro
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```


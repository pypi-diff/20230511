# Comparing `tmp/tor_downloader-1.0.0.tar.gz` & `tmp/tor_downloader-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tor_downloader-1.0.0.tar", last modified: Wed Aug  3 17:59:02 2022, max compression
+gzip compressed data, was "tor_downloader-1.0.3.tar", last modified: Thu May 11 15:23:24 2023, max compression
```

## Comparing `tor_downloader-1.0.0.tar` & `tor_downloader-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-08-03 17:59:02.364421 tor_downloader-1.0.0/
--rw-rw-rw-   0        0        0     1087 2022-08-03 17:03:01.000000 tor_downloader-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4213 2022-08-03 17:59:02.361537 tor_downloader-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2331 2022-08-03 17:57:08.000000 tor_downloader-1.0.0/README.md
--rw-rw-rw-   0        0        0      975 2022-08-03 17:42:30.000000 tor_downloader-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-03 17:59:02.365623 tor_downloader-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      138 2022-08-03 17:40:41.000000 tor_downloader-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-03 17:59:02.252559 tor_downloader-1.0.0/tor_downloader/
--rw-rw-rw-   0        0        0      458 2022-08-03 17:15:09.000000 tor_downloader-1.0.0/tor_downloader/__init__.py
--rw-rw-rw-   0        0        0     8358 2022-08-03 17:39:37.000000 tor_downloader-1.0.0/tor_downloader/__main__.py
--rw-rw-rw-   0        0        0    12843 2022-08-03 16:56:58.000000 tor_downloader-1.0.0/tor_downloader/file_downloader.py
-drwxrwxrwx   0        0        0        0 2022-08-03 17:59:02.351933 tor_downloader-1.0.0/tor_downloader/utils/
--rw-rw-rw-   0        0        0       90 2022-08-03 14:01:40.000000 tor_downloader-1.0.0/tor_downloader/utils/__init__.py
--rw-rw-rw-   0        0        0      481 2022-08-03 14:01:40.000000 tor_downloader-1.0.0/tor_downloader/utils/check_tor.py
--rw-rw-rw-   0        0        0     1393 2022-08-03 17:39:21.000000 tor_downloader-1.0.0/tor_downloader/utils/download_links.py
--rw-rw-rw-   0        0        0     3510 2022-08-03 17:39:27.000000 tor_downloader-1.0.0/tor_downloader/utils/logging_handlers.py
-drwxrwxrwx   0        0        0        0 2022-08-03 17:59:02.302894 tor_downloader-1.0.0/tor_downloader.egg-info/
--rw-rw-rw-   0        0        0     4213 2022-08-03 17:59:02.000000 tor_downloader-1.0.0/tor_downloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2022-08-03 17:59:02.000000 tor_downloader-1.0.0/tor_downloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-03 17:59:02.000000 tor_downloader-1.0.0/tor_downloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2022-08-03 17:59:02.000000 tor_downloader-1.0.0/tor_downloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-08-03 17:59:02.000000 tor_downloader-1.0.0/tor_downloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:24.200353 tor_downloader-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4481 2023-05-11 15:23:24.199353 tor_downloader-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2599 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/README.md
+-rw-rw-rw-   0        0        0      975 2023-05-11 15:20:19.000000 tor_downloader-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:23:24.200353 tor_downloader-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      138 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:24.192351 tor_downloader-1.0.3/tor_downloader/
+-rw-rw-rw-   0        0        0      458 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/tor_downloader/__init__.py
+-rw-rw-rw-   0        0        0     9265 2023-05-11 15:10:12.000000 tor_downloader-1.0.3/tor_downloader/__main__.py
+-rw-rw-rw-   0        0        0    12901 2023-05-11 14:53:04.000000 tor_downloader-1.0.3/tor_downloader/file_downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:24.199353 tor_downloader-1.0.3/tor_downloader/utils/
+-rw-rw-rw-   0        0        0       90 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/tor_downloader/utils/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/tor_downloader/utils/check_tor.py
+-rw-rw-rw-   0        0        0     1393 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/tor_downloader/utils/download_links.py
+-rw-rw-rw-   0        0        0     3510 2023-05-11 14:27:03.000000 tor_downloader-1.0.3/tor_downloader/utils/logging_handlers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:24.196353 tor_downloader-1.0.3/tor_downloader.egg-info/
+-rw-rw-rw-   0        0        0     4481 2023-05-11 15:23:24.000000 tor_downloader-1.0.3/tor_downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-05-11 15:23:24.000000 tor_downloader-1.0.3/tor_downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:23:24.000000 tor_downloader-1.0.3/tor_downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-05-11 15:23:24.000000 tor_downloader-1.0.3/tor_downloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 15:23:24.000000 tor_downloader-1.0.3/tor_downloader.egg-info/top_level.txt
```

### Comparing `tor_downloader-1.0.0/LICENSE` & `tor_downloader-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tor_downloader-1.0.0/PKG-INFO` & `tor_downloader-1.0.3/tor_downloader.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tor_downloader
-Version: 1.0.0
+Name: tor-downloader
+Version: 1.0.3
 Summary: Download dark web files using Tor.
 Author-email: Ian Costa <costa.ian18@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Ian Costa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,15 @@
 ## Installing TorDownloader
 
 ### Using Pip
 
 TorDownloader can be easily installed through pip:
 - First, create a virtual environment: `python -m venv .venv`
 - Then activate it: `.venv\Scripts\activate` on Windows or `.venv/activate` on Linux
-- Finally install the tor_downloader package: `python -m pip install tor_downloader`
+- Finally install the tor_downloader package: `python -m pip install tor-downloader`
 
 If installing TorDownloader through pip, it will be installed in your Python path. This is important as the path is used for default options such as the output directory, input directory, and log directory.
 Because of this, you can give TorDownloader the argument `path` to find the folder TorDownloader was installed into.
 Example of this command:
 ```python -m tor_downloader path```
 
 ## Running TorDownloader
@@ -65,19 +65,20 @@
 The config file must be a JSON file with a single dictionary.
 The command line arguments must be formatted like so:
     ```CONFIG=SETTING```
 
 Configuration options:
     socks_port: Port of Tor Socks5 proxy.
     max_downloads: Maximum number of downloads to run at once.
+    max_tor_checks: Number of times the Tor proxy will be checked to ensure Tor is working before crashing. Default is 5.
     tor_path: Path to the Tor executable (tor.exe). Often found in Tor Browser if installed (Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe).
     links_file: Path to the file containing the list of URLs to download. Must be a .json file with a single list of URLs.
     log_file: Path to the log file. Log file will be created if it does not exist.
-    output_directory: Path to the directory to download the files to.
-    config_file: Path to the configuration file. Only usable through the command line arguments.
+    output_dir: Path to the directory to download the files to.
+    config: Path to the configuration file. Only usable through the command line arguments.
 
 Example command:
     ```python -m tor_downloader max_downloads=7 tor_path="Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe" links_file=links.json output_directory=output```
 
 ## Getting Results
 
-All files will be
+All files will be installed into the output directory specified in the config file or command line argument. By default, the output directory is `tor_downloader/data/input`.
```

### Comparing `tor_downloader-1.0.0/README.md` & `tor_downloader-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## Installing TorDownloader
 
 ### Using Pip
 
 TorDownloader can be easily installed through pip:
 - First, create a virtual environment: `python -m venv .venv`
 - Then activate it: `.venv\Scripts\activate` on Windows or `.venv/activate` on Linux
-- Finally install the tor_downloader package: `python -m pip install tor_downloader`
+- Finally install the tor_downloader package: `python -m pip install tor-downloader`
 
 If installing TorDownloader through pip, it will be installed in your Python path. This is important as the path is used for default options such as the output directory, input directory, and log directory.
 Because of this, you can give TorDownloader the argument `path` to find the folder TorDownloader was installed into.
 Example of this command:
 ```python -m tor_downloader path```
 
 ## Running TorDownloader
@@ -27,19 +27,20 @@
 The config file must be a JSON file with a single dictionary.
 The command line arguments must be formatted like so:
     ```CONFIG=SETTING```
 
 Configuration options:
     socks_port: Port of Tor Socks5 proxy.
     max_downloads: Maximum number of downloads to run at once.
+    max_tor_checks: Number of times the Tor proxy will be checked to ensure Tor is working before crashing. Default is 5.
     tor_path: Path to the Tor executable (tor.exe). Often found in Tor Browser if installed (Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe).
     links_file: Path to the file containing the list of URLs to download. Must be a .json file with a single list of URLs.
     log_file: Path to the log file. Log file will be created if it does not exist.
-    output_directory: Path to the directory to download the files to.
-    config_file: Path to the configuration file. Only usable through the command line arguments.
+    output_dir: Path to the directory to download the files to.
+    config: Path to the configuration file. Only usable through the command line arguments.
 
 Example command:
     ```python -m tor_downloader max_downloads=7 tor_path="Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe" links_file=links.json output_directory=output```
 
 ## Getting Results
 
-All files will be
+All files will be installed into the output directory specified in the config file or command line argument. By default, the output directory is `tor_downloader/data/input`.
```

### Comparing `tor_downloader-1.0.0/pyproject.toml` & `tor_downloader-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tor_downloader"
-version = "1.0.0"
+version = "1.0.3"
 description = "Download dark web files using Tor."
 readme = "README.md"
 authors = [{ name = "Ian Costa", email = "costa.ian18@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `tor_downloader-1.0.0/tor_downloader/__main__.py` & `tor_downloader-1.0.3/tor_downloader/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 The config file must be a JSON file with a single dictionary.
 The command line arguments must be formatted like so:
     ```CONFIG=SETTING```
 
 Configuration options:
     socks_port: Port of Tor Socks5 proxy.
     max_downloads: Maximum number of downloads to run at once.
+    max_tor_checks: Number of times the Tor proxy will be checked to ensure Tor is working before crashing. Default is 5.
     tor_path: Path to the Tor executable (tor.exe). Often found in Tor Browser if installed (Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe).
     links_file: Path to the file containing the list of URLs to download. Must be a .json file with a single list of URLs.
     log_file: Path to the log file. Log file will be created if it does not exist.
     output_dir: Path to the directory to download the files to.
-    config_file: Path to the configuration file. Only usable through the command line arguments.
+    config: Path to the configuration file. Only usable through the command line arguments.
 
 Example command:
     ```python main.py max_downloads=7 tor_path=Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe links_file=links.json output_directory=output```
 """
 
 # sourcery skip: assign-if-exp
 import json
@@ -29,17 +30,16 @@
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from typing import Dict
 
 from stemquests import TorConnectionError, TorInstance
 
-from tor_downloader.file_downloader import FileDownloader
-from tor_downloader.utils import (TDFormatter, TqdmLoggingHandler,
-                                  get_download_links_json)
+from .file_downloader import FileDownloader
+from .utils import TDFormatter, TqdmLoggingHandler, get_download_links_json
 
 CURRENT_PATH = Path(__file__).parent
 DEFAULT_CONFIG = {
     "socks_port": 9051,
     "max_downloads": 7,
     "links_file": CURRENT_PATH / "data\\input\\links.json",
     "log_file": CURRENT_PATH / "log\\TorDownloader.log",
@@ -67,18 +67,18 @@
     with open(config_file, "r", encoding="utf-8") as file:
         for key, value in json.load(file).items():
             # Do not load empty strings or None values into the config
             if value == "" or value is None:
                 continue
             # Convert the value to the correct type
             match key:
-                case "socks_port" | "max_downloads":
+                case "socks_port" | "max_downloads" | "max_tor_checks":
                     clean_config[key] = int(value)
                 case _:
-                    clean_config[key] = value
+                    clean_config[key] = value.lower()
     return clean_config
 
 def get_config_args() -> Dict:
     """Get configurations from command line arguments.
 
     Returns:
         Dict: Dictionary of configuration options.
@@ -91,37 +91,41 @@
     for arg in sys.argv[1:]:
         arg_split = arg.split("=")
         if len(arg_split) != 2:
             raise ValueError(f"Invalid command line argument: '{arg}'. Arguments must be formatted like so: 'CONFIG=SETTING'.")
         arg_key, arg_val = arg_split
         if arg_val.isnumeric():
             arg_val = int(arg_val)
-        if arg_val.lower() == "true":
+        elif arg_val.lower() == "true":
             arg_val = True
-        if arg_val.lower() == "false":
+        elif arg_val.lower() == "false":
             arg_val = False
         arg_dict[arg_key] = arg_val
 
     return arg_dict
 
 def main():
     """Main function for TorDownloader. Runs the program using system arguments or a config file."""
     # Check if user passed the "path" argument
     if len(sys.argv) >= 2:
         if sys.argv[1] == "path":
             print(CURRENT_PATH)
             sys.exit(0)
     # Get the configuration options from the arguments and config file
     arg_config = get_config_args()
-    file_config = get_config_file(arg_config["config_file"]) if arg_config.get("config_file") is not None else DEFAULT_CONFIG
+    # Overwrite the default config with the config options from the file
+    file_config = {**DEFAULT_CONFIG, **get_config_file(arg_config["config"])} \
+                  if arg_config.get("config") is not None \
+                  else DEFAULT_CONFIG
 
     # Merge the config dictionaries, with the cmd arguments taking precedence
     CONFIG = {**file_config, **arg_config}
 
     # Add a new line to the end of the log file before starting
+    Path(CONFIG["log_file"]).parents[0].mkdir(parents=True, exist_ok=True) # Make the parent directories first
     with open(CONFIG["log_file"], "a", encoding="utf-8") as log_file:
         log_file.write("\n")
     # Setup logging
     logger = logging.getLogger()
     logger.setLevel(logging.DEBUG)
     for handler in logging.root.handlers[:]:
         logging.root.removeHandler(handler)
@@ -131,62 +135,70 @@
     logger.addHandler(handler)
 
     # Set up Tor Downloader logger
     td_logger = logging.getLogger("tor_downloader")
     tqdm_handler = TqdmLoggingHandler(logging.INFO)
     tqdm_handler.setFormatter(TDFormatter())
     td_logger.addHandler(tqdm_handler)
+    logger.addHandler(tqdm_handler)
 
     logger.info("Starting TorDownloader on %s", datetime.now().isoformat())
+    logger.debug("Using config options: %s", str(CONFIG))
 
     download_links = get_download_links_json(CONFIG.get("links_file"))
     if download_links is None:
         logger.error("Links file is empty.")
         return
 
     # Create a Tor instance for the downloader
     tor_instance = TorInstance(CONFIG["socks_port"], CONFIG.get("tor_path"))
     files = {}
     with ThreadPoolExecutor(max_workers=CONFIG["max_downloads"]) as executor:
         try: # Catch keyboard interrupts and other exceptions
             # Submit the jobs to the executor.
+            logger.info("Submitting %d jobs to the executor.", len(download_links))
             futures = {}
             for download_link in download_links:
                 downloader = FileDownloader(tor_instance=tor_instance, tor_port=CONFIG["socks_port"])
                 future = executor.submit(downloader.download_file, download_link, target_dir=CONFIG["output_dir"])
                 futures[future] = download_link
+                logger.info("Submitted job for URL '%s' using session #%d.", download_link, downloader.session_num) # TODO: Session number needs to be 1 less
+            logger.info("Submitted %d jobs to the executor.", len(futures))
             # Get the results for the downloads
             for future in as_completed(futures):
                 url = futures[future]
                 # TODO: Handle more exceptions by restarting the download
                 future_exception = future.exception()
                 if isinstance(future_exception, TorConnectionError):
                     logger.error("Could not connect to Tor for URL '%s', readding the URL to the queue.", url)
                     downloader = FileDownloader(tor_instance=tor_instance, tor_port=CONFIG["socks_port"])
                     retry_url_future = executor.submit(downloader.download_file, url, target_dir=CONFIG["output_dir"])
                     futures[retry_url_future] = url
                     continue
                 if future_exception is not None:
                     files[url] = future.exception()
-                    td_logger.error("Error downloading %s: %s", url, future.exception())
+                    logger.error("Error downloading %s: %s", url, future.exception())
                     continue
-                if CONFIG["output_dir"] in (result := future.result()):
-                    td_logger.info("Download finished! Filepath: %s | URL: %s", result, url)
+                if str(CONFIG["output_dir"]) in (result := future.result()):
+                    logger.info("Download finished! Filepath: %s | URL: %s", result, url)
                 else:
-                    td_logger.error("Download failed! Reason: %s | URL: %s", result, url)
+                    logger.error("Download failed! Reason: %s | URL: %s", result, url)
                 files[url] = result
+                logger.info("%d files finished so far.", len(files))
+        except ConnectionError:
+            logger.error("Connection error, restarting script...")
+            return main()
         except KeyboardInterrupt:
             # TODO: Fix this, it doesn't work. For now manually kill the program.
-            print('Keyboard Interrupt')
             logger.info("Keyboard Interrupt, stopping program...")
             sys.exit(1)
         except Exception as err:
-            logger.error("Fatal Error (time = %s): %s", datetime.now().isoformat(), err)
-            raise err
+            logger.error("Fatal Error, restarting script... Error: %s", err)
+            return main()
 
-    print("-"*25)
-    print("All Downloads Finished:")
+    logger.info("-"*25)
+    logger.info("All Downloads Finished:")
     for url, result in files.items():
-        print(f"\t- {url}: {result}")
+        logger.info("\t- %s: %s", url, result)
 
 if __name__ == '__main__':
     main()
```

### Comparing `tor_downloader-1.0.0/tor_downloader/file_downloader.py` & `tor_downloader-1.0.3/tor_downloader/file_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                  use_tor: bool=True, requests_session: requests.Session=None, max_retries: int=5) -> None:
         if not use_tor and tor_instance is not None:
             raise ValueError("use_tor cannot be false if tor_instance is provided.")
 
         if use_tor:
             self.tor_instance = tor_instance or TorInstance(socks_port=tor_port)
             if requests_session is None:
-                self.requests_session, self.session_num = self.tor_instance.get_requests_session()
+                self.requests_session, self.session_num = self.tor_instance.get_session_with_number()
             else:
                 self.requests_session = requests_session
                 self.session_num = -1
         else:
             self.tor_instance = None
             self.requests_session = requests_session or requests.Session()
 
@@ -149,21 +149,22 @@
             logger.error("Max retries (#%d) exceeded for URL: %s", self.num_retries, url)
             return None
         self.num_retries += 1
 
         logger.debug("Starting download from URL: %s", url)
 
         # Check if the target_dir is a valid directory
-        if target_dir and not os.path.isdir(target_dir):
-            if os.path.isfile(target_dir):
+        target_path = Path(target_dir)
+        if target_dir and not target_path.is_dir():
+            if target_path.is_file():
                 raise ValueError(f'Invalid target_dir={target_dir} specified, target_dir is a file.')
             try:
                 # Create the target_dir if it doesn't exist
                 logger.warning("Directory '%s' does not exist, attempting to create it.", target_dir)
-                os.mkdirs(target_dir)
+                target_path.mkdir(parents=True, exist_ok=True)
                 logger.info("Directory '%s' successfully created.", target_dir)
             except OSError as err:
                 logger.error("Error creating target_dir: %s", err)
                 raise ValueError(f'Invalid target_dir={target_dir} specified') from err
 
         # Get filename from URL if not given
         filename = self._get_url_filename(url, self.requests_session) if filename is None else filename
```

### Comparing `tor_downloader-1.0.0/tor_downloader/utils/download_links.py` & `tor_downloader-1.0.3/tor_downloader/utils/download_links.py`

 * *Files identical despite different names*

### Comparing `tor_downloader-1.0.0/tor_downloader/utils/logging_handlers.py` & `tor_downloader-1.0.3/tor_downloader/utils/logging_handlers.py`

 * *Files identical despite different names*

### Comparing `tor_downloader-1.0.0/tor_downloader.egg-info/PKG-INFO` & `tor_downloader-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tor-downloader
-Version: 1.0.0
+Name: tor_downloader
+Version: 1.0.3
 Summary: Download dark web files using Tor.
 Author-email: Ian Costa <costa.ian18@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Ian Costa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,15 @@
 ## Installing TorDownloader
 
 ### Using Pip
 
 TorDownloader can be easily installed through pip:
 - First, create a virtual environment: `python -m venv .venv`
 - Then activate it: `.venv\Scripts\activate` on Windows or `.venv/activate` on Linux
-- Finally install the tor_downloader package: `python -m pip install tor_downloader`
+- Finally install the tor_downloader package: `python -m pip install tor-downloader`
 
 If installing TorDownloader through pip, it will be installed in your Python path. This is important as the path is used for default options such as the output directory, input directory, and log directory.
 Because of this, you can give TorDownloader the argument `path` to find the folder TorDownloader was installed into.
 Example of this command:
 ```python -m tor_downloader path```
 
 ## Running TorDownloader
@@ -65,19 +65,20 @@
 The config file must be a JSON file with a single dictionary.
 The command line arguments must be formatted like so:
     ```CONFIG=SETTING```
 
 Configuration options:
     socks_port: Port of Tor Socks5 proxy.
     max_downloads: Maximum number of downloads to run at once.
+    max_tor_checks: Number of times the Tor proxy will be checked to ensure Tor is working before crashing. Default is 5.
     tor_path: Path to the Tor executable (tor.exe). Often found in Tor Browser if installed (Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe).
     links_file: Path to the file containing the list of URLs to download. Must be a .json file with a single list of URLs.
     log_file: Path to the log file. Log file will be created if it does not exist.
-    output_directory: Path to the directory to download the files to.
-    config_file: Path to the configuration file. Only usable through the command line arguments.
+    output_dir: Path to the directory to download the files to.
+    config: Path to the configuration file. Only usable through the command line arguments.
 
 Example command:
     ```python -m tor_downloader max_downloads=7 tor_path="Tor Browser\\Browser\\TorBrowser\\Tor\\tor.exe" links_file=links.json output_directory=output```
 
 ## Getting Results
 
-All files will be
+All files will be installed into the output directory specified in the config file or command line argument. By default, the output directory is `tor_downloader/data/input`.
```


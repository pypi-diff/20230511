# Comparing `tmp/pytest_qaseio-1.0.1.tar.gz` & `tmp/pytest_qaseio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_qaseio-1.0.1.tar", max compression
+gzip compressed data, was "pytest_qaseio-1.1.0.tar", max compression
```

## Comparing `pytest_qaseio-1.0.1.tar` & `pytest_qaseio-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-1.0.1/LICENSE
--rw-r--r--   0        0        0     5444 2023-04-07 04:31:19.166683 pytest_qaseio-1.0.1/README.md
--rw-r--r--   0        0        0     2818 2023-05-02 03:08:38.235157 pytest_qaseio-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-1.0.1/pytest_qaseio/__init__.py
--rw-r--r--   0        0        0     2387 2023-04-05 13:30:53.380549 pytest_qaseio-1.0.1/pytest_qaseio/api_client.py
--rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-1.0.1/pytest_qaseio/constants.py
--rw-r--r--   0        0        0     8055 2023-04-06 07:51:22.681371 pytest_qaseio-1.0.1/pytest_qaseio/converter.py
--rw-r--r--   0        0        0     3140 2023-04-06 08:04:30.704357 pytest_qaseio-1.0.1/pytest_qaseio/debug_info.py
--rw-r--r--   0        0        0      295 2023-04-05 14:41:26.341327 pytest_qaseio-1.0.1/pytest_qaseio/hooks.py
--rw-r--r--   0        0        0     8448 2023-04-07 06:26:41.054493 pytest_qaseio-1.0.1/pytest_qaseio/plugin.py
--rw-r--r--   0        0        0     1419 2023-04-05 14:02:37.660306 pytest_qaseio-1.0.1/pytest_qaseio/plugin_exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-1.0.1/pytest_qaseio/py.typed
--rw-r--r--   0        0        0     1156 2023-04-05 13:30:57.987221 pytest_qaseio-1.0.1/pytest_qaseio/storage.py
--rw-r--r--   0        0        0     6602 1970-01-01 00:00:00.000000 pytest_qaseio-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5785 2023-05-11 09:07:18.681663 pytest_qaseio-1.1.0/README.md
+-rw-r--r--   0        0        0     2818 2023-05-11 09:07:29.704666 pytest_qaseio-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-1.1.0/pytest_qaseio/__init__.py
+-rw-r--r--   0        0        0     2387 2023-04-05 13:30:53.380549 pytest_qaseio-1.1.0/pytest_qaseio/api_client.py
+-rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-1.1.0/pytest_qaseio/constants.py
+-rw-r--r--   0        0        0     8055 2023-04-06 07:51:22.681371 pytest_qaseio-1.1.0/pytest_qaseio/converter.py
+-rw-r--r--   0        0        0     3140 2023-04-06 08:04:30.704357 pytest_qaseio-1.1.0/pytest_qaseio/debug_info.py
+-rw-r--r--   0        0        0      295 2023-04-05 14:41:26.341327 pytest_qaseio-1.1.0/pytest_qaseio/hooks.py
+-rw-r--r--   0        0        0     8868 2023-05-11 09:07:18.683103 pytest_qaseio-1.1.0/pytest_qaseio/plugin.py
+-rw-r--r--   0        0        0     1419 2023-04-05 14:02:37.660306 pytest_qaseio-1.1.0/pytest_qaseio/plugin_exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-1.1.0/pytest_qaseio/py.typed
+-rw-r--r--   0        0        0     1156 2023-04-05 13:30:57.987221 pytest_qaseio-1.1.0/pytest_qaseio/storage.py
+-rw-r--r--   0        0        0     6943 1970-01-01 00:00:00.000000 pytest_qaseio-1.1.0/PKG-INFO
```

### Comparing `pytest_qaseio-1.0.1/LICENSE` & `pytest_qaseio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.1/README.md` & `pytest_qaseio-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,24 @@
 import pytest
 
 @pytest.mark.qase("https://app.qase.io/case/DEMO-1")
 def test_demo():
     """Check qaseio plugin works as expected."""
 ```
 
-Then run your tests with flag `--qase-enabled`:
+Since this package is mostly used for selenium tests, you need to provide a
+value for `--webdriver` flag. If you set `--webdriver=remote` and want to specify
+name of remote browser (not just Remote), use `--remote-browser`
+flag or set capabilities via `variables`. This will be used in test run name and
+in attachments path.
+
+To enable plugin use flag `--qase-enabled`.
 
 ```bash
-pytest tests/ --qase-enabled
+pytest tests/ --qase-enabled --webdriver=chrome
 ```
 
 ## Work with Selenium
 
 This plugin expects to be used with selenium and provides additional debug
 info from browser. To make it possible, prepare fixture that provides webdriver
 and use the following snippet to set `_webdriver` attribute for each test:
```

### Comparing `pytest_qaseio-1.0.1/pyproject.toml` & `pytest_qaseio-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pytest-qaseio"
 description = "Pytest plugin for Qase.io integration"
-version = "1.0.1"
+version = "1.1.0"
 license = "MIT"
 
 authors = [
   "Saritasa <pypi@saritasa.com>",
 ]
 
 readme = "README.md"
```

### Comparing `pytest_qaseio-1.0.1/pytest_qaseio/api_client.py` & `pytest_qaseio-1.1.0/pytest_qaseio/api_client.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.1/pytest_qaseio/converter.py` & `pytest_qaseio-1.1.0/pytest_qaseio/converter.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.1/pytest_qaseio/debug_info.py` & `pytest_qaseio-1.1.0/pytest_qaseio/debug_info.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.1/pytest_qaseio/plugin.py` & `pytest_qaseio-1.1.0/pytest_qaseio/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,28 @@
         "qase": storage.QaseFileStorage(
             qase_token=os.environ["QASE_TOKEN"],
             qase_project_code=os.environ["QASE_PROJECT_CODE"],
         ),
     }
 
 
+def _get_browser_name(config: pytest.Config, default: str = "remote"):
+    """Try to get browser name from options and variables.
+
+    Since `pytest-selenium` uses `pytest-variables` and recommends to put
+    capabilities there we try to get `browserName` from `config._variables`.
+
+    """
+    browser_name = getattr(config, "_variables", {}).get("capabilities", {}).get(
+        "browserName",
+        None,
+    )
+    return browser_name or config.getoption("--remote-browser", default=default)
+
+
 @pytest.hookimpl(trylast=True)
 def pytest_configure(config: pytest.Config):
     """Configure pytest-qaseio plugin.
 
     Add `qase` marker for pytest.
     If qase enabled, register qase plugin.
     Get file storage for qase plugin.
@@ -76,18 +90,15 @@
         "qase(test_case_url): Mark test for qase",
     )
     qase_enabled = config.getoption("--qase-enabled")
     if not qase_enabled:
         return
     browser = config.getoption("--webdriver")
     if browser == "remote":
-        browser = config._variables.get(  # type: ignore
-            "capabilities",
-            {},
-        ).get("browserName", "chrome")
+        browser = _get_browser_name(config, default=browser)
 
     config.pluginmanager.register(
         plugin=QasePlugin(
             browser=browser,
             file_storage=_get_file_storage(config),
         ),
         name="qase_plugin",
```

### Comparing `pytest_qaseio-1.0.1/pytest_qaseio/plugin_exceptions.py` & `pytest_qaseio-1.1.0/pytest_qaseio/plugin_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.1/pytest_qaseio/storage.py` & `pytest_qaseio-1.1.0/pytest_qaseio/storage.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.0.1/PKG-INFO` & `pytest_qaseio-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-qaseio
-Version: 1.0.1
+Version: 1.1.0
 Summary: Pytest plugin for Qase.io integration
 Home-page: https://pypi.org/project/pytest-qaseio/
 License: MIT
 Keywords: pytest,qase,qaseio,selenium,autotests
 Author: Saritasa
 Author-email: pypi@saritasa.com
 Requires-Python: >=3.10,<4.0
@@ -79,18 +79,24 @@
 import pytest
 
 @pytest.mark.qase("https://app.qase.io/case/DEMO-1")
 def test_demo():
     """Check qaseio plugin works as expected."""
 ```
 
-Then run your tests with flag `--qase-enabled`:
+Since this package is mostly used for selenium tests, you need to provide a
+value for `--webdriver` flag. If you set `--webdriver=remote` and want to specify
+name of remote browser (not just Remote), use `--remote-browser`
+flag or set capabilities via `variables`. This will be used in test run name and
+in attachments path.
+
+To enable plugin use flag `--qase-enabled`.
 
 ```bash
-pytest tests/ --qase-enabled
+pytest tests/ --qase-enabled --webdriver=chrome
 ```
 
 ## Work with Selenium
 
 This plugin expects to be used with selenium and provides additional debug
 info from browser. To make it possible, prepare fixture that provides webdriver
 and use the following snippet to set `_webdriver` attribute for each test:
```


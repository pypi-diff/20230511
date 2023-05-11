# Comparing `tmp/platformdirs-3.5.0.tar.gz` & `tmp/platformdirs-3.5.1.tar.gz`

## Comparing `platformdirs-3.5.0.tar` & `platformdirs-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    18902 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/version.py
--rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/conftest.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_android.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_api.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_main.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.0/LICENSE
--rw-r--r--   0        0        0     7403 2020-02-02 00:00:00.000000 platformdirs-3.5.0/README.rst
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 platformdirs-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 platformdirs-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tox.ini
+-rw-r--r--   0        0        0    18902 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/android.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/version.py
+-rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 platformdirs-3.5.1/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_android.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_api.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_main.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 platformdirs-3.5.1/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.1/LICENSE
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 platformdirs-3.5.1/README.rst
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 platformdirs-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 platformdirs-3.5.1/PKG-INFO
```

### Comparing `platformdirs-3.5.0/src/platformdirs/__init__.py` & `platformdirs-3.5.1/src/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/src/platformdirs/__main__.py` & `platformdirs-3.5.1/src/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/src/platformdirs/android.py` & `platformdirs-3.5.1/src/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/src/platformdirs/api.py` & `platformdirs-3.5.1/src/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/src/platformdirs/macos.py` & `platformdirs-3.5.1/src/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/src/platformdirs/unix.py` & `platformdirs-3.5.1/src/platformdirs/unix.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import os
 import sys
 from configparser import ConfigParser
 from pathlib import Path
 
 from .api import PlatformDirsABC
 
-if sys.platform.startswith("linux"):  # pragma: no branch # no op check, only to please the type checker
-    from os import getuid
-else:
+if sys.platform == "win32":
 
     def getuid() -> int:
-        raise RuntimeError("should only be used on Linux")
+        raise RuntimeError("should only be used on Unix")
+
+else:
+    from os import getuid
 
 
 class Unix(PlatformDirsABC):
     """
     On Unix/Linux, we follow the
     `XDG Basedir Spec <https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html>`_. The spec allows
     overriding directories with environment variables. The examples show are the default values, alongside the name of
```

### Comparing `platformdirs-3.5.0/src/platformdirs/windows.py` & `platformdirs-3.5.1/src/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/tests/conftest.py` & `platformdirs-3.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/tests/test_android.py` & `platformdirs-3.5.1/tests/test_android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/tests/test_api.py` & `platformdirs-3.5.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/tests/test_comp_with_appdirs.py` & `platformdirs-3.5.1/tests/test_comp_with_appdirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 
     if sys.platform == "darwin":
         msg = {  # pragma: no cover
             "user_log_dir": "without appname produces NoneType error",
         }
         if func in msg:  # pragma: no cover
             pytest.skip(f"`appdirs.{func}` {msg[func]} on macOS")  # pragma: no cover
-    if sys.platform == "linux":
+    elif sys.platform != "win32":
         msg = {  # pragma: no cover
             "user_log_dir": "Uses XDG_STATE_DIR instead of appdirs.user_data_dir per the XDG spec",
         }
         if func in msg:  # pragma: no cover
-            pytest.skip(f"`appdirs.{func}` {msg[func]} on Linux")  # pragma: no cover
+            pytest.skip(f"`appdirs.{func}` {msg[func]} on Unix")  # pragma: no cover
 
     new = getattr(platformdirs, func)(*params)
     old = getattr(appdirs, func)(*params)
 
     assert new == old.rstrip("/")
```

### Comparing `platformdirs-3.5.0/tests/test_macos.py` & `platformdirs-3.5.1/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/tests/test_unix.py` & `platformdirs-3.5.1/tests/test_unix.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import typing
 from pathlib import Path
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from pytest_mock import MockerFixture
 
+from platformdirs import unix
 from platformdirs.unix import Unix
 
 
 @pytest.mark.parametrize("prop", ["user_documents_dir", "user_pictures_dir", "user_videos_dir", "user_music_dir"])
 def test_user_media_dir(mocker: MockerFixture, prop: str) -> None:
     example_path = "/home/example/ExampleMediaFolder"
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
@@ -124,26 +125,24 @@
         return
 
     monkeypatch.setenv(xdg_variable.name, "/tmp/custom-dir")
     result = getattr(dirs_instance, func)
     assert result == "/tmp/custom-dir"
 
 
-def test_platform_non_linux(monkeypatch: MonkeyPatch) -> None:
-    from platformdirs import unix
-
+def test_platform_on_win32(monkeypatch: MonkeyPatch, mocker: MockerFixture) -> None:
+    monkeypatch.delenv("XDG_RUNTIME_DIR", raising=False)
+    mocker.patch("sys.platform", "win32")
+    prev_unix = unix
+    importlib.reload(unix)
     try:
-        with monkeypatch.context() as context:
-            context.setattr(sys, "platform", "magic")
-            monkeypatch.delenv("XDG_RUNTIME_DIR", raising=False)
-            importlib.reload(unix)
-        with pytest.raises(RuntimeError, match="should only be used on Linux"):
+        with pytest.raises(RuntimeError, match="should only be used on Unix"):
             unix.Unix().user_runtime_dir
     finally:
-        importlib.reload(unix)
+        sys.modules["platformdirs.unix"] = prev_unix
 
 
 def test_ensure_exists_creates_folder(mocker: MockerFixture, tmp_path: Path) -> None:
     mocker.patch.dict(os.environ, {"XDG_DATA_HOME": str(tmp_path)})
     data_path = Unix(appname="acme", ensure_exists=True).user_data_path
     assert data_path.exists()
```

### Comparing `platformdirs-3.5.0/LICENSE` & `platformdirs-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.0/README.rst` & `platformdirs-3.5.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 and configuration varies per platform. Even for single-platform apps, there
 may by plenty of nuances in figuring out the right location.
 
 For example, if running on macOS, you should use::
 
     ~/Library/Application Support/<AppName>
 
-If on Windows (at least English Win XP) that should be::
+If on Windows (at least English Win) that should be::
 
     C:\Documents and Settings\<User>\Application Data\Local Settings\<AppAuthor>\<AppName>
 
 or possibly::
 
     C:\Documents and Settings\<User>\Application Data\<AppAuthor>\<AppName>
 
@@ -67,15 +67,15 @@
     >>> user_log_dir(appname, appauthor)
     '/Users/trentm/Library/Logs/SuperApp'
     >>> user_documents_dir()
     '/Users/trentm/Documents'
     >>> user_runtime_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
-On Windows 7:
+On Windows:
 
 .. code-block:: pycon
 
     >>> from platformdirs import *
     >>> appname = "SuperApp"
     >>> appauthor = "Acme"
     >>> user_data_dir(appname, appauthor)
```

### Comparing `platformdirs-3.5.0/pyproject.toml` & `platformdirs-3.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.14",
+  "hatchling>=1.14.1",
 ]
 
 [project]
 name = "platformdirs"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 readme = "README.rst"
 keywords = [
@@ -27,35 +27,35 @@
 requires-python = ">=3.7"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   'typing-extensions>=4.5; python_version < "3.8"',
 ]
 optional-dependencies.docs = [
   "furo>=2023.3.27",
   "proselint>=0.13",
-  "sphinx>=6.1.3",
+  "sphinx>=6.2.1",
   "sphinx-autodoc-typehints!=1.23.4,>=1.23",
 ]
 optional-dependencies.test = [
   "appdirs==1.4.4",
   "covdefaults>=2.3",
   "pytest>=7.3.1",
   "pytest-cov>=4",
@@ -64,15 +64,15 @@
 urls.Documentation = "https://platformdirs.readthedocs.io"
 urls.Homepage = "https://github.com/platformdirs/platformdirs"
 urls.Source = "https://github.com/platformdirs/platformdirs"
 urls.Tracker = "https://github.com/platformdirs/platformdirs/issues"
 
 [tool.hatch]
 build.hooks.vcs.version-file = "src/platformdirs/version.py"
-build.targets.sdist.include = ["/src", "/tests"]
+build.targets.sdist.include = ["/src", "/tests", "/tox.ini"]
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
```

### Comparing `platformdirs-3.5.0/PKG-INFO` & `platformdirs-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.5.0
+Version: 3.5.1
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: appdirs,application,cache,directory,log,user
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: typing-extensions>=4.5; python_version < '3.8'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.3.27; extra == 'docs'
 Requires-Dist: proselint>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
-Requires-Dist: sphinx>=6.1.3; extra == 'docs'
+Requires-Dist: sphinx>=6.2.1; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: appdirs==1.4.4; extra == 'test'
 Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: pytest-cov>=4; extra == 'test'
 Requires-Dist: pytest-mock>=3.10; extra == 'test'
 Requires-Dist: pytest>=7.3.1; extra == 'test'
 Description-Content-Type: text/x-rst
@@ -50,15 +50,15 @@
 and configuration varies per platform. Even for single-platform apps, there
 may by plenty of nuances in figuring out the right location.
 
 For example, if running on macOS, you should use::
 
     ~/Library/Application Support/<AppName>
 
-If on Windows (at least English Win XP) that should be::
+If on Windows (at least English Win) that should be::
 
     C:\Documents and Settings\<User>\Application Data\Local Settings\<AppAuthor>\<AppName>
 
 or possibly::
 
     C:\Documents and Settings\<User>\Application Data\<AppAuthor>\<AppName>
 
@@ -109,15 +109,15 @@
     >>> user_log_dir(appname, appauthor)
     '/Users/trentm/Library/Logs/SuperApp'
     >>> user_documents_dir()
     '/Users/trentm/Documents'
     >>> user_runtime_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
-On Windows 7:
+On Windows:
 
 .. code-block:: pycon
 
     >>> from platformdirs import *
     >>> appname = "SuperApp"
     >>> appauthor = "Acme"
     >>> user_data_dir(appname, appauthor)
```


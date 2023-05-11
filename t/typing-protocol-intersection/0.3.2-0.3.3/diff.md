# Comparing `tmp/typing-protocol-intersection-0.3.2.tar.gz` & `tmp/typing-protocol-intersection-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing-protocol-intersection-0.3.2.tar", last modified: Thu Apr 13 21:00:03 2023, max compression
+gzip compressed data, was "typing-protocol-intersection-0.3.3.tar", last modified: Thu May 11 21:09:36 2023, max compression
```

## Comparing `typing-protocol-intersection-0.3.2.tar` & `typing-protocol-intersection-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-04-13 21:00:03.704826 typing-protocol-intersection-0.3.2/
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     1067 2022-03-12 15:38:10.000000 typing-protocol-intersection-0.3.2/LICENSE
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5899 2023-04-13 21:00:03.704826 typing-protocol-intersection-0.3.2/PKG-INFO
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5113 2023-04-13 20:48:17.000000 typing-protocol-intersection-0.3.2/README.md
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     1997 2023-02-15 22:47:16.000000 typing-protocol-intersection-0.3.2/pyproject.toml
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      883 2023-04-13 21:00:03.704826 typing-protocol-intersection-0.3.2/setup.cfg
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-04-13 21:00:03.701493 typing-protocol-intersection-0.3.2/tests/
--rw-------   0 mbiel     (1000) mbiel     (1000)     5365 2023-04-13 20:48:17.000000 typing-protocol-intersection-0.3.2/tests/test_mypy_plugin.py
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      649 2022-03-12 12:10:18.000000 typing-protocol-intersection-0.3.2/tests/test_python_module.py
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-04-13 21:00:03.701493 typing-protocol-intersection-0.3.2/typing_protocol_intersection/
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)       76 2022-03-11 17:16:39.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection/__init__.py
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     9105 2023-04-13 20:48:17.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection/mypy_plugin.py
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)        0 2022-03-09 10:02:04.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection/py.typed
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      865 2023-02-15 22:47:16.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection/types.py
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-04-13 21:00:03.704826 typing-protocol-intersection-0.3.2/typing_protocol_intersection.egg-info/
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5899 2023-04-13 21:00:03.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection.egg-info/PKG-INFO
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      473 2023-04-13 21:00:03.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection.egg-info/SOURCES.txt
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)        1 2023-04-13 21:00:03.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection.egg-info/dependency_links.txt
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)       29 2023-04-13 21:00:03.000000 typing-protocol-intersection-0.3.2/typing_protocol_intersection.egg-info/top_level.txt
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-05-11 21:09:36.208230 typing-protocol-intersection-0.3.3/
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     1067 2022-03-12 15:38:10.000000 typing-protocol-intersection-0.3.3/LICENSE
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5899 2023-05-11 21:09:36.208230 typing-protocol-intersection-0.3.3/PKG-INFO
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5113 2023-05-11 21:04:04.000000 typing-protocol-intersection-0.3.3/README.md
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     1997 2023-02-15 22:47:16.000000 typing-protocol-intersection-0.3.3/pyproject.toml
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      883 2023-05-11 21:09:36.208230 typing-protocol-intersection-0.3.3/setup.cfg
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-05-11 21:09:36.208230 typing-protocol-intersection-0.3.3/tests/
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5429 2023-05-11 21:04:04.000000 typing-protocol-intersection-0.3.3/tests/test_mypy_plugin.py
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      649 2022-03-12 12:10:18.000000 typing-protocol-intersection-0.3.3/tests/test_python_module.py
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-05-11 21:09:36.208230 typing-protocol-intersection-0.3.3/typing_protocol_intersection/
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)       76 2022-03-11 17:16:39.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection/__init__.py
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     9105 2023-05-11 21:04:04.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection/mypy_plugin.py
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)        0 2022-03-09 10:02:04.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection/py.typed
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      865 2023-02-15 22:47:16.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection/types.py
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2023-05-11 21:09:36.208230 typing-protocol-intersection-0.3.3/typing_protocol_intersection.egg-info/
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5899 2023-05-11 21:09:36.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection.egg-info/PKG-INFO
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      473 2023-05-11 21:09:36.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection.egg-info/SOURCES.txt
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)        1 2023-05-11 21:09:36.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection.egg-info/dependency_links.txt
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)       29 2023-05-11 21:09:36.000000 typing-protocol-intersection-0.3.3/typing_protocol_intersection.egg-info/top_level.txt
```

### Comparing `typing-protocol-intersection-0.3.2/LICENSE` & `typing-protocol-intersection-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.3.2/PKG-INFO` & `typing-protocol-intersection-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing-protocol-intersection
-Version: 0.3.2
+Version: 0.3.3
 Summary: Protocol intersection for mypy
 Home-page: https://github.com/klausweiss/typing-protocol-intersection
 Project-URL: Bug Tracker, https://github.com/klausweiss/typing-protocol-intersection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,15 @@
 The `ProtocolIntersection` type tells mypy that an object implements multiple protocols.
 It can be used either as a function parameter or as a return value.
 A mypy plugin that ships with the package is required for this to work.
 See the [examples](#examples) section below.
 
 ## Supported versions
 
-The plugin supports python 3.7, 3.8, 3.9, 3.10 and 3.11 and mypy >= 0.920 and <= 1.2.x.
+The plugin supports python 3.7, 3.8, 3.9, 3.10 and 3.11 and mypy >= 0.920 and <= 1.3.x.
 
 ## Installation
 
 The `typing-protocol-intersection` package is pip-installable:
 
 ```shell
 pip install typing-protocol-intersection
```

### Comparing `typing-protocol-intersection-0.3.2/README.md` & `typing-protocol-intersection-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 The `ProtocolIntersection` type tells mypy that an object implements multiple protocols.
 It can be used either as a function parameter or as a return value.
 A mypy plugin that ships with the package is required for this to work.
 See the [examples](#examples) section below.
 
 ## Supported versions
 
-The plugin supports python 3.7, 3.8, 3.9, 3.10 and 3.11 and mypy >= 0.920 and <= 1.2.x.
+The plugin supports python 3.7, 3.8, 3.9, 3.10 and 3.11 and mypy >= 0.920 and <= 1.3.x.
 
 ## Installation
 
 The `typing-protocol-intersection` package is pip-installable:
 
 ```shell
 pip install typing-protocol-intersection
```

### Comparing `typing-protocol-intersection-0.3.2/pyproject.toml` & `typing-protocol-intersection-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.3.2/setup.cfg` & `typing-protocol-intersection-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = typing-protocol-intersection
-version = 0.3.2
+version = 0.3.3
 description = Protocol intersection for mypy
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klausweiss/typing-protocol-intersection
 project_urls = 
 	Bug Tracker = https://github.com/klausweiss/typing-protocol-intersection/issues
 classifiers =
```

### Comparing `typing-protocol-intersection-0.3.2/tests/test_mypy_plugin.py` & `typing-protocol-intersection-0.3.3/tests/test_mypy_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 
 @pytest.mark.parametrize(
     "version",
     [
         pytest.param("0.910", id="0.910 - before the first supported 0.920"),
         pytest.param("0.992", id="0.992 - non-existent version greater than the last tested 0.x"),
-        pytest.param("1.3.0", id="1.3.0 - first greater than 1.2.x with breaking changes"),
+        pytest.param("1.4.0", id="1.4.0 - first greater than 1.3.x with breaking changes"),
     ],
 )
 def test_raises_for_unsupported_mypy_versions(version: str) -> None:
     with pytest.raises(NotImplementedError):
         typing_protocol_intersection.mypy_plugin.plugin(version)
 
 
@@ -137,13 +137,14 @@
     [
         pytest.param("0.920", id="0.920 - the first supported version"),
         pytest.param("0.991", id="0.991 - the last known 0.x version"),
         pytest.param("1.0.0", id="1.0.0 - the first 1.0.x version"),
         pytest.param("1.0.100", id="1.0.100 - some other 1.0.x version"),
         pytest.param("1.1.1", id="1.1.1 - some 1.1.x version"),
         pytest.param("1.2.0", id="1.2.0 - some 1.2.x version"),
+        pytest.param("1.3.0", id="1.3.0 - some 1.3.x version"),
     ],
 )
 def test_initializes_for_supported_mypy_versions(version: str) -> None:
     # when
     _plugin = typing_protocol_intersection.mypy_plugin.plugin(version)
     # then no exception
```

### Comparing `typing-protocol-intersection-0.3.2/tests/test_python_module.py` & `typing-protocol-intersection-0.3.3/tests/test_python_module.py`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.3.2/typing_protocol_intersection/mypy_plugin.py` & `typing-protocol-intersection-0.3.3/typing_protocol_intersection/mypy_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
 
 def plugin(version: str) -> typing.Type[mypy.plugin.Plugin]:
     version_prefix, *_ = version.split("dev.", maxsplit=1)  # stripping +dev.f6a8037cc... suffix if applicable
     numeric_prefixes = (_numeric_prefix(x) for x in version_prefix.split("."))
     parted_version = tuple(int(prefix) if prefix else None for prefix in numeric_prefixes)
     if (len(parted_version) == 2 and (0, 920) <= parted_version <= (0, 991)) or (
-        len(parted_version) == 3 and (1, 0, 0) <= parted_version < (1, 3, 0)
+        len(parted_version) == 3 and (1, 0, 0) <= parted_version < (1, 4, 0)
     ):
         return ProtocolIntersectionPlugin
 
     raise NotImplementedError(f"typing-protocol-intersection does not support mypy=={version}")
 
 
 def _numeric_prefix(string: str) -> Optional[str]:
```

### Comparing `typing-protocol-intersection-0.3.2/typing_protocol_intersection/types.py` & `typing-protocol-intersection-0.3.3/typing_protocol_intersection/types.py`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.3.2/typing_protocol_intersection.egg-info/PKG-INFO` & `typing-protocol-intersection-0.3.3/typing_protocol_intersection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing-protocol-intersection
-Version: 0.3.2
+Version: 0.3.3
 Summary: Protocol intersection for mypy
 Home-page: https://github.com/klausweiss/typing-protocol-intersection
 Project-URL: Bug Tracker, https://github.com/klausweiss/typing-protocol-intersection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,15 @@
 The `ProtocolIntersection` type tells mypy that an object implements multiple protocols.
 It can be used either as a function parameter or as a return value.
 A mypy plugin that ships with the package is required for this to work.
 See the [examples](#examples) section below.
 
 ## Supported versions
 
-The plugin supports python 3.7, 3.8, 3.9, 3.10 and 3.11 and mypy >= 0.920 and <= 1.2.x.
+The plugin supports python 3.7, 3.8, 3.9, 3.10 and 3.11 and mypy >= 0.920 and <= 1.3.x.
 
 ## Installation
 
 The `typing-protocol-intersection` package is pip-installable:
 
 ```shell
 pip install typing-protocol-intersection
```


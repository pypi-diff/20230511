# Comparing `tmp/pyaml-23.5.7.tar.gz` & `tmp/pyaml-23.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaml-23.5.7.tar", last modified: Fri May  5 17:04:11 2023, max compression
+gzip compressed data, was "pyaml-23.5.8.tar", last modified: Sat May  6 07:45:15 2023, max compression
```

## Comparing `pyaml-23.5.7.tar` & `pyaml-23.5.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.721541 pyaml-23.5.7/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.7/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.7/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9729 2023-05-05 17:04:11.721541 pyaml-23.5.7/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9025 2023-05-05 13:06:24.000000 pyaml-23.5.7/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.720541 pyaml-23.5.7/pyaml/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8951 2023-05-05 16:33:35.000000 pyaml-23.5.7/pyaml/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.7/pyaml/__main__.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.721541 pyaml-23.5.7/pyaml/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.7/pyaml/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17672 2023-05-05 13:24:38.000000 pyaml-23.5.7/pyaml/tests/test_dump.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 17:04:11.721541 pyaml-23.5.7/pyaml.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9729 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/requires.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-05 17:04:11.000000 pyaml-23.5.7/pyaml.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      805 2023-05-05 08:02:00.000000 pyaml-23.5.7/pyproject.toml
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-05 17:04:11.721541 pyaml-23.5.7/setup.cfg
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.7/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 07:45:15.421797 pyaml-23.5.8/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.8/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.8/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9727 2023-05-06 07:45:15.421797 pyaml-23.5.8/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9023 2023-05-05 19:19:16.000000 pyaml-23.5.8/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 07:45:15.421797 pyaml-23.5.8/pyaml/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8977 2023-05-06 07:43:09.000000 pyaml-23.5.8/pyaml/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.8/pyaml/__main__.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 07:45:15.421797 pyaml-23.5.8/pyaml/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.8/pyaml/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17672 2023-05-06 07:43:17.000000 pyaml-23.5.8/pyaml/tests/test_dump.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 07:45:15.421797 pyaml-23.5.8/pyaml.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9727 2023-05-06 07:45:15.000000 pyaml-23.5.8/pyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-06 07:45:15.000000 pyaml-23.5.8/pyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-06 07:45:15.000000 pyaml-23.5.8/pyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-06 07:45:15.000000 pyaml-23.5.8/pyaml.egg-info/requires.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-06 07:45:15.000000 pyaml-23.5.8/pyaml.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      805 2023-05-06 07:44:35.000000 pyaml-23.5.8/pyproject.toml
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-06 07:45:15.421797 pyaml-23.5.8/setup.cfg
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.8/setup.py
```

### Comparing `pyaml-23.5.7/PKG-INFO` & `pyaml-23.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.5.7
+Version: 23.5.8
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
@@ -283,15 +283,15 @@
 Using pip_ is how you generally install it, usually coupled with venv_ usage
 (which will also provide "pip" tool itself)::
 
   % pip install pyaml
 
 Current-git version can be installed like this::
 
-  % pip install 'git+https://github.com/mk-fg/pretty-yaml'
+  % pip install git+https://github.com/mk-fg/pretty-yaml
 
 pip will default to installing into currently-active venv, then user's home
 directory (under ``~/.local/lib/python...``), and maybe system-wide when running
 as root (only useful in specialized environments like docker containers).
 
 There are many other python packaging tools - pipenv_, poetry_, pdm_, etc -
 use whatever is most suitable for specific project/environment.
```

### Comparing `pyaml-23.5.7/README.rst` & `pyaml-23.5.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 Using pip_ is how you generally install it, usually coupled with venv_ usage
 (which will also provide "pip" tool itself)::
 
   % pip install pyaml
 
 Current-git version can be installed like this::
 
-  % pip install 'git+https://github.com/mk-fg/pretty-yaml'
+  % pip install git+https://github.com/mk-fg/pretty-yaml
 
 pip will default to installing into currently-active venv, then user's home
 directory (under ``~/.local/lib/python...``), and maybe system-wide when running
 as root (only useful in specialized environments like docker containers).
 
 There are many other python packaging tools - pipenv_, poetry_, pdm_, etc -
 use whatever is most suitable for specific project/environment.
```

### Comparing `pyaml-23.5.7/pyaml/__init__.py` & `pyaml-23.5.8/pyaml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 	def represent_undefined(self, data):
 		if isinstance(data, tuple) and hasattr(data, '_make') and hasattr(data, '_asdict'):
 			return self.represent_dict(data._asdict()) # assuming namedtuple
 		if isinstance(data, cs.abc.Mapping): return self.represent_dict(data) # dict-like
 		if type(data).__class__.__module__ == 'enum':
 			node = self.represent_data(data.value)
 			node.value = self.str_ext(node.value)
-			node.value.ext = f'# {str(data)}'
+			node.value.ext = f'# {data.__class__.__name__}.{data.name}'
 			return node
 		if hasattr(type(data), '__dataclass_fields__'):
 			try: import dataclasses as dcs
 			except ImportError: pass # can still be something else
 			else: return self.represent_dict(dcs.asdict(data))
 		try: # this is for numpy arrays, and the likes
 			if not callable(getattr(data, 'tolist', None)): raise AttributeError
```

### Comparing `pyaml-23.5.7/pyaml/__main__.py` & `pyaml-23.5.8/pyaml/__main__.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.7/pyaml/tests/test_dump.py` & `pyaml-23.5.8/pyaml/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.7/pyaml.egg-info/PKG-INFO` & `pyaml-23.5.8/pyaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.5.7
+Version: 23.5.8
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
@@ -283,15 +283,15 @@
 Using pip_ is how you generally install it, usually coupled with venv_ usage
 (which will also provide "pip" tool itself)::
 
   % pip install pyaml
 
 Current-git version can be installed like this::
 
-  % pip install 'git+https://github.com/mk-fg/pretty-yaml'
+  % pip install git+https://github.com/mk-fg/pretty-yaml
 
 pip will default to installing into currently-active venv, then user's home
 directory (under ``~/.local/lib/python...``), and maybe system-wide when running
 as root (only useful in specialized environments like docker containers).
 
 There are many other python packaging tools - pipenv_, poetry_, pdm_, etc -
 use whatever is most suitable for specific project/environment.
```

### Comparing `pyaml-23.5.7/pyproject.toml` & `pyaml-23.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pyaml"
-version = "23.05.07"
+version = "23.05.08"
 
 description = "PyYAML-based module to produce a bit more pretty and readable YAML-serialized data"
 authors = [{name="Mike Kazantsev", email="mk.fraggod@gmail.com"}]
 license = {text="WTFPL"}
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
```


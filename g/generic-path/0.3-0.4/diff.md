# Comparing `tmp/generic-path-0.3.tar.gz` & `tmp/generic-path-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-path-0.3.tar", last modified: Tue May  2 02:14:41 2023, max compression
+gzip compressed data, was "generic-path-0.4.tar", last modified: Thu May 11 04:06:33 2023, max compression
```

## Comparing `generic-path-0.3.tar` & `generic-path-0.4.tar`

### file list

```diff
@@ -1,16 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 02:14:41.629828 generic-path-0.3/
--rw-rw-rw-   0        0        0      900 2023-05-02 02:11:59.000000 generic-path-0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0    17098 2023-05-02 02:11:14.000000 generic-path-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     7270 2023-05-02 02:14:41.629828 generic-path-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4712 2023-05-02 02:11:59.000000 generic-path-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 02:14:41.628829 generic-path-0.3/generic_path.egg-info/
--rw-rw-rw-   0        0        0     7270 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      298 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    32101 2023-05-02 02:11:59.000000 generic-path-0.3/gpath.py
--rw-rw-rw-   0        0        0     2231 2023-05-02 02:11:59.000000 generic-path-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 02:14:41.629828 generic-path-0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 02:14:41.628829 generic-path-0.3/tests/
--rw-rw-rw-   0        0        0    35856 2023-05-02 02:11:59.000000 generic-path-0.3/tests/test_gpath.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.193546 generic-path-0.4/
+-rw-rw-rw-   0        0        0     4131 2023-05-11 03:24:36.000000 generic-path-0.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0    17098 2023-05-02 02:11:14.000000 generic-path-0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       22 2023-05-11 03:48:03.000000 generic-path-0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    11410 2023-05-11 04:06:33.193546 generic-path-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5648 2023-05-11 03:52:10.000000 generic-path-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.177546 generic-path-0.4/docs/
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.186546 generic-path-0.4/docs/html/
+-rw-rw-rw-   0        0        0     3123 2023-05-06 01:58:24.000000 generic-path-0.4/docs/html/favicon.png
+-rw-rw-rw-   0        0        0   522801 2023-05-11 03:49:45.000000 generic-path-0.4/docs/html/gpath.html
+-rw-rw-rw-   0        0        0      136 2023-05-11 03:49:45.000000 generic-path-0.4/docs/html/index.html
+-rw-rw-rw-   0        0        0   221953 2023-05-11 03:49:45.000000 generic-path-0.4/docs/html/search.js
+-rw-rw-rw-   0        0        0     2208 2023-05-11 03:48:24.000000 generic-path-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 04:06:33.193546 generic-path-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.177546 generic-path-0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.189547 generic-path-0.4/src/generic_path.egg-info/
+-rw-rw-rw-   0        0        0    11410 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      300 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.190546 generic-path-0.4/src/gpath/
+-rw-rw-rw-   0        0        0       97 2023-05-11 04:06:05.000000 generic-path-0.4/src/gpath/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_compat.py
+-rw-rw-rw-   0        0        0    36829 2023-05-11 02:28:52.000000 generic-path-0.4/src/gpath/_gpath.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.191546 generic-path-0.4/src/gpath/_rules/
+-rw-rw-rw-   0        0        0      129 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_rules/__init__.py
+-rw-rw-rw-   0        0        0      146 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_rules/_common.py
+-rw-rw-rw-   0        0        0      409 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_rules/_rules.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.192547 generic-path-0.4/tests/
+-rw-rw-rw-   0        0        0    37854 2023-05-11 02:28:00.000000 generic-path-0.4/tests/test_gpath.py
```

### Comparing `generic-path-0.3/LICENSE.txt` & `generic-path-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `generic-path-0.3/README.md` & `generic-path-0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GPath
 
-**GPath** is a Python package that provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
+**GPath** is a Python package that provides a robust, generalised abstract file path that allows path manipulations independent from the local environment, maximising cross-platform compatibility.
 
 [![](https://img.shields.io/badge/PyPI--inactive?style=social&logo=pypi)](https://pypi.org/project/generic-path/) [![](https://img.shields.io/badge/GitHub--inactive?style=social&logo=github)](https://github.com/yushiyangk/GPath) [![](https://img.shields.io/badge/Documentation--inactive?style=social&logo=readthedocs)](https://gpath.gnayihs.uy/)
 
 ## Install
 
 ```
 pip install generic-path
@@ -53,14 +53,28 @@
 }
 ```
 
 ## Issues
 
 Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls).
 
+## Compatibility
+
+The default `GPath()` interface supports the vast majority of valid file paths on Windows, Linux and macOS (and other POSIX-like operating systems), with some limited caveats.
+
+### Linux, macOS and POSIX
+
+- any backslashes `\` in the path will be treated as path separators
+- if the second character of the path is a colon <code><var>x</var>:</code>, the first character <var>`x`</var> will be treated as a drive letter
+
+### Windows and MS-DOS
+
+- any trailing dots `.` and spaces ` ` will not be stripped
+- reserved MS-DOS device names (such as AUX, CLOCK$, COM0 through COM9, CON, LPT0 through LPT9, NUL, PRN) will be treated as normal file names
+
 ## Development
 
 Clone the repository with `git clone https://github.com/yushiyangk/GPath.git`.
 
 The source for the package is entirely contained in `gpath.py`, with tests in `tests/`.
 
 ### Virtual environment
@@ -71,14 +85,18 @@
 
 Later, to deactivate the venv, run `deactivate`.
 
 ### Dependencies
 
 Run `pip install -r requirements.dev.txt`.
 
+### Install
+
+To install the package locally (in the venv) for development, run `pip install -e `.
+
 ### Tasks
 
 For unit tests, run `pytest`.
 
 To run unit tests across all supported Python versions, run `tox p -m testall`. This is slower than just `pytest`. Note that only Python versions that are installed locally will be run.
 
 To run the full set of tests and tasks, run `tox p -m prepare`. This should be done prior to package publication. Alternatively, see below for manually running individual steps in this process.
@@ -93,27 +111,32 @@
 
 Run `tox r -m docs`.
 
 The documentation is generated in `docs/html/`, using template files in `docs/template/`. However, note that the favicon file must be placed at `docs/html/favicon.png` manually as pdoc is unable to do so.
 
 #### Packaging
 
-Before packaging, check the package config by running `pyroma .` or `tox r -m config`.
+Before packaging, check the package metadata by running `pyroma .` or `tox r -m metadata`.
 
 To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
 
 ### Config files
 
+- `MANIFEST.in` Additional files to include in published sdist package
 - `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
 - `tox.ini` Config file for tox
 
 ### Troubleshooting
 
 #### Unable to uninstall the local package
 
 Sometimes, if gpath was installed using `pip install .`, pip might have difficulty uninstalling the package, giving the contradictory message
 <pre><code>Found existing installation: gpath <var>version</var>
 Can't uninstall 'gpath'. No files were found to uninstall.</code></pre>
 
 In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, then run `pip uninstall generic-path` again. This should allow pip to successfully uninstall the package.
+
+#### Tox always fails with exit 1
+
+Delete the contents of `.tox/` and try again.
```

### Comparing `generic-path-0.3/gpath.py` & `generic-path-0.4/src/gpath/_gpath.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,233 +1,336 @@
 """
-	GPath is a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
+	GPath is a robust, generalised abstract file path that provides path manipulations independent from the local environment, maximising cross-platform compatibility.
 """
 
 from __future__ import annotations
 
-import functools
 import os
 import sys
-from collections.abc import Collection, Iterator, Sequence
-#from typing import Any, ClassVar, Final
+from collections.abc import Collection, Hashable, Iterator, Iterable, Sequence, Sized
+from typing import Any, overload
+
+from . import _rules
+
+
+from ._compat import Final, Optional, Union
+
+
+__all__ = ('GPath', 'GPathLike')
 
 
-# Type hinting prior to 3.10
-# Using generics in built-in collections, e.g. list[int], is supported from 3.7 by __future__.annotations
-from typing import Any, ClassVar, Optional, Union
-if sys.version_info >= (3, 8):
-	from typing import Final
-else:
-	Final = Any
 if sys.version_info >= (3, 10):
 	def _is_gpathlike(obj: Any) -> bool:
 		return isinstance(obj, GPathLike)
 else:
 	def _is_gpathlike(obj: Any) -> bool:
 		return isinstance(obj, GPath) or isinstance(obj, str) or isinstance(obj, os.PathLike)
 
 
-__version__ = '0.3'
+DEFAULT_ENCODING: Final = 'utf-8'
 
 
-PATH_SEPARATOR: Final = "/" if os.sep == '/' or os.altsep == '/' else os.sep
-PATH_CURRENT: Final = os.curdir
-PATH_PARENT: Final = os.pardir
 
-PathLike = Union[str, os.PathLike]
+def _split_relative(
+	path: str,
+	delimiters: Union[str, Collection[str]],
+	collapse: bool=True
+) -> list[str]:
+	if path == "":
+		return [path]
+
+	if delimiters == "" or len(delimiters) == 0:
+		return [path]
+
+	if isinstance(delimiters, Iterable):
+		delimiter_iter = iter(delimiters)
+		delimiter = next(delimiter_iter)
+		for d in delimiter_iter:
+			path = path.replace(d, delimiter)
+
+	if collapse:
+		# Assumes len(delimiter) == 1
+		new_path = delimiter
+		for c in path:
+			if c == delimiter and new_path[-1] == delimiter:
+				pass
+			else:
+				new_path += c
+		path = new_path[1:]
 
+	return path.split(delimiter)
 
-@functools.total_ordering
-class GPath():
-	"""
-		A normalised and generalised abstract file path that has no dependency on the layout of any real filesystem. This allows us to manipulate file paths that were generated on a different system, particularly one with a different operating environment as compared to the local system.
 
-		The path can be manipulated with various methods before being rendered in a format that is meaningful to the local operating system using `__str__()`.
+def _normalise_relative(
+	parts: Sequence[str],
+	current_dirs: Collection[str]=_rules.COMMON_CURRENT_INDICATOR,
+	parent_dirs: Collection[str]=_rules.COMMON_PARENT_INDICATOR,
+):
+	output = []
+	for part in parts:
+		if part == "":
+			pass
+		elif part == current_dirs:
+			pass
+		elif part == parent_dirs:
+			if len(output) > 0 and output[-1] != parent_dirs:
+				output.pop()
+			else:
+				output.append(part)
+		else:
+			output.append(part)
+	return output
+
+
+class GPath(Hashable, Sized, Iterable):
 	"""
+		An immutable generalised abstract file path that has no dependency on any real filesystem.
 
-	__slots__ = ('_parts', '_device', '_absolute', '_parent')
+		The path can be manipulated on a system that is different from where it originated, particularly with a different operating environment, and it can represent file paths on a system other than local. Examples where this is useful include remote management of servers and when cross-compiling source code for a different platform. Since GPath objects are immutable, all operations return a new instance.
 
-	separator: ClassVar[str] = PATH_SEPARATOR
-	"""Path separator character, usually `/`"""
+		The path is always stored in a normalised state, and is always treated as case sensitive.
 
-	current_dir: ClassVar[str] = PATH_CURRENT
-	"""Path component that indicates the current directory; usually `.`"""
+		The path can be rendered as a string using <code>str(<var>g</var>)</code>, which will use `/` as the path separator if possible to maximise cross-platform compatibility.
+	"""
 
-	parent_dir: ClassVar[str] = PATH_PARENT
-	"""Path component that indicates a parent directory; usually `..`"""
+	__slots__ = (
+		'_parts',
+		'_root',
+		'_drive',
+		'_parent_level',
+		'_encoding',
+	)
 
 
-	def __init__(self, path: Union[PathLike, GPath, None]=""):
+	def __init__(self, path: Union[str, bytes, os.PathLike, GPath, None]="", encoding: Optional[str]=None):
 		"""
 			Initialise a normalised and generalised abstract file path, possibly by copying an existing GPath object.
 
 			Parameters
 			----------
 			`path`
 			: path-like object representing a (possibly unnormalised) file path, or a GPath object to be copied
 
+			`​encoding`
+			: the text encoding that should be used to decode paths given as bytes-like objects; if not specified, `'utf-8'` will be used by default. The name should be one of the standard Python text encodings, as listed in the `codecs` module of the standard library. The specified encoding will propagate to new GPaths that result from operations on this GPath. If a binary operation involves two GPaths, the encoding specified by the left operand will be propagated to the result.
+
 			Raises
 			------
 			`ValueError` if `other` is an invalid GPath
 
 			Examples
 			--------
 			```python
 			GPath("/")
 			GPath("/usr/bin")
 			GPath("C:/Program Files")
 			```
 		"""
+
 		self._parts: tuple[str, ...] = tuple()  # root- or parent- relative path
-		self._device: str = ""
-		self._absolute: bool = False
-		self._parent: int = 0
-		if path is not None and path != "":
-			if isinstance(path, GPath):
-				path._validate()
-				self._parts = path._parts
-				self._device = path._device
-				self._absolute = path._absolute
-				self._parent = path._parent
-			else:
-				# Remove redundant '.'s and '..'s and use OS-default path separators
-				path = os.path.normpath(path)  # sets empty path to '.' and removes trailing slash
-
-				if path == os.curdir:
-					path = ""
-				(self._device, path) = os.path.splitdrive(path)
-				self._absolute = os.path.isabs(path)
-
-				parts = path.split(os.sep)  # os.path.normpath previously rewrote the path to use os.sep
-				if len(parts) > 0 and parts[0] == "":  # First element is '' if root
-					parts = parts[1:]
-				if len(parts) > 0 and parts[-1] == "":  # Last element is '' if there is a trailing slash, which should only happen when the path is exactly root ('/')
-					parts = parts[:-1]
-
-				dotdot = 0
-				while dotdot < len(parts) and parts[dotdot] == GPath.parent_dir:  # GPath.parent_dir == '..' usually
-					dotdot += 1
-				self._parts = tuple(parts[dotdot:])
-				self._parent = dotdot
+		self._root: bool = False
+		self._drive: str = ""
+		self._parent_level: int = 0
+
+		self._encoding: Optional[str] = encoding
+
+		if path is None or path == "":
+			return
+
+		if isinstance(path, GPath):
+			path._validate()
+			self._parts = path._parts
+			self._root = path._root
+			self._drive = path._drive
+			self._parent_level = path._parent_level
+
+			self._encoding = path._encoding if encoding is None else encoding
+			return
+
+		path = os.fspath(path)
+
+		if isinstance(path, bytes):
+			if self._encoding is None:
+				path = path.decode(DEFAULT_ENCODING)
+			else:
+				path = path.decode(self._encoding)
 
+		# path is a str
 
-	@staticmethod
-	def from_parts(parts: Sequence[str]) -> GPath:
-		"""
-			Create a GPath object from a sequence of strings, such as that generated by `get_parts()`.
+		if len(path) >= 2 and path[1] in _rules.generic_rules.drive_postfixes:
+			self._drive = path[0]
+			deviceless_path = path[2:]
+		else:
+			deviceless_path = path
 
-			Note that unlike `GPath.join()`, this method expects each item in the sequence to be a single string representing a path component, without any separators. Absolute paths are represented in the same manner as returned by `get_parts()`.
-		"""
-		return GPath(GPath.separator.join(parts))
+		for root in _rules.generic_rules.roots:
+			if deviceless_path.startswith(root):
+				self._root = True
+				break
 
+		if self._root:
+			rootless_path = deviceless_path[1:]
+		else:
+			rootless_path = deviceless_path
 
-	@staticmethod
-	def find_common(path1: GPathLike, path2: GPathLike, allow_current: bool=True, allow_parents: bool=False) -> Optional[GPath]:
+
+		parts = _split_relative(rootless_path, delimiters=(set(_rules.generic_rules.separators) | set(_rules.generic_rules.separators)))
+		parts = _normalise_relative(parts)
+		parent_level = 0
+		while parent_level < len(parts) and parts[parent_level] in _rules.generic_rules.parent_indicators:
+			parent_level += 1
+		self._parts = tuple(parts[parent_level:])
+		if self._root == False:
+			self._parent_level = parent_level
+
+
+	@property
+	def named_parts(self) -> list[str]:
 		"""
-			Find the longest common base path shared by the two paths, or return None if no such path exists.
+			Read-only named components of the path, not including the filesystem root, device name, or any parent directories
 
-			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different device names), or in other cases as controlled by the `allow_current` and `allow_parents` options.
+			Examples
+			--------
+			```python
+			GPath("usr/local/bin").named_parts     # ["usr", "local", "bin"]
+			GPath("../../Documents").named_parts   # ["Documents"]
+			GPath("/usr/bin").named_parts          # ["usr", "bin"]
+			GPath("C:/Program Files").named_parts  # ["Program Files"]
+			```
+		"""
+		return list(self._parts)
 
-			Parameters
-			----------
-			`path1`, `path2`
-			: the paths to compare
+	@property
+	def parent_level(self) -> int:
+		"""
+			Read-only number of levels of parent directories that the path is relative to, which may be 0
 
-			`allow_current`
-			: whether two non-parent relative paths that do not share any components should be considered to have a common base path, namely the imaginary current working directory. For instance, `GPath.find_common("some/rel/path", "another/rel/path")` will return `GPath("")` if set to True, or return None if set to False.
+			Examples
+			--------
+			```python
+			GPath("../../Documents").parent_level  # 2
+			GPath("usr/local/bin").parent_level    # 0
+			```
+		"""
+		return self._parent_level
 
-			`allow_parents`
-			: whether two relative paths that are relative to different levels of parent directories should be considered to have a common base path, which is the highest level of parent directory between the two paths. For instance, `GPath.find_common("../rel/to/parent", "../../rel/to/grandparent")` will return `GPath("../..")` if set to True, or return None if set to False. **Warning**: when set to True, given a higher level of parent directory as output, it may not be possible to find the relative path to one of the inputs (see `relpath_from()`); in most cases False is more appropriate.
+	@property
+	def parent_parts(self) -> list[str]:
+		"""
+			Read-only path components representing a parent directory that it is relative to, if any, with a copy of `parent_indicator` for each level of parent directory
 
-			Returns
-			-------
-			`GPath`
-			: the longest common base path, which may be empty, if it exists
+			Examples
+			--------
+			```python
+			GPath("../../Documents").parent_parts  # ["..", ".."]
+			GPath("usr/local/bin").parent_parts    # []
+			```
+		"""
+		return [_rules.generic_rules.parent_indicators[0] for i in range(self._parent_level)]
 
-			`None`
-			: otherwise
+	@property
+	def relative_parts(self) -> list[str]:
+		"""
+			Read-only relative components of the path, not including the filesystem root or device name, with a copy of `parent_indicator` for each level of parent directory
 
-			Raises
-			------
-			`ValueError` if either GPath is invalid
+			Examples
+			--------
+			```python
+			GPath("usr/local/bin").relative_parts     # ["usr", "local", "bin"]
+			GPath("../../Documents").relative_parts   # ["..", "..", "Documents"]
+			GPath("/usr/bin").relative_parts          # ["usr", "bin"]
+			GPath("C:/Program Files").relative_parts  # ["Program Files"]
+			```
+		"""
+		return self.parent_parts + list(self._parts)
+
+	@property
+	def drive(self) -> str:
+		"""
+			Read-only device name
 
 			Examples
 			--------
 			```python
-			GPath.find_common("/usr/bin", "/usr/local/bin")               # GPath("/usr")
-			GPath.find_common("C:/Windows/System32", "C:/Program Files")  # GPath("C:/")
-			GPath.find_common("../Documents", "../Pictures")              # GPath("..")
+			GPath("C:/Windows").device       # "C:"
+			GPath("/usr/bin").device         # ""
+			GPath("../../Documents").device  # ""
 			```
 		"""
-		if isinstance(path1, GPath):
-			path1._validate()
-		else:
-			path1 = GPath(path1)
-		if isinstance(path2, GPath):
-			path2._validate()
-		else:
-			path2 = GPath(path2)
+		return self._drive
 
-		if path1._device != path2._device:
-			return None
-		if path1._absolute != path2._absolute:
-			return None
+	@property
+	def absolute(self) -> bool:
+		"""
+			Read-only flag for whether the path is an absolute path
 
-		if allow_parents:
-			allow_current = True
+			Examples
+			--------
+			```python
+			GPath("/").absolute                # True
+			GPath("C:/Windows").absolute       # True
+			GPath("local/bin").absolute        # False
+			GPath("../../Documents").absolute  # False
+			```
+		"""
+		return self._root
 
-		parts = []
-		if path1._absolute:
-			common_path = GPath()
-			for part1, part2 in zip(path1._parts, path2._parts):
-				if part1 == part2:
-					parts.append(part1)
-			common_path._absolute = True
-			# dotdot must be 0
-		else:
-			if path1._parent != path2._parent:
-				if not allow_parents:
-					return None
+	@property
+	def root(self) -> bool:
+		"""
+			Read-only flag for whether the path is exactly the root of the filesystem
 
-				common_path = GPath()
-				common_path._parent = max(path1._parent, path2._parent)
-			else:
-				common_path = GPath()
-				common_path._parent = path1._parent
-				for part1, part2 in zip(path1._parts, path2._parts):
-					if part1 == part2:
-						parts.append(part1)
+			Examples
+			--------
+			```python
+			GPath("/").root                # True
+			GPath("C:/").root              # True
+			GPath("/usr/bin").root         # False
+			GPath("C:/Windows").root       # False
+			GPath("../../Documents").root  # False
+			```
+		"""
+		return self._root and len(self._parts) == 0
 
-		common_path._device = path1._device
-		common_path._parts = tuple(parts)
+	@property
+	def encoding(self) -> Union[str, None]:
+		"""
+			Read-only encoding used to decode other paths that are given as bytes-like objects
+		"""
+		return self._encoding
 
-		if not allow_current and not bool(common_path):
-			if common_path != path1 or common_path != path2:
-				return None
-		return common_path
 
+	@overload
+	def partition(paths: Iterable[GPathLike], **kwargs) -> dict[GPath, list[GPath]]:
+		...
+	@overload
+	def partition(*paths: GPathLike, **kwargs) -> dict[GPath, list[GPath]]:
+		...
 	@staticmethod
-	def partition(*paths: Union[Collection[GPathLike], GPathLike], allow_current: bool=True, allow_parents: bool=False) -> dict[GPath, list[GPath]]:
+	def partition(*paths, allow_current: bool=True, allow_parents: bool=True, encoding: Optional[str]=None) -> dict[GPath, list[GPath]]:
 		"""
 			Partition a collection of paths based on shared common base paths such that each path belongs to one partition.
 
 			For each partition, return a list of relative paths from the base path of that partition to each corresponding input path within that partition, unless `allow_parents` is True (see below). If the input collection is ordered, the output order is preserved within each partition. If the input collection contains duplicates, the corresponding output lists will as well.
 
-			The number of partitions is minimised by merging partitions as much as possible, so that each partition represents the highest possible level base path. Two partitions can no longer be merged when there is no common base path between them, as determined by `GPath.find_common()`. This method takes the same optional arguments as `GPath.find_common()`, with the same default values.
+			The number of partitions is minimised by merging partitions as much as possible, so that each partition represents the highest possible level base path. Two partitions can no longer be merged when there is no common base path between them, as determined by `common_with()`. This method takes the same optional arguments as `common_with()`, with the same default values.
 
 			Parameters
 			----------
-			`paths: Collection[GPath | str | os.PathLike]` or `*paths: GPath | str | os.PathLike`
+			`paths: Iterable[GPath | str | bytes | os.PathLike]` or `*paths: GPath | str | bytes | os.PathLike`
 			: the paths to be partitioned, which can be given as either a list-like object or as variadic arguments
 
 			`allow_current`
-			: whether non-parent relative paths with no shared components should be considered to have a common base path (see `GPath.find_common()`)
+			: whether non-parent relative paths with no shared components should be considered to have a common base path (see `common_with()`)
 
 			`allow_parents`
-			: whether paths that are relative to different levels of parent directories should be considered to have a common base path (see `GPath.find_common()`). **Warning**: when set to True, the output lists for each partition are invalidated, and explicitly set to empty. This is because it is not possible in general to obtain a relative path from the base path to its members if the base path is a parent directory of a higher level than the member (see `relpath_from()`). This  option should be True if and only if the list of members in each partition are not of interest; in most cases False is more appropriate.
+			: whether paths that are relative to different levels of parent directories should be considered to have a common base path (see `common_with()`). **Warning**: when set to True, the output lists for each partition are invalidated, and explicitly set to empty. This is because it is not possible in general to obtain a relative path from the base path to its members if the base path is a parent directory of a higher level than the member (see `relpath_from()`). This  option should be True if and only if the list of members in each partition are not of interest; in most cases False is more appropriate.
+
+			`​encoding`
+			: the text encoding that should be used to decode bytes-like objects in `paths`, if any (see `__init__()`).
 
 			Returns
 			-------
 			a dictionary that maps the common base path of each partition to a list of relative paths
 
 			Raises
 			------
@@ -248,27 +351,27 @@
 		"""
 		flattened_paths: list[GPathLike] = []
 		for path_or_list in paths:
 			if _is_gpathlike(path_or_list):
 				flattened_paths.append(path_or_list)
 			else:
 				flattened_paths.extend(path_or_list)
-		gpaths = [path if isinstance(path, GPath) else GPath(path) for path in flattened_paths]
+		gpaths = [path if isinstance(path, GPath) else GPath(path, encoding=encoding) for path in flattened_paths]
 
 		partition_map = {}
 		if len(gpaths) > 0:
 			if allow_parents == True:
 				partition_map[gpaths[0]] = []
 			else:
 				partition_map[gpaths[0]] = [gpaths[0]]
 
 		for path in gpaths[1:]:
 			partition_found = False
 			for partition in partition_map:
-				candidate_common = GPath.find_common(partition, path, allow_current=allow_current, allow_parents=allow_parents)
+				candidate_common = partition.common_with(path, allow_current=allow_current, allow_parents=allow_parents)
 				if candidate_common is not None:
 					partition_found = True
 					if candidate_common != partition:
 						partition_map[candidate_common] = partition_map[partition]
 						del partition_map[partition]
 					if allow_parents == False:
 						partition_map[candidate_common].append(path)
@@ -281,24 +384,33 @@
 
 		for partition, path_list in partition_map.items():
 			partition_map[partition] = [path.subpath_from(partition) for path in path_list]
 
 		return partition_map
 
 
+	@overload
+	def join(paths: Iterable[GPathLike], **kwargs) -> GPath:
+		...
+	@overload
+	def join(*paths: GPathLike, **kwargs) -> GPath:
+		...
 	@staticmethod
-	def join(*paths: Union[Collection[GPathLike], GPathLike]) -> GPath:
+	def join(*paths, encoding: Optional[str]=None) -> GPath:
 		"""
 			Join a sequence of paths into a single path. Apart from the first item in the sequence, all subsequent paths should be relative paths and any absolute paths will be ignored.
 
 			Parameters
 			----------
-			`paths`: `Collection[GPath | str | os.PathLike]` or `*paths: GPath | str | os.PathLike`
+			`paths`: `Sequence[GPath | str | bytes | os.PathLike]` or `*paths: GPath | str | bytes | os.PathLike`
 			: the paths to be combined, which can be given as either a list-like object or as variadic arguments
 
+			`​encoding`
+			: the text encoding that should be used to decode bytes-like objects in `paths`, if any (see `__init__()`).
+
 			Returns
 			-------
 			the combined path
 
 			Raises
 			------
 			`ValueError` if any of the GPaths are invalid
@@ -315,147 +427,226 @@
 		for path_or_list in paths:
 			if _is_gpathlike(path_or_list):
 				flattened_paths.append(path_or_list)
 			else:
 				flattened_paths.extend(path_or_list)
 
 		if len(flattened_paths) == 0:
-			return GPath()
+			return GPath(encoding=encoding)
 
 		combined_path = flattened_paths[0]
 		if not isinstance(combined_path, GPath):
-			combined_path = GPath(combined_path)
+			combined_path = GPath(combined_path, encoding=encoding)
 		for path in flattened_paths[1:]:
 			combined_path = combined_path + path
 
 		return combined_path
 
 
-	def get_parts(self, root: bool=True, parent: bool=True) -> list[str]:
+	def as_relative(self, parent_level: Optional[int]=None) -> GPath:
 		"""
-			Convert the path to a list of strings that unambiguously represents the given path.
-
-			The list of strings is given in such a way that a valid path can be reconstructed as a single string using <code>GPath.separator.join(<var>g</var>.get_parts())</code>. By default, the list of strings represents the full input path, but this behaviour can be changed using the optional arguments.
-
-			If it is an absolute path, the first item in the returned list will contain the device name if it exists, or be an empty string otherwise. If the path is the filesystem root exactly, the returned list will contain exactly two items, with the second being an empty string.
-
-			If the path is relative to a parent directory, e.g. `../..`, each parent level will be given as a separate item in the returned list.
+			Convert the path to a relative path and return a new copy.
 
 			Parameters
 			----------
-			`root`
-			: whether to include any components that indicate the filesystem root or device name. If set to True, the returned list will represent an absolute path as described above if the input path is absolute. If set to False, the returned list will always represent a relative path.
-
-			`parent`
-			: whether to include any components that indicate parent directories for a relative path. If set to False, the returned list will always be either an absolute path or a path relative to the imaginary current working directory.
+			`​parent_level`
+			: the number of levels of parent directories that the returned path should be relative to, which may be 0. If set to None, the returned path will have the same parent level as the current path if it is currently a relative path, or have no parent level (i.e. 0) otherwise.
 
-			Returns
-			-------
-			list of strings representing the path
+			Raises
+			------
+			`TypeError` if `​parent_level` is not a valid type
 
 			Examples
 			--------
 			```python
-			GPath("usr/local/bin").get_parts()     # ["usr", "local", "bin"]
-			GPath("/usr/bin").get_parts()          # ["", "usr", "bin"]
-			GPath("C:/Program Files").get_parts()  # ["C:", "Program Files"]
-			GPath("../../Documents").get_parts()   # ["..", "..", "Documents"]
+			GPath("/usr/bin").as_relative()      # GPath("usr/bin")
+			GPath("C:/Windows").as_relative()    # GPath("C:Windows")
+			GPath("../Documents").as_relative()  # GPath("../Documents")
 			```
 		"""
-		if root and self._absolute:
-			if len(self._parts) == 0:
-				return [self._device, ""]
-
-			base_parts = [self._device]
-
-		elif parent and self._parent > 0:
-			base_parts = self.get_parent_parts()
 
+		new_path = GPath(self)
+		new_path._root = False
+		if parent_level is None:
+			pass
+		elif isinstance(parent_level, int):
+			new_path._parent_level = parent_level
 		else:
-			if len(self._parts) == 0:
-				# bool(self) == False
-				return [GPath.current_dir]
+			raise TypeError(f"parent_level must be an int: {parent_level} ({type(parent_level)})")
 
-			base_parts = []
-
-		return base_parts + list(self._parts)
+		return new_path
 
 
-	def get_parent_parts(self) -> list[str]:
+	def as_absolute(self) -> GPath:
 		"""
-			Get a list of strings representing the parent directory that the path is relative to, if any.
+			Convert the path to an absolute path and return a new copy.
 
-			For each parent level, the returned list will contain one copy of `GPath.parent_dir`. If the path is not relative to a parent directory, the returned list will be empty.
+			Any parent directory that the path is relative to will be removed. If the path is already absolute, an identical copy is returned.
 
 			Examples
 			--------
 			```python
-			GPath("../../Documents").get_parent_parts()  # ["..", ".."]
-			GPath("usr/local/bin").get_parent_parts()    # []
+			GPath("usr/bin").as_absolute()       # GPath("/usr/bin")
+			GPath("../Documents").as_absolute()  # GPath("/Documents")
+			GPath("C:Windows").as_absolute()     # GPath("C:/Windows")
 			```
 		"""
-		return [GPath.parent_dir for i in range(self._parent)]
+		new_path = GPath(self)
+		new_path._root = True
+		new_path._parent_level = 0
+		return new_path
 
-	def get_parent_level(self) -> int:
-		"""
-			Get the number of levels of parent directories that the path is relative to, which may be 0.tain one copy of `GPath.parent_dir`. If the path is not relative to a parent directory, the returned list will be empty.
 
-			Examples
-			--------
-			```python
-			GPath("../../Documents").get_parent_level()  # 2
-			GPath("usr/local/bin").get_parent_level()    # 0
-			```
+	def with_drive(self, drive: Union[str, bytes, None]=None) -> GPath:
 		"""
-		return self._parent
+			Return a new copy of the path with the drive set to `​drive`.
 
-	def get_device(self) -> Optional[str]:
-		"""
-			Get the device name.
+			If `​drive` is `""` or None, this would be equivalent to `without_drive()`.
+
+			Parameters
+			----------
+			`​drive`
+			: the drive for the returned path, or either `""` or None if the returned path should have no drive
+
+			Returns
+			-------
+			`GPath`
+			: a new path with the given drive
+
+			Raises
+			------
+			- `TypeError` if `​drive` is not a valid type
+			- `ValueError` if `​drive` has more than one character
 
 			Examples
 			--------
 			```python
-			GPath("C:/Windows").get_device()       # "C:"
-			GPath("/usr/bin").get_device()         # ""
-			GPath("../../Documents").get_device()  # ""
+			GPath("C:/Windows").with_drive()      # GPath("/Windows")
+			GPath("C:/Windows").with_drive("D")   # GPath("D:/Windows")
+			GPath("/Windows").with_drive("C")     # GPath("C:/Windows")
 			```
 		"""
-		return self._device
+		if drive is None:
+			drive = ""
+		elif isinstance(drive, bytes):
+			if self._encoding is None:
+				drive = drive.decode(DEFAULT_ENCODING)
+			else:
+				drive = drive.decode(self._encoding)
+		elif isinstance(drive, str):
+			pass
+		else:
+			raise TypeError(f"drive must be a str or bytes object: {drive} ({type(drive)})")
+
+		if len(drive) > 1:
+			raise ValueError(f"drive can only be a single character, an empty string or None: {drive}")
+
+		new_path = GPath(self)
+		new_path._drive = drive
+		return new_path
+
 
-	def is_absolute(self) -> bool:
+	def without_drive(self) -> GPath:
 		"""
-			Check if the path is an absolute path.
+			Return a new copy of the path without a drive.
+
+			Equivalent to `with_drive("")` or `with_drive(None)`.
+
+			Returns
+			-------
+			`GPath`
+			: a new path without a drive
 
 			Examples
 			--------
 			```python
-			GPath("/").is_absolute()                # True
-			GPath("C:/Windows").is_absolute()       # True
-			GPath("local/bin").is_absolute()        # False
-			GPath("../../Documents").is_absolute()  # False
+			GPath("C:/Windows").without_drive()      # GPath("/Windows")
 			```
 		"""
-		return self._absolute
+		return self.with_drive(None)
+
 
-	def is_root(self) -> bool:
+	def common_with(self, other: GPathLike, allow_current: bool=True, allow_parents: bool=False) -> Optional[GPath]:
 		"""
-			Check if the path is exactly the root of the filesystem.
+			Find the longest common base path shared between `self` and `other`, or return None if no such path exists.
+
+			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different device names), or in other cases as controlled by the `allow_current` and `allow_parents` options.
+
+			If using the default options of `allow_current=True` and `allow_parent=False`, the binary operator for bitwise-and can be used: `__and__()` (usage: <code><var>g1</var> & <var>g2</var></code>).
+
+			Parameters
+			----------
+			`other`
+			: the path to compare with
+
+			`allow_current`
+			: whether two non-parent relative paths that do not share any components should be considered to have a common base path, namely the imaginary current working directory. For instance, `GPath("some/rel/path").find_common("another/rel/path")` will return `GPath("")` if set to True, or return None if set to False.
+
+			`allow_parents`
+			: whether two relative paths that are relative to different levels of parent directories should be considered to have a common base path, which is the highest level of parent directory between the two paths. For instance, `GPath("../rel/to/parent").find_common("../../rel/to/grandparent")` will return `GPath("../..")` if set to True, or return None if set to False. **Warning**: when set to True, given a higher level of parent directory as output, it may not be possible to find the relative path to one of the inputs (see `relpath_from()`); in most cases False is more appropriate.
+
+			Returns
+			-------
+			`GPath`
+			: the longest common base path, which may be empty, if it exists
+
+			`None`
+			: otherwise
+
+			Raises
+			------
+			`ValueError` if either `self` or `other` is an invalid GPath
 
 			Examples
 			--------
 			```python
-			GPath("/").is_root()                # True
-			GPath("C:/").is_root()              # True
-			GPath("/usr/bin").is_root()         # False
-			GPath("C:/Windows").is_root()       # False
-			GPath("../../Documents").is_root()  # False
+			GPath("/usr/bin").find_common("/usr/local/bin")               # GPath("/usr")
+			GPath("C:/Windows/System32").find_common("C:/Program Files")  # GPath("C:/")
+			GPath("../Documents").find_common("../Pictures")              # GPath("..")
 			```
 		"""
-		return self._absolute and len(self._parts) == 0
+		self._validate()
+		if isinstance(other, GPath):
+			other._validate()
+		else:
+			other = GPath(other, encoding=self._encoding)
+
+		if self._drive != other._drive:
+			return None
+		if self._root != other._root:
+			return None
+
+		if allow_parents:
+			allow_current = True
+
+		parts = []
+		if self._root:
+			common_path = GPath(self)
+			for part1, part2 in zip(self._parts, other._parts):
+				if part1 == part2:
+					parts.append(part1)
+		else:
+			if self._parent_level != other._parent_level:
+				if not allow_parents:
+					return None
+
+				common_path = GPath(self)
+				common_path._parent_level = max(self._parent_level, other._parent_level)
+			else:
+				common_path = GPath(self)
+				for part1, part2 in zip(self._parts, other._parts):
+					if part1 == part2:
+						parts.append(part1)
+
+		common_path._parts = tuple(parts)
+
+		if not allow_current and not bool(common_path):
+			if common_path != self or common_path != other:
+				return None
+		return common_path
 
 
 	def subpath_from(self, base: GPathLike) -> Optional[GPath]:
 		"""
 			Find the relative subpath from `base` to `self` if possible and if `base` contains `self`, or return None otherwise.
 
 			None will also be returned if there are unknown components in the subpath from `base` to `self`. For instance, if `self` is relative to the parent directory while `base` is relative to the grandparent directory, the path from the grandparent directory `../..` to the parent directory `..` cannot be known.
@@ -484,21 +675,24 @@
 			```python
 			GPath("/usr/local/bin").subpath_from("/usr")      # GPath("local/bin")
 			GPath("/usr/bin").subpath_from("/usr/local/bin")  # None
 			GPath("/usr/bin").subpath_from("../Documents")    # None
 			```
 		"""
 		if not isinstance(base, GPath):
-			base = GPath(base)
+			base = GPath(base, encoding=self._encoding)
 
-		if GPath.find_common(self, base, allow_current=True, allow_parents=False) is not None and self in base:
-			# If self._dotdot > base._dotdot, self is not in base, whereas if self._dotdot < base._dotdot, path from base to self's parent cannot be known
+		if self.common_with(base, allow_current=True, allow_parents=False) is not None and self in base:
+			# If self._parent_level > base._parent_level, self is not in base, whereas if self._parent_level < base._parent_level, path from base to self's parent cannot be known
 			base_length = len(base._parts)
-			new_path = GPath()
+			new_path = GPath(self)
 			new_path._parts = self._parts[base_length:]  # () when self == base
+			new_path._drive = ""
+			new_path._root = False
+			new_path._parent_level = 0
 			return new_path
 		else:
 			return None
 
 
 	def relpath_from(self, origin: GPathLike) -> Optional[GPath]:
 		"""
@@ -531,103 +725,82 @@
 			GPath("/usr/local/bin").subpath_from("/usr")      # GPath("local/bin")
 			GPath("/usr/bin").subpath_from("/usr/local/bin")  # GPath("../../bin")
 			GPath("/usr/bin").subpath_from("../Documents")    # None
 			```
 		"""
 		self._validate()
 		if not isinstance(origin, GPath):
-			origin = GPath(origin)
+			origin = GPath(origin, encoding=self._encoding)
 
-		if origin._absolute:
-			common = GPath.find_common(self, origin)
+		if origin._root:
+			common = self.common_with(origin)
 			if common is None:
 				return None
 
-			new_path = GPath()
-			new_path._parent = len(origin) - len(common)
+			new_path = GPath(self)
+			new_path._parent_level = len(origin) - len(common)
 			new_path._parts = self._parts[len(common):]
+			new_path._drive = ""
+			new_path._root = False
 			return new_path
 
 		else:
-			common = GPath.find_common(self, origin, allow_current=True, allow_parents=True)
+			common = self.common_with(origin, allow_current=True, allow_parents=True)
 			if common is None:
 				return None
-			if common._parent > self._parent:
+			if common._parent_level > self._parent_level:
 				return None  # Path from common to self's parent cannot be known
 
 			# common._dotdot == self._dotdot
 			# origin._dotdot <= self._dotdot
 
-			new_path = GPath()
+			new_path = GPath(self)
+			new_path._drive = ""
+			new_path._root = False
 			if len(common) == 0:
-				if origin._parent == self._parent:
-					new_path._parent = len(origin)
+				if origin._parent_level == self._parent_level:
+					new_path._parent_level = len(origin)
 				else:
-					new_path._parent = (common._parent - origin._parent) + len(origin)
+					new_path._parent_level = (common._parent_level - origin._parent_level) + len(origin)
 				new_path._parts = self._parts
 			else:
-				new_path._parent = len(origin) - len(common)
+				new_path._parent_level = len(origin) - len(common)
 				new_path._parts = self._parts[len(common):]
 
 			return new_path
 
 
 	def __hash__(self) -> int:
 		"""
 			Calculate hash of the GPath object.
 
 			Usage: <code>hash(<var>g</var>)</code>
 		"""
-		return hash((tuple(self._parts), self._device, self._absolute, self._parent))
+		return hash(self._tuple)
 
 
-	def __eq__(self, other: Any) -> bool:
+	def __eq__(self, other: GPathLike) -> bool:
 		"""
 			Check if two GPaths are completely identical.
 
 			Always return False if `other` is not a GPath object, even if it is a GPath-like object.
 
 			Usage: <code><var>g1</var> == <var>g2</var></code>
 
 			Examples
 			--------
 			```python
 			GPath("/usr/bin") == GPath("/usr/bin")  # True
 			GPath("/usr/bin") == GPath("usr/bin")   # False
 			GPath("C:/") == GPath("D:/")            # False
-			GPath("/usr/bin") == "/usr/bin"         # False
-			```
-		"""
-		if isinstance(other, GPath):
-			return ((self._absolute, self._device, self._parent) + self._parts) == ((other._absolute, other._device, other._parent) + other._parts)
-		else:
-			return False
-
-
-	def __lt__(self, other: GPathLike) -> bool:
-		"""
-			Check if `self` should be collated before `other` by comparing them in component-wise lexicographical order.
-
-			Absolute paths come before (is less than) parent relative paths, which come before (is less than) non-parent relative paths. Between two parent relative paths, the path with the higher parent level comes first (is lesser).
-
-			Usage: <code><var>self</var> < <var>other</var></code>
-
-			Examples
-			--------
-			```python
-			GPath("/") < GPath("C:/")      # True
-			GPath("C:/") < GPath("../..")  # True
-			GPath("../..") < GPath("..")   # True
-			GPath("..") < GPath("")        # True
-			GPath("/") < GPath("/usr")     # True
 			```
 		"""
 		if not isinstance(other, GPath):
-			other = GPath(other)
-		return ((not self._absolute, self._device, -1 * self._parent) + self._parts) < ((not other._absolute, other._device, -1 * other._parent) + other._parts)
+			other = GPath(other, encoding=self._encoding)
+		return self._tuple == other._tuple
 
 
 	def __bool__(self) -> bool:
 		"""
 			Truthy if `self` is an absolute path, if `self` is relative to a parent directory, or if `self` has at least one named component.
 
 			Usage: <code>bool(<var>g</var>)</code>, <code>not <var>g</var></code>, or <code>if <var>g</var>:</code>
@@ -637,51 +810,62 @@
 			```python
 			bool(GPath("/"))    # True
 			bool(GPath(".."))   # True
 			bool(GPath("doc"))  # True
 			bool(GPath(""))     # False
 			```
 		"""
-		return self._absolute or self._parent != 0 or len(self._parts) > 0
+		return self._root or self._drive != "" or self._parent_level != 0 or len(self._parts) > 0
 
 
 	def __str__(self) -> str:
 		"""
 			Return a string representation of the path.
 
 			Usage: <code>str(<var>g</var>)</code>
 		"""
-		return GPath.separator.join(self.get_parts())
+		if bool(self):
+			if self.root and self._drive == "":
+				return _rules.generic_rules.roots[0]
+			else:
+				return (self._drive + _rules.generic_rules.drive_postfixes[0] if self._drive != "" else "") + (_rules.generic_rules.roots[0] if self._root else "") + _rules.generic_rules.separators[0].join(self.relative_parts)
+		else:
+			return _rules.generic_rules.current_indicators[0]
 
 
 	def __repr__(self) -> str:
 		"""
 			Return a string that, when printed, gives the Python code associated with instantiating the GPath object.
 
 			Usage: <code>repr(<var>g</var>)</code>
 		"""
+		if self._encoding is None:
+			encoding_repr = ""
+		else:
+			encoding_repr = f", encoding={repr(self._encoding)}"
+
 		if bool(self):
-			return f"GPath({repr(str(self))})"
+			return f"GPath({repr(str(self))}{encoding_repr})"
 		else:
-			return f"GPath({repr('')})"
+			return f"GPath({repr('')}{encoding_repr})"
 
 
 	def __len__(self) -> int:
 		"""
 			Get the number of named path components, excluding any device name or parent directories.
 
 			Usage: <code>len(<var>g</var>)</code>
 
 			Examples
 			--------
 			```python
-			len(GPath("/usr/bin"))   # 2
-			len(GPath("/"))          # 0
-			len(GPath("C:/Windows))  # 0
-			len(GPath("C:/))         # 0
+			len(GPath("/usr/bin"))    # 2
+			len(GPath("/"))           # 0
+			len(GPath("C:/Windows"))  # 0
+			len(GPath("C:/"))         # 0
 			```
 		"""
 		return len(self._parts)
 
 
 	def __getitem__(self, index: Union[int, slice]) -> Union[str, list[str]]:
 		"""
@@ -727,64 +911,71 @@
 			GPath("/usr/local/bin") in GPath("/usr")  # True
 			GPath("/usr/local/bin") in GPath("/bin")  # False
 			GPath("..") in GPath("../..")             # True
 			GPath("..") in GPath("C:/")               # False
 			```
 		"""
 		if not isinstance(other, GPath):
-			other = GPath(other)
+			other = GPath(other, encoding=self._encoding)
 
-		common_path = GPath.find_common(self, other, allow_current=True, allow_parents=True)
+		common_path = self.common_with(other, allow_current=True, allow_parents=True)
 		return common_path is not None and common_path == self
 
 
 	def __add__(self, other: GPathLike) -> GPath:
 		"""
-			Add (concatenate) `other` to the end of `self` if `other` is a relative path, and return a new copy.
+			Add (concatenate) `other` to the end of `self`, and return a new copy.
+
+			If `other` is an absolute path, the returned path will be an absolute path that matches `other`, apart from the device name.
 
-			If `other` is an absolute path, or if `other` has a different device name, return an unchanged copy of `self`.
+			If `other` has a device name, the returned path will have the same device name as `other`. Otherwise, the returned path will have the same device name as `self`. If neither has a device name, the returned path will not have a device name as well.
 
-			Alias: `__div__()`
+			Alias: `__truediv__()`
 
 			Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var> / <var>other</var></code>
 
 			Raises `ValueError` if either GPath is invalid
 
 			Examples
 			--------
 			```python
 			GPath("/usr") + GPath("local/bin")                   # GPath("/usr/local/bin")
 			GPath("C:/Windows/System32") + GPath("../SysWOW64")  # GPath("C:/Windows/SysWOW64")
+			GPath("C:/Windows/System32") + GPath("/usr/bin")     # GPath("C:/usr/bin")
 			GPath("..") + GPath("../..")                         # GPath("../../..")
 			GPath("..") / GPath("../..")                         # GPath("../../..")
 			```
 		"""
 		if isinstance(other, GPath):
 			other._validate
 		else:
-			other = GPath(other)
+			other = GPath(other, encoding=self._encoding)
 
-		if other._absolute:
-			return GPath(self)
-		elif other._device != None and other._device != "" and self._device != other._device:
-			return GPath(self)
+		new_path = GPath(self)
+		if other._root:
+			new_path._parts = other._parts
+			new_path._root = other._root
+			new_path._parent_level = other._parent_level
 		else:
-			new_path = GPath(self)
 			new_parts = [part for part in self._parts]
-			for i in range(other._parent):
+			for i in range(other._parent_level):
 				if len(new_parts) > 0:
 					new_parts.pop()
-				elif not new_path._absolute:
-					new_path._parent += 1
+				elif not new_path._root:
+					new_path._parent_level += 1
 				else:
 					pass  # parent of directory of root is still root
 
 			new_parts.extend(other._parts)
 			new_path._parts = tuple(new_parts)
-			return new_path
+
+		if other._drive != "":
+			new_path._drive = other._drive
+
+		return new_path
 
 
 	def __sub__(self, n: int) -> GPath:
 		"""
 			Remove `n` components from the end of the path and return a new copy.
 
 			Usage: <code><var>self</var> - <var>n</var></code>
@@ -797,23 +988,23 @@
 			GPath("C:/Windows/System32") - 1  # GPath("C:/Windows")
 			GPath("/usr/bin") - 2             # GPath("/")
 			GPath("Documents") - 3            # GPath("..")
 			GPath("/") - 1                    # GPath("/")
 			```
 		"""
 		if n < 0:
-			raise ValueError("cannot subtract a negative number of components from the path; use __add__() instead")
+			raise ValueError("cannot subtract a negative number of components from the path: {n}; use __add__() instead")
 
 		new_path = GPath(self)
 		new_parts = [part for part in self._parts]
 		for i in range(n):
 			if len(new_parts) > 0:
 				new_parts.pop()
-			elif not new_path._absolute:
-				new_path._parent += 1
+			elif not new_path._root:
+				new_path._parent_level += 1
 			else:
 				pass  # removing components from root should still give root
 		new_path._parts = tuple(new_parts)
 		return new_path
 
 
 	def __mul__(self, n: int) -> GPath:
@@ -833,28 +1024,39 @@
 			```python
 			GPath("/usr/bin") * 2    # GPath("/usr/bin/usr/bin")
 			GPath("../docs") * 2     # GPath("../../docs/docs")
 			GPath("C:/Windows") * 0  # GPath("C:/")
 			```
 		"""
 		if n < 0:
-			raise ValueError("cannot multiply path by a negative integer")
+			raise ValueError("cannot multiply path by a negative integer: {n}")
 		new_path = GPath(self)
-		new_path._parent = self._parent * n
+		new_path._parent_level = self._parent_level * n
 		new_path._parts = self._parts * n
 		return new_path
 
 
-	def __div__(self, other: GPathLike) -> GPath:
+	def __truediv__(self, other: GPathLike) -> GPath:
 		"""
 			Alias of `__add__()`.
+
+			Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var> / <var>other</var></code>
 		"""
 		return self.__add__(other)
 
 
+	def __and__(self, other: GPathLike) -> Union[GPath, None]:
+		"""
+			Equivalent to `self.common_with(other)`, using the default options of `common_with()`.
+
+			Usage: <code><var>g1</var> & <var>g2</var></code>
+		"""
+		return self.common_with(other)
+
+
 	def __lshift__(self, n: int) -> GPath:
 		"""
 			Move the imaginary current working directory `n` steps up the filesystem tree.
 
 			If `self` is a relative path, remove up to `n` levels of parent directories from the start of the path and return a copy. If it is an absolute path, return a copy of `self` unchanged.
 
 			If `n` is negative, this is equivalent to `__rshift__(-n)`.
@@ -870,16 +1072,16 @@
 			GPath("../doc") << 2               # GPath("doc")
 			GPath("/usr/bin") << 2             # GPath("/usr/bin")
 			```
 		"""
 		if n < 0:
 			return self.__rshift__(-1 * n)
 		new_path = GPath(self)
-		if not new_path._absolute:
-			new_path._parent = max(new_path._parent - n, 0)
+		if not new_path._root:
+			new_path._parent_level = max(new_path._parent_level - n, 0)
 		return new_path
 
 
 	def __rshift__(self, n: int) -> GPath:
 		"""
 			Move the imaginary current working directory `n` steps down the filesystem tree.
 
@@ -897,26 +1099,36 @@
 			GPath("../SysWOW64/drivers") >> 1  # GPath("../../SysWOW64/drivers")
 			GPath("/usr/bin") >> 2             # GPath("/usr/bin")
 			```
 		"""
 		if n < 0:
 			return self.__lshift__(-1 * n)
 		new_path = GPath(self)
-		if not new_path._absolute:
-			new_path._parent += n
+		if not new_path._root:
+			new_path._parent_level += n
 		return new_path
 
+
+	@property
+	def _tuple(self) -> tuple:
+		# Get a tuple of all fields
+		return (
+			self._root,
+			self._drive,
+			self._parent_level,
+			self._parts,
+			self._encoding,
+		)
+
+
 	def _validate(self) -> bool:
 		# Check if self is in a valid state
-		if self._parent < 0:
+		if self._parent_level < 0:
 			raise ValueError(f"invalid GPath, _parent cannot be negative: {repr(self)}")
-		if self._absolute:
-			if self._parent != 0:
+		if self._root:
+			if self._parent_level != 0:
 				raise ValueError(f"invalid GPath, _parent must be 0 when root is True: {repr(self)}")
-		else:
-			if self._device != "" and self._device is not None:
-				raise ValueError(f"invalid GPath, _device must be unset when root is False: {repr(self)}")
 		return True
 
 
-GPathLike = Union[GPath, PathLike]
-"""Union type of GPath-like objects that can be used as the argument for most GPath methods."""
+GPathLike = Union[GPath, str, bytes, os.PathLike]
+"""Union type of GPath-like objects that can be used as the argument for most `GPath` methods."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `generic-path-0.3/pyproject.toml` & `generic-path-0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "generic-path"  # "gpath" is taken on PyPI, and "g-path" is too similar
 dynamic = ["version", "readme"]
 authors = [
 	{name = "Yu Shiyang", email = "yu.shiyang@gnayihs.uy"}
 ]
-description = "GPath provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system."
+description = "Generalised abstract file path that provides path manipulations independent from the local environment"
 license = {text = "MPL-2.0"}
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Intended Audience :: Developers",
 	"Intended Audience :: System Administrators",
 	"License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 	"Operating System :: OS Independent",
@@ -31,32 +31,33 @@
 requires-python = ">=3.7"
 dependencies = []
 
 [project.optional-dependencies]
 dev = ["pytest ~= 7.3.1", "coverage ~= 7.2.3", "pdoc ~= 13.1.1", "pyroma ~= 4.2", "build ~= 0.10.0", "tox ~= 4.5.1", "tox-extras >= 0.0.1"]
 test = ["pytest ~= 7.3.1", "coverage ~= 7.2.3"]
 docs = ["pdoc ~= 13.1.1"]
-config = ["pyroma ~= 4.2"]
+metadata = ["pyroma ~= 4.2"]
 package = ["build ~= 0.10.0"]
 packagetest = ["twine ~= 4.0.2"]
 ci = ["tox ~= 4.5.1", "tox-extras >= 0.0.1"]
 publish = ["twine ~= 4.0.2"]
 
 [project.urls]
 # key is used verbatim on PyPI
 Homepage = "https://github.com/yushiyangk/GPath"
 Documentation = "https://gpath.gnayihs.uy/"
 Issues = "https://github.com/yushiyangk/GPath/issues"
 
 [tool.pytest.ini_options]
 addopts = "tests"
 
-[tool.coverage.report]
-include = ["gpath.py"]
+[tool.coverage.run]
+source_pkgs = ["gpath"]
 
-[tool.setuptools]
-packages = []
-py-modules = ["gpath"]
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["*"]
+namespaces = false
 
 [tool.setuptools.dynamic]
 version = {attr = "gpath.__version__"}
 readme = {file = ["README.md", "CHANGELOG.md"], content-type = "text/markdown"}
```

### Comparing `generic-path-0.3/tests/test_gpath.py` & `generic-path-0.4/tests/test_gpath.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
+import itertools
+import os
+
 import pytest
 
 from gpath import GPath
 
-
-# Type hinting prior to 3.10
-# Using generics in built-in collections, e.g. list[int], is supported from 3.7 by __future__.annotations
-from typing import Optional, Union
+from gpath._compat import Optional, Union
 
 
 class TestGPath:
 
 	@pytest.fixture
 	def gpath1(self, request: pytest.FixtureRequest) -> GPath:
 		return GPath(request.param)
@@ -25,80 +25,83 @@
 		if request.param is None:
 			return None
 		else:
 			return GPath(request.param)
 
 
 	@pytest.mark.parametrize(
-		('path', 'expected_parts', 'expected_device', 'expected_absolute', 'expected_parent'),
+		('path', 'expected_parts', 'expected_drive', 'expected_root', 'expected_parent_level'),
 		[
 			(None, tuple(), "", False, 0),
 			("", tuple(), "", False, 0),
 			(".", tuple(), "", False, 0),
 			("./", tuple(), "", False, 0),
 			("./.", tuple(), "", False, 0),
 			(".//", tuple(), "", False, 0),
 			("/", tuple(), "", True, 0),
 			("/.", tuple(), "", True, 0),
 			("/..", tuple(), "", True, 0),
 			("/./", tuple(), "", True, 0),
 			("/./.", tuple(), "", True, 0),
 			("/.//", tuple(), "", True, 0),
 			("/./..", tuple(), "", True, 0),
-			("C:/", tuple(), "C:", True, 0),
-			("C:/.", tuple(), "C:", True, 0),
-			("c:/", tuple(), "c:", True, 0),
+			("C:/", tuple(), "C", True, 0),
+			("C:/.", tuple(), "C", True, 0),
+			("C:/./.", tuple(), "C", True, 0),
+			("C:/.//", tuple(), "C", True, 0),
+			("C:", tuple(), "C", False, 0),
+			("C:.", tuple(), "C", False, 0),
+			("C:./.", tuple(), "C", False, 0),
+			("C:.//", tuple(), "C", False, 0),
+			("c:/", tuple(), "c", True, 0),
+			("c:", tuple(), "c", False, 0),
 		]
 	)
 	def test_constructor_root(self,
 		path: Optional[str],
 		expected_parts: tuple[str, ...],
-		expected_device: str,
-		expected_absolute: bool,
-		expected_parent: int,
+		expected_drive: str,
+		expected_root: bool,
+		expected_parent_level: int,
 	):
 		"""
-			Test constructor `__init__()` as well as getters `is_absolute()`, `get_device()`, `get_parent_parts()`, `get_parent_level()`, but not `get_parts()`, for paths requiring special treatment.
+			Test constructor `__init__()` as well as property getters for `absolute`, `drive`, `named_parts` and `parent_level`, for paths requiring special treatment.
 		"""
 		if path is None:
 			gpath = GPath()
 		else:
 			gpath = GPath(path)
 
-		if expected_absolute and expected_parent > 0:
-			expected_parent = 0
+		if expected_root and expected_parent_level > 0:
+			expected_parent_level = 0
 
 		assert gpath._parts == expected_parts
-		assert gpath._device == expected_device
-		assert gpath._absolute == expected_absolute
-		assert gpath._parent == expected_parent
-
-		assert gpath.is_absolute() == expected_absolute
-		assert gpath.get_device() == expected_device
-		assert gpath.get_parent_level() == expected_parent
+		assert gpath._drive == expected_drive
+		assert gpath._root == expected_root
+		assert gpath._parent_level == expected_parent_level
+
+		assert gpath.absolute == expected_root
+		assert gpath.drive == expected_drive
+		assert gpath.named_parts == list(expected_parts)
+		assert gpath.parent_level == expected_parent_level
 
 		gpath_copy = GPath(gpath)
 		assert gpath_copy._parts == expected_parts
-		assert gpath_copy._device == expected_device
-		assert gpath_copy._absolute == expected_absolute
-		assert gpath_copy._parent == expected_parent
-
-		assert gpath_copy.is_absolute() == expected_absolute
-		assert gpath_copy.get_device() == expected_device
-		assert gpath_copy.get_parent_level() == expected_parent
+		assert gpath_copy._drive == expected_drive
+		assert gpath_copy._root == expected_root
+		assert gpath_copy._parent_level == expected_parent_level
 
-		expected_parent_parts = []
-		for i in range(expected_parent):
-			expected_parent_parts.append("..")
-		assert gpath.get_parent_parts() == expected_parent_parts
-		assert gpath_copy.get_parent_parts() == expected_parent_parts
+		assert gpath_copy.absolute == expected_root
+		assert gpath_copy.drive == expected_drive
+		assert gpath_copy.named_parts == list(expected_parts)
+		assert gpath_copy.parent_level == expected_parent_level
 
 
 	@pytest.mark.parametrize(
-		('path', 'expected_parts', 'expected_parent'),
+		('path', 'expected_parts', 'expected_parent_level'),
 		[
 			("..", tuple(), 1),
 			("../..", tuple(), 2),
 			("bin", ("bin", ), 0),
 			("usr/bin", ("usr", "bin"), 0),
 			("../usr/bin", ("usr", "bin"), 1),
 			("../../usr/bin", ("usr", "bin"), 2),
@@ -120,134 +123,144 @@
 			("directory/русский язык", ("directory", "русский язык"), 0),
 			("directory/中文", ("directory", "中文"), 0),
 			("directory/اَلْعَرَبِيَّةُ", ("directory", "اَلْعَرَبِيَّةُ"), 0),
 		]
 	)
 	@pytest.mark.parametrize('path_suffix', ["", "/", "//", "/.", "/./", "/././/"])
 	@pytest.mark.parametrize(
-		('path_prefix', 'expected_device', 'expected_absolute'),
+		('path_prefix', 'expected_drive', 'expected_root'),
 		[
 			("", "", False),
 			("/", "", True),
 			#("//", "", True),
-			("C:/", "C:", True),
-			("c:/", "c:", True),
-			#("C:", "C:", False),
+			("C:/", "C", True),
+			("c:/", "c", True),
+			("C:", "C", False),
+			("1:", "1", False),
+			("::", ":", False),
 		]
 	)
 	def test_constructor(self,
 		path: str,
 		path_prefix: str,
 		path_suffix: str,
 		expected_parts: tuple[str, ...],
-		expected_device: str,
-		expected_absolute: bool,
-		expected_parent: int,
+		expected_drive: str,
+		expected_root: bool,
+		expected_parent_level: int,
 	):
 		"""
-			Test constructor `__init__()` as well as getters `is_absolute()`, `get_device()`, `get_parent_parts()`, `get_parent_level()`, but not `get_parts()`.
+			Test constructor `__init__()` as well as property getters for `absolute`, `device`, `named_parts` and `parent_level`.
 		"""
 		gpath = GPath(path_prefix + path + path_suffix)
-		if expected_absolute and expected_parent > 0:
-			expected_parent = 0
+		if expected_root and expected_parent_level > 0:
+			expected_parent_level = 0
 
 		assert gpath._parts == expected_parts
-		assert gpath._device == expected_device
-		assert gpath._absolute == expected_absolute
-		assert gpath._parent == expected_parent
-
-		assert gpath.is_absolute() == expected_absolute
-		assert gpath.get_device() == expected_device
-		assert gpath.get_parent_level() == expected_parent
+		assert gpath._drive == expected_drive
+		assert gpath._root == expected_root
+		assert gpath._parent_level == expected_parent_level
+
+		assert gpath.absolute == expected_root
+		assert gpath.drive == expected_drive
+		assert gpath.named_parts == list(expected_parts)
+		assert gpath.parent_level == expected_parent_level
 
 		gpath_copy = GPath(gpath)
 
 		assert gpath_copy._parts == expected_parts
-		assert gpath_copy._device == expected_device
-		assert gpath_copy._absolute == expected_absolute
-		assert gpath_copy._parent == expected_parent
-
-		assert gpath_copy.is_absolute() == expected_absolute
-		assert gpath_copy.get_device() == expected_device
-		assert gpath_copy.get_parent_level() == expected_parent
-
-		expected_parent_parts = []
-		for i in range(expected_parent):
-			expected_parent_parts.append("..")
-		assert gpath.get_parent_parts() == expected_parent_parts
-		assert gpath_copy.get_parent_parts() == expected_parent_parts
-
-
-	@pytest.mark.parametrize(
-		('gpath1', 'parts'),
-		[
-			("/", ["", ""]),
-			("/a", ["", "a"]),
-			("/a/b", ["", "a", "b"]),
-			("", ["."]),
-			("a", ["a"]),
-			("a/b", ["a", "b"]),
-			("..", [".."]),
-			("../a", ["..", "a"]),
-			("../a/b", ["..", "a", "b"]),
-			("../..", ["..", ".."]),
-			("../../a", ["..", "..", "a"]),
-			("../../a/b", ["..", "..", "a", "b"]),
-			("C:/", ["C:", ""]),
-			("C:/a", ["C:", "a"]),
-			("C:/a/b", ["C:", "a", "b"]),
-		],
-		indirect=['gpath1']
-	)
-	def test_get_parts_from_parts(self, gpath1: GPath, parts: list[str]):
-		"""
-			Test `get_parts()` and `from_parts()`.
-		"""
-		result = gpath1.get_parts()
-		assert result == parts
-
-		result = GPath.from_parts(parts)
-		assert result == gpath1
+		assert gpath_copy._drive == expected_drive
+		assert gpath_copy._root == expected_root
+		assert gpath_copy._parent_level == expected_parent_level
+
+		assert gpath_copy.absolute == expected_root
+		assert gpath_copy.drive == expected_drive
+		assert gpath_copy.named_parts == list(expected_parts)
+		assert gpath_copy.parent_level == expected_parent_level
 
 
 	@pytest.mark.parametrize(
 		('gpath1', 'expected'),
 		[
 			("/", True),
 			("", False),
 			("..", False),
 			("C:/", True),
+			("C:", False),
+			("C:..", False),
 			("/a", False),
 			("a", False),
 			("../a", False),
 			("C:/a", False),
+			("C:a", False),
+			("C:../a", False),
 		],
 		indirect=['gpath1']
 	)
-	def test_is_root(self, gpath1: GPath, expected: bool):
+	def test_root(self, gpath1: GPath, expected: bool):
 		"""
-			Test `is_root()`.
+			Test property getter for `root`.
 		"""
-		result = gpath1.is_root()
+		result = gpath1.root
 		assert result == expected
 
 
 	@pytest.mark.parametrize(
+		('gpath1', 'expected_parent_parts', 'expected_relative_parts'),
+		[
+			("/", [], []),
+			("/a", [], ["a"]),
+			("/a/b", [], ["a", "b"]),
+			("", [], []),
+			("a", [], ["a"]),
+			("a/b", [], ["a", "b"]),
+			("..", [".."], [".."]),
+			("../a", [".."], ["..", "a"]),
+			("../a/b", [".."], ["..", "a", "b"]),
+			("../..", ["..", ".."], ["..", ".."]),
+			("../../a", ["..", ".."], ["..", "..", "a"]),
+			("../../a/b", ["..", ".."], ["..", "..", "a", "b"]),
+			("C:/", [], []),
+			("C:/a", [], ["a"]),
+			("C:/a/b", [], ["a", "b"]),
+			("C:", [], []),
+			("C:a", [], ["a"]),
+			("C:a/b", [], ["a", "b"]),
+			("C:..", [".."], [".."]),
+			("C:../a", [".."], ["..", "a"]),
+			("C:../a/b", [".."], ["..", "a", "b"]),
+			("C:../..", ["..", ".."], ["..", ".."]),
+			("C:../../a", ["..", ".."], ["..", "..", "a"]),
+			("C:../../a/b", ["..", ".."], ["..", "..", "a", "b"]),
+		],
+		indirect=['gpath1']
+	)
+	def test_parent_relative_parts(self, gpath1: GPath, expected_parent_parts: list[str], expected_relative_parts: list[str]):
+		"""
+			Test property getters for `parent_parts` and `relative_parts`.
+		"""
+		assert gpath1.parent_parts == expected_parent_parts
+		assert gpath1.relative_parts == expected_relative_parts
+
+
+	@pytest.mark.parametrize(
 		('path1', 'path2', 'expected'),
 		[
 			("/", "/", True),
 			("", "", True),
 			("..", "..", True),
 			("C:/", "C:/", True),
+			("C:", "C:", True),
 			("/", "", False),
 			("..", "", False),
 			("..", "/", False),
 			("..", "../..", False),
 			("C:/", "c:/", False),
 			("C:/", "D:/", False),
+			("C:/", "C:", False),
 			("/usr/bin", "/usr/bin", True),
 			("/usr/bin", "/usr/./bin", True),
 			("usr/bin", "usr/bin", True),
 			("usr/bin", "usr/./bin", True),
 			("/usr/bin", "/../usr/bin", True),
 			("usr/bin", "../usr/bin", False),
 			("../usr/bin", "../usr/bin", True),
@@ -276,129 +289,39 @@
 		gpath2 = GPath(path2)
 		result = gpath1 == gpath2
 		assert result == expected
 		result = gpath2 == gpath1
 		assert result == expected
 
 		result = gpath1 == path2
-		assert result == False
+		assert result == expected
 		result = gpath2 == path1
-		assert result == False
+		assert result == expected
 
 		if expected is True:
 			assert hash(gpath1) == hash(gpath2)
 		else:
 			assert hash(gpath1) != hash(gpath2)
 
 
 	@pytest.mark.parametrize(
-		('gpath1', 'gpath2', 'gt_expected', 'eq_expected'),
-		[
-			("/", "/", False, True),
-			("/a/b", "/a/b", False, True),
-			("", "", False, True),
-			("a/b", "a/b", False, True),
-			("..", "..", False, True),
-			("../..", "../..", False, True),
-			("../../a/b", "../../a/b", False, True),
-			("C:/", "C:/", False, True),
-			("C:/a/b", "C:/a/b", False, True),
-
-			("", "/", True, False),
-			("", "..", True, False),
-			("..", "/", True, False),
-			("..", "../..", True, False),
-			("C:/", "/", True, False),
-			("", "C:/", True, False),
-			("..", "C:/", True, False),
-
-			("b", "a", True, False),
-			("aa", "a", True, False),
-			("a", "", True, False),
-			("a", "..", True, False),
-			("a", "/", True, False),
-			("a/b", "a/a", True, False),
-			("b/a", "a/b", True, False),
-
-			("/b", "/a", True, False),
-			("/aa", "/a", True, False),
-			("/a", "/", True, False),
-			("", "/a", True, False),
-			("..", "/a", True, False),
-			("/a/b", "/a/a", True, False),
-			("/b/a", "/a/b", True, False),
-
-			("../b", "../a", True, False),
-			("../aa", "../a", True, False),
-			("../a", "..", True, False),
-			("../a", "/", True, False),
-			("", "../a", True, False),
-			("../a/b", "../a/a", True, False),
-			("../b/a", "../a/b", True, False),
-			("../a", "../../b", True, False),
-
-			("D:/", "C:/", True, False),
-			("CC:/", "C:/", True, False),
-			("C:/b", "C:/a", True, False),
-			("C:/aa", "C:/a", True, False),
-			("C:/a", "C:/", True, False),
-			("D:/", "C:/a", True, False),
-			("C:/a", "/", True, False),
-			("", "C:/a", True, False),
-			("..", "C:/a", True, False),
-			("C:/a/b", "C:/a/a", True, False),
-			("C:/b/a", "C:/a/b", True, False),
-		],
-		indirect=['gpath1', 'gpath2']
-	)
-	def test_gt_lt_gte_lte(self, gpath1: GPath, gpath2: GPath, gt_expected: bool, eq_expected: bool):
-		"""
-			Test `__gt__()`, `__lt__()`, `__gte__()` and `__lte__()`, which are automatically generated based on the definition of `__gt__()` (and `__eq__()`).
-		"""
-		lt_expected = ((not gt_expected) and (not eq_expected))
-		gte_expected = gt_expected or eq_expected
-		lte_expected = lt_expected or eq_expected
-
-		result = gpath1 == gpath2
-		assert result == eq_expected
-
-		result = gpath1 > gpath2
-		assert result == gt_expected
-		result = gpath2 < gpath1
-		assert result == gt_expected
-
-		result = gpath2 > gpath1
-		assert result == lt_expected
-		result = gpath1 < gpath2
-		assert result == lt_expected
-
-		result = gpath1 >= gpath2
-		assert result == gte_expected
-		result = gpath2 <= gpath1
-		assert result == gte_expected
-
-		result = gpath2 >= gpath1
-		assert result == lte_expected
-		result = gpath1 <= gpath2
-		assert result == lte_expected
-
-
-	@pytest.mark.parametrize(
 		('gpath1', 'expected'),
 		[
 			("/", True),
 			("", False),
 			("..", True),
 			("../..", True),
 			("C:/", True),
+			("C:", True),
 
 			("/a", True),
 			("a", True),
 			("../a", True),
 			("C:/a", True),
+			("C:a", True),
 		],
 		indirect=['gpath1']
 	)
 	def test_bool(self, gpath1: GPath, expected: bool):
 		"""
 			Test `__bool__()`.
 		"""
@@ -407,58 +330,82 @@
 		result = not gpath1
 		assert result == (not expected)
 
 
 	@pytest.mark.parametrize(
 		('path'),
 		[
-			("/"),
 			("."),
 			(".."),
 			("../.."),
 			("C:/"),
+			("C:"),
 			("/a"),
 			("/a/b"),
 			("a"),
 			("a/b"),
 			("../a"),
 			("../a/b"),
 			("C:/a"),
 			("C:/a/b"),
+			("C:a"),
+			("C:a/b"),
 		]
 	)
 	def test_str_repr(self, path: str):
 		"""
-			Test `__str__()` and `__repr__()`.
+			Test `__str__()` and `__repr__()` for cross-platform outputs.
 		"""
 		gpath = GPath(path)
 		result = str(gpath)
 		assert result == path
 
 		result = repr(gpath)
 		result_eval = eval(result)
 		assert result_eval == gpath
 
 
 	@pytest.mark.parametrize(
+		('path', 'expected'),
+		[
+			("/", {'posix': "/", 'nt': "/", 'java': "/"}),
+		]
+	)
+	def test_str_repr_platform(self, path: str, expected: dict[str, str]):
+		"""
+			Test `__str__()` and `__repr__()` for platform-dependent outputs.
+		"""
+		gpath = GPath(path)
+		result = str(gpath)
+		assert result == expected[os.name]
+
+		result = repr(gpath)
+		result_eval = eval(result)
+		assert result_eval == gpath
+
+
+	@pytest.mark.parametrize(
 		('gpath1', 'expected'),
 		[
 			("/", 0),
 			("", 0),
 			("..", 0),
 			("../..", 0),
 			("C:/", 0),
+			("C:", 0),
 			("/a", 1),
 			("/a/b", 2),
 			("a", 1),
 			("a/b", 2),
 			("../a", 1),
 			("../a/b", 2),
 			("C:/a", 1),
 			("C:/a/b", 2),
+			("C:a", 1),
+			("C:a/b", 2),
 		],
 		indirect=['gpath1']
 	)
 	def test_len(self, gpath1: GPath, expected: int):
 		"""
 			Test `__len__()`.
 		"""
@@ -478,14 +425,16 @@
 			("/a/b", ["a", "b"]),
 			("a", ["a"]),
 			("a/b", ["a", "b"]),
 			("../a", ["a"]),
 			("../a/b", ["a", "b"]),
 			("C:/a", ["a"]),
 			("C:/a/b", ["a", "b"]),
+			("C:a", ["a"]),
+			("C:a/b", ["a", "b"]),
 		],
 		indirect=['gpath1']
 	)
 	@pytest.mark.parametrize(
 		('index'),
 		[
 			0, 1, 2, -1, -2, -3,
@@ -519,31 +468,38 @@
 	@pytest.mark.parametrize(
 		('gpath1', 'gpath2', 'expected'),
 		[
 			("/", "", False),
 			("", "/", False),
 			("/", "..", False),
 			("..", "/", False),
-			("C:/", "/", False),
 			("/", "C:/", False),
+			("C:/", "/", False),
+			("/", "C:", False),
+			("C:", "/", False),
+
 			("C:/", "", False),
 			("", "C:/", False),
 			("C:/", "..", False),
 			("..", "C:/", False),
 			("C:/", "D:/", False),
 			("D:/", "C:/", False),
+			("C:/", "C:", False),
+			("C:", "C:/", False),
 
 			("a", "b", False),
 			("b", "a", False),
 			("/a", "/b", False),
 			("/b", "/a", False),
 			("../a", "../b", False),
 			("../b", "../a", False),
 			("C:/a", "C:/b", False),
 			("C:/b", "C:/a", False),
+			("C:a", "C:b", False),
+			("C:b", "C:a", False),
 
 			("..", "", True),
 			("../..", "", True),
 			("../..", "..", True),
 			("", "a", True),
 			("..", "a", True),
 			("../..", "a", True),
@@ -552,19 +508,21 @@
 			("../a", "a", False),
 			("a", "../a", False),
 
 			("a", "a/b", True),
 			("/a", "/a/b", True),
 			("../a", "../a/b", True),
 			("C:/a", "C:/a/b", True),
+			("C:a", "C:a/b", True),
 
 			("a", "a", True),
 			("/a", "/a", True),
 			("../a", "../a", True),
 			("C:/a", "C:/a", True),
+			("C:a", "C:a", True),
 		],
 		indirect=['gpath1', 'gpath2']
 	)
 	def test_contains(self, gpath1: GPath, gpath2: GPath, expected: bool):
 		"""
 			Test `__contains__()`.
 		"""
@@ -579,24 +537,26 @@
 	@pytest.mark.parametrize(
 		('gpath1', 'gpath2', 'subpath_expected', 'relpath_expected'),
 		[
 			("/", "/", "", ""),
 			("/", "", None, None),
 			("/", "..", None, None),
 			("/", "C:/", None, None),
+			("/", "C:", None, None),
 			("/a", "/", "a", "a"),
 			("/a", "/a", "", ""),
 			("/a/b", "/", "a/b", "a/b"),
 			("/a/b", "/a", "b", "b"),
 			("/a/b", "/b", None, "../a/b"),
 
 			("", "/", None, None),
 			("", "", "", ""),
 			("", "..", None, None),
 			("", "C:/", None, None),
+			("", "C:", None, None),
 			("", "a", None, ".."),
 			("", "../a", None, None),
 			("a", "", "a", "a"),
 			("a", "a", "", ""),
 			("a", "..", None, None),
 			("a", "../a", None, None),
 			("a/b", "", "a/b", "a/b"),
@@ -604,14 +564,15 @@
 			("a/b", "b", None, "../a/b"),
 
 			("..", "/", None, None),
 			("..", "", None, ".."),
 			("..", "..", "", ""),
 			("..", "../..", None, None),
 			("..", "C:/", None, None),
+			("..", "C:", None, None),
 			("..", "a", None, "../.."),
 			("..", "../a", None, ".."),
 			("../a", "..", "a", "a"),
 			("../a", "../a", "", ""),
 			("../a", "", None, "../a"),
 			("../a", "a", None, "../../a"),
 			("../a/b", "..", "a/b", "a/b"),
@@ -619,14 +580,15 @@
 			("../a/b", "../b", None, "../a/b"),
 
 			("../..", "/", None, None),
 			("../..", "", None, "../.."),
 			("../..", "..", None, ".."),
 			("../..", "../..", "", ""),
 			("../..", "C:/", None, None),
+			("../..", "C:", None, None),
 			("../..", "a", None, "../../.."),
 			("../..", "../a", None, "../.."),
 			("../..", "../../a", None, ".."),
 			("../../a", "../..", "a", "a"),
 			("../../a", "../../a", "", ""),
 			("../../a", "..", None, "../a"),
 			("../../a", "../a", None, "../../a"),
@@ -637,20 +599,34 @@
 			("../../a/b", "../../b", None, "../a/b"),
 
 			("C:/", "/", None, None),
 			("C:/", "", None, None),
 			("C:/", "..", None, None),
 			("C:/", "C:/", "", ""),
 			("C:/", "D:/", None, None),
+			("C:/", "C:", None, None),
 			("C:/a", "C:/", "a", "a"),
 			("C:/a", "C:/a", "", ""),
 			("C:/a/b", "C:/", "a/b", "a/b"),
 			("C:/a/b", "C:/a", "b", "b"),
 			("C:/a/b", "D:/a", None, None),
 			("C:/a/b", "C:/b", None, "../a/b"),
+
+			("C:", "/", None, None),
+			("C:", "", None, None),
+			("C:", "..", None, None),
+			("C:", "C:/", None, None),
+			("C:", "C:", "", ""),
+			("C:", "D:", None, None),
+			("C:a", "C:", "a", "a"),
+			("C:a", "C:a", "", ""),
+			("C:a/b", "C:", "a/b", "a/b"),
+			("C:a/b", "C:a", "b", "b"),
+			("C:a/b", "D:a", None, None),
+			("C:a/b", "C:b", None, "../a/b"),
 		],
 		indirect=['gpath1', 'gpath2']
 	)
 	def test_subpath_relpath(self, gpath1: GPath, gpath2: GPath, subpath_expected: str, relpath_expected: Union[str, GPath]):
 		"""
 			Test `subpath_from()` and `relpath_from()`.
 		"""
@@ -671,84 +647,94 @@
 			assert relpath_expected_gpath is not None
 
 			if gpath1 != gpath2:
 				result = gpath2.subpath_from(gpath1)
 				assert result == None
 
 		result = gpath1.relpath_from(gpath2)
-		if gpath1._device != "" and result != None:
-			print(result._parts, result._absolute, result._device, result._parent)
 		assert result == relpath_expected_gpath
 
 
 	@pytest.mark.parametrize(
 		('gpath1', 'gpath2', 'expected_gpath'),
 		[
 			("/", "/", "/"),
 			("/", "", "/"),
 			("/", "..", "/"),
-			("/", "C:/", "/"),
+			("/", "C:/", "C:/"),
+			("/", "C:", "C:/"),
 			("/", "a", "/a"),
 			("/", "../a", "/a"),
-			("/a", "/", "/a"),
+			("/a", "/", "/"),
 			("/a", "", "/a"),
 			("/a", "..", "/"),
-			("/a", "C:/", "/a"),
+			("/a", "C:/", "C:/"),
+			("/a", "C:", "C:/a"),
 			("/a", "b", "/a/b"),
 			("/a", "../b", "/b"),
 
-			("", "/", ""),
+			("", "/", "/"),
 			("", "", ""),
 			("", "..", ".."),
-			("", "C:/", ""),
+			("", "C:/", "C:/"),
+			("", "C:", "C:"),
 			("", "a", "a"),
 			("", "../a", "../a"),
-			("a", "/", "a"),
+			("a", "/", "/"),
 			("a", "", "a"),
 			("a", "..", ""),
-			("a", "C:/", "a"),
+			("a", "C:/", "C:/"),
+			("a", "C:", "C:a"),
 			("a", "b", "a/b"),
 			("a", "../b", "b"),
 
-			("..", "/", ".."),
+			("..", "/", "/"),
 			("..", "", ".."),
 			("..", "..", "../.."),
-			("..", "C:/", ".."),
+			("..", "C:/", "C:/"),
+			("..", "C:", "C:.."),
 			("..", "a", "../a"),
 			("..", "../a", "../../a"),
-			("../a", "/", "../a"),
+			("../a", "/", "/"),
 			("../a", "", "../a"),
 			("../a", "..", ".."),
-			("../a", "C:/", "../a"),
+			("../a", "C:/", "C:/"),
+			("../a", "C:", "C:../a"),
 			("../a", "b", "../a/b"),
 			("../a", "../b", "../b"),
 
 			("C:/", "/", "C:/"),
 			("C:/", "", "C:/"),
 			("C:/", "..", "C:/"),
 			("C:/", "C:/", "C:/"),
-			("C:/", "D:/", "C:/"),
+			("C:/", "C:", "C:/"),
+			("C:/", "D:/", "D:/"),
+			("C:/", "D:", "D:/"),
 			("C:/", "a", "C:/a"),
 			("C:/", "../a", "C:/a"),
-			("C:/a", "/", "C:/a"),
+			("C:/a", "/", "C:/"),
 			("C:/a", "", "C:/a"),
 			("C:/a", "..", "C:/"),
-			("C:/a", "C:/", "C:/a"),
-			("C:/a", "D:/", "C:/a"),
+			("C:/a", "C:/", "C:/"),
+			("C:/a", "C:", "C:/a"),
+			("C:/a", "D:/", "D:/"),
+			("C:/a", "D:", "D:/a"),
 			("C:/a", "b", "C:/a/b"),
 			("C:/a", "../b", "C:/b"),
 		],
 		indirect=True
 	)
 	def test_add(self, gpath1: GPath, gpath2: GPath, expected_gpath: GPath):
 		"""
 			Test `__add__()`.
 		"""
 		result = gpath1 + gpath2
 		assert result == expected_gpath
+		result = gpath1 / gpath2
+		assert result == expected_gpath
 
 
 	@pytest.mark.parametrize(
 		('gpath1', 'sub_value', 'expected_gpath'),
 		[
 			("/", 0, "/"),
 			("/", 1, "/"),
@@ -773,28 +759,35 @@
 
 			("C:/", 0, "C:/"),
 			("C:/", 1, "C:/"),
 			("C:/a/b", 0, "C:/a/b"),
 			("C:/a/b", 1, "C:/a"),
 			("C:/a/b", 2, "C:/"),
 			("C:/a/b", 3, "C:/"),
+
+			("C:", 0, "C:"),
+			("C:", 1, "C:.."),
+			("C:a/b", 0, "C:a/b"),
+			("C:a/b", 1, "C:a"),
+			("C:a/b", 2, "C:"),
+			("C:a/b", 3, "C:.."),
 		],
 		indirect=['gpath1', 'expected_gpath']
 	)
 	def test_sub(self, gpath1: GPath, sub_value: int, expected_gpath: GPath):
 		"""
 			Test `__sub__()`.
 		"""
 		result = gpath1 - sub_value
 		assert result == expected_gpath
 
 
 	@pytest.mark.parametrize(
 		('gpath1'),
-		[("/"), ("/a/b"), (""), ("a/b"), (".."), ("../a/b"), ("../.."), ("../../a/b"), ("C:/"), ("C:/a/b")],
+		[("/"), ("/a/b"), (""), ("a/b"), (".."), ("../a/b"), ("../.."), ("../../a/b"), ("C:/"), ("C:/a/b"), ("C:"), ("C:a/b")],
 		indirect=['gpath1']
 	)
 	@pytest.mark.parametrize(('sub_value'), [-1])
 	def test_sub_negative(self, gpath1: GPath, sub_value: int):
 		"""
 			Test `__sub__()` with negative inputs which should give errors.
 		"""
@@ -835,28 +828,35 @@
 
 			("C:/", 1, "C:/"),
 			("C:/", 2, "C:/"),
 			("C:/", 0, "C:/"),
 			("C:/a/b", 1, "C:/a/b"),
 			("C:/a/b", 2, "C:/a/b/a/b"),
 			("C:/a/b", 0, "C:/"),
+
+			("C:", 1, "C:"),
+			("C:", 2, "C:"),
+			("C:", 0, "C:"),
+			("C:a/b", 1, "C:a/b"),
+			("C:a/b", 2, "C:a/b/a/b"),
+			("C:a/b", 0, "C:"),
 		],
 		indirect=['gpath1', 'expected_gpath']
 	)
 	def test_mul(self, gpath1: GPath, mul_value: int, expected_gpath: GPath):
 		"""
 			Test `__mul__()`.
 		"""
 		result = gpath1 * mul_value
 		assert result == expected_gpath
 
 
 	@pytest.mark.parametrize(
 		('gpath1'),
-		[("/"), ("/a/b"), (""), ("a/b"), (".."), ("../a/b"), ("../.."), ("../../a/b"), ("C:/"), ("C:/a/b")],
+		[("/"), ("/a/b"), (""), ("a/b"), (".."), ("../a/b"), ("../.."), ("../../a/b"), ("C:/"), ("C:/a/b"), ("C:"), ("C:a/b")],
 		indirect=['gpath1']
 	)
 	@pytest.mark.parametrize(('mul_value'), [-1, -2])
 	def test_mul_negative(self, gpath1: GPath, mul_value: int):
 		"""
 			Test `__mul__()` with negative inputs which should give errors.
 		"""
@@ -891,14 +891,19 @@
 			("../../a/b", 1, "../a/b", "../../../a/b"),
 			("../../a/b", 2, "a/b", "../../../../a/b"),
 
 			("C:/", 0, "C:/", "C:/"),
 			("C:/", 1, "C:/", "C:/"),
 			("C:/a/b", 0, "C:/a/b", "C:/a/b"),
 			("C:/a/b", 1, "C:/a/b", "C:/a/b"),
+
+			("C:", 0, "C:", "C:"),
+			("C:", 1, "C:", "C:.."),
+			("C:a/b", 0, "C:a/b", "C:a/b"),
+			("C:a/b", 1, "C:a/b", "C:../a/b"),
 		],
 		indirect=['gpath1']
 	)
 	def test_lshift_rshift(self, gpath1: GPath, shift_value: int, lshift_expected: str, rshift_expected: str):
 		"""
 			Test `__lshift__()` and `__rshift__()`.
 		"""
@@ -913,143 +918,256 @@
 		result = gpath1 >> shift_value
 		assert result == rshift_expected_gpath
 		result = gpath1 >> (-1 * shift_value)
 		assert result == lshift_expected_gpath
 
 
 	@pytest.mark.parametrize(
+		('gpath1', 'parent_level', 'expected_gpath'),
+		[
+			("/", None, ""),
+			("/", 0, ""),
+			("/", 2, "../.."),
+			("/a/b", None, "a/b"),
+			("/a/b", 0, "a/b"),
+			("/a/b", 2, "../../a/b"),
+
+			("", None, ""),
+			("", 0, ""),
+			("", 2, "../.."),
+			("a/b", None, "a/b"),
+			("a/b", 0, "a/b"),
+			("a/b", 2, "../../a/b"),
+
+			("..", None, ".."),
+			("..", 0, ""),
+			("..", 2, "../.."),
+			("../a/b", None, "../a/b"),
+			("../a/b", 0, "a/b"),
+			("../a/b", 2, "../../a/b"),
+
+			("C:/", None, "C:"),
+			("C:/", 0, "C:"),
+			("C:/", 2, "C:../.."),
+			("C:/a/b", None, "C:a/b"),
+			("C:/a/b", 0, "C:a/b"),
+			("C:/a/b", 2, "C:../../a/b"),
+
+			("C:", None, "C:"),
+			("C:", 0, "C:"),
+			("C:", 2, "C:../.."),
+			("C:a/b", None, "C:a/b"),
+			("C:a/b", 0, "C:a/b"),
+			("C:a/b", 2, "C:../../a/b"),
+		],
+		indirect=['gpath1', 'expected_gpath']
+	)
+	def test_as_relative(self, gpath1: GPath, parent_level: int, expected_gpath: GPath):
+		"""
+			Test `as_relative()`.
+		"""
+		result = gpath1.as_relative(parent_level)
+		assert result == expected_gpath
+
+
+	@pytest.mark.parametrize(
+		('gpath1', 'expected_gpath'),
+		[
+			("/", "/"),
+			("/a/b", "/a/b"),
+			("", "/"),
+			("a/b", "/a/b"),
+			("..", "/"),
+			("../a/b", "/a/b"),
+			("C:/", "C:/"),
+			("C:/a/b", "C:/a/b"),
+			("C:", "C:/"),
+			("C:a/b", "C:/a/b"),
+		],
+		indirect=['gpath1', 'expected_gpath']
+	)
+	def test_as_absolute(self, gpath1: GPath, expected_gpath: GPath):
+		"""
+			Test `as_absolute()`.
+		"""
+		result = gpath1.as_absolute()
+		assert result == expected_gpath
+
+
+	@pytest.mark.parametrize(
+		('gpath1', 'drive', 'expected_gpath', 'unset_expected'),
+		[
+			("/", "K", "K:/", "/"),
+			("/a/b", "K", "K:/a/b", "/a/b"),
+			("", "K", "K:", ""),
+			("a/b", "K", "K:a/b", "a/b"),
+			("..", "K", "K:..", ".."),
+			("../a/b", "K", "K:../a/b", "../a/b"),
+			("C:/", "K", "K:/", "/"),
+			("C:/a/b", "K", "K:/a/b", "/a/b"),
+			("C:", "K", "K:", ""),
+			("C:a/b", "K", "K:a/b", "a/b"),
+		],
+		indirect=['gpath1', 'expected_gpath']
+	)
+	def test_with_drive(self, gpath1: GPath, drive: str, expected_gpath: GPath, unset_expected: str):
+		"""
+			Test `with_drive()` and `without_drive`.
+		"""
+		result = gpath1.with_drive(drive)
+		assert result == expected_gpath
+
+		unset_expected_gpath = GPath(unset_expected)
+		for unset in ["", None]:
+			result = gpath1.with_drive(unset)
+			assert result == unset_expected_gpath
+		result = gpath1.without_drive()
+		assert result == unset_expected_gpath
+
+
+	@pytest.mark.parametrize(
+		('gpath1'),
+		[
+			("/"),
+			("/a/b"),
+			(""),
+			("a/b"),
+			(".."),
+			("../a/b"),
+			("C:/"),
+			("C:/a/b"),
+			("C:"),
+			("C:a/b"),
+		],
+		indirect=['gpath1']
+	)
+	@pytest.mark.parametrize(('drive'), ["CC", 1, False])
+	def test_with_drive_invalid(self, gpath1: GPath, drive: str):
+		"""
+			Test `with_drive()` when `drive` is longer than one character
+		"""
+		if isinstance(drive, str):
+			with pytest.raises(ValueError):
+				gpath1.with_drive(drive)
+		else:
+			with pytest.raises(TypeError):
+				gpath1.with_drive(drive)
+
+
+
+	@pytest.mark.parametrize(
 		#('path1', 'path2', 'allow_current', 'allow_parents', 'expected_path'),
 		('path1', 'path2', 'allow_current_expected', 'allow_parents_expected', 'allow_current_parent_expected', 'no_common_expected'),
 		[
 			("/", "/", "/", "/", "/", "/"),
 			("/", "", None, None, None, None),
 			("/", "..", None, None, None, None),
 			("/", "C:/", None, None, None, None),
+			("/", "C:", None, None, None, None),
 			("/", "/a", "/", "/", "/", "/"),
 			("/", "a", None, None, None, None),
 			("/", "../a", None, None, None, None),
 			("/a", "/", "/", "/", "/", "/"),
 			("/a", "", None, None, None, None),
 			("/a", "..", None, None, None, None),
 			("/a", "C:/", None, None, None, None),
+			("/a", "C:", None, None, None, None),
 			("/a", "/b", "/", "/", "/", "/"),
 			("/a", "b", None, None, None, None),
 			("/a", "../b", None, None, None, None),
 
 			("", "", "", "", "", ""),
 			("", "..", None, "..", "..", None),
 			("", "C:/", None, None, None, None),
+			("", "C:", None, None, None, None),
 			("", "a", "", "", "", None),
 			("", "../a", None, "..", "..", None),
 			#("a", "", "", "", "", None),
 			("a", "..", None, "..", "..", None),
 			("a", "C:/", None, None, None, None),
+			("a", "C:", None, None, None, None),
 			("a", "b", "", "", "", None),
 			("a", "../b", None, "..", "..", None),
 
 			("..", "..", "..", "..", "..", ".."),
 			("..", "../..", None, "../..", "../..", None),
 			("..", "C:/", None, None, None, None),
+			("..", "C:", None, None, None, None),
 			("..", "../a", "..", "..", "..", ".."),
 			("..", "../../a", None, "../..", "../..", None),
 			("../a", "..", "..", "..", "..", ".."),
 			("../a", "../..", None, "../..", "../..", None),
 			("../a", "C:/", None, None, None, None),
+			("../a", "C:", None, None, None, None),
 			("../a", "../b", "..", "..", "..", ".."),
 			("../a", "../../b", None, "../..", "../..", None),
 
 			("C:/", "C:/", "C:/", "C:/", "C:/", "C:/"),
+			("C:/", "C:", None, None, None, None),
 			("C:/", "D:/", None, None, None, None),
+			("C:/", "D:", None, None, None, None),
 			("C:/a", "C:/", "C:/", "C:/", "C:/", "C:/"),
+			("C:/a", "C:", None, None, None, None),
 			("C:/a", "D:/", None, None, None, None),
+			("C:/a", "D:", None, None, None, None),
 			("C:/a", "C:/b", "C:/", "C:/", "C:/", "C:/"),
 		]
 	)
-	def test_find_common(self,
+	def test_common_with(self,
 		path1: str,
 		path2: str,
 		allow_current_expected: str,
 		allow_parents_expected: str,
 		allow_current_parent_expected: str,
 		no_common_expected: str
 	):
 		"""
-			Test `find_common()`.
+			Test `common_with()` and `__and__()`.
 		"""
 		assert allow_parents_expected == allow_current_parent_expected
 
 		if allow_current_expected is not None:
 			allow_current_expected_gpath = GPath(allow_current_expected)
 		else:
 			allow_current_expected_gpath = None
 
-		result = GPath.find_common(path1, path2)
-		assert result == allow_current_expected_gpath
-		result = GPath.find_common(path2, path1)
-		assert result == allow_current_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2))
-		assert result == allow_current_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1))
-		assert result == allow_current_expected_gpath
-
-		result = GPath.find_common(path1, path2, allow_current=True, allow_parents=False)
-		assert result == allow_current_expected_gpath
-		result = GPath.find_common(path2, path1, allow_current=True, allow_parents=False)
-		assert result == allow_current_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=True, allow_parents=False)
-		assert result == allow_current_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=True, allow_parents=False)
-		assert result == allow_current_expected_gpath
-
 		if allow_parents_expected is not None:
 			allow_parents_expected_gpath = GPath(allow_parents_expected)
 		else:
 			allow_parents_expected_gpath = None
 
-		result = GPath.find_common(path1, path2, allow_current=False, allow_parents=True)
-		assert result == allow_parents_expected_gpath
-		result = GPath.find_common(path2, path1, allow_current=False, allow_parents=True)
-		assert result == allow_parents_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=False, allow_parents=True)
-		assert result == allow_parents_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=False, allow_parents=True)
-		assert result == allow_parents_expected_gpath
-
 		if allow_current_parent_expected is not None:
 			allow_current_parent_expected_gpath = GPath(allow_current_parent_expected)
 		else:
 			allow_current_parent_expected_gpath = None
 
-		result = GPath.find_common(path1, path2, allow_current=True, allow_parents=True)
-		assert result == allow_current_parent_expected_gpath
-		result = GPath.find_common(path2, path1, allow_current=True, allow_parents=True)
-		assert result == allow_current_parent_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=True, allow_parents=True)
-		assert result == allow_current_parent_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=True, allow_parents=True)
-		assert result == allow_current_parent_expected_gpath
-
 		if no_common_expected is not None:
 			no_common_expected_gpath = GPath(no_common_expected)
 		else:
 			no_common_expected_gpath = None
 
-		result = GPath.find_common(path1, path2, allow_current=False, allow_parents=False)
-		assert result == no_common_expected_gpath
-		result = GPath.find_common(path2, path1, allow_current=False, allow_parents=False)
-		assert result == no_common_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=False, allow_parents=False)
-		assert result == no_common_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=False, allow_parents=False)
-		assert result == no_common_expected_gpath
+		for lhs, rhs in itertools.chain(itertools.product([path1], [path2, GPath(path2)]), itertools.product([path2], [path1, GPath(path1)])):
+			gpath = GPath(lhs)
+
+			result = gpath.common_with(rhs)
+			assert result == allow_current_expected_gpath
+			result = gpath & rhs
+			assert result == allow_current_expected_gpath
+
+			result = gpath.common_with(rhs, allow_current=True, allow_parents=False)
+			assert result == allow_current_expected_gpath
+
+			result = gpath.common_with(rhs, allow_current=False, allow_parents=True)
+			assert result == allow_parents_expected_gpath
+
+			result = gpath.common_with(rhs, allow_current=True, allow_parents=True)
+			assert result == allow_current_parent_expected_gpath
+
+			result = gpath.common_with(rhs, allow_current=False, allow_parents=False)
+			assert result == no_common_expected_gpath
 
 
 
 	@pytest.mark.parametrize(
 		('paths', 'allow_current', 'allow_parents', 'expected'),
 		[
 			(
@@ -1062,16 +1180,17 @@
 					"../usr/bin",
 					"../usr/bin/python",
 					"../../usr/bin",
 					"../../usr/bin/python",
 					"C:/Program Files",
 					"C:/Program Files/python.exe",
 					"D:/Documents",
-					"E:/",
-					"E:/Secret Documents/Secret Document.txt",
+					"E:",
+					"E:Apples",
+					"E:Secret Documents/Secret Document.txt",
 				],
 				True,
 				False,
 				{
 					GPath("/"): [
 						GPath("usr/bin"),
 						GPath("usr/bin/python"),
@@ -1092,16 +1211,17 @@
 					GPath("C:/Program Files"): [
 						GPath(""),
 						GPath("python.exe"),
 					],
 					GPath("D:/Documents"): [
 						GPath(""),
 					],
-					GPath("E:/"): [
+					GPath("E:"): [
 						GPath(""),
+						GPath("Apples"),
 						GPath("Secret Documents/Secret Document.txt"),
 					],
 				}
 			),
 			([""], True, False, {GPath(""): [GPath("")]}),
 			([""], True, True, {GPath(""): []}),
 			([""], False, True, {GPath(""): []}),
@@ -1169,58 +1289,64 @@
 		result = GPath.partition(*gpaths, allow_current=allow_current, allow_parents=allow_parents)
 		assert result == expected
 
 
 	@pytest.mark.parametrize(
 		('paths', 'expected_gpath'),
 		[
-			(["", "/", "usr", "bin"], "usr/bin"),
+			(["", "usr", "bin"], "usr/bin"),
+			(["", "/", "usr", "bin"], "/usr/bin"),
 			(["/", "", "usr", "bin"], "/usr/bin"),
 			(["/", "usr", "", "bin"], "/usr/bin"),
 			(["/", "usr", "bin", ""], "/usr/bin"),
-			(["..", "/", "usr", "bin"], "../usr/bin"),
+			(["..", "usr", "bin"], "../usr/bin"),
+			(["..", "/", "usr", "bin"], "/usr/bin"),
 			(["/", "..", "usr", "bin"], "/usr/bin"),
 			(["/", "usr", "..", "bin"], "/bin"),
 			(["/", "usr", "bin", ".."], "/usr"),
 
 			(["/usr", "local", "bin"], "/usr/local/bin"),
-			(["/usr", "/local", "bin"], "/usr/bin"),
+			(["/usr", "/local", "bin"], "/local/bin"),
 			(["/usr", "../local", "bin"], "/local/bin"),
 			(["/usr", "../../local", "bin"], "/local/bin"),
 			(["/usr", "../local", "../bin"], "/bin"),
-			(["/usr", "C:/local", "bin"], "/usr/bin"),
-			(["/", "usr", "bin"], "/usr/bin"),
+			(["/usr", "C:/local", "bin"], "C:/local/bin"),
+			(["/usr", "C:local", "bin"], "C:/usr/local/bin"),
 			(["/", "usr", "bin"], "/usr/bin"),
 
 			(["usr", "local", "bin"], "usr/local/bin"),
-			(["usr", "/local", "bin"], "usr/bin"),
+			(["usr", "/local", "bin"], "/local/bin"),
 			(["usr", "../local", "bin"], "local/bin"),
 			(["usr", "../../local", "bin"], "../local/bin"),
 			(["usr", "../local", "../bin"], "bin"),
-			(["usr", "C:/local", "bin"], "usr/bin"),
+			(["usr", "C:/local", "bin"], "C:/local/bin"),
+			(["usr", "C:local", "bin"], "C:usr/local/bin"),
 			(["", "usr", "bin"], "usr/bin"),
 
 			(["../usr", "local", "bin"], "../usr/local/bin"),
-			(["../usr", "/local", "bin"], "../usr/bin"),
+			(["../usr", "/local", "bin"], "/local/bin"),
 			(["../usr", "../local", "bin"], "../local/bin"),
 			(["../usr", "../../local", "bin"], "../../local/bin"),
 			(["../usr", "../local", "../bin"], "../bin"),
 			(["../usr", "../local", "../../bin"], "../../bin"),
-			(["../usr", "C:/local", "bin"], "../usr/bin"),
+			(["../usr", "C:/local", "bin"], "C:/local/bin"),
+			(["../usr", "C:local", "bin"], "C:../usr/local/bin"),
 			(["..", "usr", "bin"], "../usr/bin"),
 			(["../..", "usr", "bin"], "../../usr/bin"),
 			(["..", "..", "usr", "bin"], "../../usr/bin"),
 
 			(["C:/Windows", "System32", "drivers"], "C:/Windows/System32/drivers"),
-			(["C:/Windows", "/System32", "Containers"], "C:/Windows/Containers"),
+			(["C:/Windows", "/System32", "Containers"], "C:/System32/Containers"),
 			(["C:/Windows", "../System32", "Containers"], "C:/System32/Containers"),
 			(["C:/Windows", "../../System32", "Containers"], "C:/System32/Containers"),
 			(["C:/Windows", "../System32", "../Containers"], "C:/Containers"),
-			(["C:/Windows", "C:/System32", "Containers"], "C:/Windows/Containers"),
-			(["C:/Windows", "D:/System32", "Containers"], "C:/Windows/Containers"),
+			(["C:/Windows", "C:/System32", "Containers"], "C:/System32/Containers"),
+			(["C:/Windows", "C:System32", "Containers"], "C:/Windows/System32/Containers"),
+			(["C:/Windows", "D:/System32", "Containers"], "D:/System32/Containers"),
+			(["C:/Windows", "D:System32", "Containers"], "D:/Windows/System32/Containers"),
 			(["C:/", "Windows", "System32"], "C:/Windows/System32"),
 		],
 		indirect=['expected_gpath']
 	)
 	def test_join(self, paths: list[str], expected_gpath: GPath):
 		"""
 			Test `join()`.
```


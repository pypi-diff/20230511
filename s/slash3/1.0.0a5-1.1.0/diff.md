# Comparing `tmp/slash3-1.0.0a5-py3-none-any.whl.zip` & `tmp/slash3-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7412 bytes, number of entries: 11
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-01 09:52 slash3/VERSION
--rw-r--r--  2.0 unx     2569 b- defN 23-Apr-01 09:52 slash3/__init__.py
--rw-r--r--  2.0 unx     4595 b- defN 23-Apr-01 09:52 slash3/key.py
--rw-r--r--  2.0 unx       60 b- defN 23-Apr-01 09:52 slash3/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-01 09:52 slash3/py.typed
--rw-r--r--  2.0 unx     4035 b- defN 23-Apr-01 09:52 slash3/uri.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-01 09:52 slash3-1.0.0a5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2901 b- defN 23-Apr-01 09:52 slash3-1.0.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-01 09:52 slash3-1.0.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-01 09:52 slash3-1.0.0a5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      814 b- defN 23-Apr-01 09:52 slash3-1.0.0a5.dist-info/RECORD
-11 files, 16154 bytes uncompressed, 6046 bytes compressed:  62.6%
+Zip file size: 8572 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        6 b- defN 23-May-11 16:52 slash3/VERSION
+-rw-r--r--  2.0 unx     3975 b- defN 23-May-11 16:51 slash3/__init__.py
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-11 16:51 slash3/key.py
+-rw-r--r--  2.0 unx       60 b- defN 23-May-11 16:51 slash3/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-11 16:51 slash3/py.typed
+-rw-r--r--  2.0 unx     3938 b- defN 23-May-11 16:51 slash3/uri.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4567 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      804 b- defN 23-May-11 16:52 slash3-1.1.0.dist-info/RECORD
+11 files, 20322 bytes uncompressed, 7226 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: slash3/py.typed
 Comment: 
 
 Filename: slash3/uri.py
 Comment: 
 
-Filename: slash3-1.0.0a5.dist-info/LICENSE
+Filename: slash3-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: slash3-1.0.0a5.dist-info/METADATA
+Filename: slash3-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: slash3-1.0.0a5.dist-info/WHEEL
+Filename: slash3-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: slash3-1.0.0a5.dist-info/top_level.txt
+Filename: slash3-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: slash3-1.0.0a5.dist-info/RECORD
+Filename: slash3-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## slash3/VERSION

```diff
@@ -1 +1 @@
-1.0.0a5
+1.1.0
```

## slash3/__init__.py

```diff
@@ -1,96 +1,168 @@
 """
 [![codecov](https://codecov.io/gh/cariad/slash3/branch/main/graph/badge.svg?token=Vq0w74e8YY)](https://codecov.io/gh/cariad/slash3)
 
-## Introduction
+# Introduction
 
 **Slash3** is a Python package for building and navigating Amazon Web Services
 S3 URIs.
 
-## Examples
+# What's an S3 URI?
 
-To construct an S3 URI from its component parts:
+An S3 URI (Uniform Resource Identifier) is a string that identifies a bucket,
+and optionally a key, in Amazon Web Services S3.
+
+The pattern for an S3 URI is `s3://BUCKET/KEY`.
+
+For example:
+
+- The bucket named "circus" can be described by the URI `s3://circus/`
+- The key prefix for all circus images can be described by the URI
+`s3://circus/images/`
+- The path to Steve's staff photograph can be described by the URI
+`s3://circus/images/steve.jpg`
+
+# Installation
+
+Slash3 requires Python 3.9 or later and can be installed from
+[PyPI](https://pypi.org/project/slash3/).
+
+```shell
+pip install slash3
+```
+
+# Usage
+
+## Construct a URI from a URI
+
+If you've already got a string URI then pass it directly to `S3Uri`:
+
+```python
+from slash3 import S3Uri
+
+uri = S3Uri("s3://circus/")
+
+uri.bucket  # circus
+uri.key     #
+
+uri = S3Uri("s3://circus/images/clowns.jpg")
+
+uri.bucket  # circus
+uri.key     # images/clowns.jpg
+```
+
+## Construct a URI from a bucket and key
+
+To construct an S3 URI from a bucket name and an optional key, call
+`S3Uri.to_uri`:
 
 ```python
 from slash3 import S3Uri
 
-S3Uri.to_uri("circus", "images/clowns.jpg")  # s3://circus/images/clowns.jpg
+uri = S3Uri.to_uri("circus")
+# s3://circus/
+
+uri = S3Uri.to_uri("circus", "images/clowns.jpg")
+# s3://circus/images/clowns.jpg
 ```
 
-To join to a key:
+## Join a key suffix with a "/" delimiter
+
+To join a key suffix with a "/" delimiter -- for example, to join an object's
+name to a key prefix -- call `S3Uri.join()` or use the `/` operator:
 
 ```python
 from slash3 import S3Uri
 
-images = S3Uri("s3://circus/") / "images"  # s3://circus/images
-clowns = images / "clowns.jpg"  # s3://circus/images/clowns.jpg
+uri = S3Uri("s3://circus/")
+
+images = uri / "images"
+# s3://circus/images
+
+clowns = images / "clowns.jpg"
+# s3://circus/images/clowns.jpg
 ```
 
-To append to a key:
+Slash3 will automatically normalise away any consecutive "/" delimiters.
+
+## Append a key suffix without a delimiter
+
+To append a key suffix without a delimiter, call `S3Uri.append()` or use the `+`
+operator:
 
 ```python
 from slash3 import S3Uri
 
-staff = S3Uri("s3://circus/") / "staff-"  # s3://circus/staff-
-steve = staff + "steve.jpg"  # s3://circus/staff-steve.jpg
-penny = staff + "penny.jpg"  # s3://circus/staff-penny.jpg
+staff = S3Uri("s3://circus/staff-")
+
+steve = staff + "steve.jpg"
+# s3://circus/staff-steve.jpg
+
+penny = staff + "penny.jpg"
+# s3://circus/staff-penny.jpg
 ```
 
-To navigate to a parent path:
+## Get the parent key prefix
+
+To get a URI's parent key prefix, call `S3Uri.parent`:
 
 ```python
 from slash3 import S3Uri
 
 steve = S3Uri("s3://circus/images/steve.jpg")
-images = steve.parent  # s3://circus/images/
+
+steve.parent
+# s3://circus/images/
 ```
 
-To discover a relative path:
+## Get the key's leaf / file name
 
 ```python
 from slash3 import S3Uri
 
-steve = S3Uri("s3://circus/images/staff/steve.jpg")
-relative = steve.relative_to("s3://circus/images/")  # staff/steve.jpg
+steve = S3Uri("s3://circus/images/steve.jpg")
+
+steve.leaf
+# steve.jpg
 ```
 
-## Installation
+## Get a relative key path
 
-Slash3 requires Python 3.9 or later and can be installed from
-[PyPI](https://pypi.org/project/slash3/).
+To discover the relative path between a specific URI and a parent URI, call
+`S3Uri.relative_to`:
 
-```shell
-pip install slash3
-```
+```python
+from slash3 import S3Uri
 
-## Logging
+avatar = S3Uri("s3://circus/images/staff/steve.jpg")
+images = "s3://circus/images/"
 
-Slash3 respects your root logger configuration. To configure the package's
-logger directly, get the logger named "slash3".
+avatar.relative_to(images)
+# staff/steve.jpg
+```
 
-## Support
+# Support
 
 Please submit all your questions, feature requests and bug reports at
-[github.com/cariad/slash3/issues](https://github.com/cariad/slash3/issues).
-Thank you!
+[github.com/cariad/slash3/issues](https://github.com/cariad/slash3/issues). Thank you!
 
-## Licence
+# Licence
 
-Slash3 is [open-source](https://github.com/cariad/slash3) and published under
-the [MIT License](https://github.com/cariad/slash3/blob/main/LICENSE).
+Slash3 is [open-source](https://github.com/cariad/slash3) and released under the
+[MIT License](https://github.com/cariad/slash3/blob/main/LICENSE).
 
 You don't have to give attribution in your project, but -- as a freelance
 developer with rent to pay -- I appreciate it!
 
-## The Author
+# Author
 
 Hello! 👋 I'm **Cariad Eccleston**, and I'm a freelance Amazon Web Services
-architect, DevOps evangelist, CI/CD deployer and backend developer.
+architect, DevOps evangelist, CI/CD pipeline engineer and backend developer.
 
-You can find me at [cariad.earth](https://cariad.earth),
+You can find me at [cariad.earth](https://www.cariad.earth),
 [github/cariad](https://github.com/cariad),
 [linkedin/cariad](https://linkedin.com/in/cariad) and on Mastodon at
 [@cariad@tech.lgbt](https://tech.lgbt/@cariad).
 """
 
 from importlib.resources import open_text
```

## slash3/key.py

```diff
@@ -1,20 +1,17 @@
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 from slash3.logging import logger
 
 MAX_LENGTH = 1024
 
 
 class S3Key:
     """
-    An Amazon Web Services S3 object key.
-
-    `key` is either an object key (e.g. "photos/clowns.jpg") or None to describe
-    the root of the bucket.
+    An Amazon Web Services S3 key.
     """
 
     def __init__(self, key: Optional[str] = None) -> None:
         logger.debug('Creating new S3Key from "%s"', key)
         key = key or ""
 
         if key.startswith("/"):
@@ -53,18 +50,20 @@
     def append(self, suffix: str) -> "S3Key":
         """
         Appends a string to the key.
 
         ```python
         images = S3Key("images/staff-")
 
-        steve = images.append("steve.jpg")  # "images/staff-steve.jpg"
+        steve = images.append("steve.jpg")
+        # "images/staff-steve.jpg"
 
         # Or use "+":
-        penny = images + "penny.jpg"  # "images/staff-penny.jpg"
+        penny = images + "penny.jpg"
+        # "images/staff-penny.jpg"
         ```
 
         To add a suffix with a "/" delimiter, use `join()` instead.
         """
 
         logger.debug('Appending base "%s" and suffix "%s"', self._key, suffix)
 
@@ -80,18 +79,20 @@
     def join(self, suffix: str) -> "S3Key":
         """
         Joins a string to the key with a "/" delimiter.
 
         ```python
         images = S3Key("images/staff")
 
-        steve = images.join("steve.jpg")  # "images/staff/steve.jpg"
+        steve = images.join("steve.jpg")
+        # "images/staff/steve.jpg"
 
         # Or use "/":
-        penny = images / "penny.jpg"  # "images/staff/penny.jpg"
+        penny = images / "penny.jpg"
+        # "images/staff/penny.jpg"
         ```
 
         To append a string without a "/" delimiter, use `append()` instead.
         """
 
         logger.debug('Joining base "%s" and suffix "%s"', self._key, suffix)
 
@@ -102,40 +103,54 @@
         logger.debug('Suffix normalised to "%s"', suffix)
 
         return S3Key(base + suffix)
 
     @property
     def key(self) -> str:
         """
-        Key (e.g. "private/clowns.jpg").
+        Key.
+
+        For example, "private/clowns.jpg".
         """
 
         return self._key
 
+    @property
+    def leaf(self) -> str:
+        """
+        Key leaf.
+
+        In a file system metaphor, the leaf would be the file's name.
+
+        For example, the leaf of "private/clowns.jpg" is "clowns.jpg".
+        """
+
+        return self.relative_to(self.parent)
+
     @staticmethod
     def normal_left(key: str, slash: bool = False) -> str:
         """
         Normalises the left of the key.
 
-        If `slash` is true then key is returned with exactly one leading slash,
-        otherwise no leading slashes.
+        If `slash` is true then the key is returned with exactly one leading
+        slash, otherwise the key is returned with no leading slashes.
         """
 
         while key.startswith("/"):
             key = key[1:]
 
         return "/" + key if slash else key
 
     @staticmethod
     def normal_right(key: str, slash: bool = False) -> str:
         """
         Normalises the right of the key.
 
-        If `slash` is true then key is returned with exactly one trailing slash,
-        otherwise no trailing slashes.
+        If `slash` is true then the key is returned with exactly one trailing
+        slash, otherwise the key is returned with no trailing slashes.
         """
 
         while key.endswith("/"):
             key = key[:-1]
 
         return key + "/" if slash else key
 
@@ -167,7 +182,40 @@
         logger.debug('Final "/" in key "%s" is at index %s', self._key, index)
 
         parent_key = self._key[0:index]
 
         logger.debug('Key "%s" parent is "%s"', self._key, parent_key)
 
         return S3Key(parent_key)
+
+    def relative_to(self, parent: Union["S3Key", str]) -> str:
+        """
+        Gets the relative key path from this key to a `parent` key.
+
+        For example, the relative path to "private/clowns.jpg" from parent
+        "private" is "clowns.jpg".
+        """
+
+        logger.debug(
+            'Calculating the relative key from "%s" to "%s"',
+            self,
+            parent,
+        )
+
+        parent = str(parent)
+        normal = self.normal_right(parent, slash=True) if parent else parent
+
+        logger.debug('Normalised the parent key to "%s"', normal)
+
+        if not self._key.startswith(normal):
+            raise ValueError(f'"{parent}" is not a parent of "{self}"')
+
+        relative_key = self._key[len(normal) :]  # noqa: E203
+
+        logger.debug(
+            'The relative path from "%s" to "%s" is "%s"',
+            parent,
+            self,
+            relative_key,
+        )
+
+        return relative_key
```

## slash3/uri.py

```diff
@@ -1,24 +1,23 @@
 from re import match
 from typing import Any, Optional, Union
 
 from slash3.key import S3Key
-from slash3.logging import logger
 
 
 class S3Uri:
     """
     An Amazon Web Services S3 URI.
 
-    `uri` is an S3 URI string (e.g. "s3://circus/clowns.jpg"). To construct a
-    URI from its component parts, use the `to_uri()` class method instead.
+    To construct a URI from a bucket's name and optional key, use the
+    `to_uri()` class method instead.
     """
 
     def __init__(self, uri: str) -> None:
-        m = match(r"s3:\/\/([^/]*)(\/(.*))?", uri)
+        m = match(r"[sS]3:\/\/([^/]*)(\/(.*))?", uri)
 
         if not m:
             raise ValueError(f'"{uri}" is not an S3 URI')
 
         self._bucket = str(m.group(1))
         self._key = S3Key(m.group(3))
 
@@ -37,18 +36,20 @@
     def append(self, other: str) -> "S3Uri":
         """
         Appends a string to the URI.
 
         ```python
         images = S3Uri("s3://circus/staff-")
 
-        steve = images.append("steve.jpg")  # "s3://circus/staff-steve.jpg"
+        steve = images.append("steve.jpg")
+        # "s3://circus/staff-steve.jpg"
 
         # Or use "+":
-        penny = images + "penny.jpg"  # "s3://circus/staff-penny.jpg"
+        penny = images + "penny.jpg"
+        # "s3://circus/staff-penny.jpg"
         ```
 
         To add a suffix with a "/" delimiter, use `join()` instead.
         """
 
         return S3Uri.to_uri(self._bucket, self._key.append(other))
 
@@ -63,18 +64,20 @@
     def join(self, suffix: str) -> "S3Uri":
         """
         Joins a string to the URI with a "/" delimiter.
 
         ```python
         images = S3Uri("s3://circus/staff")
 
-        steve = images.join("steve.jpg")  # "s3://circus/staff/steve.jpg"
+        steve = images.join("steve.jpg")
+        # "s3://circus/staff/steve.jpg"
 
         # Or use "/":
-        penny = images / "penny.jpg"  # "s3://circus/staff/penny.jpg"
+        penny = images / "penny.jpg"
+        # "s3://circus/staff/penny.jpg"
         ```
 
         To append a string without a "/" delimiter, use `append()` instead.
         """
 
         return S3Uri.to_uri(self._bucket, self._key.join(suffix))
 
@@ -83,71 +86,73 @@
         """
         Key.
         """
 
         return self._key
 
     @property
+    def leaf(self) -> str:
+        """
+        URI leaf.
+
+        In a file system metaphor, the leaf would be the file's name.
+
+        For example, the leaf of "s3://circus/private/clowns.jpg" is
+        "clowns.jpg".
+        """
+
+        return self.key.leaf
+
+    @property
     def parent(self) -> "S3Uri":
         """
         Parent URI.
 
         For example, the parent of "s3://circus/private/clowns.jpg" is
         "s3://circus/private/".
         """
 
         return S3Uri.to_uri(self._bucket, self.key.parent)
 
     def relative_to(self, parent: Union["S3Uri", str]) -> str:
         """
         Gets the relative key path from this URI to a `parent` URI.
 
-        For example, the relative path to "s3://circus/private/clowns" from
-        "s3://circus/" is "private/clowns".
+        For example, the relative path to "s3://circus/private/clowns.jpg" from
+        "s3://circus/" is "private/clowns.jpg".
         """
 
         parent = S3Uri(parent) if isinstance(parent, str) else parent
 
         if parent._bucket != self._bucket:
             raise ValueError(
                 f'There is no relative path from "{parent}" to "{self}" '
                 "because these URIs describe different buckets"
             )
 
-        if not self.key.key.startswith(parent.key.key):
-            raise ValueError(f'"{parent}" is not a parent of "{self}"')
-
-        relative_key = self.key.key[len(parent.key) :]  # noqa: E203
-        logger.debug(
-            'The relative path from "%s" to "%s" is "%s"',
-            parent,
-            self,
-            relative_key,
-        )
-
-        return relative_key
+        return self._key.relative_to(parent.key)
 
     @staticmethod
     def to_string(bucket: str, key: Optional[Union[S3Key, str]]) -> str:
         """
-        Constructs a string S3 URI from its component parts.
+        Constructs a string S3 URI from a bucket and optional key.
 
-        To construct an `S3Uri` from component parts, use `to_uri()` instead.
+        To construct an `S3Uri` instance, use `to_uri()` instead.
         """
 
         return f"s3://{bucket}/{key or ''}"
 
     @classmethod
     def to_uri(
         cls,
         bucket: str,
         key: Optional[Union[S3Key, str]] = None,
     ) -> "S3Uri":
         """
-        Constructs an `S3Uri` from its component parts.
+        Constructs an `S3Uri` from a bucket and optional key.
         """
 
         return cls(cls.to_string(bucket, key=key))
 
     @property
     def uri(self) -> str:
         """
```

## Comparing `slash3-1.0.0a5.dist-info/LICENSE` & `slash3-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*


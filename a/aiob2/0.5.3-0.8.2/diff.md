# Comparing `tmp/aiob2-0.5.3.tar.gz` & `tmp/aiob2-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiob2-0.5.3.tar", max compression
+gzip compressed data, was "aiob2-0.8.2.tar", max compression
```

## Comparing `aiob2-0.5.3.tar` & `aiob2-0.8.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      310 2022-12-18 04:57:08.758799 aiob2-0.5.3/aiob2/__init__.py
--rw-r--r--   0        0        0     7598 2022-12-18 02:48:09.522590 aiob2-0.5.3/aiob2/bucket.py
--rw-r--r--   0        0        0     2160 2022-12-17 09:44:55.282684 aiob2-0.5.3/aiob2/errors.py
--rw-r--r--   0        0        0    13960 2022-12-18 04:56:14.120414 aiob2-0.5.3/aiob2/http.py
--rw-r--r--   0        0        0      127 2022-12-17 08:38:08.074394 aiob2-0.5.3/aiob2/models/__init__.py
--rw-r--r--   0        0        0      478 2022-12-17 11:31:07.755401 aiob2-0.5.3/aiob2/models/account.py
--rw-r--r--   0        0        0      179 2022-12-17 07:39:07.143639 aiob2-0.5.3/aiob2/models/archetypes.py
--rw-r--r--   0        0        0     6103 2022-12-18 02:15:27.855867 aiob2-0.5.3/aiob2/models/file.py
--rw-r--r--   0        0        0        0 2022-12-18 02:37:28.221445 aiob2-0.5.3/aiob2/py.typed
--rw-r--r--   0        0        0     1243 2022-12-17 10:38:51.564807 aiob2-0.5.3/aiob2/utils.py
--rw-r--r--   0        0        0     1083 2022-12-17 15:35:09.735014 aiob2-0.5.3/LICENSE
--rw-r--r--   0        0        0     1394 2022-12-18 04:57:19.850801 aiob2-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2479 2022-12-18 04:37:33.561426 aiob2-0.5.3/README.md
--rw-r--r--   0        0        0     3265 2022-12-18 04:57:34.227170 aiob2-0.5.3/setup.py
--rw-r--r--   0        0        0     3481 2022-12-18 04:57:34.227170 aiob2-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      572 2023-01-28 13:05:37.648223 aiob2-0.8.2/aiob2/__init__.py
+-rw-r--r--   0        0        0    13983 2023-01-28 10:54:53.685618 aiob2-0.8.2/aiob2/bucket.py
+-rw-r--r--   0        0        0     2075 2022-12-22 14:53:54.000000 aiob2-0.8.2/aiob2/errors.py
+-rw-r--r--   0        0        0     5195 2023-01-28 12:53:49.352504 aiob2-0.8.2/aiob2/file.py
+-rw-r--r--   0        0        0    30865 2023-01-28 12:52:02.958331 aiob2-0.8.2/aiob2/http.py
+-rw-r--r--   0        0        0      120 2022-12-22 14:10:30.000000 aiob2-0.8.2/aiob2/models/__init__.py
+-rw-r--r--   0        0        0      458 2022-12-22 14:10:30.000000 aiob2-0.8.2/aiob2/models/account.py
+-rw-r--r--   0        0        0      165 2023-01-28 09:44:52.174003 aiob2-0.8.2/aiob2/models/archetypes.py
+-rw-r--r--   0        0        0     9313 2023-01-23 20:48:03.257995 aiob2-0.8.2/aiob2/models/file.py
+-rw-r--r--   0        0        0        0 2022-12-22 14:10:30.000000 aiob2-0.8.2/aiob2/py.typed
+-rw-r--r--   0        0        0     5617 2023-01-22 13:30:50.579525 aiob2-0.8.2/aiob2/utils.py
+-rw-r--r--   0        0        0     1063 2022-12-22 14:10:30.000000 aiob2-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1616 2023-01-28 13:06:01.196080 aiob2-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2369 2023-01-22 19:02:53.209438 aiob2-0.8.2/README.md
+-rw-r--r--   0        0        0     3193 2023-01-28 14:26:03.666969 aiob2-0.8.2/setup.py
+-rw-r--r--   0        0        0     3399 2023-01-28 14:26:03.666969 aiob2-0.8.2/PKG-INFO
```

### Comparing `aiob2-0.5.3/aiob2/models/file.py` & `aiob2-0.8.2/aiob2/models/file.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import datetime
-from typing import TypedDict, Literal, Optional, Union
+from typing import TypedDict, Literal, Optional, Union, Dict, Any
 from typing_extensions import NotRequired
 
 from .archetypes import B2Object
 from ..utils import format_timestamp
 
 __all__ = ('File', 'DeletedFile', 'DownloadedFile')
 
@@ -11,37 +13,42 @@
 class PartialFilePayload(TypedDict):
     fileName: str
     fileId: Optional[str]
 
 
 class UploadPayload(PartialFilePayload):
     accountId: str
-    action: Literal['upload']
+    action: Literal['start', 'upload', 'hide', 'folder']
     bucketId: str
     contentLength: Optional[int]
     contentSha1: Optional[str]
     contentMd5: NotRequired[Optional[str]]
     contentType: Optional[str]
-    fileInfo: dict
-    fileRetention: NotRequired[Optional[dict]]
-    legalHold: NotRequired[dict]
+    fileInfo: Dict[Any, Any]
+    fileRetention: NotRequired[Optional[Dict[Any, Any]]]
+    legalHold: NotRequired[Dict[Any, Any]]
     replicationStatus: NotRequired[Literal['PENDING', 'COMPLETED', 'FAILED', 'REPLICA']]
-    serverSideEncryption: NotRequired[Optional[dict]]
+    serverSideEncryption: NotRequired[Optional[Dict[Any, Any]]]
     uploadTimestamp: Union[int, Literal[0]]
 
 
 DownloadPayloadHeaders = TypedDict('DownloadPayloadHeaders', {
     'Content-Length': int,
     'Content-Type': str,
     'X-Bz-File-Id': str,
     'X-Bz-File-Name': str,
     'X-Bz-Content-Sha1': str,
     'X-Bz-Upload-Timestamp': str,
     'Accept-Ranges': str,
-    'Date': str
+    'Date': str,
+    'Content-Disposition': NotRequired[str],
+    'Content-Language': NotRequired[str],
+    'Expires': NotRequired[str],
+    'Content-Encoding': NotRequired[str],
+    'X-Bz-Server-Side-Encryption': NotRequired[Literal['AES256']]
 })
 
 
 class PartialFile(B2Object):
     """Represents a "partial" file from Backblaze.
 
     Attributes
@@ -60,44 +67,62 @@
 
         self.name: str = data['fileName']
         self.id: str = data['fileId']
 
     def __str__(self):
         return self.name
 
-    def __eq__(self, other):
-        if isinstance(other, File):
-            return self.id == other.id
+    def __eq__(self, other: Any):
+        return isinstance(other, File) and self.id == other.id
+
 
-        return False
+class LargeFilePartPayload(TypedDict):
+    fileId: str
+    partNumber: int
+    contentLength: int
+    contentSha1: str
+    contentMd5: Optional[str]
+    serverSideEncryption: Optional[Dict[Any, Any]]
+    uploadTimestamp: int
+
+
+class LargeFilePart(B2Object):
+    def __init__(self, payload: LargeFilePartPayload) -> None:
+        self.file_id: str = payload['fileId']
+        self.part_number: int = payload['partNumber']
+        self.content_length: int = payload['contentLength']
+        self.content_sha1: str = payload['contentSha1']
+        self.content_md5: Optional[str] = payload['contentMd5']
+        self.server_side_encryption: Optional[Dict[Any, Any]] = payload['serverSideEncryption']
+        self.upload_timestamp: datetime.datetime = format_timestamp(payload['uploadTimestamp'])
 
 
 class File(PartialFile):
     """Represents a file uploaded to Backblaze.
 
     Attributes
     ----------
     account_id: :class:`str`
         The account's ID that owns the file.
     action: Literal[``'upload'``]
         This will always be ``upload``.
     bucket_id: :class:`str`
-        The bucket's ID that the file is in.
+        The file's bucket ID.
     content_length: :class:`int`
         The file's size represented in number of bytes.
     content_sha1: :class:`str`
         The file's SHA-1.
     content_md5: Optional[:class:`str`]
         The MD5 of the file's bytes as a 40-digit hex string.
     content_type: :class:`str`
         The file's content type, e.g. image/jpeg.
     id: :class:`str`
         The file's ID.
     info: :class:`dict`
-        Any info regarding the file submitted at upload.
+        Any custom info regarding the file submitted at upload.
     name: :class:`str`
         The file's name.
     retention: Optional[:class:`dict`]
         The file's object lock retention settings.
     legal_hold: Optional[:class:`dict`]
         The file's object lock legal hold status.
     replication_status: Optional[Literal[``'PENDING'``, ``'COMPLETED'``, ``'FAILED'``, ``'REPLICA'``]
@@ -115,25 +140,25 @@
 
         # appease type checker
         assert data['contentLength'] is not None
         assert data['contentSha1'] is not None
         assert data['contentType'] is not None
 
         self.account_id: str = data['accountId']
-        self.action: Literal['upload'] = data['action']
+        self.action: Literal['upload'] = data['action']  # type: ignore
         self.bucket_id: str = data['bucketId']
         self.content_length: int = data['contentLength']
         self.content_sha1: str = data['contentSha1']
         self.content_md5: Optional[str] = data.get('contentMd5')
         self.content_type: str = data['contentType']
-        self.info: dict = data['fileInfo']
-        self.retention: Optional[dict] = data.get('fileRetention')
-        self.legal_hold: Optional[dict] = data.get('legalHold')
+        self.info: Dict[Any, Any] = data['fileInfo']
+        self.retention: Optional[Dict[Any, Any]] = data.get('fileRetention')
+        self.legal_hold: Optional[Dict[Any, Any]] = data.get('legalHold')
         self.replication_status: Optional[Literal['PENDING', 'COMPLETED', 'FAILED', 'REPLICA']] = data.get('replicationStatus')  # noqa
-        self.server_side_encryption: Optional[dict] = data.get('serverSideEncryption')
+        self.server_side_encryption: Optional[Dict[Any, Any]] = data.get('serverSideEncryption')
         self.created: datetime.datetime = format_timestamp(data['uploadTimestamp'])
 
 
 class DeletedFile(PartialFile):
     """Represents a deleted file from Backblaze.
 
     Attributes
@@ -165,26 +190,65 @@
         The file's size represented in number of bytes.
     content_sha1: :class:`str`
         The file's SHA-1.
     created: :class:`datetime.datetime`
         The time at which the file was uploaded.
     downloaded_at: :class:`str`
         The date at which the download was requested.
+    content_disposition: Optional[:class:`str`]
+        Whether or not the content is intended to be played inline, or downloaded locally and optionally the filename.
+    content_language: Optional[:class:`str`]
+        The content's intended language audience.
+    expires: Optional[:class:`datetime.datetime`]
+        The intended expiration date of the content.
+    content_encoding: Optional[:class:`str`]
+        The content's encoding in the order they were performed in.
+    server_side_encryption: Optional[Literal[``AES256``]]
+        The server side encryption performed on the content including the algorithm.
+    comments: Optional[Dict[:class:`str`, :class:`str`]]
+        The comments uploaded with the file.
     content: :class:`bytes`
         The raw bytes of the downloaded file.
     """
     def __init__(
         self,
         content: bytes,
-        headers: DownloadPayloadHeaders
+        headers_: DownloadPayloadHeaders
     ):
-        self.content_length: int = headers['Content-Length']
-        self.content_type: str = headers['Content-Type']
-        self.id: str = headers['X-Bz-File-Id']
-        self.name: str = headers['X-Bz-File-Name']
-        self.content_sha1: str = headers['X-Bz-Content-Sha1']
-        self.created: datetime.datetime = format_timestamp(int(headers['X-Bz-Upload-Timestamp']))
+        headers: Dict[str, Any] = {k.lower(): v for k, v in headers_.items()}
+        b2_info_headers = (
+            'b2-content-disposition',
+            'b2-content-language',
+            'b2-expires',
+            'b2-cache-control',
+            'b2-content-encoding',
+            'b2-content-type'
+        )
+        # comments are turned to lower case by Backblaze
+        # so the above lowercasing won't impact anything
+        comments: Dict[str, str] = {
+            k[10:]: v for k, v in headers.items() if k.startswith('x-bz-info-') and not k.endswith(b2_info_headers)
+        }
+
+        self.content_length: int = headers['content-length']
+        self.content_type: str = headers['content-type']
+        self.id: str = headers['x-bz-file-id']
+        self.name: str = headers['x-bz-file-name']
+        self.content_sha1: str = headers['x-bz-content-sha1']
+        self.created: datetime.datetime = format_timestamp(int(headers['x-bz-upload-timestamp']))
         self.downloaded_at: datetime.datetime = datetime.datetime.strptime(
-            headers['Date'],
+            headers['date'],
             '%a, %d %b %Y %H:%M:%S %Z'
         )
+
+        self.content_disposition: Optional[str] = headers.get('content-disposition')
+        self.content_language: Optional[str] = headers.get('content-language')
+        if (expires := headers.get('cache-control')) is not None:
+            expires = datetime.datetime.strptime(expires, '%a, %d %b %Y %H:%M:%S %Z')
+        else:
+            expires = None
+        self.expires: Optional[datetime.datetime] = expires
+        self.content_encoding: Optional[str] = headers.get('content-encoding')
+        self.server_side_encryption: Optional[Literal['AES256']] = headers.get('x-bz-server-side-encryption')
+        self.comments: Optional[Dict[str, str]] = comments or None
+
         self.content: bytes = content
```

### Comparing `aiob2-0.5.3/pyproject.toml` & `aiob2-0.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiob2"
-version = "0.5.3"
+version = "0.8.2"
 description = "A simple and easy to use async wrapper for Backblaze's B2 bucket API."
 license = "MIT"
 authors = ["Dan <the.void.altacc@gmail.com>"]
 
 readme = "README.md"
 repository = "https://github.com/Void-ux/aiob2"
 documentation = "https://aiob2.readthedocs.io/en/latest/"
@@ -21,30 +21,38 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Void-ux/aiob2/issues/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.1"
-pytest-asyncio = "^0.19.0"
 typing-extensions = "^4.4.0"
 
 [tool.poetry.extras]
 speed = ["orjson"]
 
 [tool.poetry.dev-dependencies]
+pytest-asyncio = "^0.19.0"
 furo = "^2022.12.7"
 sphinxcontrib-trio = "^1.1.2"
+pytest-order = "^1.0.1"
+pytest-env = "^0.8.1"
 
 [tool.pyright]
 typeCheckingVersion = "strict"
 pythonVersion = "3.8"
 reportUnusedImport = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportIncompatibleMethodOverride = "warning"
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
+env = [
+    "KEY_ID=0027cdd0e482c250000000013",
+    "KEY=K002jL/XjzaBvoQumQkI8nzwvf8sOys",
+    "BUCKET_ID=a78ccd0d80bea4b8822c0215",
+    "BUCKET_NAME=aiob2-testing",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aiob2-0.5.3/README.md` & `aiob2-0.8.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,76 @@
-# aiob2
-
----
-
-<p align="center">
-    <a href="https://www.python.org/downloads/">
-        <img src="https://img.shields.io/pypi/pyversions/aiob2?style=for-the-badge" alt="Python version">
-    </a>
-    <a href="https://github.com/Void-ux/aiob2/actions">
-        <img src="https://img.shields.io/github/actions/workflow/status/Void-ux/aiob2/build.yaml?branch=master&style=for-the-badge" alt="Build status">
-    </a>
-    <a href="https://pypi.org/project/aiob2/">
-        <img src="https://img.shields.io/pypi/v/aiob2?color=8BC34A&style=for-the-badge" alt="PyPi">
-    </a>
-    <a href="https://opensource.org/licenses/MIT">
-        <img src="https://img.shields.io/pypi/l/aiob2?color=C0C0C0&style=for-the-badge" alt="License">
-    </a>
-</p>
-
-aiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).
-
-It will allow you to interact with your B2 bucket, it's files and anything else that the B2 API allows in a modern, object-oriented fashion.
-
-__**NOTE:**__ This API wrapper is by no means *complete* and has many endpoints to cover, though the main ones have been covered (they will be listed below)
-
-## Installation
-
----
-
-aiob2 is compatible with Python 3.8+ (this is an estimate). To install aiob2, run the following command in your (virtual) environment.
-
-```
-pip install aiob2
-```
-
-Alternatively, for the latest though least stable version, you can download it from the GitHub repo:
-
-```
-pip install git+https://github.com/Void-ux/aiob2.git
-```
-
-## Usage
-
-### Uploading
-
-```python
-import aiohttp
-import asyncio
-
-from aiob2 import Client
-
-# Our image to upload to our bucket
-with open(r'C:\Users\MS1\Pictures\Camera Roll\IMG_5316.jpeg', 'rb') as file:
-    data = file.read()
-
-async def main():
-    async with Client('key_id', 'key') as client:
-        file = await client.upload_file(
-            content_bytes=data,
-            content_type='image/jpeg',
-            file_name='test.jpg',
-            bucket_id='bucket_id',
-        )
-
-
-if __name__ == '__main__':
-    asyncio.run(main())
-```
-
-And that's it! `upload_file()` returns a `File` object that neatly wraps everything Backblaze's API has provided us with.
-The `File` object's documentation can be found [here](https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)
-
-## License
-
----
-
-This project is released under the [MIT License](https://opensource.org/licenses/MIT).
+# aiob2
+
+---
+
+<p align="center">
+    <a href="https://www.python.org/downloads/">
+        <img src="https://img.shields.io/pypi/pyversions/aiob2?style=for-the-badge" alt="Python version">
+    </a>
+    <a href="https://github.com/Void-ux/aiob2/actions">
+        <img src="https://img.shields.io/github/actions/workflow/status/Void-ux/aiob2/build.yaml?branch=master&style=for-the-badge" alt="Build status">
+    </a>
+    <a href="https://pypi.org/project/aiob2/">
+        <img src="https://img.shields.io/pypi/v/aiob2?color=8BC34A&style=for-the-badge" alt="PyPi">
+    </a>
+    <a href="https://opensource.org/licenses/MIT">
+        <img src="https://img.shields.io/pypi/l/aiob2?color=C0C0C0&style=for-the-badge" alt="License">
+    </a>
+</p>
+
+aiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).
+
+It will allow you to interact with your B2 bucket, it's files and anything else that the B2 API allows in a modern, object-oriented fashion.
+
+**NOTE:** This API wrapper is by no means *complete* and has many endpoints to cover, though the main ones have been covered (they will be listed below)
+
+## Installation
+
+---
+
+aiob2 is compatible with Python 3.8+ (this is an estimate). To install aiob2, run the following command in your (virtual) environment.
+
+```shell
+pip install aiob2
+```
+
+Alternatively, for the latest though least stable version, you can download it from the GitHub repo:
+
+```shell
+pip install git+https://github.com/Void-ux/aiob2.git
+```
+
+## Usage
+
+### Uploading
+
+```python
+import aiohttp
+import asyncio
+
+from aiob2 import Client
+
+# Our image to upload to our bucket
+with open(r'C:\Users\MS1\Pictures\Camera Roll\IMG_5316.jpeg', 'rb') as file:
+    data = file.read()
+
+async def main():
+    async with Client('key_id', 'key') as client:
+        file = await client.upload_file(
+            content_bytes=data,
+            file_name='test.jpg',
+            bucket_id='bucket_id',
+        )
+
+
+if __name__ == '__main__':
+    asyncio.run(main())
+```
+
+And that's it! `upload_file()` returns a `File` object that neatly wraps everything Backblaze's API has provided us with.
+The `File` object's documentation can be found [here](https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)
+
+## License
+
+---
+
+This project is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `aiob2-0.5.3/setup.py` & `aiob2-0.8.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 packages = \
 ['aiob2', 'aiob2.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiohttp>=3.8.1,<4.0.0',
- 'pytest-asyncio>=0.19.0,<0.20.0',
- 'typing-extensions>=4.4.0,<5.0.0']
+['aiohttp>=3.8.1,<4.0.0', 'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'aiob2',
-    'version': '0.5.3',
+    'version': '0.8.2',
     'description': "A simple and easy to use async wrapper for Backblaze's B2 bucket API.",
-    'long_description': '# aiob2\n\n---\n\n<p align="center">\n    <a href="https://www.python.org/downloads/">\n        <img src="https://img.shields.io/pypi/pyversions/aiob2?style=for-the-badge" alt="Python version">\n    </a>\n    <a href="https://github.com/Void-ux/aiob2/actions">\n        <img src="https://img.shields.io/github/actions/workflow/status/Void-ux/aiob2/build.yaml?branch=master&style=for-the-badge" alt="Build status">\n    </a>\n    <a href="https://pypi.org/project/aiob2/">\n        <img src="https://img.shields.io/pypi/v/aiob2?color=8BC34A&style=for-the-badge" alt="PyPi">\n    </a>\n    <a href="https://opensource.org/licenses/MIT">\n        <img src="https://img.shields.io/pypi/l/aiob2?color=C0C0C0&style=for-the-badge" alt="License">\n    </a>\n</p>\n\naiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).\n\nIt will allow you to interact with your B2 bucket, it\'s files and anything else that the B2 API allows in a modern, object-oriented fashion.\n\n__**NOTE:**__ This API wrapper is by no means *complete* and has many endpoints to cover, though the main ones have been covered (they will be listed below)\n\n## Installation\n\n---\n\naiob2 is compatible with Python 3.8+ (this is an estimate). To install aiob2, run the following command in your (virtual) environment.\n\n```\npip install aiob2\n```\n\nAlternatively, for the latest though least stable version, you can download it from the GitHub repo:\n\n```\npip install git+https://github.com/Void-ux/aiob2.git\n```\n\n## Usage\n\n### Uploading\n\n```python\nimport aiohttp\nimport asyncio\n\nfrom aiob2 import Client\n\n# Our image to upload to our bucket\nwith open(r\'C:\\Users\\MS1\\Pictures\\Camera Roll\\IMG_5316.jpeg\', \'rb\') as file:\n    data = file.read()\n\nasync def main():\n    async with Client(\'key_id\', \'key\') as client:\n        file = await client.upload_file(\n            content_bytes=data,\n            content_type=\'image/jpeg\',\n            file_name=\'test.jpg\',\n            bucket_id=\'bucket_id\',\n        )\n\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\nAnd that\'s it! `upload_file()` returns a `File` object that neatly wraps everything Backblaze\'s API has provided us with.\nThe `File` object\'s documentation can be found [here](https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)\n\n## License\n\n---\n\nThis project is released under the [MIT License](https://opensource.org/licenses/MIT).\n',
+    'long_description': '# aiob2\n\n---\n\n<p align="center">\n    <a href="https://www.python.org/downloads/">\n        <img src="https://img.shields.io/pypi/pyversions/aiob2?style=for-the-badge" alt="Python version">\n    </a>\n    <a href="https://github.com/Void-ux/aiob2/actions">\n        <img src="https://img.shields.io/github/actions/workflow/status/Void-ux/aiob2/build.yaml?branch=master&style=for-the-badge" alt="Build status">\n    </a>\n    <a href="https://pypi.org/project/aiob2/">\n        <img src="https://img.shields.io/pypi/v/aiob2?color=8BC34A&style=for-the-badge" alt="PyPi">\n    </a>\n    <a href="https://opensource.org/licenses/MIT">\n        <img src="https://img.shields.io/pypi/l/aiob2?color=C0C0C0&style=for-the-badge" alt="License">\n    </a>\n</p>\n\naiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).\n\nIt will allow you to interact with your B2 bucket, it\'s files and anything else that the B2 API allows in a modern, object-oriented fashion.\n\n**NOTE:** This API wrapper is by no means *complete* and has many endpoints to cover, though the main ones have been covered (they will be listed below)\n\n## Installation\n\n---\n\naiob2 is compatible with Python 3.8+ (this is an estimate). To install aiob2, run the following command in your (virtual) environment.\n\n```shell\npip install aiob2\n```\n\nAlternatively, for the latest though least stable version, you can download it from the GitHub repo:\n\n```shell\npip install git+https://github.com/Void-ux/aiob2.git\n```\n\n## Usage\n\n### Uploading\n\n```python\nimport aiohttp\nimport asyncio\n\nfrom aiob2 import Client\n\n# Our image to upload to our bucket\nwith open(r\'C:\\Users\\MS1\\Pictures\\Camera Roll\\IMG_5316.jpeg\', \'rb\') as file:\n    data = file.read()\n\nasync def main():\n    async with Client(\'key_id\', \'key\') as client:\n        file = await client.upload_file(\n            content_bytes=data,\n            file_name=\'test.jpg\',\n            bucket_id=\'bucket_id\',\n        )\n\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\nAnd that\'s it! `upload_file()` returns a `File` object that neatly wraps everything Backblaze\'s API has provided us with.\nThe `File` object\'s documentation can be found [here](https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)\n\n## License\n\n---\n\nThis project is released under the [MIT License](https://opensource.org/licenses/MIT).\n',
     'author': 'Dan',
     'author_email': 'the.void.altacc@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Void-ux/aiob2',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['aiob2',
 'aiob2.models'] package_data = \ {'': ['*']} install_requires = \
-['aiohttp>=3.8.1,<4.0.0', 'pytest-asyncio>=0.19.0,<0.20.0', 'typing-
-extensions>=4.4.0,<5.0.0'] setup_kwargs = { 'name': 'aiob2', 'version':
-'0.5.3', 'description': "A simple and easy to use async wrapper for Backblaze's
-B2 bucket API.", 'long_description': '# aiob2\n\n---\n\n
+['aiohttp>=3.8.1,<4.0.0', 'typing-extensions>=4.4.0,<5.0.0'] setup_kwargs =
+{ 'name': 'aiob2', 'version': '0.8.2', 'description': "A simple and easy to use
+async wrapper for Backblaze's B2 bucket API.", 'long_description': '#
+aiob2\n\n---\n\n
 \n \n_[Python_version]\n\n \n_[Build_status]\n\n \n_[PyPi]\n\n \n_[License]\n\n
 \n\naiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API]
 (https://www.backblaze.com/b2/docs/calling.html).\n\nIt will allow you to
 interact with your B2 bucket, it\'s files and anything else that the B2 API
-allows in a modern, object-oriented fashion.\n\n__**NOTE:**__ This API wrapper
-is by no means *complete* and has many endpoints to cover, though the main ones
+allows in a modern, object-oriented fashion.\n\n**NOTE:** This API wrapper is
+by no means *complete* and has many endpoints to cover, though the main ones
 have been covered (they will be listed below)\n\n## Installation\n\n---
 \n\naiob2 is compatible with Python 3.8+ (this is an estimate). To install
-aiob2, run the following command in your (virtual) environment.\n\n```\npip
-install aiob2\n```\n\nAlternatively, for the latest though least stable
-version, you can download it from the GitHub repo:\n\n```\npip install
-git+https://github.com/Void-ux/aiob2.git\n```\n\n## Usage\n\n###
-Uploading\n\n```python\nimport aiohttp\nimport asyncio\n\nfrom aiob2 import
-Client\n\n# Our image to upload to our bucket\nwith open(r\'C:
+aiob2, run the following command in your (virtual)
+environment.\n\n```shell\npip install aiob2\n```\n\nAlternatively, for the
+latest though least stable version, you can download it from the GitHub repo:
+\n\n```shell\npip install git+https://github.com/Void-ux/aiob2.git\n```\n\n##
+Usage\n\n### Uploading\n\n```python\nimport aiohttp\nimport asyncio\n\nfrom
+aiob2 import Client\n\n# Our image to upload to our bucket\nwith open(r\'C:
 \\Users\\MS1\\Pictures\\Camera Roll\\IMG_5316.jpeg\', \'rb\') as file:\n data =
 file.read()\n\nasync def main():\n async with Client(\'key_id\', \'key\') as
 client:\n file = await client.upload_file(\n content_bytes=data,\n
-content_type=\'image/jpeg\',\n file_name=\'test.jpg\',\n
-bucket_id=\'bucket_id\',\n )\n\n\nif __name__ == \'__main__\':\n asyncio.run
-(main())\n```\n\nAnd that\'s it! `upload_file()` returns a `File` object that
-neatly wraps everything Backblaze\'s API has provided us with.\nThe `File`
-object\'s documentation can be found [here](https://aiob2.readthedocs.io/en/
-latest/pages/api.html#aiob2.File)\n\n## License\n\n---\n\nThis project is
-released under the [MIT License](https://opensource.org/licenses/MIT).\n',
-'author': 'Dan', 'author_email': 'the.void.altacc@gmail.com', 'maintainer':
-None, 'maintainer_email': None, 'url': 'https://github.com/Void-ux/aiob2',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+file_name=\'test.jpg\',\n bucket_id=\'bucket_id\',\n )\n\n\nif __name__ ==
+\'__main__\':\n asyncio.run(main())\n```\n\nAnd that\'s it! `upload_file()`
+returns a `File` object that neatly wraps everything Backblaze\'s API has
+provided us with.\nThe `File` object\'s documentation can be found [here]
+(https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)\n\n##
+License\n\n---\n\nThis project is released under the [MIT License](https://
+opensource.org/licenses/MIT).\n', 'author': 'Dan', 'author_email':
+'the.void.altacc@gmail.com', 'maintainer': None, 'maintainer_email': None,
+'url': 'https://github.com/Void-ux/aiob2', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `aiob2-0.5.3/PKG-INFO` & `aiob2-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiob2
-Version: 0.5.3
+Version: 0.8.2
 Summary: A simple and easy to use async wrapper for Backblaze's B2 bucket API.
 Home-page: https://github.com/Void-ux/aiob2
 License: MIT
 Keywords: backblaze,b2,cloud,storage
 Author: Dan
 Author-email: the.void.altacc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: speed
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: pytest-asyncio (>=0.19.0,<0.20.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/Void-ux/aiob2/issues/
 Project-URL: Documentation, https://aiob2.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Void-ux/aiob2
 Description-Content-Type: text/markdown
 
 # aiob2
@@ -44,29 +43,29 @@
     </a>
 </p>
 
 aiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).
 
 It will allow you to interact with your B2 bucket, it's files and anything else that the B2 API allows in a modern, object-oriented fashion.
 
-__**NOTE:**__ This API wrapper is by no means *complete* and has many endpoints to cover, though the main ones have been covered (they will be listed below)
+**NOTE:** This API wrapper is by no means *complete* and has many endpoints to cover, though the main ones have been covered (they will be listed below)
 
 ## Installation
 
 ---
 
 aiob2 is compatible with Python 3.8+ (this is an estimate). To install aiob2, run the following command in your (virtual) environment.
 
-```
+```shell
 pip install aiob2
 ```
 
 Alternatively, for the latest though least stable version, you can download it from the GitHub repo:
 
-```
+```shell
 pip install git+https://github.com/Void-ux/aiob2.git
 ```
 
 ## Usage
 
 ### Uploading
 
@@ -80,15 +79,14 @@
 with open(r'C:\Users\MS1\Pictures\Camera Roll\IMG_5316.jpeg', 'rb') as file:
     data = file.read()
 
 async def main():
     async with Client('key_id', 'key') as client:
         file = await client.upload_file(
             content_bytes=data,
-            content_type='image/jpeg',
             file_name='test.jpg',
             bucket_id='bucket_id',
         )
 
 
 if __name__ == '__main__':
     asyncio.run(main())
```


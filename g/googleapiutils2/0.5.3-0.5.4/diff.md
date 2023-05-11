# Comparing `tmp/googleapiutils2-0.5.3.tar.gz` & `tmp/googleapiutils2-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.5.3.tar", max compression
+gzip compressed data, was "googleapiutils2-0.5.4.tar", max compression
```

## Comparing `googleapiutils2-0.5.3.tar` & `googleapiutils2-0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2022-12-30 01:32:12.340806 googleapiutils2-0.5.3/LICENSE
--rw-r--r--   0        0        0     2215 2023-05-09 19:39:40.689070 googleapiutils2-0.5.3/README.md
--rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.3/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.3/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    14800 2023-05-10 19:25:05.643910 googleapiutils2-0.5.3/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      297 2022-12-30 01:32:12.341593 googleapiutils2-0.5.3/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.3/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.5.3/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.3/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.3/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.3/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    12383 2023-05-10 19:07:50.328467 googleapiutils2-0.5.3/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     4919 2023-05-10 19:06:58.729468 googleapiutils2-0.5.3/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     6822 2023-05-09 17:40:05.660193 googleapiutils2-0.5.3/googleapiutils2/utils.py
--rw-r--r--   0        0        0      811 2023-05-10 19:26:10.044961 googleapiutils2-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 googleapiutils2-0.5.3/setup.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 googleapiutils2-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-12-30 01:32:12.340806 googleapiutils2-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2215 2023-05-09 19:39:40.689070 googleapiutils2-0.5.4/README.md
+-rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.4/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.4/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    14898 2023-05-10 19:39:46.420891 googleapiutils2-0.5.4/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      297 2022-12-30 01:32:12.341593 googleapiutils2-0.5.4/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.4/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.5.4/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.4/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.4/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.4/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    12383 2023-05-10 19:07:50.328467 googleapiutils2-0.5.4/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     4919 2023-05-10 19:06:58.729468 googleapiutils2-0.5.4/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     6822 2023-05-09 17:40:05.660193 googleapiutils2-0.5.4/googleapiutils2/utils.py
+-rw-r--r--   0        0        0      811 2023-05-10 19:39:59.956274 googleapiutils2-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 googleapiutils2-0.5.4/setup.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 googleapiutils2-0.5.4/PKG-INFO
```

### Comparing `googleapiutils2-0.5.3/LICENSE` & `googleapiutils2-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/README.md` & `googleapiutils2-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/googleapiutils2/drive/drive.py` & `googleapiutils2-0.5.4/googleapiutils2/drive/drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         """Get a file by its ID."""
         file_id = parse_file_id(file_id)
         return self.files.get(fileId=file_id, fields=fields, **kwargs).execute()
 
     def get_name(
         self, name: str, parents: List[str], q: str | None = None
     ) -> Optional[File]:
-        return next(self._query_children(name, parents, q), None)
+        parents = list(map(parse_file_id, parents)) if parents is not None else []
+        return next(self._query_children(name=name, parents=parents, q=q), None)
 
     def _download(self, file_id: str, out_filepath: Path, mime_type: GoogleMimeTypes):
         request = self.files.export_media(fileId=file_id, mimeType=mime_type.value)
         with out_filepath.open("wb") as out_file:
             downloader = googleapiclient.http.MediaIoBaseDownload(out_file, request)
             done = False
             while done is False:
```

### Comparing `googleapiutils2-0.5.3/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.5.4/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.5.4/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.5.4/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.5.4/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.5.4/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/googleapiutils2/utils.py` & `googleapiutils2-0.5.4/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.3/pyproject.toml` & `googleapiutils2-0.5.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.5.3"
+version = "0.5.4"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.5.3/setup.py` & `googleapiutils2-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.1,<0.6.0',
  'pandas>=1.5.3,<2.0.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'googleapiutils2',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': "Wrapper for Google's Python API.",
     'long_description': '# googleapiutils2\n\nUtilities for\n[Google\'s v2 Python API](https://github.com/googleapis/google-api-python-client).\nCurrently supports sections of the following resources:\n\n-   Drive: `FilesResource`, `...`\n-   Sheets: `SpreadsheetsResource`, `...`\n-   Geocoding\n\n## Quickstart\n\nThis project requires Python `^3.10` to run.\n\nSeveral dependencies are needed, namely the aforesaid Google Python API, but also\nGoogle\'s oauth library, and `requests`. Pre-bundled for ease of use are the fairly\nmonolithic `google-api-stubs`, which greatly improves the usage experience.\n\n### via [`poetry`](https://python-poetry.org/docs/)\n\nInstall poetry, then run\n\n> poetry install\n\nAnd you\'re done.\n\n## Drive\n\n...\n\n## Sheets\n\nSimple example:\n\n```python\n...\ncreds = get_oauth2_creds(client_config=config_path)\nsheets = Sheets(creds=creds)\n\nsheet_id = "id"\nSheet1 = SheetsValueRange(sheets, sheet_id, sheet_name="Sheet1")\n\nrows = [\n    {\n        "Heyy": "99",\n    }\n]\nSheet1[2:3, ...].update(rows)\n```\n\nWhat the above does is: - Get the OAuth2 credentials from the `client_config.json`\nfile - create a `Sheets` object thereupon. - Create a `SheetsValueRange` object, which\nis a wrapper around the `spreadsheets.values` API. - Update the range `Sheet1!A2:B3`\nwith the given rows.\n\nNote the slicing syntax, which will feel quite familiar for any Python programmer.\n\n### SheetSlice\n\nA `SheetsValueRange` object can be sliced in a similar manner to that of a Numpy array.\nThe syntax is as follows:\n\n    slc = Sheet[rows, cols]\n\nWherein `rows` and `cols` are either integers, slices of integers (stride is not\nsupported), strings (in A1 notation), or ellipses (`...`).\n\n```py\nix = SheetSlice["Sheet1", 1:3, 2:4] #  "Sheet1!B2:D4"\nix = SheetSlice["Sheet1", "A1:B2"]  #  "Sheet1!A1:B2"\nix = SheetSlice[1:3, 2:4]           #  "Sheet1!B2:D4"\nix = SheetSlice["A1:B2"]            #  "Sheet1!A1:B2"\nix = SheetSlice[..., 1:3]           #  "Sheet1!A1:Z3"\n```\n\n`SheetSlice` object can also be used as a key into a `SheetsValueRange` object, or a\ndictionary (to use in updating a sheet\'s range, for example). Further, a\n`SheetsValueRange` object can be sliced in a similar manner to that of a `SheetSlice`\nobject, and also be used as a dictionary key.\n',
     'author': 'Mike Babb',
     'author_email': 'mike7400@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mkbabb/googleapiutils2',
```

### Comparing `googleapiutils2-0.5.3/PKG-INFO` & `googleapiutils2-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.5.3
+Version: 0.5.4
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```


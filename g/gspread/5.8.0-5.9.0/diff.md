# Comparing `tmp/gspread-5.8.0.tar.gz` & `tmp/gspread-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread-5.8.0.tar", last modified: Tue Apr  4 22:38:29 2023, max compression
+gzip compressed data, was "gspread-5.9.0.tar", last modified: Thu May 11 10:04:02 2023, max compression
```

## Comparing `gspread-5.8.0.tar` & `gspread-5.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:38:29.511859 gspread-5.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-04 22:37:54.000000 gspread-5.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-04 22:37:54.000000 gspread-5.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-04 22:38:29.511859 gspread-5.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-04 22:37:54.000000 gspread-5.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:38:29.499859 gspread-5.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/advanced.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:38:29.503859 gspread-5.8.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:38:29.503859 gspread-5.8.0/docs/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/models/cell.rst
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/models/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/models/spreadsheet.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/models/worksheet.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/top-level.rst
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/index.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/oauth2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-04 22:37:54.000000 gspread-5.8.0/docs/user-guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:38:29.507859 gspread-5.8.0/gspread/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25508 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    96975 2023-04-04 22:37:54.000000 gspread-5.8.0/gspread/worksheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:38:29.511859 gspread-5.8.0/gspread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-04 22:38:29.000000 gspread-5.8.0/gspread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-04 22:38:29.000000 gspread-5.8.0/gspread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:38:29.000000 gspread-5.8.0/gspread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 22:38:29.000000 gspread-5.8.0/gspread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 22:38:29.000000 gspread-5.8.0/gspread.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:38:29.511859 gspread-5.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-04 22:37:54.000000 gspread-5.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:04:02.522096 gspread-5.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 10:03:18.000000 gspread-5.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 10:03:18.000000 gspread-5.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-11 10:04:02.518096 gspread-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-11 10:03:18.000000 gspread-5.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:04:02.514095 gspread-5.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/advanced.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:04:02.514095 gspread-5.9.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:04:02.514095 gspread-5.9.0/docs/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/models/cell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/models/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/models/spreadsheet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/models/worksheet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/top-level.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/oauth2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-11 10:03:18.000000 gspread-5.9.0/docs/user-guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:04:02.518096 gspread-5.9.0/gspread/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19438 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25006 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98894 2023-05-11 10:03:18.000000 gspread-5.9.0/gspread/worksheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:04:02.518096 gspread-5.9.0/gspread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-11 10:04:02.000000 gspread-5.9.0/gspread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-11 10:04:02.000000 gspread-5.9.0/gspread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:04:02.000000 gspread-5.9.0/gspread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 10:04:02.000000 gspread-5.9.0/gspread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 10:04:02.000000 gspread-5.9.0/gspread.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:04:02.522096 gspread-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-11 10:03:18.000000 gspread-5.9.0/setup.py
```

### Comparing `gspread-5.8.0/LICENSE.txt` & `gspread-5.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/PKG-INFO` & `gspread-5.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread
-Version: 5.8.0
+Version: 5.9.0
 Summary: Google Spreadsheets Python API
 Home-page: https://github.com/burnash/gspread
 Author: Anton Burnashev
 Author-email: fuss.here@gmail.com
 Maintainer: Alexandre Lavigne
 Maintainer-email: lavigne958@gmail.com
 License: MIT
```

### Comparing `gspread-5.8.0/README.md` & `gspread-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/docs/advanced.rst` & `gspread-5.9.0/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/docs/api/exceptions.rst` & `gspread-5.9.0/docs/api/exceptions.rst`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/docs/conf.py` & `gspread-5.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/docs/index.rst` & `gspread-5.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/docs/index.txt` & `gspread-5.9.0/docs/index.txt`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/docs/oauth2.rst` & `gspread-5.9.0/docs/oauth2.rst`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/docs/user-guide.rst` & `gspread-5.9.0/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/gspread/__init__.py` & `gspread-5.9.0/gspread/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ~~~~~~~
 
 Google Spreadsheets client library.
 
 """
 
 
-__version__ = "5.8.0"
+__version__ = "5.9.0"
 __author__ = "Anton Burnashev"
 
 
 from .auth import (
     authorize,
     oauth,
     oauth_from_dict,
```

### Comparing `gspread-5.8.0/gspread/auth.py` & `gspread-5.9.0/gspread/auth.py`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/gspread/cell.py` & `gspread-5.9.0/gspread/cell.py`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/gspread/client.py` & `gspread-5.9.0/gspread/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,32 @@
         )
 
         if response.ok:
             return response
         else:
             raise APIError(response)
 
+    def _get_file_drive_metadata(self, id):
+        """Get the metadata from the Drive API for a specific file
+        This method is mainly here to retrieve the create/update time
+        of a file (these metadata are only accessible from the Drive API).
+        """
+
+        url = DRIVE_FILES_API_V3_URL + "/{}".format(id)
+
+        params = {
+            "supportsAllDrives": True,
+            "includeItemsFromAllDrives": True,
+            "fields": "id,name,createdTime,modifiedTime",
+        }
+
+        res = self.request("get", url, params=params)
+
+        return res.json()
+
     def list_spreadsheet_files(self, title=None, folder_id=None):
         """List all the spreadsheet files
 
         Will list all spreadsheet files owned by/shared with this user account.
 
         :param str title: Filter only spreadsheet files with this title
         :param str folder_id: Only look for spreadsheet files in this folder
```

### Comparing `gspread-5.8.0/gspread/exceptions.py` & `gspread-5.9.0/gspread/exceptions.py`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/gspread/spreadsheet.py` & `gspread-5.9.0/gspread/spreadsheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,35 +51,25 @@
 
     @property
     def creationTime(self):
         """Spreadsheet Creation time."""
         try:
             return self._properties["createdTime"]
         except KeyError:
-            # Filter the list using the name to reduce the request size
-            # Filter the item using the unique ID to ensure we update the exacte same item
-            metadata = finditem(
-                lambda x: x["id"] == self.id,
-                self.client.list_spreadsheet_files(self.title),
-            )
+            metadata = self.client._get_file_drive_metadata(self.id)
             self._properties.update(metadata)
             return self._properties["createdTime"]
 
     @property
     def lastUpdateTime(self):
         """Spreadsheet last updated time."""
         try:
             return self._properties["modifiedTime"]
         except KeyError:
-            # Filter the list using the name to reduce the request size
-            # Filter the item using the unique ID to ensure we update the exacte same item
-            metadata = finditem(
-                lambda x: x["id"] == self.id,
-                self.client.list_spreadsheet_files(self.title),
-            )
+            metadata = self.client._get_file_drive_metadata(self.id)
             self._properties.update(metadata)
             return self._properties["modifiedTime"]
 
     @property
     def updated(self):
         """.. deprecated:: 2.0
```

### Comparing `gspread-5.8.0/gspread/urls.py` & `gspread-5.9.0/gspread/urls.py`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/gspread/utils.py` & `gspread-5.9.0/gspread/utils.py`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/gspread/worksheet.py` & `gspread-5.9.0/gspread/worksheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2290,41 +2290,75 @@
                 "note"
             ]
         except (IndexError, KeyError):
             note = ""
 
         return note
 
+    def update_notes(self, notes):
+        """update multiple notes. The notes are attached to a certain cell.
+
+        :param notes dict: A dict of notes with their cells coordinates and respective content
+
+            dict format is:
+
+            * key: the cell coordinates as A1 range format
+            * value: the string content of the cell
+
+            Example::
+
+                {
+                    "D7": "Please read my notes",
+                    "GH42": "this one is too far",
+                }
+
+        .. versionadded:: 5.9
+        """
+
+        body = {"requests": []}
+
+        for range, content in notes.items():
+            if not isinstance(content, str):
+                raise TypeError(
+                    "Only string allowed as content for a note: '{} - {}'".format(
+                        range, content
+                    )
+                )
+
+            req = {
+                "updateCells": {
+                    "range": a1_range_to_grid_range(range, self.id),
+                    "fields": "note",
+                    "rows": [
+                        {
+                            "values": [
+                                {
+                                    "note": content,
+                                },
+                            ],
+                        },
+                    ],
+                },
+            }
+
+            body["requests"].append(req)
+
+        self.spreadsheet.batch_update(body)
+
+    @cast_to_a1_notation
     def update_note(self, cell, content):
         """Update the content of the note located at `cell`.
 
         :param str cell: A string with cell coordinates in A1 notation,
             e.g. 'D7'.
         :param str note: The text note to insert.
 
         .. versionadded:: 3.7
         """
-
-        if not isinstance(content, str):
-            raise TypeError("Only string allowed as content for a note.")
-
-        grid_range = a1_range_to_grid_range(cell, self.id)
-
-        body = {
-            "requests": [
-                {
-                    "updateCells": {
-                        "range": grid_range,
-                        "rows": [{"values": [{"note": content}]}],
-                        "fields": "note",
-                    }
-                }
-            ]
-        }
-        self.spreadsheet.batch_update(body)
+        self.update_notes({cell: content})
 
     @cast_to_a1_notation
     def insert_note(self, cell, content):
         """Insert a note. The note is attached to a certain cell.
 
         :param str cell: A string with cell coordinates in A1 notation,
             e.g. 'D7'.
@@ -2336,15 +2370,46 @@
         :param int first_row: First row number
         :param int first_col: First column number
         :param int last_row: Last row number
         :param int last_col: Last column number
 
         .. versionadded:: 3.7
         """
-        self.update_note(cell, content)
+        self.update_notes({cell: content})
+
+    def insert_notes(self, notes):
+        """insert multiple notes. The notes are attached to a certain cell.
+
+        :param notes dict: A dict of notes with their cells coordinates and respective content
+
+            dict format is:
+
+            * key: the cell coordinates as A1 range format
+            * value: the string content of the cell
+
+            Example::
+
+                {
+                    "D7": "Please read my notes",
+                    "GH42": "this one is too far",
+                }
+
+        .. versionadded:: 5.9
+        """
+        self.update_notes(notes)
+
+    def clear_notes(self, ranges):
+        """Clear all notes located at the at the coordinates
+        pointed to by ``ranges``.
+
+        :param ranges list: List of A1 coordinates where to clear the notes.
+            e.g. ``["A1", "GH42", "D7"]``
+        """
+        notes = {range: "" for range in ranges}
+        self.update_notes(notes)
 
     @cast_to_a1_notation
     def clear_note(self, cell):
         """Clear a note. The note is attached to a certain cell.
 
         :param str cell: A string with cell coordinates in A1 notation,
             e.g. 'D7'.
@@ -2356,15 +2421,15 @@
         :param int first_col: First column number
         :param int last_row: Last row number
         :param int last_col: Last column number
 
         .. versionadded:: 3.7
         """
         # set the note to <empty string> will clear it
-        self.update_note(cell, "")
+        self.update_notes({cell: ""})
 
     @cast_to_a1_notation
     def define_named_range(self, name, range_name):
         """
         :param str name: A string with range value in A1 notation,
             e.g. 'A1:A5'.
```

### Comparing `gspread-5.8.0/gspread.egg-info/PKG-INFO` & `gspread-5.9.0/gspread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread
-Version: 5.8.0
+Version: 5.9.0
 Summary: Google Spreadsheets Python API
 Home-page: https://github.com/burnash/gspread
 Author: Anton Burnashev
 Author-email: fuss.here@gmail.com
 Maintainer: Alexandre Lavigne
 Maintainer-email: lavigne958@gmail.com
 License: MIT
```

### Comparing `gspread-5.8.0/gspread.egg-info/SOURCES.txt` & `gspread-5.9.0/gspread.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gspread-5.8.0/setup.py` & `gspread-5.9.0/setup.py`

 * *Files identical despite different names*


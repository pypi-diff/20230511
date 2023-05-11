# Comparing `tmp/camerahub_tagger-0.4.1.tar.gz` & `tmp/camerahub_tagger-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.4.1.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.5.0.tar", max compression
```

## Comparing `camerahub_tagger-0.4.1.tar` & `camerahub_tagger-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2908 2023-05-10 15:15:49.738581 camerahub_tagger-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-05-10 15:15:49.738581 camerahub_tagger-0.4.1/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2159 2023-05-10 15:15:49.738581 camerahub_tagger-0.4.1/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2037 2023-05-10 15:15:49.738581 camerahub_tagger-0.4.1/camerahub_tagger/config.py
--rw-r--r--   0        0        0     6899 2023-05-10 15:15:49.738581 camerahub_tagger-0.4.1/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     7724 2023-05-10 15:15:49.738581 camerahub_tagger-0.4.1/camerahub_tagger/main.py
--rw-r--r--   0        0        0      670 2023-05-10 15:16:14.530782 camerahub_tagger-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 camerahub_tagger-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2908 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2628 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2037 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     7204 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     8988 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      670 2023-05-11 14:28:41.697508 camerahub_tagger-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 camerahub_tagger-0.5.0/PKG-INFO
```

### Comparing `camerahub_tagger-0.4.1/README.md` & `camerahub_tagger-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.4.1/camerahub_tagger/api.py` & `camerahub_tagger-0.5.0/camerahub_tagger/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,38 +21,39 @@
             auth=l_auth,
             timeout=10
         )
 
     return bool(response.status_code == 200)
 
 
-def create_scan(l_negative, l_filename, l_server, l_auth):
+def create_scan(filename, server, auth, negative=None, printid=None):
     """
-    Creates a new Scan record in CameraHub, associated with a Negative record
+    Creates a new Scan record in CameraHub, associated with a Negative or Print record
     Returns the uuid of the new Scan record
     {
         "negative": null,
         "print": null,
         "filename": "",
         "date": null
     }
     """
 
     # Only write the basename of the file
-    l_filename = basename(l_filename)
+    filename = basename(filename)
 
     # Create dict
     data = {
-        'negative': l_negative,
-        'filename': l_filename,
+        'negative': negative,
+        'print': printid,
+        'filename': filename,
         'date': date.today()}
-    url = l_server+'/scan/'
+    url = server+'/scan/'
     response = requests.post(
         url,
-        auth=l_auth,
+        auth=auth,
         data = data,
         timeout=10
     )
     response.raise_for_status()
     data=json.loads(response.text)
     return data["uuid"]
 
@@ -94,7 +95,28 @@
     response.raise_for_status()
 
     data=json.loads(response.text)
     if data["count"] == 1:
         negative = data["results"][0]["slug"]
 
     return negative
+
+
+def get_print(l_print, l_server, l_auth):
+    """
+    Get a print by ID
+    """
+    payload = {'id_owner': l_print}
+    url = l_server+'/print/'+l_print
+    response = requests.get(
+        url,
+        auth=l_auth,
+        params=payload,
+        timeout=10
+    )
+    response.raise_for_status()
+
+    data=json.loads(response.text)
+    printid = data["id_owner"]
+    negative = data["negative"]["slug"]
+
+    return printid, negative
```

### Comparing `camerahub_tagger-0.4.1/camerahub_tagger/config.py` & `camerahub_tagger-0.5.0/camerahub_tagger/config.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.4.1/camerahub_tagger/funcs.py` & `camerahub_tagger-0.5.0/camerahub_tagger/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,22 @@
     Guess a negative's film id and frame id based on its filename
     Assumes a format of [film]-[frame]-title.jpg
     for example 123-22-holiday.jpg
     """
     filename = basename(filepath)
     match = re.search(r'^(\d+)-(\w+)-.*\.[Jj][Pp][Ee]?[Gg]$', filename)
     if match and match.group(1) and match.group(2):
-        returnval = (match.group(1), match.group(2))
+        returnval = {'type': 'negative', 'film':match.group(1), 'frame':match.group(2)}
     else:
-        returnval = None
+        # try a print match
+        match = re.search(r'^P(\d+)-.*\.[Jj][Pp][Ee]?[Gg]$', filename)
+        if match and match.group(1):
+            returnval = {'type':'print', 'print':match.group(1)}
+        else:
+            returnval = None
     return returnval
 
 
 def prompt_frame(filename):
     """
     Prompt user to enter film id and frame id
     At the moment these questions are asked sequentially
@@ -138,14 +143,15 @@
         'Copyright': 'Exif.Image.Copyright',
         'FocalLengthIn35mmFilm': 'Exif.Photo.FocalLengthIn35mmFilm',
         'GPSLatitude': 'Exif.GPSInfo.GPSLatitude',
         'GPSLatitudeRef': 'Exif.GPSInfo.GPSLatitudeRef',
         'GPSLongitude': 'Exif.GPSInfo.GPSLongitude',
         'GPSLongitudeRef': 'Exif.GPSInfo.GPSLongitudeRef',
         'ImageID': 'Exif.Image.ImageID',
+        'DocumentName': 'Exif.Image.DocumentName',
     }
 
     exiftag = mapping.get(apitag)
     return exiftag
 
 
 def api2exif(l_apidata):
```

### Comparing `camerahub_tagger-0.4.1/camerahub_tagger/main.py` & `camerahub_tagger-0.5.0/camerahub_tagger/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 import os
 from pathlib import Path
 import pyexiv2
 from requests.models import HTTPError
 from termcolor import cprint
 from camerahub_tagger.config import get_setting
-from camerahub_tagger.api import get_negative, get_scan, create_scan, test_credentials
+from camerahub_tagger.api import get_negative, get_scan, create_scan, test_credentials, get_print
 from camerahub_tagger.funcs import is_valid_uuid, guess_frame, prompt_frame, api2exif, diff_tags, yes_or_no, asciiart, print_summary
 
 # ----------------------------------------------------------------------
 def main():
     cprint(asciiart(), 'light_blue')
 
     # Read in args
@@ -125,52 +125,76 @@
         else:
             # need to match it with a neg/print and generate a scan id
             print(f"{file} does not have an EXIF scan ID")
 
             # else prompt user to identify the scan
             #	guess film/frame from filename
             guess = guess_frame(file)
-            if type(guess) is tuple:
-                film, frame = guess
-                print(f"Deduced Film ID {film} and Frame {frame}")
-
-            else:
-                print(f"{file} does not match FILM-FRAME notation")
-                # prompt user for film/frame
-                #	either accept film/frame or just film then prompt frame
-                film, frame = prompt_frame(file)
-
-            # Lookup Negative from API
-            try:
-                negative = get_negative(film, frame, server, auth)
-            except HTTPError as err:
-                cprint(err, "red")
-                failed.append(file)
-                continue
-            except:
-                cprint(f"Couldn't find Negative ID for {file}", "red")
-                failed.append(file)
-                continue
-            else:
-                print(f"{file} corresponds to Negative {negative}")
-
-            # Create Scan record associated with the Negative
-            try:
-                scan = create_scan(negative, file, server, auth)
-
-                # Opportunistically write the new Scan ID to the file in case Tagger runs into problems
-                # later - otherwise the Scan ID would be lost and a new one generated next time
-                with pyexiv2.Image(file) as img:
-                    img.modify_exif({'Exif.Photo.ImageUniqueID': scan})
-            except:
-                cprint(f"Couldn't generate Scan ID for Negative {negative}", "red")
-                failed.append(file)
-                continue
-            else:
-                print(f"Created new Scan ID {scan}")
+            if type(guess) is dict:
+                if guess['type'] == 'negative':
+                    film = guess['film']
+                    frame = guess['frame']
+                    print(f"Deduced Film ID {film} and Frame {frame}")
+
+                    # Lookup Negative from API
+                    try:
+                        negative = get_negative(film, frame, server, auth)
+                    except HTTPError as err:
+                        cprint(err, "red")
+                        failed.append(file)
+                        continue
+                    except:
+                        cprint(f"Couldn't find Negative ID for {file}", "red")
+                        failed.append(file)
+                        continue
+                    else:
+                        print(f"{file} corresponds to Negative {negative}")
+
+                    # Create Scan record associated with the Negative
+                    try:
+                        scan = create_scan(negative=negative, filename=file, server=server, auth=auth)
+                    except:
+                        cprint(f"Couldn't generate Scan ID for Negative {negative}", "red")
+                        failed.append(file)
+                        continue
+                    else:
+                        print(f"Created new Scan ID {scan}")
+
+                elif guess['type'] == 'print':
+                    printid = guess['print']
+                    print(f"Deduced Print ID {printid}")
+
+                    # Lookup Print from API
+                    try:
+                        (printid, negative) = get_print(printid, server, auth)
+                    except HTTPError as err:
+                        cprint(err, "red")
+                        failed.append(file)
+                        continue
+                    except:
+                        cprint(f"Couldn't find Print ID for {file}", "red")
+                        failed.append(file)
+                        continue
+                    else:
+                        print(f"{file} corresponds to Print {printid}")
+
+                    # Create Scan record associated with the Print *and* Negative
+                    try:
+                        scan = create_scan(printid=printid, negative=negative, filename=file, server=server, auth=auth)
+                    except:
+                        cprint(f"Couldn't generate Scan ID for Print {printid}", "red")
+                        failed.append(file)
+                        continue
+                    else:
+                        print(f"Created new Scan ID {scan}")
+                else:
+                    print(f"{file} does not match FILM-FRAME notation")
+                    # prompt user for film/frame
+                    #	either accept film/frame or just film then prompt frame
+                    film, frame = prompt_frame(file)
 
         # Lookup extended Scan details in API
         try:
             apidata = get_scan(scan, server, auth)
         except:
             cprint(f"Couldn't retrieve data for Scan {scan}", "red")
             failed.append(file)
```

### Comparing `camerahub_tagger-0.4.1/pyproject.toml` & `camerahub_tagger-0.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub-tagger"
-version = "0.4.1"
+version = "0.5.0"
 description = "EXIF tagger for CameraHub"
 authors = ["Jonathan Gazeley <me@jonathangazeley.com>"]
 repository = "https://github.com/camerahub/tagger"
 homepage = "https://camerahub.info/"
 readme = ["README.md"]
 keywords = ["EXIF", "photography", "CameraHub", "metadata"]
```

### Comparing `camerahub_tagger-0.4.1/PKG-INFO` & `camerahub_tagger-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.4.1
+Version: 0.5.0
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/join_eos_exif-1.1.1.tar.gz` & `tmp/join_eos_exif-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "join_eos_exif-1.1.1.tar", max compression
+gzip compressed data, was "join_eos_exif-1.1.2.tar", max compression
```

## Comparing `join_eos_exif-1.1.1.tar` & `join_eos_exif-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      447 2022-12-01 20:57:27.924861 join_eos_exif-1.1.1/README.md
--rw-r--r--   0        0        0     6758 2022-12-01 20:57:27.924861 join_eos_exif-1.1.1/join_eos_exif/OrthoRenamer.py
--rw-r--r--   0        0        0      136 2022-12-01 20:57:27.924861 join_eos_exif-1.1.1/join_eos_exif/__init__.py
--rw-r--r--   0        0        0      537 2022-12-01 20:58:49.457955 join_eos_exif-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 join_eos_exif-1.1.1/setup.py
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 join_eos_exif-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      447 2023-05-11 17:48:25.898827 join_eos_exif-1.1.2/README.md
+-rw-r--r--   0        0        0     7315 2023-05-11 17:48:25.898827 join_eos_exif-1.1.2/join_eos_exif/OrthoRenamer.py
+-rw-r--r--   0        0        0      136 2023-05-11 17:48:25.898827 join_eos_exif-1.1.2/join_eos_exif/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-11 17:51:10.846030 join_eos_exif-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 join_eos_exif-1.1.2/setup.py
+-rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 join_eos_exif-1.1.2/PKG-INFO
```

### Comparing `join_eos_exif-1.1.1/join_eos_exif/OrthoRenamer.py` & `join_eos_exif-1.1.2/join_eos_exif/OrthoRenamer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,34 @@
+import logging
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 
 import numpy as np
 import pandas as pd
 
+logger = logging.getLogger(__name__)
+
 
 class OrthoRenamer(ABC):
     def __init__(self, verbose=True):
         super().__init__()
         self.verbose = verbose
         self.errors = []  # list of filenames that can not be matched.
 
     @staticmethod
     def _get_eos_header_offset(filename: str) -> int:
-        offset = 0
         with open(filename) as f:
-            while f.readline().strip() != "Record Format:":
-                offset += 1
-        return offset + 7  # Additional 7 lines of info after "Record Format:"
+            lines = [line.strip() for line in f.readlines()]
+        try:
+            return lines.index("Record Format:") + 7
+        except ValueError:
+            logger.error(
+                'Invalid EOS file, could not find "Record Format" line in file.'
+            )
+            exit(1)
 
     def read_eos_file(self, filename: str) -> pd.DataFrame:
         """
         Reads the EoS file
         returns list of lists
         EoS file uses tab delimiters
         """
@@ -47,48 +54,52 @@
         returns list if lists
         skip one header line in EXIF
         EXIF file uses comma separator
         """
         exif = pd.read_csv(filename)
 
         # Filter extras headers from file concatenation
-        exif = exif[exif['Filename'] != 'Filename']
+        exif = exif[exif["Filename"] != "Filename"]
 
         # Filter missing date rows
-        exif = exif[exif['GPS Time'] != 'XX:XX:XX.XXXXXX']
+        exif = exif[exif["GPS Time"] != "XX:XX:XX.XXXXXX"]
 
         return exif
 
     @staticmethod
     def truncate_float(number: float, decimals: int = 3) -> float:
-        return np.floor(number * 10 ** decimals) / 10 ** decimals
+        return np.floor(number * 10**decimals) / 10**decimals
 
     def log(self, message):
         if self.verbose:
             print(message)
 
     def join_eos_exif_data(self, eos: pd.DataFrame, exif: pd.DataFrame) -> pd.DataFrame:
         """
         Truncates times to 3 decimals to match them, eg 123.4567 -> 123.456
 
         returns list of lists
         """
         # Cast event IDs and drop missing
-        eos['# EVENT'] = pd.to_numeric(eos['# EVENT'], errors='coerce', downcast='integer').dropna()
-        exif['GPS Event'] = pd.to_numeric(exif['GPS Event'], errors='coerce', downcast='integer').dropna()
+        eos["# EVENT"] = pd.to_numeric(
+            eos["# EVENT"], errors="coerce", downcast="integer"
+        ).dropna()
+        exif["GPS Event"] = pd.to_numeric(
+            exif["GPS Event"], errors="coerce", downcast="integer"
+        ).dropna()
 
         # Inner join on event #s
-        joined = pd.merge(eos, exif, left_on='# EVENT', right_on='GPS Event')
+        joined = pd.merge(eos, exif, left_on="# EVENT", right_on="GPS Event")
 
         # Create updated filename column
-        joined['CIR_Filename'] = joined['Filename'].str[:-4] + "_rgbi.tif"
+        joined["CIR_Filename"] = joined["Filename"].str[:-4] + "_rgbi.tif"
 
         # Populate the errors list
-        unmatched_exif = exif[(~exif['Filename'].isin(joined['Filename']))]
-        self.errors = list(unmatched_exif['Filename'])
+        unmatched_exif = exif[(~exif["Filename"].isin(joined["Filename"]))]
+        self.errors = list(unmatched_exif["Filename"])
 
         # Print some info
         num_matched = len(joined)
         num_not_matched = len(exif) - num_matched
 
         self.log(f"Matched records: {num_matched}")
         self.log(f"Unmatched records: {num_not_matched}")
@@ -98,26 +109,28 @@
 
         return joined
 
     @property
     @abstractmethod
     def csv2df_map(self) -> OrderedDict:
         """Define a mapping from the output CSV column header names
-            to the corresponding joined Pandas dataframe column name."""
-        raise NotImplemented
+        to the corresponding joined Pandas dataframe column name."""
+        raise NotImplementedError
 
     @property
     def output_csv_column_names(self) -> list:
         return list(self.csv2df_map.keys())
 
     @property
     def dataframe_columns_to_output(self) -> list:
         return list(self.csv2df_map.values())
 
-    def join_eos_exif_and_write_output(self, eos_path: str, exif_path: str, output_path: str, separator: str = ","):
+    def join_eos_exif_and_write_output(
+        self, eos_path: str, exif_path: str, output_path: str, separator: str = ","
+    ):
         # skip some header lines in eos file
         eos = self.read_eos_file(eos_path)
         exif = self.read_exif_file(exif_path)
         joined = self.join_eos_exif_data(eos, exif)
 
         # Create a dataframe with just the output data and write it to file
         csv_data = joined[self.dataframe_columns_to_output]
@@ -129,71 +142,91 @@
         """Call self.join_eos_exif_and_write_output when instance is called."""
         return self.join_eos_exif_and_write_output(*args, **kwargs)
 
 
 class GeographicOrthoRenamer(OrthoRenamer):
     @property
     def csv2df_map(self):
-        """Defines the mapping from the output CSV column header names to appropriate Pandas dataframe column name."""
-        return OrderedDict({
-            'CIR_Filename': 'CIR_Filename',
-            'Lon': 'LONG',
-            'Lat': 'LAT',
-            'Altitude': 'ORTHOMETRIC HEIGHT',
-            'Omega': 'OMEGA',
-            'Phi': 'PHI',
-            'Kappa': 'KAPPA'
-        })
+        """
+        Defines the mapping from the output CSV column header names to
+            appropriate Pandas dataframe column name.
+        """
+        return OrderedDict(
+            {
+                "CIR_Filename": "CIR_Filename",
+                "Lon": "LONG",
+                "Lat": "LAT",
+                "Altitude": "ORTHOMETRIC HEIGHT",
+                "Omega": "OMEGA",
+                "Phi": "PHI",
+                "Kappa": "KAPPA",
+            }
+        )
 
 
 class GeographicEllipsRenamer(OrthoRenamer):
     @property
     def csv2df_map(self):
-        """Defines the mapping from the output CSV column header names to appropriate Pandas dataframe column name."""
-        return OrderedDict({
-            'CIR_Filename': 'CIR_Filename',
-            'Lon': 'LONG',
-            'Lat': 'LAT',
-            'Ellips': 'ELLIPSOID HEIGHT',
-            'Omega': 'OMEGA',
-            'Phi': 'PHI',
-            'Kappa': 'KAPPA'
-        })
+        """
+        Defines the mapping from the output CSV column header names to appropriate
+            Pandas dataframe column name.
+        """
+        return OrderedDict(
+            {
+                "CIR_Filename": "CIR_Filename",
+                "Lon": "LONG",
+                "Lat": "LAT",
+                "Ellips": "ELLIPSOID HEIGHT",
+                "Omega": "OMEGA",
+                "Phi": "PHI",
+                "Kappa": "KAPPA",
+            }
+        )
 
 
 class UTMOrthoRenamer(OrthoRenamer):
     @property
     def csv2df_map(self):
-        """Defines the mapping from the output CSV column header names to appropriate Pandas dataframe column name."""
-        return OrderedDict({
-            'CIR_Filename': 'CIR_Filename',
-            'Easting': 'EASTING',
-            'Northing': 'NORTHING',
-            'Altitude': 'ORTHOMETRIC HEIGHT',
-            'Omega': 'OMEGA',
-            'Phi': 'PHI',
-            'Kappa': 'KAPPA'
-        })
+        """
+        Defines the mapping from the output CSV column header names to appropriate
+            Pandas dataframe column name.
+        """
+        return OrderedDict(
+            {
+                "CIR_Filename": "CIR_Filename",
+                "Easting": "EASTING",
+                "Northing": "NORTHING",
+                "Altitude": "ORTHOMETRIC HEIGHT",
+                "Omega": "OMEGA",
+                "Phi": "PHI",
+                "Kappa": "KAPPA",
+            }
+        )
 
 
 class UTMEllipsRenamer(OrthoRenamer):
     @property
     def csv2df_map(self):
-        """Defines the mapping from the output CSV column header names to appropriate Pandas dataframe column name."""
-        return OrderedDict({
-            'CIR_Filename': 'CIR_Filename',
-            'Easting': 'EASTING',
-            'Northing': 'NORTHING',
-            'Ellips': 'ELLIPSOID HEIGHT',
-            'Omega': 'OMEGA',
-            'Phi': 'PHI',
-            'Kappa': 'KAPPA'
-        })
+        """
+        Defines the mapping from the output CSV column header names to appropriate
+            Pandas dataframe column name.
+        """
+        return OrderedDict(
+            {
+                "CIR_Filename": "CIR_Filename",
+                "Easting": "EASTING",
+                "Northing": "NORTHING",
+                "Ellips": "ELLIPSOID HEIGHT",
+                "Omega": "OMEGA",
+                "Phi": "PHI",
+                "Kappa": "KAPPA",
+            }
+        )
 
 
 if __name__ == "__main__":
-    eos_file = '../sample_files/4/EoS.txt'
-    exif_file = '../sample_files/4/ExifLog.csv'
-    output_file = '../sample_files/4/eos_exif_joined.txt'
+    eos_file = "../sample_files/4/EoS.txt"
+    exif_file = "../sample_files/4/ExifLog.csv"
+    output_file = "../sample_files/4/eos_exif_joined.txt"
 
     ortho_renamer = UTMOrthoRenamer()
     ortho_renamer.join_eos_exif_and_write_output(eos_file, exif_file, output_file)
```

### Comparing `join_eos_exif-1.1.1/setup.py` & `join_eos_exif-1.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['join_eos_exif']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyQt6>=6.4.0,<7.0.0', 'numpy>=1.23.5,<2.0.0', 'pandas>=1.5.2,<2.0.0']
+['PyQt6>=6.4.0,<7.0.0', 'numpy>=1.23.5,<2.0.0', 'pandas>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'join-eos-exif',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'Join EOS files to images using EXIF data',
     'long_description': '# joinEOStoEXIF\n\nApplication to join EOS and EXIF data files for image processing\n\nUI made with PyQt5 v5.14.1\nexe generated using Pyinstaller 3.4\n\n## Installation\n\n```sh\npip install -r requirements.txt\n```\n\n## Running\n\nUse join_data.exe or\n\n```sh\npython join_data.py\n```\n\n## Tests\n\nThe test.py file runs tests on sample input files stored in the sample_files folder.\n\nIt looks for one CSV and one txt file in each folder\n\n```sh\npython test.py\n```\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `join_eos_exif-1.1.1/PKG-INFO` & `join_eos_exif-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: join-eos-exif
-Version: 1.1.1
+Version: 1.1.2
 Summary: Join EOS files to images using EXIF data
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyQt6 (>=6.4.0,<7.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # joinEOStoEXIF
 
 Application to join EOS and EXIF data files for image processing
 
 UI made with PyQt5 v5.14.1
```


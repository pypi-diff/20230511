# Comparing `tmp/adapterio-1.4.3.tar.gz` & `tmp/adapterio-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapterio-1.4.3.tar", last modified: Tue May 10 16:30:55 2022, max compression
+gzip compressed data, was "adapterio-1.5.1.tar", last modified: Fri Feb 24 00:27:47 2023, max compression
```

## Comparing `adapterio-1.4.3.tar` & `adapterio-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2022-05-10 16:30:55.576899 adapterio-1.4.3/
--rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2022-05-10 16:30:55.576577 adapterio-1.4.3/PKG-INFO
--rw-r--r--   0 mgrahovac   (502) staff       (20)     7012 2022-04-14 23:31:20.000000 adapterio-1.4.3/README.md
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2022-05-10 16:30:55.573941 adapterio-1.4.3/adapter/
--rw-r--r--   0 mgrahovac   (502) staff       (20)      120 2021-05-09 21:50:30.000000 adapterio-1.4.3/adapter/Secret_example.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)      167 2022-05-10 16:23:01.000000 adapterio-1.4.3/adapter/__init__.py
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2022-05-10 16:30:55.574866 adapterio-1.4.3/adapter/comm/
--rw-r--r--   0 mgrahovac   (502) staff       (20)        0 2021-05-09 21:13:44.000000 adapterio-1.4.3/adapter/comm/__init__.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    25380 2021-10-24 03:02:36.000000 adapterio-1.4.3/adapter/comm/excel.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)     5015 2021-05-09 21:17:58.000000 adapterio-1.4.3/adapter/comm/sql.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)     5438 2022-05-10 16:23:01.000000 adapterio-1.4.3/adapter/comm/tools.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    27665 2022-05-10 16:23:01.000000 adapterio-1.4.3/adapter/i_o.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)      632 2021-05-09 21:17:58.000000 adapterio-1.4.3/adapter/label_map.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    14699 2022-01-29 00:09:54.000000 adapterio-1.4.3/adapter/to_python.py
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2022-05-10 16:30:55.576232 adapterio-1.4.3/adapterio.egg-info/
--rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2022-05-10 16:30:55.000000 adapterio-1.4.3/adapterio.egg-info/PKG-INFO
--rw-r--r--   0 mgrahovac   (502) staff       (20)      389 2022-05-10 16:30:55.000000 adapterio-1.4.3/adapterio.egg-info/SOURCES.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)        1 2022-05-10 16:30:55.000000 adapterio-1.4.3/adapterio.egg-info/dependency_links.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)       88 2022-05-10 16:30:55.000000 adapterio-1.4.3/adapterio.egg-info/requires.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)        8 2022-05-10 16:30:55.000000 adapterio-1.4.3/adapterio.egg-info/top_level.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)      103 2021-08-24 01:33:33.000000 adapterio-1.4.3/pyproject.toml
--rw-r--r--   0 mgrahovac   (502) staff       (20)       38 2022-05-10 16:30:55.577048 adapterio-1.4.3/setup.cfg
--rw-r--r--   0 mgrahovac   (502) staff       (20)     2779 2022-01-21 18:37:00.000000 adapterio-1.4.3/setup.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-02-24 00:27:47.553971 adapterio-1.5.1/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-02-24 00:27:47.553586 adapterio-1.5.1/PKG-INFO
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     7012 2022-04-14 23:31:20.000000 adapterio-1.5.1/README.md
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-02-24 00:27:47.548087 adapterio-1.5.1/adapter/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      120 2021-05-09 21:50:30.000000 adapterio-1.5.1/adapter/Secret_example.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      167 2023-02-24 00:25:20.000000 adapterio-1.5.1/adapter/__init__.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-02-24 00:27:47.550899 adapterio-1.5.1/adapter/comm/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        0 2021-05-09 21:13:44.000000 adapterio-1.5.1/adapter/comm/__init__.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    25380 2021-10-24 03:02:36.000000 adapterio-1.5.1/adapter/comm/excel.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     5015 2021-05-09 21:17:58.000000 adapterio-1.5.1/adapter/comm/sql.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     6547 2023-02-24 00:25:20.000000 adapterio-1.5.1/adapter/comm/tools.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    27742 2023-02-24 00:25:20.000000 adapterio-1.5.1/adapter/i_o.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      632 2021-05-09 21:17:58.000000 adapterio-1.5.1/adapter/label_map.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    14700 2023-02-24 00:25:20.000000 adapterio-1.5.1/adapter/to_python.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-02-24 00:27:47.553097 adapterio-1.5.1/adapterio.egg-info/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-02-24 00:27:47.000000 adapterio-1.5.1/adapterio.egg-info/PKG-INFO
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      389 2023-02-24 00:27:47.000000 adapterio-1.5.1/adapterio.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        1 2023-02-24 00:27:47.000000 adapterio-1.5.1/adapterio.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)       88 2023-02-24 00:27:47.000000 adapterio-1.5.1/adapterio.egg-info/requires.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        8 2023-02-24 00:27:47.000000 adapterio-1.5.1/adapterio.egg-info/top_level.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      103 2021-08-24 01:33:33.000000 adapterio-1.5.1/pyproject.toml
+-rw-r--r--   0 mgrahovac   (502) staff       (20)       38 2023-02-24 00:27:47.554102 adapterio-1.5.1/setup.cfg
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     2779 2023-02-24 00:25:20.000000 adapterio-1.5.1/setup.py
```

### Comparing `adapterio-1.4.3/PKG-INFO` & `adapterio-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapterio
-Version: 1.4.3
+Version: 1.5.1
 Summary: I/O module
 Home-page: https://github.com/LBNL-ETA/Adapter
 Author: Milica Grahovac, Youness Bennani, Thomas Burke, Katie Coughlin, Mohan Ganeshalingam, Akhil Mathur, Evan Neill, Akshay Sharma, Zheng He and Lyra Lan
 License: BSD-3-Clause-LBNL
 Keywords: data,tables,IO for research computation,sql,excel,csv,dataframe,connection
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `adapterio-1.4.3/README.md` & `adapterio-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `adapterio-1.4.3/adapter/comm/excel.py` & `adapterio-1.5.1/adapter/comm/excel.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.4.3/adapter/comm/sql.py` & `adapterio-1.5.1/adapter/comm/sql.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.4.3/adapter/comm/tools.py` & `adapterio-1.5.1/adapter/comm/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 import sys
+from datetime import datetime
 from pathlib import PureWindowsPath, PurePosixPath
 
 
 def process_column_labels(list_of_labels):
     """Removes undesired spaces.
 
     Parameters:
@@ -173,7 +174,45 @@
         else:
             fpath = fd.askopenfilename(
                 title=user_message,
                 filetypes=[("Excel", "*.xlsx *.xls"), ("Database", "*.db")],
             )
 
         return fpath
+
+
+def mark_time(prefix: str = "", ts_format: str = "short") -> str:
+    """This method creates a string using prefix string and a timestamp.
+
+    Parameters
+    ----------
+    prefix : str
+        The prefix to use in the return string. e.g. "adapter"
+    ts_format : str
+        The timestamp format to use in the return string. e.g. 'short', 'long'
+
+    Returns
+    -------
+    str
+        A string with a timestamp. e.g. "adapter_2022_08_08_10h_51m".
+
+    Raises
+    ------
+    ValueError
+        If `ts_format` is neither 'short' nor 'long'.
+
+    Examples
+    --------
+    >>> mark_time(prefix="adapter")
+    "adapter_220808_1051"
+    >>> mark_time(prefix="adapter", ts_format='short')
+    "adapter_220808_1051"
+    >>> mark_time(prefix="adapter",ts_format="long")
+    "adapter_2022_08_08_10h_51m"
+
+    """
+    if ts_format == "short":
+        return f'{prefix}_{datetime.now().strftime("%y%m%d_%H%M")}'
+    elif ts_format == "long":
+        return f'{prefix}_{datetime.now().strftime("%Y_%m_%d_%Hh_%Mm")}'
+    else:
+        raise ValueError("Unsupported timestamp format!")
```

### Comparing `adapterio-1.4.3/adapter/i_o.py` & `adapterio-1.5.1/adapter/i_o.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
+import logging
+import ntpath
 import os
-import numpy as np
-import pandas as pd
-from adapter.to_python import Excel, Db, Db_sqlalchemy, Debugger
-from adapter.label_map import Labels
-
-from adapter.comm.tools import convert_network_drive_path
-
-from datetime import datetime
 import re
 import sqlite3
 from shutil import copy
-import ntpath
 
-import logging
+import numpy as np
+import pandas as pd
+
+from adapter.comm.tools import convert_network_drive_path, mark_time
+from adapter.label_map import Labels
+from adapter.to_python import Excel, Db, Db_sqlalchemy, Debugger
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
-from pdb import set_trace as bp
-
 
 class IO(object):
     """Connects to the main input
     file that can be an excel sheet,
     a csv file or a database,
     loads the data, looks for
     additional input data paths
@@ -121,14 +117,15 @@
         close_db=True,
         save_input=True,
         skip_writeout=False,
         set_first_col_as_index=False,
         quick_db_out_filename=None,
         clean_labels=True,
         to_numeric=None,
+        ts_format="short",
     ):
         """Loads tables from the input file
         as a dictionary of python dataframes.
 
         Recognizes any special table names, such
         as:
 
@@ -140,14 +137,17 @@
             additional input files of file types: csv, excel, db.
             See examples in the test folders on the master
             branch of the adapter repo for details on the
             structure and labels of the table.
 
         Parameters:
 
+            ts_format : str
+                The timestamp format to use in the return string. e.g. 'short', 'long'
+
             create_db: bool
                 Write all tables read from input files
                 into a run database
 
             db_flavor: string
                 Database type. Currently implemented:
                 'sqlite'
@@ -318,15 +318,15 @@
 
             # otherwise declare current folder + "/output" as the output
             # path
             else:
                 outpath_base = os.path.join(os.getcwd(), "output")
                 version = ""
 
-            run_tag = version + "_" + datetime.now().strftime("%Y_%m_%d-%Hh_%Mm")
+            run_tag = mark_time(prefix=version, ts_format=ts_format)
 
             outpath = os.path.join(outpath_base, run_tag)
 
         else:
             outpath = os.getcwd()
             run_tag = quick_db_out_filename
```

### Comparing `adapterio-1.4.3/adapter/label_map.py` & `adapterio-1.5.1/adapter/label_map.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.4.3/adapter/to_python.py` & `adapterio-1.5.1/adapter/to_python.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             Keys is the previously loaded
             dictionary of dataframes
     """
 
     def __init__(self, file_path, pre_existing_keys=None):
         self.file_path = file_path
         self.wb = openpyxl.load_workbook(
-            self.file_path, data_only=True, read_only=False, keep_vba=True
+            self.file_path, data_only=True, read_only=False, keep_vba=False
         )
         self.pre_existing_keys = pre_existing_keys
 
         log.info("Connected to: {}".format(self.file_path))
 
     def load(self, data_object_names=None, kind="all"):
         """Grabs all or a subset of named tables and ranges
```

### Comparing `adapterio-1.4.3/adapterio.egg-info/PKG-INFO` & `adapterio-1.5.1/adapterio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapterio
-Version: 1.4.3
+Version: 1.5.1
 Summary: I/O module
 Home-page: https://github.com/LBNL-ETA/Adapter
 Author: Milica Grahovac, Youness Bennani, Thomas Burke, Katie Coughlin, Mohan Ganeshalingam, Akhil Mathur, Evan Neill, Akshay Sharma, Zheng He and Lyra Lan
 License: BSD-3-Clause-LBNL
 Keywords: data,tables,IO for research computation,sql,excel,csv,dataframe,connection
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `adapterio-1.4.3/setup.py` & `adapterio-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,11 +41,11 @@
     ],
     keywords="data, tables, IO for research computation, sql, excel, csv, dataframe, connection",
     packages=find_packages(exclude=["*.tests", "*.tests"]),
     install_requires=[
         "pandas>=1.0.4",
         "xlwings>=0.19.4",
         "psycopg2-binary>=2.8.6",
-        "SQLAlchemy>=1.4.28",
-        "openpyxl>=3.0.9",
+        "SQLAlchemy==1.4.29",
+        "openpyxl==3.0.9",
     ],
 )
```

